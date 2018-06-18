---
title: Notas de versão da CLI do Azure 2.0
description: Saiba mais sobre as últimas atualizações da CLI do Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/01/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 72e667d74ff8d55f26ecbf3b3c8845c9c03b56be
ms.sourcegitcommit: 5c80e96e96f9608c92a94fa4a9c4afb25099f3fc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/13/2018
ms.locfileid: "35512896"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="286a1-103">Notas de versão da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="286a1-103">Azure CLI 2.0 release notes</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="286a1-104">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="286a1-104">June 13, 2018</span></span>

<span data-ttu-id="286a1-105">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="286a1-105">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="286a1-106">AKS</span><span class="sxs-lookup"><span data-stu-id="286a1-106">AKS</span></span>

* <span data-ttu-id="286a1-107">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="286a1-107">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="286a1-108">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="286a1-108">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span> 
* <span data-ttu-id="286a1-109">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="286a1-109">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="286a1-110">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="286a1-110">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="286a1-111">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="286a1-111">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-112">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-112">AppService</span></span>

* <span data-ttu-id="286a1-113">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="286a1-113">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="286a1-114">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="286a1-114">June 5, 2018</span></span>

<span data-ttu-id="286a1-115">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="286a1-115">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="286a1-116">Interativo</span><span class="sxs-lookup"><span data-stu-id="286a1-116">Interactive</span></span>

* <span data-ttu-id="286a1-117">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="286a1-117">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="286a1-118">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="286a1-118">June 5, 2018</span></span>

<span data-ttu-id="286a1-119">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="286a1-119">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="286a1-120">Núcleo</span><span class="sxs-lookup"><span data-stu-id="286a1-120">Core</span></span>

* <span data-ttu-id="286a1-121">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="286a1-121">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="286a1-122">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="286a1-122">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="286a1-123">ACR</span><span class="sxs-lookup"><span data-stu-id="286a1-123">ACR</span></span>

* <span data-ttu-id="286a1-124">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="286a1-124">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="286a1-125">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="286a1-125">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="286a1-126">AKS</span><span class="sxs-lookup"><span data-stu-id="286a1-126">AKS</span></span>

* <span data-ttu-id="286a1-127">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="286a1-127">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="286a1-128">Lote</span><span class="sxs-lookup"><span data-stu-id="286a1-128">Batch</span></span>

* <span data-ttu-id="286a1-129">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="286a1-129">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="286a1-130">IOT</span><span class="sxs-lookup"><span data-stu-id="286a1-130">IOT</span></span>

* <span data-ttu-id="286a1-131">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="286a1-131">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="286a1-132">Rede</span><span class="sxs-lookup"><span data-stu-id="286a1-132">Network</span></span>

* <span data-ttu-id="286a1-133">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="286a1-133">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="286a1-134">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="286a1-134">Policy Insights</span></span>

* <span data-ttu-id="286a1-135">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="286a1-135">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="286a1-136">ARM</span><span class="sxs-lookup"><span data-stu-id="286a1-136">ARM</span></span>

* <span data-ttu-id="286a1-137">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="286a1-137">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="286a1-138">SQL</span><span class="sxs-lookup"><span data-stu-id="286a1-138">SQL</span></span>

* <span data-ttu-id="286a1-139">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="286a1-139">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="286a1-140">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="286a1-140">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="286a1-141">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="286a1-141">Storage</span></span>

* <span data-ttu-id="286a1-142">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="286a1-142">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-143">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-143">VM</span></span>

* <span data-ttu-id="286a1-144">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="286a1-144">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="286a1-145">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="286a1-145">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="286a1-146">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="286a1-146">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="286a1-147">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="286a1-147">May 22, 2018</span></span>

<span data-ttu-id="286a1-148">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="286a1-148">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="286a1-149">Núcleo</span><span class="sxs-lookup"><span data-stu-id="286a1-149">Core</span></span>

* <span data-ttu-id="286a1-150">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="286a1-150">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="286a1-151">ACS</span><span class="sxs-lookup"><span data-stu-id="286a1-151">ACS</span></span>

* <span data-ttu-id="286a1-152">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="286a1-152">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="286a1-153">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="286a1-153">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-154">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-154">AppService</span></span>

* <span data-ttu-id="286a1-155">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="286a1-155">Improved generic update commands</span></span>
* <span data-ttu-id="286a1-156">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="286a1-156">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="286a1-157">Contêiner</span><span class="sxs-lookup"><span data-stu-id="286a1-157">Container</span></span>

* <span data-ttu-id="286a1-158">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="286a1-158">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="286a1-159">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="286a1-159">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="286a1-160">Extensão</span><span class="sxs-lookup"><span data-stu-id="286a1-160">Extension</span></span>

* <span data-ttu-id="286a1-161">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="286a1-161">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="286a1-162">Interativo</span><span class="sxs-lookup"><span data-stu-id="286a1-162">Interactive</span></span>

* <span data-ttu-id="286a1-163">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="286a1-163">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="286a1-164">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="286a1-164">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="286a1-165">KeyVault</span><span class="sxs-lookup"><span data-stu-id="286a1-165">KeyVault</span></span>

* <span data-ttu-id="286a1-166">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="286a1-166">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="286a1-167">Rede</span><span class="sxs-lookup"><span data-stu-id="286a1-167">Network</span></span>

* <span data-ttu-id="286a1-168">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="286a1-168">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="286a1-169">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="286a1-169">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="286a1-170">SQL</span><span class="sxs-lookup"><span data-stu-id="286a1-170">SQL</span></span>

* <span data-ttu-id="286a1-171">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="286a1-171">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="286a1-172">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="286a1-172">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="286a1-173">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="286a1-173">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span> 
    * <span data-ttu-id="286a1-174">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="286a1-174">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="286a1-175">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="286a1-175">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="286a1-176">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="286a1-176">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="286a1-177">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="286a1-177">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="286a1-178">`edition`.</span><span class="sxs-lookup"><span data-stu-id="286a1-178">`edition`.</span></span> <span data-ttu-id="286a1-179">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="286a1-179">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="286a1-180">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="286a1-180">`elasticPoolName`.</span></span> <span data-ttu-id="286a1-181">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="286a1-181">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="286a1-182">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="286a1-182">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="286a1-183">`edition`.</span><span class="sxs-lookup"><span data-stu-id="286a1-183">`edition`.</span></span> <span data-ttu-id="286a1-184">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="286a1-184">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="286a1-185">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="286a1-185">`dtu`.</span></span> <span data-ttu-id="286a1-186">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="286a1-186">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="286a1-187">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="286a1-187">`databaseDtuMin`.</span></span> <span data-ttu-id="286a1-188">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="286a1-188">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="286a1-189">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="286a1-189">`databaseDtuMax`.</span></span> <span data-ttu-id="286a1-190">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="286a1-190">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="286a1-191">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="286a1-191">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="286a1-192">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="286a1-192">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="286a1-193">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="286a1-193">Storage</span></span>

* <span data-ttu-id="286a1-194">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="286a1-194">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="286a1-195">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="286a1-195">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-196">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-196">VM</span></span>

* <span data-ttu-id="286a1-197">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="286a1-197">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="286a1-198">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="286a1-198">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="286a1-199">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="286a1-199">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="286a1-200">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="286a1-200">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="286a1-201">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="286a1-201">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="286a1-202">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="286a1-202">May 7, 2018</span></span>

<span data-ttu-id="286a1-203">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="286a1-203">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="286a1-204">Núcleo</span><span class="sxs-lookup"><span data-stu-id="286a1-204">Core</span></span>

* <span data-ttu-id="286a1-205">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="286a1-205">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="286a1-206">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="286a1-206">Added limited support for positional arguments</span></span>
* <span data-ttu-id="286a1-207">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="286a1-207">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="286a1-208">#5591</span><span class="sxs-lookup"><span data-stu-id="286a1-208">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="286a1-209">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="286a1-209">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="286a1-210">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="286a1-210">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="286a1-211">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="286a1-211">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="286a1-212">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="286a1-212">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="286a1-213">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="286a1-213">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="286a1-214">ACR</span><span class="sxs-lookup"><span data-stu-id="286a1-214">ACR</span></span>

* <span data-ttu-id="286a1-215">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="286a1-215">Added ACR Build commands</span></span>
* <span data-ttu-id="286a1-216">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="286a1-216">Improved resource not found error messages</span></span>
* <span data-ttu-id="286a1-217">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="286a1-217">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="286a1-218">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="286a1-218">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="286a1-219">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="286a1-219">Improved repository commands error messages</span></span>
* <span data-ttu-id="286a1-220">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="286a1-220">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="286a1-221">ACS</span><span class="sxs-lookup"><span data-stu-id="286a1-221">ACS</span></span>

* <span data-ttu-id="286a1-222">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="286a1-222">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="286a1-223">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="286a1-223">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="286a1-224">AMS</span><span class="sxs-lookup"><span data-stu-id="286a1-224">AMS</span></span>

* <span data-ttu-id="286a1-225">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="286a1-225">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-226">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-226">Appservice</span></span>

* <span data-ttu-id="286a1-227">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="286a1-227">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="286a1-228">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="286a1-228">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="286a1-229">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="286a1-229">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="286a1-230">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="286a1-230">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="286a1-231">Lote AI</span><span class="sxs-lookup"><span data-stu-id="286a1-231">Batch AI</span></span>

* <span data-ttu-id="286a1-232">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="286a1-232">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="286a1-233">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="286a1-233">Cognitive Services</span></span>

* <span data-ttu-id="286a1-234">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="286a1-234">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="286a1-235">Consumo</span><span class="sxs-lookup"><span data-stu-id="286a1-235">Consumption</span></span>

* <span data-ttu-id="286a1-236">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="286a1-236">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="286a1-237">Contêiner</span><span class="sxs-lookup"><span data-stu-id="286a1-237">Container</span></span>

* <span data-ttu-id="286a1-238">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="286a1-238">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="286a1-239">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="286a1-239">Cosmos DB</span></span>

* <span data-ttu-id="286a1-240">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="286a1-240">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="286a1-241">DMS</span><span class="sxs-lookup"><span data-stu-id="286a1-241">DMS</span></span>

* <span data-ttu-id="286a1-242">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="286a1-242">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="286a1-243">Extensão</span><span class="sxs-lookup"><span data-stu-id="286a1-243">Extension</span></span>

* <span data-ttu-id="286a1-244">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="286a1-244">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="286a1-245">Interativo</span><span class="sxs-lookup"><span data-stu-id="286a1-245">Interactive</span></span>

* <span data-ttu-id="286a1-246">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="286a1-246">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="286a1-247">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="286a1-247">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="286a1-248">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="286a1-248">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="286a1-249">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="286a1-249">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="286a1-250">Laboratório</span><span class="sxs-lookup"><span data-stu-id="286a1-250">Lab</span></span>

* <span data-ttu-id="286a1-251">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="286a1-251">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="286a1-252">Rede</span><span class="sxs-lookup"><span data-stu-id="286a1-252">Network</span></span>

* <span data-ttu-id="286a1-253">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="286a1-253">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span> 
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="286a1-254">Perfil</span><span class="sxs-lookup"><span data-stu-id="286a1-254">Profile</span></span>

* <span data-ttu-id="286a1-255">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="286a1-255">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="286a1-256">[ALTERAÇÃO SIGNIFICATIVA] `--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="286a1-256">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="286a1-257">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="286a1-257">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="286a1-258">Redis</span><span class="sxs-lookup"><span data-stu-id="286a1-258">Redis</span></span>

* <span data-ttu-id="286a1-259">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="286a1-259">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="286a1-260">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="286a1-260">Deprecated `redis list-all`.</span></span> <span data-ttu-id="286a1-261">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="286a1-261">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="286a1-262">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="286a1-262">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="286a1-263">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="286a1-263">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="286a1-264">Função</span><span class="sxs-lookup"><span data-stu-id="286a1-264">Role</span></span>

* <span data-ttu-id="286a1-265">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="286a1-265">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="286a1-266">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="286a1-266">Storage</span></span>

* <span data-ttu-id="286a1-267">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="286a1-267">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="286a1-268">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="286a1-268">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="286a1-269">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="286a1-269">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="286a1-270">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="286a1-270">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="286a1-271">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="286a1-271">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-272">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-272">VM</span></span>

* <span data-ttu-id="286a1-273">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="286a1-273">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="286a1-274">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="286a1-274">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="286a1-275">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="286a1-275">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="286a1-276">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="286a1-276">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="286a1-277">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="286a1-277">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="286a1-278">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="286a1-278">Added write accelerator support</span></span> 
* <span data-ttu-id="286a1-279">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="286a1-279">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="286a1-280">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="286a1-280">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="286a1-281">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="286a1-281">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="286a1-282">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="286a1-282">April 10, 2018</span></span>

<span data-ttu-id="286a1-283">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="286a1-283">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="286a1-284">ACR</span><span class="sxs-lookup"><span data-stu-id="286a1-284">ACR</span></span>

* <span data-ttu-id="286a1-285">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="286a1-285">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="286a1-286">ACS</span><span class="sxs-lookup"><span data-stu-id="286a1-286">ACS</span></span>

* <span data-ttu-id="286a1-287">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="286a1-287">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-288">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-288">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="286a1-290">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="286a1-290">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="286a1-291">BatchAI</span><span class="sxs-lookup"><span data-stu-id="286a1-291">BatchAI</span></span>

* <span data-ttu-id="286a1-292">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="286a1-292">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="286a1-293">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="286a1-293">Job level mounting</span></span>
 - <span data-ttu-id="286a1-294">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="286a1-294">Environment variables with secret values</span></span>
 - <span data-ttu-id="286a1-295">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="286a1-295">Performance counters settings</span></span>
 - <span data-ttu-id="286a1-296">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="286a1-296">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="286a1-297">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="286a1-297">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="286a1-298">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="286a1-298">Usage and limits reporting</span></span>
 - <span data-ttu-id="286a1-299">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="286a1-299">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="286a1-300">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="286a1-300">Support for custom images</span></span>
 - <span data-ttu-id="286a1-301">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="286a1-301">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="286a1-302">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="286a1-302">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="286a1-303">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="286a1-303">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="286a1-304">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="286a1-304">National clouds are supported</span></span>
* <span data-ttu-id="286a1-305">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="286a1-305">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="286a1-306">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="286a1-306">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="286a1-307">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="286a1-307">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="286a1-308">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="286a1-308">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="286a1-309">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="286a1-309">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="286a1-310">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="286a1-310">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="286a1-311">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="286a1-311">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="286a1-312">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="286a1-312">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="286a1-313">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="286a1-313">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="286a1-314">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="286a1-314">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="286a1-315">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="286a1-315">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="286a1-316">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="286a1-316">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="286a1-317">[ALTERAÇÃO SIGNIFICATIVA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="286a1-317">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="286a1-318">Cobrança</span><span class="sxs-lookup"><span data-stu-id="286a1-318">Billing</span></span>

* <span data-ttu-id="286a1-319">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="286a1-319">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="286a1-320">Consumo</span><span class="sxs-lookup"><span data-stu-id="286a1-320">Consumption</span></span>

* <span data-ttu-id="286a1-321">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="286a1-321">Added `marketplace` commands</span></span>
* <span data-ttu-id="286a1-322">[ALTERAÇÃO SIGNIFICATIVA] `reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="286a1-322">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="286a1-323">[ALTERAÇÃO SIGNIFICATIVA] `reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="286a1-323">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="286a1-324">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="286a1-324">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="286a1-325">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="286a1-325">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="286a1-326">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="286a1-326">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="286a1-327">Contêiner</span><span class="sxs-lookup"><span data-stu-id="286a1-327">Container</span></span>

* <span data-ttu-id="286a1-328">Adição dos parâmetros de montagem de volume de repositório git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="286a1-328">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="286a1-329">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="286a1-329">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="286a1-330">Extensão</span><span class="sxs-lookup"><span data-stu-id="286a1-330">Extension</span></span>

* <span data-ttu-id="286a1-331">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="286a1-331">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="286a1-332">Interativo</span><span class="sxs-lookup"><span data-stu-id="286a1-332">Interactive</span></span>

* <span data-ttu-id="286a1-333">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="286a1-333">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="286a1-334">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="286a1-334">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="286a1-335">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="286a1-335">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="286a1-336">Rede</span><span class="sxs-lookup"><span data-stu-id="286a1-336">Network</span></span>

* <span data-ttu-id="286a1-337">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="286a1-337">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="286a1-338">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="286a1-338">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="286a1-339">#4910</span><span class="sxs-lookup"><span data-stu-id="286a1-339">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="286a1-340">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="286a1-340">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="286a1-341">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="286a1-341">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="286a1-342">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="286a1-342">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="286a1-343">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="286a1-343">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="286a1-344">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="286a1-344">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="286a1-345">Perfil</span><span class="sxs-lookup"><span data-stu-id="286a1-345">Profile</span></span>

* <span data-ttu-id="286a1-346">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="286a1-346">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="286a1-347">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="286a1-347">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="286a1-348">RDBMS</span><span class="sxs-lookup"><span data-stu-id="286a1-348">RDBMS</span></span>

* <span data-ttu-id="286a1-349">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="286a1-349">Added `georestore` command</span></span>
* <span data-ttu-id="286a1-350">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="286a1-350">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="286a1-351">Recurso</span><span class="sxs-lookup"><span data-stu-id="286a1-351">Resource</span></span>

* <span data-ttu-id="286a1-352">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="286a1-352">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="286a1-353">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="286a1-353">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="286a1-354">SQL</span><span class="sxs-lookup"><span data-stu-id="286a1-354">SQL</span></span>

* <span data-ttu-id="286a1-355">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="286a1-355">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="286a1-356">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="286a1-356">Storage</span></span>

* <span data-ttu-id="286a1-357">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="286a1-357">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-358">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-358">VM</span></span>

* <span data-ttu-id="286a1-359">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="286a1-359">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="286a1-360">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="286a1-360">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="286a1-362">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="286a1-362">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="286a1-363">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="286a1-363">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="286a1-364">#5718</span><span class="sxs-lookup"><span data-stu-id="286a1-364">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="286a1-365">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="286a1-365">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="286a1-366">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="286a1-366">March 27, 2018</span></span>

<span data-ttu-id="286a1-367">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="286a1-367">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="286a1-368">Núcleo</span><span class="sxs-lookup"><span data-stu-id="286a1-368">Core</span></span>

* <span data-ttu-id="286a1-369">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="286a1-369">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="286a1-370">ACS</span><span class="sxs-lookup"><span data-stu-id="286a1-370">ACS</span></span>

* <span data-ttu-id="286a1-371">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="286a1-371">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-372">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-372">Appservice</span></span>

* <span data-ttu-id="286a1-373">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="286a1-373">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="286a1-374">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="286a1-374">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="286a1-375">Backup</span><span class="sxs-lookup"><span data-stu-id="286a1-375">Backup</span></span>

* <span data-ttu-id="286a1-376">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="286a1-376">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="286a1-377">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="286a1-377">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="286a1-378">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="286a1-378">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="286a1-379">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="286a1-379">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="286a1-380">Contêiner</span><span class="sxs-lookup"><span data-stu-id="286a1-380">Container</span></span>

* <span data-ttu-id="286a1-381">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="286a1-381">Added `container exec` command.</span></span> <span data-ttu-id="286a1-382">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="286a1-382">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="286a1-383">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="286a1-383">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="286a1-384">Extensão</span><span class="sxs-lookup"><span data-stu-id="286a1-384">Extension</span></span>

* <span data-ttu-id="286a1-385">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="286a1-385">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="286a1-386">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="286a1-386">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="286a1-387">[ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="286a1-387">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="286a1-388">Interativo</span><span class="sxs-lookup"><span data-stu-id="286a1-388">Interactive</span></span>

* <span data-ttu-id="286a1-389">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="286a1-389">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="286a1-390">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="286a1-390">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="286a1-391">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="286a1-391">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="286a1-392">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="286a1-392">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="286a1-393">Laboratório</span><span class="sxs-lookup"><span data-stu-id="286a1-393">Lab</span></span>

* <span data-ttu-id="286a1-394">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="286a1-394">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="286a1-395">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="286a1-395">Monitor</span></span>

* <span data-ttu-id="286a1-396">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="286a1-396">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="286a1-397">[#4529](https://github.com/Azure/azure-cli/issues/5785) corrigido: `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="286a1-397">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="286a1-398">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="286a1-398">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="286a1-399">Rede</span><span class="sxs-lookup"><span data-stu-id="286a1-399">Network</span></span>

* <span data-ttu-id="286a1-400">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="286a1-400">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="286a1-401">Perfil</span><span class="sxs-lookup"><span data-stu-id="286a1-401">Profile</span></span>

* <span data-ttu-id="286a1-402">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="286a1-402">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="286a1-403">RDBMS</span><span class="sxs-lookup"><span data-stu-id="286a1-403">RDBMS</span></span>

* <span data-ttu-id="286a1-404">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="286a1-404">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="286a1-405">Recurso</span><span class="sxs-lookup"><span data-stu-id="286a1-405">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="286a1-407">Função</span><span class="sxs-lookup"><span data-stu-id="286a1-407">Role</span></span>

* <span data-ttu-id="286a1-408">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="286a1-408">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="286a1-409">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="286a1-409">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="286a1-410">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="286a1-410">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="286a1-411">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="286a1-411">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="286a1-412">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="286a1-412">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="286a1-413">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="286a1-413">Storage</span></span>

* <span data-ttu-id="286a1-414">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="286a1-414">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="286a1-415">[4049#](https://github.com/Azure/azure-cli/issues/4049) corrigido: problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="286a1-415">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-416">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-416">VM</span></span>

* <span data-ttu-id="286a1-417">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="286a1-417">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="286a1-418">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="286a1-418">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="286a1-419">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="286a1-419">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="286a1-420">[ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="286a1-420">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="286a1-421">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="286a1-421">March 13, 2018</span></span>

<span data-ttu-id="286a1-422">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="286a1-422">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="286a1-423">ACR</span><span class="sxs-lookup"><span data-stu-id="286a1-423">ACR</span></span>

* <span data-ttu-id="286a1-424">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="286a1-424">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="286a1-425">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="286a1-425">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="286a1-426">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="286a1-426">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="286a1-427">ACS</span><span class="sxs-lookup"><span data-stu-id="286a1-427">ACS</span></span>

* <span data-ttu-id="286a1-428">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="286a1-428">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="286a1-429">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="286a1-429">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="286a1-430">Supervisor</span><span class="sxs-lookup"><span data-stu-id="286a1-430">Advisor</span></span>

* <span data-ttu-id="286a1-431">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="286a1-431">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="286a1-432">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="286a1-432">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="286a1-433">[ALTERAÇÃO SIGNIFICATIVA] `advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="286a1-433">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="286a1-434">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="286a1-434">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="286a1-435">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="286a1-435">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-436">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-436">Appservice</span></span>

* <span data-ttu-id="286a1-437">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="286a1-437">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="286a1-438">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="286a1-438">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="286a1-439">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="286a1-439">Eventhubs</span></span>

* <span data-ttu-id="286a1-440">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="286a1-440">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="286a1-441">Extensão</span><span class="sxs-lookup"><span data-stu-id="286a1-441">Extension</span></span>

* <span data-ttu-id="286a1-442">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="286a1-442">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="286a1-443">Interativo</span><span class="sxs-lookup"><span data-stu-id="286a1-443">Interactive</span></span>

* <span data-ttu-id="286a1-444">[5625](https://github.com/Azure/azure-cli/issues/5625) corrigido: manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="286a1-444">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="286a1-445">[3016](https://github.com/Azure/azure-cli/issues/3016) corrigido: histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="286a1-445">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="286a1-446">[5688](https://github.com/Azure/azure-cli/issues/5688) corrigido: as conclusões não aparecerão se o carregamento da tabela de comando encontrou uma exceção</span><span class="sxs-lookup"><span data-stu-id="286a1-446">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="286a1-447">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="286a1-447">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="286a1-448">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="286a1-448">Monitor</span></span>

* <span data-ttu-id="286a1-449">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="286a1-449">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="286a1-450">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="286a1-450">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="286a1-451">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="286a1-451">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="286a1-452">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="286a1-452">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="286a1-453">Rede</span><span class="sxs-lookup"><span data-stu-id="286a1-453">Network</span></span>

* <span data-ttu-id="286a1-454">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="286a1-454">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="286a1-455">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="286a1-455">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="286a1-456">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="286a1-456">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="286a1-457">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="286a1-457">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="286a1-458">Perfil</span><span class="sxs-lookup"><span data-stu-id="286a1-458">Profile</span></span>

* <span data-ttu-id="286a1-459">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="286a1-459">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="286a1-460">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="286a1-460">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="286a1-461">RDBMS</span><span class="sxs-lookup"><span data-stu-id="286a1-461">RDBMS</span></span>

* <span data-ttu-id="286a1-462">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="286a1-462">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="286a1-463">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="286a1-463">Service Bus</span></span>

* <span data-ttu-id="286a1-464">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="286a1-464">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="286a1-465">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="286a1-465">Storage</span></span>

* <span data-ttu-id="286a1-466">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="286a1-466">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="286a1-467">[5286](https://github.com/Azure/azure-cli/issues/5286) corrigido: os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="286a1-467">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-468">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-468">VM</span></span>

* <span data-ttu-id="286a1-469">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="286a1-469">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="286a1-470">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="286a1-470">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="286a1-471">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="286a1-471">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="286a1-472">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="286a1-472">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="286a1-473">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="286a1-473">February 27, 2018</span></span>

<span data-ttu-id="286a1-474">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="286a1-474">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="286a1-475">Núcleo</span><span class="sxs-lookup"><span data-stu-id="286a1-475">Core</span></span>

* <span data-ttu-id="286a1-476">Correção [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="286a1-476">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="286a1-477">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="286a1-477">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="286a1-478">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="286a1-478">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="286a1-479">ACS</span><span class="sxs-lookup"><span data-stu-id="286a1-479">ACS</span></span>

* <span data-ttu-id="286a1-480">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="286a1-480">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="286a1-481">Correção do problema de permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="286a1-481">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="286a1-482">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="286a1-482">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="286a1-483">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="286a1-483">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-484">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-484">Appservice</span></span>

* <span data-ttu-id="286a1-485">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="286a1-485">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="286a1-486">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="286a1-486">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="286a1-487">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="286a1-487">Cognitive Services</span></span>

* <span data-ttu-id="286a1-488">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="286a1-488">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="286a1-489">Consumo</span><span class="sxs-lookup"><span data-stu-id="286a1-489">Consumption</span></span>

* <span data-ttu-id="286a1-490">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="286a1-490">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="286a1-491">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="286a1-491">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="286a1-492">Contêiner</span><span class="sxs-lookup"><span data-stu-id="286a1-492">Container</span></span>

* <span data-ttu-id="286a1-493">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="286a1-493">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="286a1-494">Rede</span><span class="sxs-lookup"><span data-stu-id="286a1-494">Network</span></span>

* <span data-ttu-id="286a1-495">Correção [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="286a1-495">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="286a1-496">Recurso</span><span class="sxs-lookup"><span data-stu-id="286a1-496">Resource</span></span>

* <span data-ttu-id="286a1-497">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="286a1-497">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="286a1-498">Função</span><span class="sxs-lookup"><span data-stu-id="286a1-498">Role</span></span>

* <span data-ttu-id="286a1-499">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="286a1-499">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="286a1-500">SQL</span><span class="sxs-lookup"><span data-stu-id="286a1-500">SQL</span></span>

* <span data-ttu-id="286a1-501">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="286a1-501">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="286a1-502">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="286a1-502">Storage</span></span>

* <span data-ttu-id="286a1-503">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="286a1-503">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-504">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-504">VM</span></span>

* <span data-ttu-id="286a1-505">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="286a1-505">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="286a1-506">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="286a1-506">February 13, 2018</span></span>

<span data-ttu-id="286a1-507">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="286a1-507">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="286a1-508">Núcleo</span><span class="sxs-lookup"><span data-stu-id="286a1-508">Core</span></span>

* <span data-ttu-id="286a1-509">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="286a1-509">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="286a1-510">ACS</span><span class="sxs-lookup"><span data-stu-id="286a1-510">ACS</span></span>

* <span data-ttu-id="286a1-511">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="286a1-511">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="286a1-512">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="286a1-512">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="286a1-513">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="286a1-513">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="286a1-514">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="286a1-514">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="286a1-515">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="286a1-515">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="286a1-516">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="286a1-516">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="286a1-517">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="286a1-517">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="286a1-518">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="286a1-518">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-519">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-519">Appservice</span></span>

* <span data-ttu-id="286a1-520">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="286a1-520">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="286a1-521">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="286a1-521">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="286a1-522">CDN</span><span class="sxs-lookup"><span data-stu-id="286a1-522">CDN</span></span>

* <span data-ttu-id="286a1-523">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="286a1-523">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="286a1-524">Contêiner</span><span class="sxs-lookup"><span data-stu-id="286a1-524">Container</span></span>

* <span data-ttu-id="286a1-525">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="286a1-525">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="286a1-526">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="286a1-526">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="286a1-527">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="286a1-527">CosmosDB</span></span>

* <span data-ttu-id="286a1-528">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="286a1-528">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="286a1-529">Extensão</span><span class="sxs-lookup"><span data-stu-id="286a1-529">Extension</span></span>

* <span data-ttu-id="286a1-530">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="286a1-530">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="286a1-531">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="286a1-531">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="286a1-532">Comentários</span><span class="sxs-lookup"><span data-stu-id="286a1-532">Feedback</span></span>

* <span data-ttu-id="286a1-533">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="286a1-533">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="286a1-534">Interativo</span><span class="sxs-lookup"><span data-stu-id="286a1-534">Interactive</span></span>

* <span data-ttu-id="286a1-535">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="286a1-535">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="286a1-536">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="286a1-536">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="286a1-537">IoT</span><span class="sxs-lookup"><span data-stu-id="286a1-537">IoT</span></span>

* <span data-ttu-id="286a1-538">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="286a1-538">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="286a1-539">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="286a1-539">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="286a1-540">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="286a1-540">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="286a1-541">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="286a1-541">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="286a1-542">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="286a1-542">Monitor</span></span>

* <span data-ttu-id="286a1-543">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="286a1-543">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="286a1-544">Rede</span><span class="sxs-lookup"><span data-stu-id="286a1-544">Network</span></span>

* <span data-ttu-id="286a1-545">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="286a1-545">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="286a1-546">Perfil</span><span class="sxs-lookup"><span data-stu-id="286a1-546">Profile</span></span>

* <span data-ttu-id="286a1-547">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="286a1-547">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="286a1-548">Recurso</span><span class="sxs-lookup"><span data-stu-id="286a1-548">Resource</span></span>

* <span data-ttu-id="286a1-549">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="286a1-549">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="286a1-550">Função</span><span class="sxs-lookup"><span data-stu-id="286a1-550">Role</span></span>

* <span data-ttu-id="286a1-551">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="286a1-551">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="286a1-552">SQL</span><span class="sxs-lookup"><span data-stu-id="286a1-552">SQL</span></span>

* <span data-ttu-id="286a1-553">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="286a1-553">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="286a1-554">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="286a1-554">Added `sql db rename`</span></span>
* <span data-ttu-id="286a1-555">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="286a1-555">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="286a1-556">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="286a1-556">Storage</span></span>

* <span data-ttu-id="286a1-557">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="286a1-557">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-558">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-558">VM</span></span>

* <span data-ttu-id="286a1-559">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="286a1-559">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="286a1-560">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="286a1-560">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="286a1-561">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="286a1-561">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="286a1-562">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="286a1-562">January 31, 2018</span></span>

<span data-ttu-id="286a1-563">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="286a1-563">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="286a1-564">Núcleo</span><span class="sxs-lookup"><span data-stu-id="286a1-564">Core</span></span>

* <span data-ttu-id="286a1-565">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="286a1-565">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="286a1-566">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="286a1-566">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="286a1-567">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="286a1-567">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="286a1-568">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="286a1-568">Use `--verbose` to see</span></span>
* <span data-ttu-id="286a1-569">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="286a1-569">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="286a1-570">ACS</span><span class="sxs-lookup"><span data-stu-id="286a1-570">ACS</span></span>

* <span data-ttu-id="286a1-571">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="286a1-571">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="286a1-572">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="286a1-572">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-573">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-573">Appservice</span></span>

* <span data-ttu-id="286a1-574">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="286a1-574">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="286a1-575">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="286a1-575">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="286a1-576">CDN</span><span class="sxs-lookup"><span data-stu-id="286a1-576">CDN</span></span>

* <span data-ttu-id="286a1-577">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="286a1-577">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="286a1-578">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="286a1-578">CosmosDB</span></span>

* <span data-ttu-id="286a1-579">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="286a1-579">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="286a1-580">Interativo</span><span class="sxs-lookup"><span data-stu-id="286a1-580">Interactive</span></span>

* <span data-ttu-id="286a1-581">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="286a1-581">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="286a1-582">Rede</span><span class="sxs-lookup"><span data-stu-id="286a1-582">Network</span></span>

* <span data-ttu-id="286a1-583">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="286a1-583">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="286a1-584">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="286a1-584">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="286a1-585">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="286a1-585">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="286a1-586">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="286a1-586">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="286a1-587">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="286a1-587">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="286a1-588">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="286a1-588">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="286a1-589">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="286a1-589">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="286a1-590">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="286a1-590">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="286a1-591">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="286a1-591">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="286a1-592">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="286a1-592">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="286a1-593">Perfil</span><span class="sxs-lookup"><span data-stu-id="286a1-593">Profile</span></span>

* <span data-ttu-id="286a1-594">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="286a1-594">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="286a1-595">Recurso</span><span class="sxs-lookup"><span data-stu-id="286a1-595">Resource</span></span>

* <span data-ttu-id="286a1-596">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="286a1-596">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="286a1-597">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="286a1-597">Storage</span></span>

* <span data-ttu-id="286a1-598">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="286a1-598">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="286a1-599">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="286a1-599">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="286a1-600">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="286a1-600">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="286a1-601">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="286a1-601">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="286a1-602">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="286a1-602">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-603">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-603">VM</span></span>

* <span data-ttu-id="286a1-604">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="286a1-604">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="286a1-605">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="286a1-605">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="286a1-606">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="286a1-606">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="286a1-607">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="286a1-607">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="286a1-608">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="286a1-608">January 17, 2018</span></span>

<span data-ttu-id="286a1-609">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="286a1-609">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="286a1-610">ACR</span><span class="sxs-lookup"><span data-stu-id="286a1-610">ACR</span></span>

* <span data-ttu-id="286a1-611">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="286a1-611">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="286a1-612">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="286a1-612">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="286a1-613">ACS</span><span class="sxs-lookup"><span data-stu-id="286a1-613">ACS</span></span>

* <span data-ttu-id="286a1-614">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="286a1-614">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="286a1-615">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="286a1-615">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-616">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-616">Appservice</span></span>

* <span data-ttu-id="286a1-617">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="286a1-617">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="286a1-618">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="286a1-618">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="286a1-619">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="286a1-619">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="286a1-620">Backup</span><span class="sxs-lookup"><span data-stu-id="286a1-620">Backup</span></span>

* <span data-ttu-id="286a1-621">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="286a1-621">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="286a1-622">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="286a1-622">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="286a1-623">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="286a1-623">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="286a1-624">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="286a1-624">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="286a1-625">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="286a1-625">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="286a1-626">Lote</span><span class="sxs-lookup"><span data-stu-id="286a1-626">Batch</span></span>

* <span data-ttu-id="286a1-627">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="286a1-627">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="286a1-628">Nuvem</span><span class="sxs-lookup"><span data-stu-id="286a1-628">Cloud</span></span>

* <span data-ttu-id="286a1-629">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="286a1-629">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="286a1-630">Consumo</span><span class="sxs-lookup"><span data-stu-id="286a1-630">Consumption</span></span>

* <span data-ttu-id="286a1-631">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="286a1-631">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="286a1-632">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="286a1-632">Event Grid</span></span>

* <span data-ttu-id="286a1-633">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="286a1-633">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="286a1-634">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="286a1-634">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="286a1-635">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="286a1-635">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="286a1-636">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="286a1-636">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="286a1-637">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="286a1-637">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="286a1-638">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="286a1-638">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="286a1-639">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="286a1-639">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="286a1-640">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="286a1-640">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="286a1-641">Interativo</span><span class="sxs-lookup"><span data-stu-id="286a1-641">Interactive</span></span>

* <span data-ttu-id="286a1-642">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="286a1-642">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="286a1-643">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="286a1-643">Fixed errors on startup</span></span>
* <span data-ttu-id="286a1-644">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="286a1-644">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="286a1-645">IoT</span><span class="sxs-lookup"><span data-stu-id="286a1-645">IoT</span></span>

* <span data-ttu-id="286a1-646">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="286a1-646">Added support for device provisioning service</span></span>
* <span data-ttu-id="286a1-647">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="286a1-647">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="286a1-648">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="286a1-648">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="286a1-649">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="286a1-649">Monitor</span></span>

* <span data-ttu-id="286a1-650">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="286a1-650">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="286a1-651">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="286a1-651">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="286a1-652">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="286a1-652">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="286a1-653">Rede</span><span class="sxs-lookup"><span data-stu-id="286a1-653">Network</span></span>

* <span data-ttu-id="286a1-654">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="286a1-654">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="286a1-655">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="286a1-655">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="286a1-656">Perfil</span><span class="sxs-lookup"><span data-stu-id="286a1-656">Profile</span></span>

* <span data-ttu-id="286a1-657">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="286a1-657">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="286a1-658">Função</span><span class="sxs-lookup"><span data-stu-id="286a1-658">Role</span></span>

* <span data-ttu-id="286a1-659">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="286a1-659">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="286a1-660">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="286a1-660">Service Fabric</span></span>

* <span data-ttu-id="286a1-661">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="286a1-661">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="286a1-662">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="286a1-662">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-663">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-663">VM</span></span>

* <span data-ttu-id="286a1-664">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="286a1-664">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="286a1-665">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="286a1-665">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="286a1-666">[ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="286a1-666">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="286a1-667">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="286a1-667">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="286a1-668">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="286a1-668">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="286a1-669">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="286a1-669">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="286a1-670">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="286a1-670">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="286a1-671">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="286a1-671">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="286a1-672">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="286a1-672">December 19, 2017</span></span>

<span data-ttu-id="286a1-673">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="286a1-673">Version 2.0.23</span></span>

* <span data-ttu-id="286a1-674">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="286a1-674">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="286a1-675">Contêiner</span><span class="sxs-lookup"><span data-stu-id="286a1-675">Container</span></span>

* <span data-ttu-id="286a1-676">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="286a1-676">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="286a1-677">Rede</span><span class="sxs-lookup"><span data-stu-id="286a1-677">Network</span></span>

* <span data-ttu-id="286a1-678">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="286a1-678">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="286a1-679">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="286a1-679">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="286a1-680">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="286a1-680">Storage</span></span>

* <span data-ttu-id="286a1-681">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="286a1-681">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-682">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-682">VM</span></span>

* <span data-ttu-id="286a1-683">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="286a1-683">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="286a1-684">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="286a1-684">December 5, 2017</span></span>

<span data-ttu-id="286a1-685">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="286a1-685">Version 2.0.22</span></span>

* <span data-ttu-id="286a1-686">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="286a1-686">Removed `az component` commands.</span></span> <span data-ttu-id="286a1-687">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="286a1-687">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="286a1-688">Núcleo</span><span class="sxs-lookup"><span data-stu-id="286a1-688">Core</span></span>
* <span data-ttu-id="286a1-689">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="286a1-689">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="286a1-690">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="286a1-690">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="286a1-691">ACS</span><span class="sxs-lookup"><span data-stu-id="286a1-691">ACS</span></span>

* <span data-ttu-id="286a1-692">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="286a1-692">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="286a1-693">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="286a1-693">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="286a1-694">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="286a1-694">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="286a1-695">Supervisor</span><span class="sxs-lookup"><span data-stu-id="286a1-695">Advisor</span></span>

* <span data-ttu-id="286a1-696">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="286a1-696">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-697">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-697">Appservice</span></span>

* <span data-ttu-id="286a1-698">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="286a1-698">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="286a1-699">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="286a1-699">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="286a1-700">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="286a1-700">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="286a1-701">Consumo</span><span class="sxs-lookup"><span data-stu-id="286a1-701">Consumption</span></span>

* <span data-ttu-id="286a1-702">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="286a1-702">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="286a1-703">Contêiner</span><span class="sxs-lookup"><span data-stu-id="286a1-703">Container</span></span>

* <span data-ttu-id="286a1-704">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="286a1-704">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="286a1-705">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="286a1-705">Monitor</span></span>

* <span data-ttu-id="286a1-706">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="286a1-706">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="286a1-707">Recurso</span><span class="sxs-lookup"><span data-stu-id="286a1-707">Resource</span></span>

* <span data-ttu-id="286a1-708">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="286a1-708">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="286a1-709">Função</span><span class="sxs-lookup"><span data-stu-id="286a1-709">Role</span></span>

* <span data-ttu-id="286a1-710">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="286a1-710">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="286a1-711">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="286a1-711">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="286a1-712">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="286a1-712">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="286a1-713">SQL</span><span class="sxs-lookup"><span data-stu-id="286a1-713">SQL</span></span>

* <span data-ttu-id="286a1-714">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="286a1-714">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="286a1-715">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="286a1-715">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-716">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-716">VM</span></span>

* <span data-ttu-id="286a1-717">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="286a1-717">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="286a1-718">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="286a1-718">November 14, 2017</span></span>

<span data-ttu-id="286a1-719">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="286a1-719">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="286a1-720">ACR</span><span class="sxs-lookup"><span data-stu-id="286a1-720">ACR</span></span>

* <span data-ttu-id="286a1-721">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="286a1-721">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="286a1-722">ACS</span><span class="sxs-lookup"><span data-stu-id="286a1-722">ACS</span></span>

* <span data-ttu-id="286a1-723">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="286a1-723">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="286a1-724">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="286a1-724">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="286a1-725">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="286a1-725">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="286a1-726">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="286a1-726">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="286a1-727">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="286a1-727">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-728">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-728">Appservice</span></span>

* <span data-ttu-id="286a1-729">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="286a1-729">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="286a1-730">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="286a1-730">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="286a1-731">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="286a1-731">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="286a1-732">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="286a1-732">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="286a1-733">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="286a1-733">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="286a1-734">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="286a1-734">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="286a1-735">Lote</span><span class="sxs-lookup"><span data-stu-id="286a1-735">Batch</span></span>

* <span data-ttu-id="286a1-736">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="286a1-736">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="286a1-737">Batchai</span><span class="sxs-lookup"><span data-stu-id="286a1-737">Batchai</span></span>

* <span data-ttu-id="286a1-738">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="286a1-738">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="286a1-739">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="286a1-739">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="286a1-740">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="286a1-740">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="286a1-741">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="286a1-741">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="286a1-742">Nuvem</span><span class="sxs-lookup"><span data-stu-id="286a1-742">Cloud</span></span>

* <span data-ttu-id="286a1-743">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="286a1-743">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="286a1-744">Contêiner</span><span class="sxs-lookup"><span data-stu-id="286a1-744">Container</span></span>

* <span data-ttu-id="286a1-745">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="286a1-745">Added support to open multiple ports</span></span>
* <span data-ttu-id="286a1-746">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="286a1-746">Added container group restart policy</span></span>
* <span data-ttu-id="286a1-747">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="286a1-747">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="286a1-748">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="286a1-748">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="286a1-749">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="286a1-749">Data Lake Analytics</span></span>

* <span data-ttu-id="286a1-750">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="286a1-750">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="286a1-751">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="286a1-751">Data Lake Store</span></span>

* <span data-ttu-id="286a1-752">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="286a1-752">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="286a1-753">Extensão</span><span class="sxs-lookup"><span data-stu-id="286a1-753">Extension</span></span>

* <span data-ttu-id="286a1-754">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="286a1-754">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="286a1-755">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="286a1-755">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="286a1-756">IoT</span><span class="sxs-lookup"><span data-stu-id="286a1-756">IoT</span></span>

* <span data-ttu-id="286a1-757">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="286a1-757">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="286a1-758">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="286a1-758">Monitor</span></span>

* <span data-ttu-id="286a1-759">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="286a1-759">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="286a1-760">Rede</span><span class="sxs-lookup"><span data-stu-id="286a1-760">Network</span></span>

* <span data-ttu-id="286a1-761">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="286a1-761">Added support for CAA DNS records</span></span>
* <span data-ttu-id="286a1-762">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="286a1-762">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="286a1-763">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="286a1-763">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="286a1-764">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="286a1-764">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="286a1-765">Reservas</span><span class="sxs-lookup"><span data-stu-id="286a1-765">Reservations</span></span>

* <span data-ttu-id="286a1-766">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="286a1-766">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="286a1-767">Recurso</span><span class="sxs-lookup"><span data-stu-id="286a1-767">Resource</span></span>

* <span data-ttu-id="286a1-768">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="286a1-768">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="286a1-769">SQL</span><span class="sxs-lookup"><span data-stu-id="286a1-769">SQL</span></span>

* <span data-ttu-id="286a1-770">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="286a1-770">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="286a1-771">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="286a1-771">Storage</span></span>

* <span data-ttu-id="286a1-772">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="286a1-772">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="286a1-773">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="286a1-773">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="286a1-774">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="286a1-774">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="286a1-775">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="286a1-775">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="286a1-776">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="286a1-776">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="286a1-777">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="286a1-777">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="286a1-778">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="286a1-778">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-779">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-779">VM</span></span>

* <span data-ttu-id="286a1-780">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="286a1-780">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="286a1-781">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="286a1-781">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="286a1-782">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="286a1-782">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="286a1-783">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="286a1-783">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="286a1-784">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="286a1-784">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="286a1-785">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="286a1-785">October 24, 2017</span></span>

<span data-ttu-id="286a1-786">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="286a1-786">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="286a1-787">Núcleo</span><span class="sxs-lookup"><span data-stu-id="286a1-787">Core</span></span>

* <span data-ttu-id="286a1-788">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="286a1-788">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="286a1-789">ACR</span><span class="sxs-lookup"><span data-stu-id="286a1-789">ACR</span></span>

* <span data-ttu-id="286a1-790">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="286a1-790">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="286a1-791">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="286a1-791">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="286a1-792">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="286a1-792">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="286a1-793">ACS</span><span class="sxs-lookup"><span data-stu-id="286a1-793">ACS</span></span>

* <span data-ttu-id="286a1-794">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="286a1-794">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="286a1-795">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="286a1-795">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-796">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-796">Appservice</span></span>

* <span data-ttu-id="286a1-797">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="286a1-797">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="286a1-798">Componente</span><span class="sxs-lookup"><span data-stu-id="286a1-798">Component</span></span>

* <span data-ttu-id="286a1-799">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="286a1-799">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="286a1-800">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="286a1-800">Monitor</span></span>

* <span data-ttu-id="286a1-801">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="286a1-801">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="286a1-802">Recurso</span><span class="sxs-lookup"><span data-stu-id="286a1-802">Resource</span></span>

* <span data-ttu-id="286a1-803">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="286a1-803">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="286a1-804">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="286a1-804">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-805">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-805">VM</span></span>

* <span data-ttu-id="286a1-806">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="286a1-806">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="286a1-807">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="286a1-807">October 9, 2017</span></span>

<span data-ttu-id="286a1-808">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="286a1-808">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="286a1-809">Núcleo</span><span class="sxs-lookup"><span data-stu-id="286a1-809">Core</span></span>

* <span data-ttu-id="286a1-810">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="286a1-810">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-811">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-811">Appservice</span></span>

* <span data-ttu-id="286a1-812">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="286a1-812">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="286a1-813">Lote</span><span class="sxs-lookup"><span data-stu-id="286a1-813">Batch</span></span>

* <span data-ttu-id="286a1-814">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="286a1-814">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="286a1-815">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="286a1-815">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="286a1-816">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="286a1-816">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="286a1-817">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="286a1-817">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="286a1-818">Batchai</span><span class="sxs-lookup"><span data-stu-id="286a1-818">Batchai</span></span>

* <span data-ttu-id="286a1-819">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="286a1-819">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="286a1-820">Keyvault</span><span class="sxs-lookup"><span data-stu-id="286a1-820">Keyvault</span></span>

* <span data-ttu-id="286a1-821">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="286a1-821">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="286a1-822">(#4448)</span><span class="sxs-lookup"><span data-stu-id="286a1-822">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="286a1-823">Rede</span><span class="sxs-lookup"><span data-stu-id="286a1-823">Network</span></span>

* <span data-ttu-id="286a1-824">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="286a1-824">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="286a1-825">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="286a1-825">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="286a1-826">Recurso</span><span class="sxs-lookup"><span data-stu-id="286a1-826">Resource</span></span>

* <span data-ttu-id="286a1-827">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="286a1-827">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="286a1-828">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="286a1-828">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="286a1-829">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="286a1-829">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="286a1-830">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="286a1-830">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="286a1-831">Sql</span><span class="sxs-lookup"><span data-stu-id="286a1-831">Sql</span></span>

* <span data-ttu-id="286a1-832">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="286a1-832">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="286a1-833">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="286a1-833">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="286a1-834">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="286a1-834">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="286a1-835">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="286a1-835">Storage</span></span>

* <span data-ttu-id="286a1-836">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="286a1-836">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-837">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-837">Vm</span></span>

* <span data-ttu-id="286a1-838">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="286a1-838">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="286a1-839">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="286a1-839">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="286a1-840">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="286a1-840">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="286a1-841">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="286a1-841">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="286a1-842">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="286a1-842">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="286a1-843">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="286a1-843">September 22, 2017</span></span>

<span data-ttu-id="286a1-844">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="286a1-844">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="286a1-845">Recurso</span><span class="sxs-lookup"><span data-stu-id="286a1-845">Resource</span></span>

* <span data-ttu-id="286a1-846">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="286a1-846">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="286a1-847">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="286a1-847">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="286a1-848">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="286a1-848">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="286a1-849">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="286a1-849">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="286a1-850">Rede</span><span class="sxs-lookup"><span data-stu-id="286a1-850">Network</span></span>

* <span data-ttu-id="286a1-851">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="286a1-851">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="286a1-852">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="286a1-852">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="286a1-853">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="286a1-853">Added `asg` application security group commands</span></span>
* <span data-ttu-id="286a1-854">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="286a1-854">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="286a1-855">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="286a1-855">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="286a1-856">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="286a1-856">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="286a1-857">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="286a1-857">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="286a1-858">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="286a1-858">Storage</span></span>

* <span data-ttu-id="286a1-859">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="286a1-859">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="286a1-860">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="286a1-860">Eventgrid</span></span>

* <span data-ttu-id="286a1-861">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="286a1-861">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="286a1-862">SQL</span><span class="sxs-lookup"><span data-stu-id="286a1-862">SQL</span></span>

* <span data-ttu-id="286a1-863">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="286a1-863">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="286a1-864">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="286a1-864">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="286a1-865">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="286a1-865">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="286a1-866">Keyvault</span><span class="sxs-lookup"><span data-stu-id="286a1-866">Keyvault</span></span>

* <span data-ttu-id="286a1-867">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="286a1-867">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-868">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-868">VM</span></span>

* <span data-ttu-id="286a1-869">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="286a1-869">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="286a1-870">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="286a1-870">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="286a1-871">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="286a1-871">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="286a1-872">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="286a1-872">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="286a1-873">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="286a1-873">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="286a1-874">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="286a1-874">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="286a1-875">ACS</span><span class="sxs-lookup"><span data-stu-id="286a1-875">ACS</span></span>

* <span data-ttu-id="286a1-876">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="286a1-876">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-877">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-877">Appservice</span></span>

* <span data-ttu-id="286a1-878">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="286a1-878">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="286a1-879">Backup</span><span class="sxs-lookup"><span data-stu-id="286a1-879">Backup</span></span>

* <span data-ttu-id="286a1-880">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="286a1-880">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="286a1-881">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="286a1-881">September 11, 2017</span></span>

<span data-ttu-id="286a1-882">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="286a1-882">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="286a1-883">Núcleo</span><span class="sxs-lookup"><span data-stu-id="286a1-883">Core</span></span>

* <span data-ttu-id="286a1-884">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="286a1-884">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="286a1-885">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="286a1-885">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="286a1-886">Acs</span><span class="sxs-lookup"><span data-stu-id="286a1-886">Acs</span></span>

* <span data-ttu-id="286a1-887">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="286a1-887">Added `acs list-locations` command</span></span>
* <span data-ttu-id="286a1-888">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="286a1-888">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-889">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-889">Appservice</span></span>

* <span data-ttu-id="286a1-890">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="286a1-890">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="286a1-891">CDN</span><span class="sxs-lookup"><span data-stu-id="286a1-891">CDN</span></span>

* <span data-ttu-id="286a1-892">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="286a1-892">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="286a1-893">Extensão</span><span class="sxs-lookup"><span data-stu-id="286a1-893">Extension</span></span>

* <span data-ttu-id="286a1-894">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="286a1-894">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="286a1-895">Keyvault</span><span class="sxs-lookup"><span data-stu-id="286a1-895">Keyvault</span></span>

* <span data-ttu-id="286a1-896">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="286a1-896">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="286a1-897">Rede</span><span class="sxs-lookup"><span data-stu-id="286a1-897">Network</span></span>

* <span data-ttu-id="286a1-898">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="286a1-898">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="286a1-899">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="286a1-899">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="286a1-900">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="286a1-900">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="286a1-901">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="286a1-901">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="286a1-902">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="286a1-902">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="286a1-903">Recurso</span><span class="sxs-lookup"><span data-stu-id="286a1-903">Resource</span></span>

* <span data-ttu-id="286a1-904">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="286a1-904">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="286a1-905">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="286a1-905">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="286a1-906">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="286a1-906">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="286a1-907">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="286a1-907">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="286a1-908">SQL</span><span class="sxs-lookup"><span data-stu-id="286a1-908">SQL</span></span>

* <span data-ttu-id="286a1-909">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="286a1-909">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-910">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-910">VM</span></span>

* <span data-ttu-id="286a1-911">Corrigido: Não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="286a1-911">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="286a1-912">Corrigido: Usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="286a1-912">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="286a1-913">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="286a1-913">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="286a1-914">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="286a1-914">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="286a1-915">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="286a1-915">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="286a1-916">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="286a1-916">August 31, 2017</span></span>

<span data-ttu-id="286a1-917">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="286a1-917">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="286a1-918">Keyvault</span><span class="sxs-lookup"><span data-stu-id="286a1-918">Keyvault</span></span>

* <span data-ttu-id="286a1-919">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="286a1-919">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="286a1-920">Sf</span><span class="sxs-lookup"><span data-stu-id="286a1-920">Sf</span></span>

* <span data-ttu-id="286a1-921">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="286a1-921">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="286a1-922">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="286a1-922">Storage</span></span>

* <span data-ttu-id="286a1-923">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="286a1-923">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="286a1-924">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="286a1-924">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="286a1-925">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="286a1-925">August 28, 2017</span></span>

<span data-ttu-id="286a1-926">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="286a1-926">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="286a1-927">CLI</span><span class="sxs-lookup"><span data-stu-id="286a1-927">CLI</span></span>

* <span data-ttu-id="286a1-928">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="286a1-928">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="286a1-929">ACS</span><span class="sxs-lookup"><span data-stu-id="286a1-929">ACS</span></span>

* <span data-ttu-id="286a1-930">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="286a1-930">Corrected preview regions</span></span>
* <span data-ttu-id="286a1-931">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="286a1-931">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="286a1-932">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="286a1-932">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-933">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-933">Appservice</span></span>

* <span data-ttu-id="286a1-934">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="286a1-934">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="286a1-935">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="286a1-935">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="286a1-936">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="286a1-936">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="286a1-937">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="286a1-937">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="286a1-938">Correção: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="286a1-938">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="286a1-939">IoT</span><span class="sxs-lookup"><span data-stu-id="286a1-939">IoT</span></span>

* <span data-ttu-id="286a1-940">Correção #3934: Criação de política não limpa as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="286a1-940">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="286a1-941">Rede</span><span class="sxs-lookup"><span data-stu-id="286a1-941">Network</span></span>

* <span data-ttu-id="286a1-942">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="286a1-942">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="286a1-943">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="286a1-943">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="286a1-944">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="286a1-944">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="286a1-945">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="286a1-945">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="286a1-946">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="286a1-946">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="286a1-947">Perfil</span><span class="sxs-lookup"><span data-stu-id="286a1-947">Profile</span></span>

* <span data-ttu-id="286a1-948">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="286a1-948">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="286a1-949">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="286a1-949">Service Fabric</span></span>

* <span data-ttu-id="286a1-950">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="286a1-950">Preview release</span></span>
* <span data-ttu-id="286a1-951">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="286a1-951">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="286a1-952">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="286a1-952">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="286a1-953">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="286a1-953">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="286a1-954">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="286a1-954">Storage</span></span>

* <span data-ttu-id="286a1-955">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="286a1-955">Enabled setting blob tier</span></span>
* <span data-ttu-id="286a1-956">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="286a1-956">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="286a1-957">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="286a1-957">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="286a1-958">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="286a1-958">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="286a1-959">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="286a1-959">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="286a1-960">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="286a1-960">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-961">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-961">VM</span></span>

* <span data-ttu-id="286a1-962">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="286a1-962">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="286a1-963">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="286a1-963">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="286a1-964">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="286a1-964">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="286a1-965">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="286a1-965">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="286a1-966">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="286a1-966">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="286a1-967">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="286a1-967">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="286a1-968">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="286a1-968">August 15, 2017</span></span>

<span data-ttu-id="286a1-969">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="286a1-969">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="286a1-970">ACS</span><span class="sxs-lookup"><span data-stu-id="286a1-970">ACS</span></span>

* <span data-ttu-id="286a1-971">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="286a1-971">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-972">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-972">Appservice</span></span>

* <span data-ttu-id="286a1-973">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="286a1-973">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="286a1-974">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="286a1-974">Event Grid</span></span>

* <span data-ttu-id="286a1-975">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="286a1-975">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="286a1-976">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="286a1-976">August 11, 2017</span></span>

<span data-ttu-id="286a1-977">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="286a1-977">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="286a1-978">ACS</span><span class="sxs-lookup"><span data-stu-id="286a1-978">ACS</span></span>

* <span data-ttu-id="286a1-979">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="286a1-979">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="286a1-980">Lote</span><span class="sxs-lookup"><span data-stu-id="286a1-980">Batch</span></span>

* <span data-ttu-id="286a1-981">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="286a1-981">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="286a1-982">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="286a1-982">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="286a1-983">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="286a1-983">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="286a1-984">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="286a1-984">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="286a1-985">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="286a1-985">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="286a1-986">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="286a1-986">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="286a1-987">Componente</span><span class="sxs-lookup"><span data-stu-id="286a1-987">Component</span></span>

* <span data-ttu-id="286a1-988">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="286a1-988">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="286a1-989">Contêiner</span><span class="sxs-lookup"><span data-stu-id="286a1-989">Container</span></span>

* <span data-ttu-id="286a1-990">`create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="286a1-990">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="286a1-991">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="286a1-991">Data Lake Store</span></span>

* <span data-ttu-id="286a1-992">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="286a1-992">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="286a1-993">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="286a1-993">Event Grid</span></span>

* <span data-ttu-id="286a1-994">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="286a1-994">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="286a1-995">Rede</span><span class="sxs-lookup"><span data-stu-id="286a1-995">Network</span></span>

* <span data-ttu-id="286a1-996">`lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="286a1-996">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="286a1-997">`application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="286a1-997">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="286a1-998">`application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="286a1-998">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="286a1-999">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="286a1-999">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="286a1-1000">Perfil</span><span class="sxs-lookup"><span data-stu-id="286a1-1000">Profile</span></span>

* <span data-ttu-id="286a1-1001">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="286a1-1001">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="286a1-1002">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="286a1-1002">Storage</span></span>

* <span data-ttu-id="286a1-1003">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="286a1-1003">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-1004">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-1004">VM</span></span>

* <span data-ttu-id="286a1-1005">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="286a1-1005">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="286a1-1006">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="286a1-1006">Exposed `list-skus` command</span></span>
* <span data-ttu-id="286a1-1007">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="286a1-1007">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="286a1-1008">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="286a1-1008">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="286a1-1009">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="286a1-1009">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="286a1-1010">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="286a1-1010">July 28, 2017</span></span>

<span data-ttu-id="286a1-1011">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="286a1-1011">Version 2.0.12</span></span>

* <span data-ttu-id="286a1-1012">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="286a1-1012">Added container commands</span></span>
* <span data-ttu-id="286a1-1013">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="286a1-1013">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="286a1-1014">Núcleo</span><span class="sxs-lookup"><span data-stu-id="286a1-1014">Core</span></span>

* <span data-ttu-id="286a1-1015">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="286a1-1015">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="286a1-1016">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="286a1-1016">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="286a1-1017">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="286a1-1017">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="286a1-1018">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="286a1-1018">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="286a1-1019">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="286a1-1019">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="286a1-1020">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="286a1-1020">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="286a1-1021">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="286a1-1021">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="286a1-1022">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="286a1-1022">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="286a1-1023">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="286a1-1023">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="286a1-1024">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="286a1-1024">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="286a1-1025">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="286a1-1025">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="286a1-1026">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="286a1-1026">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="286a1-1027">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="286a1-1027">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="286a1-1028">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="286a1-1028">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="286a1-1029">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="286a1-1029">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="286a1-1030">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="286a1-1030">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="286a1-1031">ACR</span><span class="sxs-lookup"><span data-stu-id="286a1-1031">ACR</span></span>

* <span data-ttu-id="286a1-1032">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="286a1-1032">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="286a1-1033">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="286a1-1033">Support SKU update for managed registries</span></span>
* <span data-ttu-id="286a1-1034">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="286a1-1034">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="286a1-1035">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="286a1-1035">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="286a1-1036">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="286a1-1036">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="286a1-1037">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="286a1-1037">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="286a1-1038">ACS</span><span class="sxs-lookup"><span data-stu-id="286a1-1038">ACS</span></span>

* <span data-ttu-id="286a1-1039">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="286a1-1039">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-1040">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-1040">Appservice</span></span>

* <span data-ttu-id="286a1-1041">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="286a1-1041">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="286a1-1042">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="286a1-1042">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="286a1-1043">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="286a1-1043">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="286a1-1044">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="286a1-1044">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="286a1-1045">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="286a1-1045">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="286a1-1046">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="286a1-1046">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="286a1-1047">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="286a1-1047">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="286a1-1048">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="286a1-1048">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="286a1-1049">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="286a1-1049">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="286a1-1050">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="286a1-1050">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="286a1-1051">Lote</span><span class="sxs-lookup"><span data-stu-id="286a1-1051">Batch</span></span>

* <span data-ttu-id="286a1-1052">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="286a1-1052">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="286a1-1053">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="286a1-1053">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="286a1-1054">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="286a1-1054">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="286a1-1055">CDN</span><span class="sxs-lookup"><span data-stu-id="286a1-1055">CDN</span></span>

* <span data-ttu-id="286a1-1056">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="286a1-1056">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="286a1-1057">Nuvem</span><span class="sxs-lookup"><span data-stu-id="286a1-1057">Cloud</span></span>

* <span data-ttu-id="286a1-1058">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="286a1-1058">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="286a1-1059">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="286a1-1059">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="286a1-1060">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="286a1-1060">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="286a1-1061">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="286a1-1061">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="286a1-1062">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="286a1-1062">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="286a1-1063">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="286a1-1063">CosmosDB</span></span>

* <span data-ttu-id="286a1-1064">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="286a1-1064">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="286a1-1065">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="286a1-1065">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="286a1-1066">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="286a1-1066">Data Lake Analytics</span></span>

* <span data-ttu-id="286a1-1067">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="286a1-1067">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="286a1-1068">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="286a1-1068">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="286a1-1069">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="286a1-1069">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="286a1-1070">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="286a1-1070">Data Lake Store</span></span>

* <span data-ttu-id="286a1-1071">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="286a1-1071">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="286a1-1072">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="286a1-1072">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="286a1-1073">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="286a1-1073">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="286a1-1074">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="286a1-1074">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="286a1-1075">Interativo</span><span class="sxs-lookup"><span data-stu-id="286a1-1075">Interactive</span></span>

* <span data-ttu-id="286a1-1076">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="286a1-1076">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="286a1-1077">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="286a1-1077">Increased test coverage</span></span>
* <span data-ttu-id="286a1-1078">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="286a1-1078">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="286a1-1079">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="286a1-1079">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="286a1-1080">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="286a1-1080">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="286a1-1081">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="286a1-1081">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="286a1-1082">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="286a1-1082">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="286a1-1083">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="286a1-1083">Added `--progress` flag</span></span>
* <span data-ttu-id="286a1-1084">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="286a1-1084">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="286a1-1085">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="286a1-1085">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="286a1-1086">IoT</span><span class="sxs-lookup"><span data-stu-id="286a1-1086">IoT</span></span>

* <span data-ttu-id="286a1-1087">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="286a1-1087">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="286a1-1088">(#3934)</span><span class="sxs-lookup"><span data-stu-id="286a1-1088">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="286a1-1089">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="286a1-1089">Key vault</span></span>

* <span data-ttu-id="286a1-1090">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="286a1-1090">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="286a1-1091">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="286a1-1091">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="286a1-1092">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="286a1-1092">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="286a1-1093">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="286a1-1093">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="286a1-1094">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="286a1-1094">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="286a1-1095">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="286a1-1095">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="286a1-1096">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="286a1-1096">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="286a1-1097">(#3307)</span><span class="sxs-lookup"><span data-stu-id="286a1-1097">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="286a1-1098">Laboratório</span><span class="sxs-lookup"><span data-stu-id="286a1-1098">Lab</span></span>

* <span data-ttu-id="286a1-1099">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="286a1-1099">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="286a1-1100">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="286a1-1100">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="286a1-1101">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="286a1-1101">Monitor</span></span>

* <span data-ttu-id="286a1-1102">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="286a1-1102">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="286a1-1103">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="286a1-1103">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="286a1-1104">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="286a1-1104">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="286a1-1105">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="286a1-1105">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="286a1-1106">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="286a1-1106">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="286a1-1107">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="286a1-1107">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="286a1-1108">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="286a1-1108">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="286a1-1109">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="286a1-1109">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="286a1-1110">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="286a1-1110">`location` no longer required</span></span>
  * <span data-ttu-id="286a1-1111">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="286a1-1111">Add name and ID support for target</span></span>
  * <span data-ttu-id="286a1-1112">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="286a1-1112">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="286a1-1113">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="286a1-1113">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="286a1-1114">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="286a1-1114">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="286a1-1115">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="286a1-1115">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="286a1-1116">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="286a1-1116">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="286a1-1117">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="286a1-1117">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="286a1-1118">Rede</span><span class="sxs-lookup"><span data-stu-id="286a1-1118">Network</span></span>

* <span data-ttu-id="286a1-1119">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="286a1-1119">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="286a1-1120">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="286a1-1120">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="286a1-1121">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="286a1-1121">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="286a1-1122">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="286a1-1122">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="286a1-1123">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="286a1-1123">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="286a1-1124">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="286a1-1124">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="286a1-1125">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="286a1-1125">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="286a1-1126">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="286a1-1126">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="286a1-1127">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="286a1-1127">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="286a1-1128">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="286a1-1128">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="286a1-1129">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="286a1-1129">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="286a1-1130">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="286a1-1130">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="286a1-1131">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="286a1-1131">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="286a1-1132">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="286a1-1132">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="286a1-1133">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="286a1-1133">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="286a1-1134">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="286a1-1134">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="286a1-1135">Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS</span><span class="sxs-lookup"><span data-stu-id="286a1-1135">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="286a1-1136">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="286a1-1136">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="286a1-1137">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="286a1-1137">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="286a1-1138">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="286a1-1138">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="286a1-1139">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="286a1-1139">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="286a1-1140">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="286a1-1140">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="286a1-1141">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="286a1-1141">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="286a1-1142">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="286a1-1142">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="286a1-1143">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="286a1-1143">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="286a1-1144">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="286a1-1144">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="286a1-1145">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="286a1-1145">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="286a1-1146">Perfil</span><span class="sxs-lookup"><span data-stu-id="286a1-1146">Profile</span></span>

* <span data-ttu-id="286a1-1147">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="286a1-1147">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="286a1-1148">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="286a1-1148">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="286a1-1149">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="286a1-1149">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="286a1-1150">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="286a1-1150">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="286a1-1151">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="286a1-1151">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="286a1-1152">RDBMS</span><span class="sxs-lookup"><span data-stu-id="286a1-1152">RDBMS</span></span>

* <span data-ttu-id="286a1-1153">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="286a1-1153">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="286a1-1154">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="286a1-1154">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="286a1-1155">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="286a1-1155">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="286a1-1156">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="286a1-1156">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="286a1-1157">Recurso</span><span class="sxs-lookup"><span data-stu-id="286a1-1157">Resource</span></span>

* <span data-ttu-id="286a1-1158">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="286a1-1158">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="286a1-1159">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="286a1-1159">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="286a1-1160">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="286a1-1160">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="286a1-1161">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="286a1-1161">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="286a1-1162">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="286a1-1162">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="286a1-1163">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="286a1-1163">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="286a1-1164">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="286a1-1164">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="286a1-1165">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="286a1-1165">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="286a1-1166">Função</span><span class="sxs-lookup"><span data-stu-id="286a1-1166">Role</span></span>

* <span data-ttu-id="286a1-1167">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="286a1-1167">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="286a1-1168">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="286a1-1168">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="286a1-1169">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="286a1-1169">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="286a1-1170">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="286a1-1170">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="286a1-1171">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="286a1-1171">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="286a1-1172">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="286a1-1172">Service Fabric</span></span>
* <span data-ttu-id="286a1-1173">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="286a1-1173">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="286a1-1174">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="286a1-1174">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="286a1-1175">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="286a1-1175">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="286a1-1176">SQL</span><span class="sxs-lookup"><span data-stu-id="286a1-1176">SQL</span></span>

* <span data-ttu-id="286a1-1177">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="286a1-1177">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="286a1-1178">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="286a1-1178">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="286a1-1179">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="286a1-1179">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="286a1-1180">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="286a1-1180">Storage</span></span>

* <span data-ttu-id="286a1-1181">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="286a1-1181">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="286a1-1182">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="286a1-1182">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="286a1-1183">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="286a1-1183">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="286a1-1184">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="286a1-1184">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="286a1-1185">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="286a1-1185">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="286a1-1186">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="286a1-1186">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-1187">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-1187">VM</span></span>

* <span data-ttu-id="286a1-1188">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="286a1-1188">Support configuring nsg</span></span>
* <span data-ttu-id="286a1-1189">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="286a1-1189">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="286a1-1190">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="286a1-1190">Support managed service identities</span></span>
* <span data-ttu-id="286a1-1191">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="286a1-1191">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="286a1-1192">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="286a1-1192">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="286a1-1193">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="286a1-1193">May 10, 2017</span></span>

<span data-ttu-id="286a1-1194">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="286a1-1194">Version 2.0.6</span></span>

* <span data-ttu-id="286a1-1195">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="286a1-1195">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="286a1-1196">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="286a1-1196">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="286a1-1197">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="286a1-1197">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="286a1-1198">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="286a1-1198">Include Cognitive Services module</span></span>
* <span data-ttu-id="286a1-1199">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="286a1-1199">Include Service Fabric module</span></span>
* <span data-ttu-id="286a1-1200">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="286a1-1200">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="286a1-1201">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="286a1-1201">Add support for CDN commands</span></span>
* <span data-ttu-id="286a1-1202">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="286a1-1202">Remove Container module</span></span>
* <span data-ttu-id="286a1-1203">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="286a1-1203">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="286a1-1204">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="286a1-1204">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="286a1-1205">Núcleo</span><span class="sxs-lookup"><span data-stu-id="286a1-1205">Core</span></span>

* <span data-ttu-id="286a1-1206">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="286a1-1206">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="286a1-1207">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="286a1-1207">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="286a1-1208">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="286a1-1208">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="286a1-1209">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="286a1-1209">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="286a1-1210">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="286a1-1210">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="286a1-1211">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="286a1-1211">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="286a1-1212">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="286a1-1212">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="286a1-1213">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="286a1-1213">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="286a1-1214">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="286a1-1214">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="286a1-1215">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="286a1-1215">core: Improved performance</span></span>
* <span data-ttu-id="286a1-1216">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="286a1-1216">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="286a1-1217">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="286a1-1217">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="286a1-1218">ACS</span><span class="sxs-lookup"><span data-stu-id="286a1-1218">ACS</span></span>

* <span data-ttu-id="286a1-1219">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="286a1-1219">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="286a1-1220">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="286a1-1220">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="286a1-1221">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="286a1-1221">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="286a1-1222">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="286a1-1222">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-1223">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-1223">AppService</span></span>

* <span data-ttu-id="286a1-1224">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="286a1-1224">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="286a1-1225">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="286a1-1225">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="286a1-1226">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="286a1-1226">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="286a1-1227">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="286a1-1227">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="286a1-1228">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="286a1-1228">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="286a1-1229">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="286a1-1229">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="286a1-1230">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="286a1-1230">support slot swap with preview</span></span>
* <span data-ttu-id="286a1-1231">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="286a1-1231">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="286a1-1232">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="286a1-1232">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="286a1-1233">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="286a1-1233">CosmosDB</span></span>

* <span data-ttu-id="286a1-1234">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="286a1-1234">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="286a1-1235">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="286a1-1235">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="286a1-1236">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="286a1-1236">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="286a1-1237">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="286a1-1237">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="286a1-1238">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="286a1-1238">Data Lake Analytics</span></span>

* <span data-ttu-id="286a1-1239">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="286a1-1239">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="286a1-1240">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="286a1-1240">Add support for new catalog item type: package.</span></span> <span data-ttu-id="286a1-1241">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="286a1-1241">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="286a1-1242">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="286a1-1242">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="286a1-1243">Tabela</span><span class="sxs-lookup"><span data-stu-id="286a1-1243">Table</span></span>
  * <span data-ttu-id="286a1-1244">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="286a1-1244">Table valued function</span></span>
  * <span data-ttu-id="286a1-1245">Visualizar</span><span class="sxs-lookup"><span data-stu-id="286a1-1245">View</span></span>
  * <span data-ttu-id="286a1-1246">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="286a1-1246">Table Statistics.</span></span> <span data-ttu-id="286a1-1247">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="286a1-1247">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="286a1-1248">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="286a1-1248">Data Lake Store</span></span>

* <span data-ttu-id="286a1-1249">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="286a1-1249">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="286a1-1250">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="286a1-1250">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="286a1-1251">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="286a1-1251">missed help for access show.</span></span> <span data-ttu-id="286a1-1252">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="286a1-1252">adding it.</span></span> <span data-ttu-id="286a1-1253">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="286a1-1253">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="286a1-1254">Localizar</span><span class="sxs-lookup"><span data-stu-id="286a1-1254">Find</span></span>

* <span data-ttu-id="286a1-1255">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="286a1-1255">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="286a1-1256">KeyVault</span><span class="sxs-lookup"><span data-stu-id="286a1-1256">KeyVault</span></span>

* <span data-ttu-id="286a1-1257">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="286a1-1257">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="286a1-1258">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="286a1-1258">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="286a1-1259">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="286a1-1259">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="286a1-1260">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="286a1-1260">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="286a1-1261">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="286a1-1261">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="286a1-1262">Laboratório</span><span class="sxs-lookup"><span data-stu-id="286a1-1262">Lab</span></span>

* <span data-ttu-id="286a1-1263">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="286a1-1263">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="286a1-1264">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="286a1-1264">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="286a1-1265">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="286a1-1265">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="286a1-1266">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="286a1-1266">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="286a1-1267">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="286a1-1267">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="286a1-1268">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="286a1-1268">Monitor</span></span>

* <span data-ttu-id="286a1-1269">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="286a1-1269">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="286a1-1270">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="286a1-1270">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="286a1-1271">Rede</span><span class="sxs-lookup"><span data-stu-id="286a1-1271">Network</span></span>

* <span data-ttu-id="286a1-1272">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="286a1-1272">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="286a1-1273">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="286a1-1273">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="286a1-1274">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="286a1-1274">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="286a1-1275">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="286a1-1275">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="286a1-1276">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="286a1-1276">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="286a1-1277">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="286a1-1277">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="286a1-1278">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="286a1-1278">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="286a1-1279">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="286a1-1279">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="286a1-1280">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="286a1-1280">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="286a1-1281">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="286a1-1281">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="286a1-1282">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="286a1-1282">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="286a1-1283">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="286a1-1283">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="286a1-1284">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="286a1-1284">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="286a1-1285">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="286a1-1285">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="286a1-1286">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="286a1-1286">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="286a1-1287">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="286a1-1287">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="286a1-1288">Perfil</span><span class="sxs-lookup"><span data-stu-id="286a1-1288">Profile</span></span>

* <span data-ttu-id="286a1-1289">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="286a1-1289">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="286a1-1290">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="286a1-1290">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="286a1-1291">Redis</span><span class="sxs-lookup"><span data-stu-id="286a1-1291">Redis</span></span>

* <span data-ttu-id="286a1-1292">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="286a1-1292">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="286a1-1293">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="286a1-1293">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="286a1-1294">Recurso</span><span class="sxs-lookup"><span data-stu-id="286a1-1294">Resource</span></span>

* <span data-ttu-id="286a1-1295">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="286a1-1295">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="286a1-1296">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="286a1-1296">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="286a1-1297">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="286a1-1297">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="286a1-1298">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="286a1-1298">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="286a1-1299">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="286a1-1299">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="286a1-1300">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="286a1-1300">Add docs for az lock update.</span></span> <span data-ttu-id="286a1-1301">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="286a1-1301">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="286a1-1302">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="286a1-1302">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="286a1-1303">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="286a1-1303">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="286a1-1304">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="286a1-1304">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="286a1-1305">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="286a1-1305">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="286a1-1306">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="286a1-1306">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="286a1-1307">Função</span><span class="sxs-lookup"><span data-stu-id="286a1-1307">Role</span></span>

* <span data-ttu-id="286a1-1308">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="286a1-1308">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="286a1-1309">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="286a1-1309">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="286a1-1310">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="286a1-1310">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="286a1-1311">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="286a1-1311">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="286a1-1312">SQL</span><span class="sxs-lookup"><span data-stu-id="286a1-1312">SQL</span></span>

* <span data-ttu-id="286a1-1313">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="286a1-1313">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="286a1-1314">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="286a1-1314">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="286a1-1315">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="286a1-1315">Storage</span></span>

* <span data-ttu-id="286a1-1316">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="286a1-1316">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="286a1-1317">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="286a1-1317">Add support for incremental blob copy</span></span>
* <span data-ttu-id="286a1-1318">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="286a1-1318">Add support for large block blob upload</span></span>
* <span data-ttu-id="286a1-1319">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="286a1-1319">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-1320">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-1320">VM</span></span>

* <span data-ttu-id="286a1-1321">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="286a1-1321">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="286a1-1322">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="286a1-1322">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="286a1-1323">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="286a1-1323">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="286a1-1324">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="286a1-1324">az vm/vmss disk</span></span>
  3. <span data-ttu-id="286a1-1325">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="286a1-1325">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="286a1-1326">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="286a1-1326">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="286a1-1327">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="286a1-1327">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="286a1-1328">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="286a1-1328">April 3, 2017</span></span>

<span data-ttu-id="286a1-1329">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="286a1-1329">Version 2.0.2</span></span>

<span data-ttu-id="286a1-1330">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="286a1-1330">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="286a1-1331">Núcleo</span><span class="sxs-lookup"><span data-stu-id="286a1-1331">Core</span></span>

* <span data-ttu-id="286a1-1332">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="286a1-1332">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="286a1-1333">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="286a1-1333">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="286a1-1334">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="286a1-1334">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="286a1-1335">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="286a1-1335">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="286a1-1336">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="286a1-1336">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="286a1-1337">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="286a1-1337">Add prompting for missing template parameters.</span></span> <span data-ttu-id="286a1-1338">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="286a1-1338">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="286a1-1339">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="286a1-1339">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="286a1-1340">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="286a1-1340">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="286a1-1341">ACS</span><span class="sxs-lookup"><span data-stu-id="286a1-1341">ACS</span></span>

* <span data-ttu-id="286a1-1342">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="286a1-1342">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="286a1-1343">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="286a1-1343">Add support for ssh key password prompting.</span></span> <span data-ttu-id="286a1-1344">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="286a1-1344">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="286a1-1345">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="286a1-1345">Add support for windows clusters.</span></span> <span data-ttu-id="286a1-1346">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="286a1-1346">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="286a1-1347">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="286a1-1347">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="286a1-1348">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="286a1-1348">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="286a1-1349">AppService</span><span class="sxs-lookup"><span data-stu-id="286a1-1349">AppService</span></span>

* <span data-ttu-id="286a1-1350">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="286a1-1350">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="286a1-1351">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="286a1-1351">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="286a1-1352">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="286a1-1352">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="286a1-1353">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="286a1-1353">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="286a1-1354">DataLake</span><span class="sxs-lookup"><span data-stu-id="286a1-1354">DataLake</span></span>

* <span data-ttu-id="286a1-1355">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="286a1-1355">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="286a1-1356">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="286a1-1356">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="286a1-1357">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="286a1-1357">DocuemntDB</span></span>

* <span data-ttu-id="286a1-1358">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="286a1-1358">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="286a1-1359">VM</span><span class="sxs-lookup"><span data-stu-id="286a1-1359">VM</span></span>

* <span data-ttu-id="286a1-1360">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="286a1-1360">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="286a1-1361">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="286a1-1361">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="286a1-1362">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="286a1-1362">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="286a1-1363">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="286a1-1363">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="286a1-1364">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="286a1-1364">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="286a1-1365">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="286a1-1365">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="286a1-1366">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="286a1-1366">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="286a1-1367">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="286a1-1367">February 27, 2017</span></span>

<span data-ttu-id="286a1-1368">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="286a1-1368">Version 2.0.0</span></span>

<span data-ttu-id="286a1-1369">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="286a1-1369">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="286a1-1370">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="286a1-1370">Container Service (acs)</span></span>
- <span data-ttu-id="286a1-1371">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="286a1-1371">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="286a1-1372">Rede</span><span class="sxs-lookup"><span data-stu-id="286a1-1372">Networking</span></span>
- <span data-ttu-id="286a1-1373">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="286a1-1373">Storage</span></span>

<span data-ttu-id="286a1-1374">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="286a1-1374">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="286a1-1375">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="286a1-1375">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="286a1-1376">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="286a1-1376">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="286a1-1377">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="286a1-1377">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="286a1-1378">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="286a1-1378">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="286a1-1379">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="286a1-1379">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="286a1-1380">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="286a1-1380">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="286a1-1381">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="286a1-1381">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="286a1-1382">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="286a1-1382">Provide feedback from the command line with the `az feedback` command</span></span>

