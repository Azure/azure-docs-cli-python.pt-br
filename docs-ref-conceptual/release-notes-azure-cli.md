---
title: Notas de versão da CLI do Azure 2.0
description: Saiba mais sobre as últimas atualizações da CLI do Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 07/03/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 8d4f0879a18d2cf99ea7a284155bec86413406f8
ms.sourcegitcommit: da34d0eecf19c676826bd32ab254a92bd0976124
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2018
ms.locfileid: "39138229"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="e8e88-103">Notas de versão da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="e8e88-103">Azure CLI 2.0 release notes</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="e8e88-104">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="e8e88-104">July 18, 2018</span></span>

<span data-ttu-id="e8e88-105">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="e8e88-105">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="e8e88-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e8e88-106">Core</span></span>

* <span data-ttu-id="e8e88-107">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="e8e88-107">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="e8e88-108">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="e8e88-108">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="e8e88-109">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="e8e88-109">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="e8e88-110">ACR</span><span class="sxs-lookup"><span data-stu-id="e8e88-110">ACR</span></span>

* <span data-ttu-id="e8e88-111">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="e8e88-111">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="e8e88-112">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="e8e88-112">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="e8e88-113">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="e8e88-113">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="e8e88-114">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="e8e88-114">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-115">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-115">ACS</span></span>

* <span data-ttu-id="e8e88-116">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="e8e88-116">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-117">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-117">AppService</span></span>

* <span data-ttu-id="e8e88-118">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="e8e88-118">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="e8e88-119">Lote</span><span class="sxs-lookup"><span data-stu-id="e8e88-119">Batch</span></span>

* <span data-ttu-id="e8e88-120">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e8e88-120">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="e8e88-121">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="e8e88-121">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e8e88-122">Lote AI</span><span class="sxs-lookup"><span data-stu-id="e8e88-122">Batch AI</span></span>

* <span data-ttu-id="e8e88-123">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="e8e88-123">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="e8e88-124">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e8e88-124">Container</span></span>

* <span data-ttu-id="e8e88-125">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="e8e88-125">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="e8e88-126">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="e8e88-126">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-127">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-127">Network</span></span>

* <span data-ttu-id="e8e88-128">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-128">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="e8e88-129">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="e8e88-129">Added `network nic wait`</span></span>
* <span data-ttu-id="e8e88-130">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="e8e88-130">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="e8e88-131">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="e8e88-131">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="e8e88-132">Recurso</span><span class="sxs-lookup"><span data-stu-id="e8e88-132">Resource</span></span>

* <span data-ttu-id="e8e88-133">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="e8e88-133">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="e8e88-134">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="e8e88-134">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="e8e88-135">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="e8e88-135">Added `deployment wait` command</span></span>
* <span data-ttu-id="e8e88-136">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="e8e88-136">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="e8e88-137">SQL</span><span class="sxs-lookup"><span data-stu-id="e8e88-137">SQL</span></span>

* <span data-ttu-id="e8e88-138">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-138">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="e8e88-139">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="e8e88-139">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="e8e88-140">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="e8e88-140">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e8e88-141">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-141">Storage</span></span>

* <span data-ttu-id="e8e88-142">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="e8e88-142">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-143">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-143">VM</span></span>

* <span data-ttu-id="e8e88-144">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="e8e88-144">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="e8e88-145">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-145">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="e8e88-146">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="e8e88-146">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="e8e88-147">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="e8e88-147">July 3, 2018</span></span>

<span data-ttu-id="e8e88-148">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="e8e88-148">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="e8e88-149">AKS</span><span class="sxs-lookup"><span data-stu-id="e8e88-149">AKS</span></span>

* <span data-ttu-id="e8e88-150">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="e8e88-150">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="e8e88-151">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="e8e88-151">July 3, 2018</span></span>

<span data-ttu-id="e8e88-152">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="e8e88-152">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="e8e88-153">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e8e88-153">Core</span></span>

* <span data-ttu-id="e8e88-154">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="e8e88-154">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="e8e88-155">ACR</span><span class="sxs-lookup"><span data-stu-id="e8e88-155">ACR</span></span>

* <span data-ttu-id="e8e88-156">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="e8e88-156">Added polling build status</span></span>
* <span data-ttu-id="e8e88-157">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="e8e88-157">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="e8e88-158">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="e8e88-158">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-159">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-159">ACS</span></span>

* <span data-ttu-id="e8e88-160">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="e8e88-160">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="e8e88-161">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="e8e88-161">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="e8e88-162">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-162">Updated options for `aks browse` command.</span></span> <span data-ttu-id="e8e88-163">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="e8e88-163">Added `--listen-port` support</span></span>
* <span data-ttu-id="e8e88-164">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-164">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="e8e88-165">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="e8e88-165">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="e8e88-166">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="e8e88-166">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-167">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-167">AppService</span></span>

* <span data-ttu-id="e8e88-168">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="e8e88-168">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="e8e88-169">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="e8e88-169">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="e8e88-170">Backup</span><span class="sxs-lookup"><span data-stu-id="e8e88-170">Backup</span></span>

* <span data-ttu-id="e8e88-171">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="e8e88-171">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="e8e88-172">BatchAI</span><span class="sxs-lookup"><span data-stu-id="e8e88-172">BatchAI</span></span>

* <span data-ttu-id="e8e88-173">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="e8e88-173">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="e8e88-174">Nuvem</span><span class="sxs-lookup"><span data-stu-id="e8e88-174">Cloud</span></span>

* <span data-ttu-id="e8e88-175">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="e8e88-175">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="e8e88-176">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e8e88-176">Container</span></span>

* <span data-ttu-id="e8e88-177">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="e8e88-177">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="e8e88-178">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="e8e88-178">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="e8e88-179">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="e8e88-179">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="e8e88-180">Extensão</span><span class="sxs-lookup"><span data-stu-id="e8e88-180">Extension</span></span>

* <span data-ttu-id="e8e88-181">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="e8e88-181">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-182">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-182">Network</span></span>

* <span data-ttu-id="e8e88-183">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="e8e88-183">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="e8e88-184">Rdbms</span><span class="sxs-lookup"><span data-stu-id="e8e88-184">Rdbms</span></span>

* <span data-ttu-id="e8e88-185">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="e8e88-185">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="e8e88-186">Recurso</span><span class="sxs-lookup"><span data-stu-id="e8e88-186">Resource</span></span>

* <span data-ttu-id="e8e88-187">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="e8e88-187">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-188">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-188">VM</span></span>

* <span data-ttu-id="e8e88-189">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="e8e88-189">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="e8e88-190">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="e8e88-190">June 25, 2018</span></span>

<span data-ttu-id="e8e88-191">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="e8e88-191">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="e8e88-192">CLI</span><span class="sxs-lookup"><span data-stu-id="e8e88-192">CLI</span></span>

* <span data-ttu-id="e8e88-193">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="e8e88-193">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="e8e88-194">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="e8e88-194">June 19, 2018</span></span>

<span data-ttu-id="e8e88-195">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="e8e88-195">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="e8e88-196">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e8e88-196">Core</span></span>

* <span data-ttu-id="e8e88-197">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="e8e88-197">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="e8e88-198">ACR</span><span class="sxs-lookup"><span data-stu-id="e8e88-198">ACR</span></span>

* <span data-ttu-id="e8e88-199">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="e8e88-199">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="e8e88-200">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="e8e88-200">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-201">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-201">ACS</span></span>

* <span data-ttu-id="e8e88-202">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="e8e88-202">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="e8e88-203">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="e8e88-203">Added `--update` support</span></span>
* <span data-ttu-id="e8e88-204">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="e8e88-204">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="e8e88-205">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="e8e88-205">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="e8e88-206">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="e8e88-206">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="e8e88-207">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="e8e88-207">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="e8e88-208">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="e8e88-208">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="e8e88-209">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="e8e88-209">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-210">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-210">AppService</span></span>

* <span data-ttu-id="e8e88-211">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="e8e88-211">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="e8e88-212">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="e8e88-212">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="e8e88-213">Lote</span><span class="sxs-lookup"><span data-stu-id="e8e88-213">Batch</span></span>

* <span data-ttu-id="e8e88-214">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="e8e88-214">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e8e88-215">Lote AI</span><span class="sxs-lookup"><span data-stu-id="e8e88-215">Batch AI</span></span>

* <span data-ttu-id="e8e88-216">Foi adicionado suporte aos espaços de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e8e88-216">Added support for workspaces.</span></span> <span data-ttu-id="e8e88-217">Os espaços de trabalho permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="e8e88-217">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="e8e88-218">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="e8e88-218">Added support for experiments.</span></span> <span data-ttu-id="e8e88-219">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="e8e88-219">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="e8e88-220">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="e8e88-220">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="e8e88-221">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-221">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="e8e88-222">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="e8e88-222">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="e8e88-223">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="e8e88-223">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="e8e88-224">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos espaços de trabalho</span><span class="sxs-lookup"><span data-stu-id="e8e88-224">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="e8e88-225">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="e8e88-225">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="e8e88-226">[ALTERAÇÃO SIGNIFICATIVA] `--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-226">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="e8e88-227">Para montar um NFS pertencente a outro espaço de trabalho/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="e8e88-227">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="e8e88-228">[ALTERAÇÃO SIGNIFICATIVA] `--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-228">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="e8e88-229">Para enviar um trabalho em um cluster pertencente a outro espaço de trabalho/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="e8e88-229">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="e8e88-230">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="e8e88-230">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="e8e88-231">Agora, o local é um atributo de um espaço de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e8e88-231">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="e8e88-232">[ALTERAÇÃO SIGNIFICATIVA] `--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-232">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="e8e88-233">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="e8e88-233">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="e8e88-234">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="e8e88-234">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="e8e88-235">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="e8e88-235">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="e8e88-236">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="e8e88-236">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="e8e88-237">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="e8e88-237">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="e8e88-238">Mapas</span><span class="sxs-lookup"><span data-stu-id="e8e88-238">Maps</span></span>

* <span data-ttu-id="e8e88-239">[ALTERAÇÃO SIGNIFICATIVA] `maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="e8e88-239">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-240">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-240">Network</span></span>

* <span data-ttu-id="e8e88-241">Foi adicionado suporte a `https` para `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="e8e88-241">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="e8e88-242">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="e8e88-242">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="e8e88-243">#6502</span><span class="sxs-lookup"><span data-stu-id="e8e88-243">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="e8e88-244">Reservas</span><span class="sxs-lookup"><span data-stu-id="e8e88-244">Reservations</span></span>

* <span data-ttu-id="e8e88-245">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="e8e88-245">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="e8e88-246">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="e8e88-246">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="e8e88-247">[ALTERAÇÃO SIGNIFICATIVA] `kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="e8e88-247">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="e8e88-248">[ALTERAÇÃO SIGNIFICATIVA] `capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="e8e88-248">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="e8e88-249">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="e8e88-249">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="e8e88-250">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-250">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="e8e88-251">Função</span><span class="sxs-lookup"><span data-stu-id="e8e88-251">Role</span></span>

* <span data-ttu-id="e8e88-252">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="e8e88-252">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="e8e88-253">SQL</span><span class="sxs-lookup"><span data-stu-id="e8e88-253">SQL</span></span>

* <span data-ttu-id="e8e88-254">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="e8e88-254">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="e8e88-255">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-255">Storage</span></span>

* <span data-ttu-id="e8e88-256">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="e8e88-256">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-257">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-257">VM</span></span>

* <span data-ttu-id="e8e88-258">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-258">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="e8e88-259">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="e8e88-259">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="e8e88-260">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="e8e88-260">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="e8e88-261">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="e8e88-261">June 13, 2018</span></span>

<span data-ttu-id="e8e88-262">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="e8e88-262">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="e8e88-263">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e8e88-263">Core</span></span>

* <span data-ttu-id="e8e88-264">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="e8e88-264">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="e8e88-265">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="e8e88-265">June 13, 2018</span></span>

<span data-ttu-id="e8e88-266">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="e8e88-266">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="e8e88-267">AKS</span><span class="sxs-lookup"><span data-stu-id="e8e88-267">AKS</span></span>

* <span data-ttu-id="e8e88-268">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-268">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="e8e88-269">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="e8e88-269">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="e8e88-270">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-270">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="e8e88-271">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-271">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="e8e88-272">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-272">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-273">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-273">AppService</span></span>

* <span data-ttu-id="e8e88-274">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="e8e88-274">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="e8e88-275">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="e8e88-275">June 5, 2018</span></span>

<span data-ttu-id="e8e88-276">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="e8e88-276">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="e8e88-277">Interativo</span><span class="sxs-lookup"><span data-stu-id="e8e88-277">Interactive</span></span>

* <span data-ttu-id="e8e88-278">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="e8e88-278">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="e8e88-279">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="e8e88-279">June 5, 2018</span></span>

<span data-ttu-id="e8e88-280">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="e8e88-280">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="e8e88-281">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e8e88-281">Core</span></span>

* <span data-ttu-id="e8e88-282">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="e8e88-282">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="e8e88-283">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="e8e88-283">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="e8e88-284">ACR</span><span class="sxs-lookup"><span data-stu-id="e8e88-284">ACR</span></span>

* <span data-ttu-id="e8e88-285">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="e8e88-285">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="e8e88-286">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="e8e88-286">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="e8e88-287">AKS</span><span class="sxs-lookup"><span data-stu-id="e8e88-287">AKS</span></span>

* <span data-ttu-id="e8e88-288">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="e8e88-288">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="e8e88-289">Lote</span><span class="sxs-lookup"><span data-stu-id="e8e88-289">Batch</span></span>

* <span data-ttu-id="e8e88-290">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="e8e88-290">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="e8e88-291">IOT</span><span class="sxs-lookup"><span data-stu-id="e8e88-291">IOT</span></span>

* <span data-ttu-id="e8e88-292">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="e8e88-292">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-293">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-293">Network</span></span>

* <span data-ttu-id="e8e88-294">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="e8e88-294">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="e8e88-295">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="e8e88-295">Policy Insights</span></span>

* <span data-ttu-id="e8e88-296">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="e8e88-296">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="e8e88-297">ARM</span><span class="sxs-lookup"><span data-stu-id="e8e88-297">ARM</span></span>

* <span data-ttu-id="e8e88-298">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="e8e88-298">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="e8e88-299">SQL</span><span class="sxs-lookup"><span data-stu-id="e8e88-299">SQL</span></span>

* <span data-ttu-id="e8e88-300">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="e8e88-300">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="e8e88-301">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="e8e88-301">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="e8e88-302">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-302">Storage</span></span>

* <span data-ttu-id="e8e88-303">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="e8e88-303">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-304">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-304">VM</span></span>

* <span data-ttu-id="e8e88-305">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="e8e88-305">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="e8e88-306">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-306">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="e8e88-307">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-307">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="e8e88-308">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="e8e88-308">May 22, 2018</span></span>

<span data-ttu-id="e8e88-309">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="e8e88-309">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="e8e88-310">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e8e88-310">Core</span></span>

* <span data-ttu-id="e8e88-311">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="e8e88-311">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-312">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-312">ACS</span></span>

* <span data-ttu-id="e8e88-313">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="e8e88-313">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="e8e88-314">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="e8e88-314">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-315">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-315">AppService</span></span>

* <span data-ttu-id="e8e88-316">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="e8e88-316">Improved generic update commands</span></span>
* <span data-ttu-id="e8e88-317">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="e8e88-317">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="e8e88-318">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e8e88-318">Container</span></span>

* <span data-ttu-id="e8e88-319">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="e8e88-319">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="e8e88-320">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="e8e88-320">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="e8e88-321">Extensão</span><span class="sxs-lookup"><span data-stu-id="e8e88-321">Extension</span></span>

* <span data-ttu-id="e8e88-322">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="e8e88-322">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="e8e88-323">Interativo</span><span class="sxs-lookup"><span data-stu-id="e8e88-323">Interactive</span></span>

* <span data-ttu-id="e8e88-324">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="e8e88-324">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="e8e88-325">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="e8e88-325">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="e8e88-326">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e8e88-326">KeyVault</span></span>

* <span data-ttu-id="e8e88-327">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="e8e88-327">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-328">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-328">Network</span></span>

* <span data-ttu-id="e8e88-329">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="e8e88-329">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="e8e88-330">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="e8e88-330">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="e8e88-331">SQL</span><span class="sxs-lookup"><span data-stu-id="e8e88-331">SQL</span></span>

* <span data-ttu-id="e8e88-332">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="e8e88-332">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="e8e88-333">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="e8e88-333">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="e8e88-334">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="e8e88-334">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="e8e88-335">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8e88-335">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="e8e88-336">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="e8e88-336">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="e8e88-337">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-337">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="e8e88-338">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="e8e88-338">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="e8e88-339">`edition`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-339">`edition`.</span></span> <span data-ttu-id="e8e88-340">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="e8e88-340">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="e8e88-341">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-341">`elasticPoolName`.</span></span> <span data-ttu-id="e8e88-342">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="e8e88-342">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="e8e88-343">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="e8e88-343">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="e8e88-344">`edition`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-344">`edition`.</span></span> <span data-ttu-id="e8e88-345">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="e8e88-345">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="e8e88-346">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-346">`dtu`.</span></span> <span data-ttu-id="e8e88-347">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="e8e88-347">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="e8e88-348">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-348">`databaseDtuMin`.</span></span> <span data-ttu-id="e8e88-349">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="e8e88-349">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="e8e88-350">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-350">`databaseDtuMax`.</span></span> <span data-ttu-id="e8e88-351">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="e8e88-351">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="e8e88-352">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-352">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="e8e88-353">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-353">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="e8e88-354">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-354">Storage</span></span>

* <span data-ttu-id="e8e88-355">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="e8e88-355">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="e8e88-356">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="e8e88-356">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-357">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-357">VM</span></span>

* <span data-ttu-id="e8e88-358">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-358">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="e8e88-359">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="e8e88-359">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="e8e88-360">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="e8e88-360">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="e8e88-361">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="e8e88-361">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="e8e88-362">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-362">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="e8e88-363">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="e8e88-363">May 7, 2018</span></span>

<span data-ttu-id="e8e88-364">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="e8e88-364">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="e8e88-365">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e8e88-365">Core</span></span>

* <span data-ttu-id="e8e88-366">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="e8e88-366">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="e8e88-367">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="e8e88-367">Added limited support for positional arguments</span></span>
* <span data-ttu-id="e8e88-368">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-368">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="e8e88-369">#5591</span><span class="sxs-lookup"><span data-stu-id="e8e88-369">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="e8e88-370">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-370">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="e8e88-371">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="e8e88-371">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="e8e88-372">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="e8e88-372">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="e8e88-373">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="e8e88-373">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="e8e88-374">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="e8e88-374">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="e8e88-375">ACR</span><span class="sxs-lookup"><span data-stu-id="e8e88-375">ACR</span></span>

* <span data-ttu-id="e8e88-376">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="e8e88-376">Added ACR Build commands</span></span>
* <span data-ttu-id="e8e88-377">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="e8e88-377">Improved resource not found error messages</span></span>
* <span data-ttu-id="e8e88-378">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="e8e88-378">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="e8e88-379">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="e8e88-379">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="e8e88-380">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="e8e88-380">Improved repository commands error messages</span></span>
* <span data-ttu-id="e8e88-381">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="e8e88-381">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-382">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-382">ACS</span></span>

* <span data-ttu-id="e8e88-383">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="e8e88-383">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="e8e88-384">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="e8e88-384">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="e8e88-385">AMS</span><span class="sxs-lookup"><span data-stu-id="e8e88-385">AMS</span></span>

* <span data-ttu-id="e8e88-386">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="e8e88-386">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-387">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-387">Appservice</span></span>

* <span data-ttu-id="e8e88-388">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="e8e88-388">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="e8e88-389">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-389">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="e8e88-390">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="e8e88-390">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="e8e88-391">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="e8e88-391">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e8e88-392">Lote AI</span><span class="sxs-lookup"><span data-stu-id="e8e88-392">Batch AI</span></span>

* <span data-ttu-id="e8e88-393">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="e8e88-393">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e8e88-394">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="e8e88-394">Cognitive Services</span></span>

* <span data-ttu-id="e8e88-395">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="e8e88-395">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="e8e88-396">Consumo</span><span class="sxs-lookup"><span data-stu-id="e8e88-396">Consumption</span></span>

* <span data-ttu-id="e8e88-397">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-397">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="e8e88-398">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e8e88-398">Container</span></span>

* <span data-ttu-id="e8e88-399">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="e8e88-399">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="e8e88-400">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e8e88-400">Cosmos DB</span></span>

* <span data-ttu-id="e8e88-401">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e8e88-401">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="e8e88-402">DMS</span><span class="sxs-lookup"><span data-stu-id="e8e88-402">DMS</span></span>

* <span data-ttu-id="e8e88-403">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="e8e88-403">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="e8e88-404">Extensão</span><span class="sxs-lookup"><span data-stu-id="e8e88-404">Extension</span></span>

* <span data-ttu-id="e8e88-405">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="e8e88-405">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="e8e88-406">Interativo</span><span class="sxs-lookup"><span data-stu-id="e8e88-406">Interactive</span></span>

* <span data-ttu-id="e8e88-407">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="e8e88-407">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="e8e88-408">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="e8e88-408">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="e8e88-409">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="e8e88-409">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="e8e88-410">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="e8e88-410">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="e8e88-411">Laboratório</span><span class="sxs-lookup"><span data-stu-id="e8e88-411">Lab</span></span>

* <span data-ttu-id="e8e88-412">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="e8e88-412">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-413">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-413">Network</span></span>

* <span data-ttu-id="e8e88-414">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="e8e88-414">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="e8e88-415">Perfil</span><span class="sxs-lookup"><span data-stu-id="e8e88-415">Profile</span></span>

* <span data-ttu-id="e8e88-416">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="e8e88-416">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="e8e88-417">[ALTERAÇÃO SIGNIFICATIVA] `--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="e8e88-417">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="e8e88-418">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="e8e88-418">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="e8e88-419">Redis</span><span class="sxs-lookup"><span data-stu-id="e8e88-419">Redis</span></span>

* <span data-ttu-id="e8e88-420">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="e8e88-420">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="e8e88-421">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="e8e88-421">Deprecated `redis list-all`.</span></span> <span data-ttu-id="e8e88-422">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="e8e88-422">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="e8e88-423">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="e8e88-423">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="e8e88-424">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="e8e88-424">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="e8e88-425">Função</span><span class="sxs-lookup"><span data-stu-id="e8e88-425">Role</span></span>

* <span data-ttu-id="e8e88-426">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="e8e88-426">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="e8e88-427">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-427">Storage</span></span>

* <span data-ttu-id="e8e88-428">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="e8e88-428">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="e8e88-429">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="e8e88-429">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="e8e88-430">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="e8e88-430">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="e8e88-431">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="e8e88-431">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="e8e88-432">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="e8e88-432">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-433">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-433">VM</span></span>

* <span data-ttu-id="e8e88-434">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="e8e88-434">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="e8e88-435">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="e8e88-435">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="e8e88-436">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="e8e88-436">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="e8e88-437">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="e8e88-437">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="e8e88-438">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="e8e88-438">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="e8e88-439">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="e8e88-439">Added write accelerator support</span></span>
* <span data-ttu-id="e8e88-440">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="e8e88-440">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="e8e88-441">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="e8e88-441">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="e8e88-442">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="e8e88-442">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="e8e88-443">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="e8e88-443">April 10, 2018</span></span>

<span data-ttu-id="e8e88-444">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="e8e88-444">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="e8e88-445">ACR</span><span class="sxs-lookup"><span data-stu-id="e8e88-445">ACR</span></span>

* <span data-ttu-id="e8e88-446">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="e8e88-446">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-447">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-447">ACS</span></span>

* <span data-ttu-id="e8e88-448">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="e8e88-448">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-449">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-449">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="e8e88-451">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="e8e88-451">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="e8e88-452">BatchAI</span><span class="sxs-lookup"><span data-stu-id="e8e88-452">BatchAI</span></span>

* <span data-ttu-id="e8e88-453">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="e8e88-453">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="e8e88-454">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="e8e88-454">Job level mounting</span></span>
 - <span data-ttu-id="e8e88-455">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="e8e88-455">Environment variables with secret values</span></span>
 - <span data-ttu-id="e8e88-456">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="e8e88-456">Performance counters settings</span></span>
 - <span data-ttu-id="e8e88-457">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="e8e88-457">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="e8e88-458">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="e8e88-458">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="e8e88-459">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="e8e88-459">Usage and limits reporting</span></span>
 - <span data-ttu-id="e8e88-460">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="e8e88-460">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="e8e88-461">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="e8e88-461">Support for custom images</span></span>
 - <span data-ttu-id="e8e88-462">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="e8e88-462">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="e8e88-463">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="e8e88-463">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="e8e88-464">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="e8e88-464">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="e8e88-465">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="e8e88-465">National clouds are supported</span></span>
* <span data-ttu-id="e8e88-466">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="e8e88-466">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="e8e88-467">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="e8e88-467">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="e8e88-468">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="e8e88-468">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="e8e88-469">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="e8e88-469">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="e8e88-470">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="e8e88-470">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="e8e88-471">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="e8e88-471">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="e8e88-472">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="e8e88-472">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="e8e88-473">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="e8e88-473">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="e8e88-474">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="e8e88-474">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="e8e88-475">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-475">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="e8e88-476">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="e8e88-476">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="e8e88-477">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="e8e88-477">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="e8e88-478">[ALTERAÇÃO SIGNIFICATIVA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-478">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="e8e88-479">Cobrança</span><span class="sxs-lookup"><span data-stu-id="e8e88-479">Billing</span></span>

* <span data-ttu-id="e8e88-480">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="e8e88-480">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="e8e88-481">Consumo</span><span class="sxs-lookup"><span data-stu-id="e8e88-481">Consumption</span></span>

* <span data-ttu-id="e8e88-482">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="e8e88-482">Added `marketplace` commands</span></span>
* <span data-ttu-id="e8e88-483">[ALTERAÇÃO SIGNIFICATIVA] `reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="e8e88-483">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="e8e88-484">[ALTERAÇÃO SIGNIFICATIVA] `reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="e8e88-484">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="e8e88-485">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="e8e88-485">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="e8e88-486">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="e8e88-486">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="e8e88-487">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="e8e88-487">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="e8e88-488">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e8e88-488">Container</span></span>

* <span data-ttu-id="e8e88-489">Adição dos parâmetros de montagem de volume de repositório git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="e8e88-489">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="e8e88-490">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="e8e88-490">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="e8e88-491">Extensão</span><span class="sxs-lookup"><span data-stu-id="e8e88-491">Extension</span></span>

* <span data-ttu-id="e8e88-492">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="e8e88-492">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="e8e88-493">Interativo</span><span class="sxs-lookup"><span data-stu-id="e8e88-493">Interactive</span></span>

* <span data-ttu-id="e8e88-494">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="e8e88-494">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="e8e88-495">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="e8e88-495">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="e8e88-496">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="e8e88-496">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-497">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-497">Network</span></span>

* <span data-ttu-id="e8e88-498">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="e8e88-498">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="e8e88-499">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-499">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="e8e88-500">#4910</span><span class="sxs-lookup"><span data-stu-id="e8e88-500">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="e8e88-501">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="e8e88-501">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="e8e88-502">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="e8e88-502">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="e8e88-503">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-503">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="e8e88-504">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-504">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="e8e88-505">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="e8e88-505">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="e8e88-506">Perfil</span><span class="sxs-lookup"><span data-stu-id="e8e88-506">Profile</span></span>

* <span data-ttu-id="e8e88-507">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="e8e88-507">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="e8e88-508">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="e8e88-508">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="e8e88-509">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e8e88-509">RDBMS</span></span>

* <span data-ttu-id="e8e88-510">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="e8e88-510">Added `georestore` command</span></span>
* <span data-ttu-id="e8e88-511">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-511">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="e8e88-512">Recurso</span><span class="sxs-lookup"><span data-stu-id="e8e88-512">Resource</span></span>

* <span data-ttu-id="e8e88-513">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-513">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="e8e88-514">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-514">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="e8e88-515">SQL</span><span class="sxs-lookup"><span data-stu-id="e8e88-515">SQL</span></span>

* <span data-ttu-id="e8e88-516">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="e8e88-516">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="e8e88-517">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-517">Storage</span></span>

* <span data-ttu-id="e8e88-518">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="e8e88-518">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-519">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-519">VM</span></span>

* <span data-ttu-id="e8e88-520">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-520">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="e8e88-521">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-521">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="e8e88-523">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-523">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="e8e88-524">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="e8e88-524">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="e8e88-525">#5718</span><span class="sxs-lookup"><span data-stu-id="e8e88-525">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="e8e88-526">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="e8e88-526">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="e8e88-527">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="e8e88-527">March 27, 2018</span></span>

<span data-ttu-id="e8e88-528">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="e8e88-528">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="e8e88-529">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e8e88-529">Core</span></span>

* <span data-ttu-id="e8e88-530">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="e8e88-530">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-531">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-531">ACS</span></span>

* <span data-ttu-id="e8e88-532">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e8e88-532">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-533">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-533">Appservice</span></span>

* <span data-ttu-id="e8e88-534">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-534">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="e8e88-535">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-535">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="e8e88-536">Backup</span><span class="sxs-lookup"><span data-stu-id="e8e88-536">Backup</span></span>

* <span data-ttu-id="e8e88-537">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-537">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="e8e88-538">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="e8e88-538">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="e8e88-539">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="e8e88-539">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="e8e88-540">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="e8e88-540">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="e8e88-541">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e8e88-541">Container</span></span>

* <span data-ttu-id="e8e88-542">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-542">Added `container exec` command.</span></span> <span data-ttu-id="e8e88-543">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="e8e88-543">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="e8e88-544">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="e8e88-544">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="e8e88-545">Extensão</span><span class="sxs-lookup"><span data-stu-id="e8e88-545">Extension</span></span>

* <span data-ttu-id="e8e88-546">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="e8e88-546">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="e8e88-547">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="e8e88-547">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="e8e88-548">[ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="e8e88-548">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="e8e88-549">Interativo</span><span class="sxs-lookup"><span data-stu-id="e8e88-549">Interactive</span></span>

* <span data-ttu-id="e8e88-550">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="e8e88-550">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="e8e88-551">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="e8e88-551">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="e8e88-552">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="e8e88-552">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="e8e88-553">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="e8e88-553">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="e8e88-554">Laboratório</span><span class="sxs-lookup"><span data-stu-id="e8e88-554">Lab</span></span>

* <span data-ttu-id="e8e88-555">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="e8e88-555">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="e8e88-556">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e8e88-556">Monitor</span></span>

* <span data-ttu-id="e8e88-557">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="e8e88-557">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="e8e88-558">[#4529](https://github.com/Azure/azure-cli/issues/5785) corrigido: `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="e8e88-558">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="e8e88-559">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="e8e88-559">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-560">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-560">Network</span></span>

* <span data-ttu-id="e8e88-561">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="e8e88-561">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="e8e88-562">Perfil</span><span class="sxs-lookup"><span data-stu-id="e8e88-562">Profile</span></span>

* <span data-ttu-id="e8e88-563">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="e8e88-563">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e8e88-564">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e8e88-564">RDBMS</span></span>

* <span data-ttu-id="e8e88-565">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="e8e88-565">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="e8e88-566">Recurso</span><span class="sxs-lookup"><span data-stu-id="e8e88-566">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="e8e88-568">Função</span><span class="sxs-lookup"><span data-stu-id="e8e88-568">Role</span></span>

* <span data-ttu-id="e8e88-569">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-569">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="e8e88-570">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="e8e88-570">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="e8e88-571">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-571">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="e8e88-572">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-572">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="e8e88-573">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="e8e88-573">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="e8e88-574">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-574">Storage</span></span>

* <span data-ttu-id="e8e88-575">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="e8e88-575">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="e8e88-576">[4049#](https://github.com/Azure/azure-cli/issues/4049) corrigido: problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="e8e88-576">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-577">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-577">VM</span></span>

* <span data-ttu-id="e8e88-578">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="e8e88-578">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="e8e88-579">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-579">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="e8e88-580">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="e8e88-580">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="e8e88-581">[ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="e8e88-581">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="e8e88-582">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="e8e88-582">March 13, 2018</span></span>

<span data-ttu-id="e8e88-583">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="e8e88-583">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="e8e88-584">ACR</span><span class="sxs-lookup"><span data-stu-id="e8e88-584">ACR</span></span>

* <span data-ttu-id="e8e88-585">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="e8e88-585">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="e8e88-586">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="e8e88-586">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="e8e88-587">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="e8e88-587">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-588">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-588">ACS</span></span>

* <span data-ttu-id="e8e88-589">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="e8e88-589">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="e8e88-590">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="e8e88-590">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="e8e88-591">Supervisor</span><span class="sxs-lookup"><span data-stu-id="e8e88-591">Advisor</span></span>

* <span data-ttu-id="e8e88-592">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="e8e88-592">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="e8e88-593">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-593">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="e8e88-594">[ALTERAÇÃO SIGNIFICATIVA] `advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="e8e88-594">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="e8e88-595">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="e8e88-595">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="e8e88-596">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="e8e88-596">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-597">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-597">Appservice</span></span>

* <span data-ttu-id="e8e88-598">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="e8e88-598">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="e8e88-599">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="e8e88-599">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="e8e88-600">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="e8e88-600">Eventhubs</span></span>

* <span data-ttu-id="e8e88-601">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e8e88-601">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="e8e88-602">Extensão</span><span class="sxs-lookup"><span data-stu-id="e8e88-602">Extension</span></span>

* <span data-ttu-id="e8e88-603">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="e8e88-603">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="e8e88-604">Interativo</span><span class="sxs-lookup"><span data-stu-id="e8e88-604">Interactive</span></span>

* <span data-ttu-id="e8e88-605">[5625](https://github.com/Azure/azure-cli/issues/5625) corrigido: manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="e8e88-605">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="e8e88-606">[3016](https://github.com/Azure/azure-cli/issues/3016) corrigido: histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="e8e88-606">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="e8e88-607">[5688](https://github.com/Azure/azure-cli/issues/5688) corrigido: as conclusões não aparecerão se o carregamento da tabela de comando encontrou uma exceção</span><span class="sxs-lookup"><span data-stu-id="e8e88-607">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="e8e88-608">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="e8e88-608">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="e8e88-609">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e8e88-609">Monitor</span></span>

* <span data-ttu-id="e8e88-610">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="e8e88-610">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="e8e88-611">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="e8e88-611">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="e8e88-612">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="e8e88-612">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="e8e88-613">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="e8e88-613">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-614">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-614">Network</span></span>

* <span data-ttu-id="e8e88-615">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-615">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="e8e88-616">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="e8e88-616">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="e8e88-617">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="e8e88-617">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="e8e88-618">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="e8e88-618">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="e8e88-619">Perfil</span><span class="sxs-lookup"><span data-stu-id="e8e88-619">Profile</span></span>

* <span data-ttu-id="e8e88-620">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="e8e88-620">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="e8e88-621">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="e8e88-621">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e8e88-622">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e8e88-622">RDBMS</span></span>

* <span data-ttu-id="e8e88-623">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="e8e88-623">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="e8e88-624">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="e8e88-624">Service Bus</span></span>

* <span data-ttu-id="e8e88-625">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e8e88-625">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="e8e88-626">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-626">Storage</span></span>

* <span data-ttu-id="e8e88-627">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="e8e88-627">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="e8e88-628">[5286](https://github.com/Azure/azure-cli/issues/5286) corrigido: os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="e8e88-628">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-629">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-629">VM</span></span>

* <span data-ttu-id="e8e88-630">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="e8e88-630">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="e8e88-631">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="e8e88-631">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="e8e88-632">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="e8e88-632">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="e8e88-633">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="e8e88-633">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="e8e88-634">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="e8e88-634">February 27, 2018</span></span>

<span data-ttu-id="e8e88-635">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="e8e88-635">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="e8e88-636">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e8e88-636">Core</span></span>

* <span data-ttu-id="e8e88-637">Correção [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="e8e88-637">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="e8e88-638">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="e8e88-638">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="e8e88-639">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="e8e88-639">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-640">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-640">ACS</span></span>

* <span data-ttu-id="e8e88-641">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="e8e88-641">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="e8e88-642">Correção do problema de permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="e8e88-642">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="e8e88-643">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="e8e88-643">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="e8e88-644">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="e8e88-644">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-645">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-645">Appservice</span></span>

* <span data-ttu-id="e8e88-646">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="e8e88-646">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="e8e88-647">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="e8e88-647">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e8e88-648">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="e8e88-648">Cognitive Services</span></span>

* <span data-ttu-id="e8e88-649">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="e8e88-649">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="e8e88-650">Consumo</span><span class="sxs-lookup"><span data-stu-id="e8e88-650">Consumption</span></span>

* <span data-ttu-id="e8e88-651">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="e8e88-651">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="e8e88-652">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="e8e88-652">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="e8e88-653">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e8e88-653">Container</span></span>

* <span data-ttu-id="e8e88-654">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="e8e88-654">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-655">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-655">Network</span></span>

* <span data-ttu-id="e8e88-656">Correção [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="e8e88-656">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="e8e88-657">Recurso</span><span class="sxs-lookup"><span data-stu-id="e8e88-657">Resource</span></span>

* <span data-ttu-id="e8e88-658">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="e8e88-658">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="e8e88-659">Função</span><span class="sxs-lookup"><span data-stu-id="e8e88-659">Role</span></span>

* <span data-ttu-id="e8e88-660">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="e8e88-660">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="e8e88-661">SQL</span><span class="sxs-lookup"><span data-stu-id="e8e88-661">SQL</span></span>

* <span data-ttu-id="e8e88-662">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="e8e88-662">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="e8e88-663">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-663">Storage</span></span>

* <span data-ttu-id="e8e88-664">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-664">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-665">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-665">VM</span></span>

* <span data-ttu-id="e8e88-666">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="e8e88-666">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="e8e88-667">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="e8e88-667">February 13, 2018</span></span>

<span data-ttu-id="e8e88-668">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="e8e88-668">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="e8e88-669">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e8e88-669">Core</span></span>

* <span data-ttu-id="e8e88-670">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="e8e88-670">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-671">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-671">ACS</span></span>

* <span data-ttu-id="e8e88-672">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="e8e88-672">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="e8e88-673">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-673">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="e8e88-674">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="e8e88-674">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="e8e88-675">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="e8e88-675">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="e8e88-676">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="e8e88-676">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="e8e88-677">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="e8e88-677">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="e8e88-678">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="e8e88-678">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="e8e88-679">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="e8e88-679">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-680">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-680">Appservice</span></span>

* <span data-ttu-id="e8e88-681">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="e8e88-681">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="e8e88-682">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="e8e88-682">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="e8e88-683">CDN</span><span class="sxs-lookup"><span data-stu-id="e8e88-683">CDN</span></span>

* <span data-ttu-id="e8e88-684">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-684">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="e8e88-685">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e8e88-685">Container</span></span>

* <span data-ttu-id="e8e88-686">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="e8e88-686">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="e8e88-687">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="e8e88-687">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e8e88-688">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e8e88-688">CosmosDB</span></span>

* <span data-ttu-id="e8e88-689">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="e8e88-689">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="e8e88-690">Extensão</span><span class="sxs-lookup"><span data-stu-id="e8e88-690">Extension</span></span>

* <span data-ttu-id="e8e88-691">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-691">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="e8e88-692">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-692">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="e8e88-693">Comentários</span><span class="sxs-lookup"><span data-stu-id="e8e88-693">Feedback</span></span>

* <span data-ttu-id="e8e88-694">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="e8e88-694">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="e8e88-695">Interativo</span><span class="sxs-lookup"><span data-stu-id="e8e88-695">Interactive</span></span>

* <span data-ttu-id="e8e88-696">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e8e88-696">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="e8e88-697">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="e8e88-697">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="e8e88-698">IoT</span><span class="sxs-lookup"><span data-stu-id="e8e88-698">IoT</span></span>

* <span data-ttu-id="e8e88-699">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="e8e88-699">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="e8e88-700">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="e8e88-700">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="e8e88-701">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-701">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="e8e88-702">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="e8e88-702">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="e8e88-703">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e8e88-703">Monitor</span></span>

* <span data-ttu-id="e8e88-704">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-704">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-705">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-705">Network</span></span>

* <span data-ttu-id="e8e88-706">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="e8e88-706">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="e8e88-707">Perfil</span><span class="sxs-lookup"><span data-stu-id="e8e88-707">Profile</span></span>

* <span data-ttu-id="e8e88-708">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="e8e88-708">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="e8e88-709">Recurso</span><span class="sxs-lookup"><span data-stu-id="e8e88-709">Resource</span></span>

* <span data-ttu-id="e8e88-710">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="e8e88-710">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="e8e88-711">Função</span><span class="sxs-lookup"><span data-stu-id="e8e88-711">Role</span></span>

* <span data-ttu-id="e8e88-712">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-712">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="e8e88-713">SQL</span><span class="sxs-lookup"><span data-stu-id="e8e88-713">SQL</span></span>

* <span data-ttu-id="e8e88-714">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="e8e88-714">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="e8e88-715">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="e8e88-715">Added `sql db rename`</span></span>
* <span data-ttu-id="e8e88-716">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="e8e88-716">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="e8e88-717">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-717">Storage</span></span>

* <span data-ttu-id="e8e88-718">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="e8e88-718">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-719">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-719">VM</span></span>

* <span data-ttu-id="e8e88-720">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="e8e88-720">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="e8e88-721">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="e8e88-721">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="e8e88-722">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="e8e88-722">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="e8e88-723">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="e8e88-723">January 31, 2018</span></span>

<span data-ttu-id="e8e88-724">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="e8e88-724">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="e8e88-725">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e8e88-725">Core</span></span>

* <span data-ttu-id="e8e88-726">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="e8e88-726">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="e8e88-727">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="e8e88-727">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="e8e88-728">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="e8e88-728">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="e8e88-729">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="e8e88-729">Use `--verbose` to see</span></span>
* <span data-ttu-id="e8e88-730">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="e8e88-730">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-731">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-731">ACS</span></span>

* <span data-ttu-id="e8e88-732">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="e8e88-732">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="e8e88-733">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="e8e88-733">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-734">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-734">Appservice</span></span>

* <span data-ttu-id="e8e88-735">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="e8e88-735">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="e8e88-736">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="e8e88-736">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="e8e88-737">CDN</span><span class="sxs-lookup"><span data-stu-id="e8e88-737">CDN</span></span>

* <span data-ttu-id="e8e88-738">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-738">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e8e88-739">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e8e88-739">CosmosDB</span></span>

* <span data-ttu-id="e8e88-740">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="e8e88-740">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="e8e88-741">Interativo</span><span class="sxs-lookup"><span data-stu-id="e8e88-741">Interactive</span></span>

* <span data-ttu-id="e8e88-742">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="e8e88-742">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-743">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-743">Network</span></span>

* <span data-ttu-id="e8e88-744">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-744">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="e8e88-745">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="e8e88-745">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="e8e88-746">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-746">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="e8e88-747">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-747">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="e8e88-748">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="e8e88-748">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="e8e88-749">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="e8e88-749">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="e8e88-750">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="e8e88-750">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="e8e88-751">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="e8e88-751">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="e8e88-752">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="e8e88-752">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="e8e88-753">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="e8e88-753">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="e8e88-754">Perfil</span><span class="sxs-lookup"><span data-stu-id="e8e88-754">Profile</span></span>

* <span data-ttu-id="e8e88-755">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="e8e88-755">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="e8e88-756">Recurso</span><span class="sxs-lookup"><span data-stu-id="e8e88-756">Resource</span></span>

* <span data-ttu-id="e8e88-757">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="e8e88-757">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="e8e88-758">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-758">Storage</span></span>

* <span data-ttu-id="e8e88-759">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="e8e88-759">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="e8e88-760">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="e8e88-760">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="e8e88-761">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="e8e88-761">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="e8e88-762">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-762">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="e8e88-763">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="e8e88-763">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-764">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-764">VM</span></span>

* <span data-ttu-id="e8e88-765">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="e8e88-765">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="e8e88-766">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="e8e88-766">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="e8e88-767">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="e8e88-767">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="e8e88-768">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-768">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="e8e88-769">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="e8e88-769">January 17, 2018</span></span>

<span data-ttu-id="e8e88-770">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="e8e88-770">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="e8e88-771">ACR</span><span class="sxs-lookup"><span data-stu-id="e8e88-771">ACR</span></span>

* <span data-ttu-id="e8e88-772">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="e8e88-772">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="e8e88-773">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="e8e88-773">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-774">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-774">ACS</span></span>

* <span data-ttu-id="e8e88-775">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="e8e88-775">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="e8e88-776">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="e8e88-776">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-777">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-777">Appservice</span></span>

* <span data-ttu-id="e8e88-778">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="e8e88-778">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="e8e88-779">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="e8e88-779">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="e8e88-780">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="e8e88-780">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="e8e88-781">Backup</span><span class="sxs-lookup"><span data-stu-id="e8e88-781">Backup</span></span>

* <span data-ttu-id="e8e88-782">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="e8e88-782">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="e8e88-783">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="e8e88-783">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="e8e88-784">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="e8e88-784">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="e8e88-785">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="e8e88-785">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="e8e88-786">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="e8e88-786">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="e8e88-787">Lote</span><span class="sxs-lookup"><span data-stu-id="e8e88-787">Batch</span></span>

* <span data-ttu-id="e8e88-788">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="e8e88-788">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="e8e88-789">Nuvem</span><span class="sxs-lookup"><span data-stu-id="e8e88-789">Cloud</span></span>

* <span data-ttu-id="e8e88-790">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="e8e88-790">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="e8e88-791">Consumo</span><span class="sxs-lookup"><span data-stu-id="e8e88-791">Consumption</span></span>

* <span data-ttu-id="e8e88-792">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="e8e88-792">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="e8e88-793">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="e8e88-793">Event Grid</span></span>

* <span data-ttu-id="e8e88-794">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="e8e88-794">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="e8e88-795">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="e8e88-795">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="e8e88-796">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="e8e88-796">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="e8e88-797">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="e8e88-797">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="e8e88-798">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-798">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="e8e88-799">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-799">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="e8e88-800">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="e8e88-800">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="e8e88-801">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="e8e88-801">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="e8e88-802">Interativo</span><span class="sxs-lookup"><span data-stu-id="e8e88-802">Interactive</span></span>

* <span data-ttu-id="e8e88-803">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="e8e88-803">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="e8e88-804">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="e8e88-804">Fixed errors on startup</span></span>
* <span data-ttu-id="e8e88-805">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="e8e88-805">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="e8e88-806">IoT</span><span class="sxs-lookup"><span data-stu-id="e8e88-806">IoT</span></span>

* <span data-ttu-id="e8e88-807">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="e8e88-807">Added support for device provisioning service</span></span>
* <span data-ttu-id="e8e88-808">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="e8e88-808">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="e8e88-809">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="e8e88-809">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="e8e88-810">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e8e88-810">Monitor</span></span>

* <span data-ttu-id="e8e88-811">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="e8e88-811">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="e8e88-812">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-812">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="e8e88-813">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="e8e88-813">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-814">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-814">Network</span></span>

* <span data-ttu-id="e8e88-815">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-815">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="e8e88-816">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-816">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="e8e88-817">Perfil</span><span class="sxs-lookup"><span data-stu-id="e8e88-817">Profile</span></span>

* <span data-ttu-id="e8e88-818">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="e8e88-818">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="e8e88-819">Função</span><span class="sxs-lookup"><span data-stu-id="e8e88-819">Role</span></span>

* <span data-ttu-id="e8e88-820">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="e8e88-820">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e8e88-821">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e8e88-821">Service Fabric</span></span>

* <span data-ttu-id="e8e88-822">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="e8e88-822">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="e8e88-823">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="e8e88-823">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-824">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-824">VM</span></span>

* <span data-ttu-id="e8e88-825">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="e8e88-825">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="e8e88-826">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="e8e88-826">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="e8e88-827">[ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="e8e88-827">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="e8e88-828">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="e8e88-828">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="e8e88-829">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="e8e88-829">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="e8e88-830">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-830">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="e8e88-831">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-831">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="e8e88-832">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="e8e88-832">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="e8e88-833">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="e8e88-833">December 19, 2017</span></span>

<span data-ttu-id="e8e88-834">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="e8e88-834">Version 2.0.23</span></span>

* <span data-ttu-id="e8e88-835">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="e8e88-835">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="e8e88-836">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e8e88-836">Container</span></span>

* <span data-ttu-id="e8e88-837">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="e8e88-837">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-838">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-838">Network</span></span>

* <span data-ttu-id="e8e88-839">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-839">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="e8e88-840">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-840">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="e8e88-841">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-841">Storage</span></span>

* <span data-ttu-id="e8e88-842">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="e8e88-842">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-843">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-843">VM</span></span>

* <span data-ttu-id="e8e88-844">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="e8e88-844">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="e8e88-845">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="e8e88-845">December 5, 2017</span></span>

<span data-ttu-id="e8e88-846">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="e8e88-846">Version 2.0.22</span></span>

* <span data-ttu-id="e8e88-847">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="e8e88-847">Removed `az component` commands.</span></span> <span data-ttu-id="e8e88-848">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="e8e88-848">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="e8e88-849">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e8e88-849">Core</span></span>
* <span data-ttu-id="e8e88-850">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="e8e88-850">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="e8e88-851">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="e8e88-851">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-852">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-852">ACS</span></span>

* <span data-ttu-id="e8e88-853">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="e8e88-853">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="e8e88-854">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-854">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="e8e88-855">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="e8e88-855">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="e8e88-856">Supervisor</span><span class="sxs-lookup"><span data-stu-id="e8e88-856">Advisor</span></span>

* <span data-ttu-id="e8e88-857">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e8e88-857">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-858">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-858">Appservice</span></span>

* <span data-ttu-id="e8e88-859">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="e8e88-859">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="e8e88-860">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="e8e88-860">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="e8e88-861">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="e8e88-861">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="e8e88-862">Consumo</span><span class="sxs-lookup"><span data-stu-id="e8e88-862">Consumption</span></span>

* <span data-ttu-id="e8e88-863">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="e8e88-863">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="e8e88-864">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e8e88-864">Container</span></span>

* <span data-ttu-id="e8e88-865">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="e8e88-865">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="e8e88-866">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e8e88-866">Monitor</span></span>

* <span data-ttu-id="e8e88-867">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="e8e88-867">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="e8e88-868">Recurso</span><span class="sxs-lookup"><span data-stu-id="e8e88-868">Resource</span></span>

* <span data-ttu-id="e8e88-869">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="e8e88-869">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="e8e88-870">Função</span><span class="sxs-lookup"><span data-stu-id="e8e88-870">Role</span></span>

* <span data-ttu-id="e8e88-871">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="e8e88-871">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="e8e88-872">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="e8e88-872">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="e8e88-873">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="e8e88-873">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="e8e88-874">SQL</span><span class="sxs-lookup"><span data-stu-id="e8e88-874">SQL</span></span>

* <span data-ttu-id="e8e88-875">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="e8e88-875">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="e8e88-876">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="e8e88-876">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-877">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-877">VM</span></span>

* <span data-ttu-id="e8e88-878">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="e8e88-878">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="e8e88-879">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="e8e88-879">November 14, 2017</span></span>

<span data-ttu-id="e8e88-880">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="e8e88-880">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="e8e88-881">ACR</span><span class="sxs-lookup"><span data-stu-id="e8e88-881">ACR</span></span>

* <span data-ttu-id="e8e88-882">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="e8e88-882">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="e8e88-883">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-883">ACS</span></span>

* <span data-ttu-id="e8e88-884">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="e8e88-884">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="e8e88-885">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-885">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="e8e88-886">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="e8e88-886">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="e8e88-887">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="e8e88-887">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="e8e88-888">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="e8e88-888">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-889">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-889">Appservice</span></span>

* <span data-ttu-id="e8e88-890">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="e8e88-890">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="e8e88-891">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="e8e88-891">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="e8e88-892">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="e8e88-892">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="e8e88-893">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="e8e88-893">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="e8e88-894">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="e8e88-894">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="e8e88-895">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="e8e88-895">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="e8e88-896">Lote</span><span class="sxs-lookup"><span data-stu-id="e8e88-896">Batch</span></span>

* <span data-ttu-id="e8e88-897">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="e8e88-897">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="e8e88-898">Batchai</span><span class="sxs-lookup"><span data-stu-id="e8e88-898">Batchai</span></span>

* <span data-ttu-id="e8e88-899">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-899">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="e8e88-900">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-900">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="e8e88-901">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="e8e88-901">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="e8e88-902">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-902">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="e8e88-903">Nuvem</span><span class="sxs-lookup"><span data-stu-id="e8e88-903">Cloud</span></span>

* <span data-ttu-id="e8e88-904">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="e8e88-904">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="e8e88-905">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e8e88-905">Container</span></span>

* <span data-ttu-id="e8e88-906">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="e8e88-906">Added support to open multiple ports</span></span>
* <span data-ttu-id="e8e88-907">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="e8e88-907">Added container group restart policy</span></span>
* <span data-ttu-id="e8e88-908">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="e8e88-908">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="e8e88-909">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="e8e88-909">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e8e88-910">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e8e88-910">Data Lake Analytics</span></span>

* <span data-ttu-id="e8e88-911">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="e8e88-911">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e8e88-912">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e8e88-912">Data Lake Store</span></span>

* <span data-ttu-id="e8e88-913">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="e8e88-913">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="e8e88-914">Extensão</span><span class="sxs-lookup"><span data-stu-id="e8e88-914">Extension</span></span>

* <span data-ttu-id="e8e88-915">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="e8e88-915">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="e8e88-916">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="e8e88-916">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="e8e88-917">IoT</span><span class="sxs-lookup"><span data-stu-id="e8e88-917">IoT</span></span>

* <span data-ttu-id="e8e88-918">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="e8e88-918">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="e8e88-919">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e8e88-919">Monitor</span></span>

* <span data-ttu-id="e8e88-920">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="e8e88-920">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-921">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-921">Network</span></span>

* <span data-ttu-id="e8e88-922">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="e8e88-922">Added support for CAA DNS records</span></span>
* <span data-ttu-id="e8e88-923">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-923">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="e8e88-924">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="e8e88-924">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="e8e88-925">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="e8e88-925">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="e8e88-926">Reservas</span><span class="sxs-lookup"><span data-stu-id="e8e88-926">Reservations</span></span>

* <span data-ttu-id="e8e88-927">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="e8e88-927">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="e8e88-928">Recurso</span><span class="sxs-lookup"><span data-stu-id="e8e88-928">Resource</span></span>

* <span data-ttu-id="e8e88-929">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="e8e88-929">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="e8e88-930">SQL</span><span class="sxs-lookup"><span data-stu-id="e8e88-930">SQL</span></span>

* <span data-ttu-id="e8e88-931">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-931">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="e8e88-932">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-932">Storage</span></span>

* <span data-ttu-id="e8e88-933">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="e8e88-933">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="e8e88-934">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="e8e88-934">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="e8e88-935">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="e8e88-935">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="e8e88-936">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="e8e88-936">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="e8e88-937">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-937">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="e8e88-938">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="e8e88-938">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="e8e88-939">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-939">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-940">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-940">VM</span></span>

* <span data-ttu-id="e8e88-941">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="e8e88-941">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="e8e88-942">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="e8e88-942">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="e8e88-943">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="e8e88-943">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="e8e88-944">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="e8e88-944">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="e8e88-945">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="e8e88-945">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="e8e88-946">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="e8e88-946">October 24, 2017</span></span>

<span data-ttu-id="e8e88-947">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="e8e88-947">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="e8e88-948">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e8e88-948">Core</span></span>

* <span data-ttu-id="e8e88-949">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="e8e88-949">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="e8e88-950">ACR</span><span class="sxs-lookup"><span data-stu-id="e8e88-950">ACR</span></span>

* <span data-ttu-id="e8e88-951">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="e8e88-951">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="e8e88-952">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="e8e88-952">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="e8e88-953">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="e8e88-953">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-954">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-954">ACS</span></span>

* <span data-ttu-id="e8e88-955">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="e8e88-955">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="e8e88-956">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="e8e88-956">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-957">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-957">Appservice</span></span>

* <span data-ttu-id="e8e88-958">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="e8e88-958">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="e8e88-959">Componente</span><span class="sxs-lookup"><span data-stu-id="e8e88-959">Component</span></span>

* <span data-ttu-id="e8e88-960">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="e8e88-960">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="e8e88-961">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e8e88-961">Monitor</span></span>

* <span data-ttu-id="e8e88-962">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="e8e88-962">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="e8e88-963">Recurso</span><span class="sxs-lookup"><span data-stu-id="e8e88-963">Resource</span></span>

* <span data-ttu-id="e8e88-964">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="e8e88-964">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="e8e88-965">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="e8e88-965">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-966">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-966">VM</span></span>

* <span data-ttu-id="e8e88-967">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-967">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="e8e88-968">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="e8e88-968">October 9, 2017</span></span>

<span data-ttu-id="e8e88-969">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="e8e88-969">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="e8e88-970">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e8e88-970">Core</span></span>

* <span data-ttu-id="e8e88-971">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="e8e88-971">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-972">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-972">Appservice</span></span>

* <span data-ttu-id="e8e88-973">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-973">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="e8e88-974">Lote</span><span class="sxs-lookup"><span data-stu-id="e8e88-974">Batch</span></span>

* <span data-ttu-id="e8e88-975">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="e8e88-975">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="e8e88-976">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="e8e88-976">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="e8e88-977">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="e8e88-977">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="e8e88-978">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="e8e88-978">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="e8e88-979">Batchai</span><span class="sxs-lookup"><span data-stu-id="e8e88-979">Batchai</span></span>

* <span data-ttu-id="e8e88-980">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="e8e88-980">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="e8e88-981">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e8e88-981">Keyvault</span></span>

* <span data-ttu-id="e8e88-982">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="e8e88-982">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="e8e88-983">(#4448)</span><span class="sxs-lookup"><span data-stu-id="e8e88-983">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="e8e88-984">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-984">Network</span></span>

* <span data-ttu-id="e8e88-985">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="e8e88-985">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="e8e88-986">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="e8e88-986">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="e8e88-987">Recurso</span><span class="sxs-lookup"><span data-stu-id="e8e88-987">Resource</span></span>

* <span data-ttu-id="e8e88-988">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="e8e88-988">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="e8e88-989">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="e8e88-989">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="e8e88-990">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="e8e88-990">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="e8e88-991">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="e8e88-991">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="e8e88-992">Sql</span><span class="sxs-lookup"><span data-stu-id="e8e88-992">Sql</span></span>

* <span data-ttu-id="e8e88-993">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="e8e88-993">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="e8e88-994">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="e8e88-994">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="e8e88-995">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="e8e88-995">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="e8e88-996">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-996">Storage</span></span>

* <span data-ttu-id="e8e88-997">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="e8e88-997">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-998">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-998">Vm</span></span>

* <span data-ttu-id="e8e88-999">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="e8e88-999">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="e8e88-1000">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1000">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="e8e88-1001">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1001">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="e8e88-1002">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1002">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="e8e88-1003">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1003">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="e8e88-1004">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="e8e88-1004">September 22, 2017</span></span>

<span data-ttu-id="e8e88-1005">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="e8e88-1005">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="e8e88-1006">Recurso</span><span class="sxs-lookup"><span data-stu-id="e8e88-1006">Resource</span></span>

* <span data-ttu-id="e8e88-1007">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="e8e88-1007">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="e8e88-1008">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="e8e88-1008">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="e8e88-1009">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1009">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="e8e88-1010">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1010">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-1011">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-1011">Network</span></span>

* <span data-ttu-id="e8e88-1012">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1012">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="e8e88-1013">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1013">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="e8e88-1014">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8e88-1014">Added `asg` application security group commands</span></span>
* <span data-ttu-id="e8e88-1015">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1015">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="e8e88-1016">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1016">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="e8e88-1017">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1017">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="e8e88-1018">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1018">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e8e88-1019">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-1019">Storage</span></span>

* <span data-ttu-id="e8e88-1020">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="e8e88-1020">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="e8e88-1021">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="e8e88-1021">Eventgrid</span></span>

* <span data-ttu-id="e8e88-1022">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="e8e88-1022">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="e8e88-1023">SQL</span><span class="sxs-lookup"><span data-stu-id="e8e88-1023">SQL</span></span>

* <span data-ttu-id="e8e88-1024">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="e8e88-1024">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="e8e88-1025">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="e8e88-1025">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="e8e88-1026">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1026">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="e8e88-1027">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e8e88-1027">Keyvault</span></span>

* <span data-ttu-id="e8e88-1028">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="e8e88-1028">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-1029">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-1029">VM</span></span>

* <span data-ttu-id="e8e88-1030">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1030">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="e8e88-1031">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="e8e88-1031">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="e8e88-1032">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1032">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="e8e88-1033">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1033">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="e8e88-1034">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1034">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="e8e88-1035">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1035">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-1036">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-1036">ACS</span></span>

* <span data-ttu-id="e8e88-1037">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-1037">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-1038">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-1038">Appservice</span></span>

* <span data-ttu-id="e8e88-1039">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1039">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="e8e88-1040">Backup</span><span class="sxs-lookup"><span data-stu-id="e8e88-1040">Backup</span></span>

* <span data-ttu-id="e8e88-1041">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="e8e88-1041">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="e8e88-1042">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="e8e88-1042">September 11, 2017</span></span>

<span data-ttu-id="e8e88-1043">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="e8e88-1043">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="e8e88-1044">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e8e88-1044">Core</span></span>

* <span data-ttu-id="e8e88-1045">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="e8e88-1045">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="e8e88-1046">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="e8e88-1046">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-1047">Acs</span><span class="sxs-lookup"><span data-stu-id="e8e88-1047">Acs</span></span>

* <span data-ttu-id="e8e88-1048">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1048">Added `acs list-locations` command</span></span>
* <span data-ttu-id="e8e88-1049">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="e8e88-1049">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-1050">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-1050">Appservice</span></span>

* <span data-ttu-id="e8e88-1051">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="e8e88-1051">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="e8e88-1052">CDN</span><span class="sxs-lookup"><span data-stu-id="e8e88-1052">CDN</span></span>

* <span data-ttu-id="e8e88-1053">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1053">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="e8e88-1054">Extensão</span><span class="sxs-lookup"><span data-stu-id="e8e88-1054">Extension</span></span>

* <span data-ttu-id="e8e88-1055">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="e8e88-1055">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="e8e88-1056">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e8e88-1056">Keyvault</span></span>

* <span data-ttu-id="e8e88-1057">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1057">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-1058">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-1058">Network</span></span>

* <span data-ttu-id="e8e88-1059">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1059">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="e8e88-1060">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1060">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="e8e88-1061">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1061">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="e8e88-1062">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1062">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="e8e88-1063">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1063">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="e8e88-1064">Recurso</span><span class="sxs-lookup"><span data-stu-id="e8e88-1064">Resource</span></span>

* <span data-ttu-id="e8e88-1065">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1065">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="e8e88-1066">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1066">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="e8e88-1067">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="e8e88-1067">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="e8e88-1068">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="e8e88-1068">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="e8e88-1069">SQL</span><span class="sxs-lookup"><span data-stu-id="e8e88-1069">SQL</span></span>

* <span data-ttu-id="e8e88-1070">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1070">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-1071">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-1071">VM</span></span>

* <span data-ttu-id="e8e88-1072">Corrigido: Não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="e8e88-1072">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="e8e88-1073">Corrigido: Usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="e8e88-1073">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="e8e88-1074">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1074">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="e8e88-1075">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="e8e88-1075">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="e8e88-1076">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="e8e88-1076">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="e8e88-1077">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="e8e88-1077">August 31, 2017</span></span>

<span data-ttu-id="e8e88-1078">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="e8e88-1078">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="e8e88-1079">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e8e88-1079">Keyvault</span></span>

* <span data-ttu-id="e8e88-1080">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1080">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="e8e88-1081">Sf</span><span class="sxs-lookup"><span data-stu-id="e8e88-1081">Sf</span></span>

* <span data-ttu-id="e8e88-1082">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1082">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="e8e88-1083">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-1083">Storage</span></span>

* <span data-ttu-id="e8e88-1084">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="e8e88-1084">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="e8e88-1085">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="e8e88-1085">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="e8e88-1086">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="e8e88-1086">August 28, 2017</span></span>

<span data-ttu-id="e8e88-1087">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="e8e88-1087">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="e8e88-1088">CLI</span><span class="sxs-lookup"><span data-stu-id="e8e88-1088">CLI</span></span>

* <span data-ttu-id="e8e88-1089">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1089">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-1090">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-1090">ACS</span></span>

* <span data-ttu-id="e8e88-1091">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="e8e88-1091">Corrected preview regions</span></span>
* <span data-ttu-id="e8e88-1092">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1092">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="e8e88-1093">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="e8e88-1093">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-1094">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-1094">Appservice</span></span>

* <span data-ttu-id="e8e88-1095">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1095">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="e8e88-1096">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1096">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="e8e88-1097">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1097">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="e8e88-1098">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8e88-1098">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="e8e88-1099">Correção: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="e8e88-1099">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="e8e88-1100">IoT</span><span class="sxs-lookup"><span data-stu-id="e8e88-1100">IoT</span></span>

* <span data-ttu-id="e8e88-1101">Correção #3934: Criação de política não limpa as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="e8e88-1101">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-1102">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-1102">Network</span></span>

* <span data-ttu-id="e8e88-1103">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1103">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="e8e88-1104">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1104">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="e8e88-1105">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1105">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="e8e88-1106">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1106">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="e8e88-1107">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1107">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="e8e88-1108">Perfil</span><span class="sxs-lookup"><span data-stu-id="e8e88-1108">Profile</span></span>

* <span data-ttu-id="e8e88-1109">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="e8e88-1109">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e8e88-1110">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e8e88-1110">Service Fabric</span></span>

* <span data-ttu-id="e8e88-1111">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="e8e88-1111">Preview release</span></span>
* <span data-ttu-id="e8e88-1112">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="e8e88-1112">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="e8e88-1113">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="e8e88-1113">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="e8e88-1114">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="e8e88-1114">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="e8e88-1115">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-1115">Storage</span></span>

* <span data-ttu-id="e8e88-1116">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="e8e88-1116">Enabled setting blob tier</span></span>
* <span data-ttu-id="e8e88-1117">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="e8e88-1117">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="e8e88-1118">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="e8e88-1118">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="e8e88-1119">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="e8e88-1119">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="e8e88-1120">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1120">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="e8e88-1121">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="e8e88-1121">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-1122">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-1122">VM</span></span>

* <span data-ttu-id="e8e88-1123">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1123">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="e8e88-1124">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="e8e88-1124">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="e8e88-1125">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1125">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="e8e88-1126">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="e8e88-1126">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="e8e88-1127">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="e8e88-1127">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="e8e88-1128">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1128">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="e8e88-1129">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="e8e88-1129">August 15, 2017</span></span>

<span data-ttu-id="e8e88-1130">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="e8e88-1130">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-1131">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-1131">ACS</span></span>

* <span data-ttu-id="e8e88-1132">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="e8e88-1132">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-1133">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-1133">Appservice</span></span>

* <span data-ttu-id="e8e88-1134">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="e8e88-1134">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="e8e88-1135">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="e8e88-1135">Event Grid</span></span>

* <span data-ttu-id="e8e88-1136">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="e8e88-1136">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="e8e88-1137">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="e8e88-1137">August 11, 2017</span></span>

<span data-ttu-id="e8e88-1138">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="e8e88-1138">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-1139">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-1139">ACS</span></span>

* <span data-ttu-id="e8e88-1140">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="e8e88-1140">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="e8e88-1141">Lote</span><span class="sxs-lookup"><span data-stu-id="e8e88-1141">Batch</span></span>

* <span data-ttu-id="e8e88-1142">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="e8e88-1142">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="e8e88-1143">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="e8e88-1143">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="e8e88-1144">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="e8e88-1144">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="e8e88-1145">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="e8e88-1145">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="e8e88-1146">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="e8e88-1146">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="e8e88-1147">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="e8e88-1147">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="e8e88-1148">Componente</span><span class="sxs-lookup"><span data-stu-id="e8e88-1148">Component</span></span>

* <span data-ttu-id="e8e88-1149">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="e8e88-1149">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="e8e88-1150">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e8e88-1150">Container</span></span>

* <span data-ttu-id="e8e88-1151">`create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="e8e88-1151">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="e8e88-1152">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e8e88-1152">Data Lake Store</span></span>

* <span data-ttu-id="e8e88-1153">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-1153">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="e8e88-1154">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="e8e88-1154">Event Grid</span></span>

* <span data-ttu-id="e8e88-1155">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e8e88-1155">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-1156">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-1156">Network</span></span>

* <span data-ttu-id="e8e88-1157">`lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="e8e88-1157">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="e8e88-1158">`application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="e8e88-1158">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="e8e88-1159">`application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="e8e88-1159">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="e8e88-1160">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1160">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="e8e88-1161">Perfil</span><span class="sxs-lookup"><span data-stu-id="e8e88-1161">Profile</span></span>

* <span data-ttu-id="e8e88-1162">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="e8e88-1162">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="e8e88-1163">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-1163">Storage</span></span>

* <span data-ttu-id="e8e88-1164">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="e8e88-1164">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-1165">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-1165">VM</span></span>

* <span data-ttu-id="e8e88-1166">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="e8e88-1166">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="e8e88-1167">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1167">Exposed `list-skus` command</span></span>
* <span data-ttu-id="e8e88-1168">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="e8e88-1168">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="e8e88-1169">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="e8e88-1169">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="e8e88-1170">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="e8e88-1170">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="e8e88-1171">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="e8e88-1171">July 28, 2017</span></span>

<span data-ttu-id="e8e88-1172">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="e8e88-1172">Version 2.0.12</span></span>

* <span data-ttu-id="e8e88-1173">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="e8e88-1173">Added container commands</span></span>
* <span data-ttu-id="e8e88-1174">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="e8e88-1174">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="e8e88-1175">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e8e88-1175">Core</span></span>

* <span data-ttu-id="e8e88-1176">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="e8e88-1176">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="e8e88-1177">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="e8e88-1177">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="e8e88-1178">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="e8e88-1178">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="e8e88-1179">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1179">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="e8e88-1180">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="e8e88-1180">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="e8e88-1181">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1181">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="e8e88-1182">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1182">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="e8e88-1183">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1183">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="e8e88-1184">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1184">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="e8e88-1185">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="e8e88-1185">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="e8e88-1186">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="e8e88-1186">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="e8e88-1187">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1187">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="e8e88-1188">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="e8e88-1188">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="e8e88-1189">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="e8e88-1189">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="e8e88-1190">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="e8e88-1190">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="e8e88-1191">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1191">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="e8e88-1192">ACR</span><span class="sxs-lookup"><span data-stu-id="e8e88-1192">ACR</span></span>

* <span data-ttu-id="e8e88-1193">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="e8e88-1193">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="e8e88-1194">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="e8e88-1194">Support SKU update for managed registries</span></span>
* <span data-ttu-id="e8e88-1195">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="e8e88-1195">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="e8e88-1196">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="e8e88-1196">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="e8e88-1197">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="e8e88-1197">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="e8e88-1198">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="e8e88-1198">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-1199">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-1199">ACS</span></span>

* <span data-ttu-id="e8e88-1200">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="e8e88-1200">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-1201">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-1201">Appservice</span></span>

* <span data-ttu-id="e8e88-1202">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="e8e88-1202">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="e8e88-1203">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="e8e88-1203">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="e8e88-1204">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1204">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="e8e88-1205">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1205">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="e8e88-1206">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1206">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="e8e88-1207">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1207">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="e8e88-1208">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1208">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="e8e88-1209">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1209">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="e8e88-1210">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="e8e88-1210">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="e8e88-1211">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1211">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="e8e88-1212">Lote</span><span class="sxs-lookup"><span data-stu-id="e8e88-1212">Batch</span></span>

* <span data-ttu-id="e8e88-1213">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="e8e88-1213">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="e8e88-1214">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1214">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="e8e88-1215">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1215">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="e8e88-1216">CDN</span><span class="sxs-lookup"><span data-stu-id="e8e88-1216">CDN</span></span>

* <span data-ttu-id="e8e88-1217">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="e8e88-1217">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="e8e88-1218">Nuvem</span><span class="sxs-lookup"><span data-stu-id="e8e88-1218">Cloud</span></span>

* <span data-ttu-id="e8e88-1219">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="e8e88-1219">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="e8e88-1220">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="e8e88-1220">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="e8e88-1221">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="e8e88-1221">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="e8e88-1222">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="e8e88-1222">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="e8e88-1223">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1223">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e8e88-1224">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e8e88-1224">CosmosDB</span></span>

* <span data-ttu-id="e8e88-1225">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="e8e88-1225">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="e8e88-1226">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="e8e88-1226">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e8e88-1227">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e8e88-1227">Data Lake Analytics</span></span>

* <span data-ttu-id="e8e88-1228">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1228">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="e8e88-1229">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1229">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="e8e88-1230">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1230">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e8e88-1231">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e8e88-1231">Data Lake Store</span></span>

* <span data-ttu-id="e8e88-1232">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1232">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="e8e88-1233">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="e8e88-1233">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="e8e88-1234">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="e8e88-1234">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="e8e88-1235">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e8e88-1235">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="e8e88-1236">Interativo</span><span class="sxs-lookup"><span data-stu-id="e8e88-1236">Interactive</span></span>

* <span data-ttu-id="e8e88-1237">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="e8e88-1237">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="e8e88-1238">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="e8e88-1238">Increased test coverage</span></span>
* <span data-ttu-id="e8e88-1239">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="e8e88-1239">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="e8e88-1240">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1240">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="e8e88-1241">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1241">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="e8e88-1242">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1242">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="e8e88-1243">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1243">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="e8e88-1244">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1244">Added `--progress` flag</span></span>
* <span data-ttu-id="e8e88-1245">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="e8e88-1245">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="e8e88-1246">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1246">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="e8e88-1247">IoT</span><span class="sxs-lookup"><span data-stu-id="e8e88-1247">IoT</span></span>

* <span data-ttu-id="e8e88-1248">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="e8e88-1248">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="e8e88-1249">(#3934)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1249">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="e8e88-1250">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="e8e88-1250">Key vault</span></span>

* <span data-ttu-id="e8e88-1251">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="e8e88-1251">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="e8e88-1252">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1252">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="e8e88-1253">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1253">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="e8e88-1254">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1254">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="e8e88-1255">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1255">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="e8e88-1256">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1256">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="e8e88-1257">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="e8e88-1257">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="e8e88-1258">(#3307)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1258">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="e8e88-1259">Laboratório</span><span class="sxs-lookup"><span data-stu-id="e8e88-1259">Lab</span></span>

* <span data-ttu-id="e8e88-1260">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1260">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="e8e88-1261">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1261">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="e8e88-1262">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e8e88-1262">Monitor</span></span>

* <span data-ttu-id="e8e88-1263">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1263">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="e8e88-1264">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1264">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="e8e88-1265">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1265">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="e8e88-1266">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1266">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="e8e88-1267">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1267">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="e8e88-1268">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="e8e88-1268">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="e8e88-1269">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="e8e88-1269">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="e8e88-1270">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="e8e88-1270">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="e8e88-1271">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="e8e88-1271">`location` no longer required</span></span>
  * <span data-ttu-id="e8e88-1272">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="e8e88-1272">Add name and ID support for target</span></span>
  * <span data-ttu-id="e8e88-1273">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1273">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="e8e88-1274">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="e8e88-1274">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="e8e88-1275">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="e8e88-1275">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="e8e88-1276">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="e8e88-1276">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="e8e88-1277">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1277">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="e8e88-1278">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1278">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-1279">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-1279">Network</span></span>

* <span data-ttu-id="e8e88-1280">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1280">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="e8e88-1281">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1281">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="e8e88-1282">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="e8e88-1282">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="e8e88-1283">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="e8e88-1283">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="e8e88-1284">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1284">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="e8e88-1285">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1285">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="e8e88-1286">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1286">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="e8e88-1287">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1287">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="e8e88-1288">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1288">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="e8e88-1289">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1289">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="e8e88-1290">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1290">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="e8e88-1291">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1291">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="e8e88-1292">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1292">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="e8e88-1293">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1293">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="e8e88-1294">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1294">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="e8e88-1295">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1295">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="e8e88-1296">Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS</span><span class="sxs-lookup"><span data-stu-id="e8e88-1296">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="e8e88-1297">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1297">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="e8e88-1298">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1298">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="e8e88-1299">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1299">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="e8e88-1300">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1300">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="e8e88-1301">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1301">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="e8e88-1302">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1302">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="e8e88-1303">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="e8e88-1303">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="e8e88-1304">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="e8e88-1304">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="e8e88-1305">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="e8e88-1305">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="e8e88-1306">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="e8e88-1306">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="e8e88-1307">Perfil</span><span class="sxs-lookup"><span data-stu-id="e8e88-1307">Profile</span></span>

* <span data-ttu-id="e8e88-1308">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="e8e88-1308">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="e8e88-1309">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="e8e88-1309">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="e8e88-1310">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="e8e88-1310">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="e8e88-1311">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="e8e88-1311">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="e8e88-1312">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="e8e88-1312">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="e8e88-1313">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e8e88-1313">RDBMS</span></span>

* <span data-ttu-id="e8e88-1314">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1314">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="e8e88-1315">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1315">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="e8e88-1316">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1316">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="e8e88-1317">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1317">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="e8e88-1318">Recurso</span><span class="sxs-lookup"><span data-stu-id="e8e88-1318">Resource</span></span>

* <span data-ttu-id="e8e88-1319">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1319">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="e8e88-1320">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1320">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="e8e88-1321">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1321">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="e8e88-1322">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1322">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="e8e88-1323">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1323">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="e8e88-1324">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1324">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="e8e88-1325">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1325">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="e8e88-1326">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1326">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="e8e88-1327">Função</span><span class="sxs-lookup"><span data-stu-id="e8e88-1327">Role</span></span>

* <span data-ttu-id="e8e88-1328">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1328">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="e8e88-1329">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1329">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="e8e88-1330">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1330">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="e8e88-1331">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1331">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="e8e88-1332">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1332">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e8e88-1333">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e8e88-1333">Service Fabric</span></span>
* <span data-ttu-id="e8e88-1334">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1334">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="e8e88-1335">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1335">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="e8e88-1336">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1336">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="e8e88-1337">SQL</span><span class="sxs-lookup"><span data-stu-id="e8e88-1337">SQL</span></span>

* <span data-ttu-id="e8e88-1338">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1338">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="e8e88-1339">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1339">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="e8e88-1340">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1340">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="e8e88-1341">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-1341">Storage</span></span>

* <span data-ttu-id="e8e88-1342">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1342">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="e8e88-1343">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="e8e88-1343">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="e8e88-1344">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1344">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="e8e88-1345">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1345">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="e8e88-1346">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1346">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="e8e88-1347">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1347">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-1348">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-1348">VM</span></span>

* <span data-ttu-id="e8e88-1349">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="e8e88-1349">Support configuring nsg</span></span>
* <span data-ttu-id="e8e88-1350">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="e8e88-1350">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="e8e88-1351">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="e8e88-1351">Support managed service identities</span></span>
* <span data-ttu-id="e8e88-1352">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1352">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="e8e88-1353">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="e8e88-1353">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="e8e88-1354">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="e8e88-1354">May 10, 2017</span></span>

<span data-ttu-id="e8e88-1355">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="e8e88-1355">Version 2.0.6</span></span>

* <span data-ttu-id="e8e88-1356">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e8e88-1356">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="e8e88-1357">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1357">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="e8e88-1358">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e8e88-1358">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="e8e88-1359">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="e8e88-1359">Include Cognitive Services module</span></span>
* <span data-ttu-id="e8e88-1360">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e8e88-1360">Include Service Fabric module</span></span>
* <span data-ttu-id="e8e88-1361">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1361">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="e8e88-1362">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="e8e88-1362">Add support for CDN commands</span></span>
* <span data-ttu-id="e8e88-1363">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="e8e88-1363">Remove Container module</span></span>
* <span data-ttu-id="e8e88-1364">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1364">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="e8e88-1365">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1365">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="e8e88-1366">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e8e88-1366">Core</span></span>

* <span data-ttu-id="e8e88-1367">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="e8e88-1367">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="e8e88-1368">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1368">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="e8e88-1369">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1369">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="e8e88-1370">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1370">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="e8e88-1371">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1371">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="e8e88-1372">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1372">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="e8e88-1373">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1373">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="e8e88-1374">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1374">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="e8e88-1375">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1375">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="e8e88-1376">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="e8e88-1376">core: Improved performance</span></span>
* <span data-ttu-id="e8e88-1377">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="e8e88-1377">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="e8e88-1378">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="e8e88-1378">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-1379">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-1379">ACS</span></span>

* <span data-ttu-id="e8e88-1380">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8e88-1380">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="e8e88-1381">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="e8e88-1381">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="e8e88-1382">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="e8e88-1382">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="e8e88-1383">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1383">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-1384">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-1384">AppService</span></span>

* <span data-ttu-id="e8e88-1385">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="e8e88-1385">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="e8e88-1386">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="e8e88-1386">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="e8e88-1387">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1387">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="e8e88-1388">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="e8e88-1388">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="e8e88-1389">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="e8e88-1389">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="e8e88-1390">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1390">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="e8e88-1391">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="e8e88-1391">support slot swap with preview</span></span>
* <span data-ttu-id="e8e88-1392">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1392">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="e8e88-1393">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1393">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e8e88-1394">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e8e88-1394">CosmosDB</span></span>

* <span data-ttu-id="e8e88-1395">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e8e88-1395">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="e8e88-1396">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="e8e88-1396">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="e8e88-1397">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="e8e88-1397">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="e8e88-1398">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="e8e88-1398">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e8e88-1399">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e8e88-1399">Data Lake Analytics</span></span>

* <span data-ttu-id="e8e88-1400">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="e8e88-1400">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="e8e88-1401">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="e8e88-1401">Add support for new catalog item type: package.</span></span> <span data-ttu-id="e8e88-1402">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1402">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="e8e88-1403">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="e8e88-1403">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="e8e88-1404">Tabela</span><span class="sxs-lookup"><span data-stu-id="e8e88-1404">Table</span></span>
  * <span data-ttu-id="e8e88-1405">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="e8e88-1405">Table valued function</span></span>
  * <span data-ttu-id="e8e88-1406">Visualizar</span><span class="sxs-lookup"><span data-stu-id="e8e88-1406">View</span></span>
  * <span data-ttu-id="e8e88-1407">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="e8e88-1407">Table Statistics.</span></span> <span data-ttu-id="e8e88-1408">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="e8e88-1408">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e8e88-1409">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e8e88-1409">Data Lake Store</span></span>

* <span data-ttu-id="e8e88-1410">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="e8e88-1410">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="e8e88-1411">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1411">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="e8e88-1412">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="e8e88-1412">missed help for access show.</span></span> <span data-ttu-id="e8e88-1413">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="e8e88-1413">adding it.</span></span> <span data-ttu-id="e8e88-1414">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1414">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="e8e88-1415">Localizar</span><span class="sxs-lookup"><span data-stu-id="e8e88-1415">Find</span></span>

* <span data-ttu-id="e8e88-1416">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="e8e88-1416">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="e8e88-1417">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e8e88-1417">KeyVault</span></span>

* <span data-ttu-id="e8e88-1418">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="e8e88-1418">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="e8e88-1419">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="e8e88-1419">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="e8e88-1420">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="e8e88-1420">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="e8e88-1421">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="e8e88-1421">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="e8e88-1422">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1422">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="e8e88-1423">Laboratório</span><span class="sxs-lookup"><span data-stu-id="e8e88-1423">Lab</span></span>

* <span data-ttu-id="e8e88-1424">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="e8e88-1424">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="e8e88-1425">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="e8e88-1425">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="e8e88-1426">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="e8e88-1426">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="e8e88-1427">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="e8e88-1427">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="e8e88-1428">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="e8e88-1428">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="e8e88-1429">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e8e88-1429">Monitor</span></span>

* <span data-ttu-id="e8e88-1430">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1430">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="e8e88-1431">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1431">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="e8e88-1432">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-1432">Network</span></span>

* <span data-ttu-id="e8e88-1433">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1433">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="e8e88-1434">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1434">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="e8e88-1435">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8e88-1435">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="e8e88-1436">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8e88-1436">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="e8e88-1437">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="e8e88-1437">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="e8e88-1438">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="e8e88-1438">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="e8e88-1439">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="e8e88-1439">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="e8e88-1440">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="e8e88-1440">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="e8e88-1441">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1441">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="e8e88-1442">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="e8e88-1442">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="e8e88-1443">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1443">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="e8e88-1444">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1444">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="e8e88-1445">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="e8e88-1445">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="e8e88-1446">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="e8e88-1446">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="e8e88-1447">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="e8e88-1447">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="e8e88-1448">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="e8e88-1448">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="e8e88-1449">Perfil</span><span class="sxs-lookup"><span data-stu-id="e8e88-1449">Profile</span></span>

* <span data-ttu-id="e8e88-1450">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1450">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="e8e88-1451">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1451">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="e8e88-1452">Redis</span><span class="sxs-lookup"><span data-stu-id="e8e88-1452">Redis</span></span>

* <span data-ttu-id="e8e88-1453">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="e8e88-1453">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="e8e88-1454">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="e8e88-1454">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="e8e88-1455">Recurso</span><span class="sxs-lookup"><span data-stu-id="e8e88-1455">Resource</span></span>

* <span data-ttu-id="e8e88-1456">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1456">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="e8e88-1457">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1457">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="e8e88-1458">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1458">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="e8e88-1459">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="e8e88-1459">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="e8e88-1460">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1460">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="e8e88-1461">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="e8e88-1461">Add docs for az lock update.</span></span> <span data-ttu-id="e8e88-1462">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1462">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="e8e88-1463">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="e8e88-1463">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="e8e88-1464">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1464">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="e8e88-1465">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="e8e88-1465">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="e8e88-1466">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1466">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="e8e88-1467">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1467">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="e8e88-1468">Função</span><span class="sxs-lookup"><span data-stu-id="e8e88-1468">Role</span></span>

* <span data-ttu-id="e8e88-1469">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1469">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="e8e88-1470">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1470">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="e8e88-1471">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1471">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="e8e88-1472">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="e8e88-1472">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="e8e88-1473">SQL</span><span class="sxs-lookup"><span data-stu-id="e8e88-1473">SQL</span></span>

* <span data-ttu-id="e8e88-1474">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="e8e88-1474">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="e8e88-1475">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1475">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="e8e88-1476">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-1476">Storage</span></span>

* <span data-ttu-id="e8e88-1477">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1477">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="e8e88-1478">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="e8e88-1478">Add support for incremental blob copy</span></span>
* <span data-ttu-id="e8e88-1479">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="e8e88-1479">Add support for large block blob upload</span></span>
* <span data-ttu-id="e8e88-1480">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="e8e88-1480">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-1481">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-1481">VM</span></span>

* <span data-ttu-id="e8e88-1482">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="e8e88-1482">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="e8e88-1483">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="e8e88-1483">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="e8e88-1484">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="e8e88-1484">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="e8e88-1485">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="e8e88-1485">az vm/vmss disk</span></span>
  3. <span data-ttu-id="e8e88-1486">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="e8e88-1486">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="e8e88-1487">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="e8e88-1487">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="e8e88-1488">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1488">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="e8e88-1489">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="e8e88-1489">April 3, 2017</span></span>

<span data-ttu-id="e8e88-1490">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="e8e88-1490">Version 2.0.2</span></span>

<span data-ttu-id="e8e88-1491">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="e8e88-1491">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="e8e88-1492">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e8e88-1492">Core</span></span>

* <span data-ttu-id="e8e88-1493">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="e8e88-1493">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="e8e88-1494">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1494">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="e8e88-1495">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1495">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="e8e88-1496">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1496">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="e8e88-1497">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1497">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="e8e88-1498">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="e8e88-1498">Add prompting for missing template parameters.</span></span> <span data-ttu-id="e8e88-1499">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1499">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="e8e88-1500">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="e8e88-1500">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="e8e88-1501">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="e8e88-1501">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="e8e88-1502">ACS</span><span class="sxs-lookup"><span data-stu-id="e8e88-1502">ACS</span></span>

* <span data-ttu-id="e8e88-1503">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1503">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="e8e88-1504">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="e8e88-1504">Add support for ssh key password prompting.</span></span> <span data-ttu-id="e8e88-1505">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1505">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="e8e88-1506">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="e8e88-1506">Add support for windows clusters.</span></span> <span data-ttu-id="e8e88-1507">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1507">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="e8e88-1508">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="e8e88-1508">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="e8e88-1509">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1509">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="e8e88-1510">AppService</span><span class="sxs-lookup"><span data-stu-id="e8e88-1510">AppService</span></span>

* <span data-ttu-id="e8e88-1511">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1511">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="e8e88-1512">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1512">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="e8e88-1513">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1513">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="e8e88-1514">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1514">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="e8e88-1515">DataLake</span><span class="sxs-lookup"><span data-stu-id="e8e88-1515">DataLake</span></span>

* <span data-ttu-id="e8e88-1516">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e8e88-1516">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="e8e88-1517">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e8e88-1517">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="e8e88-1518">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="e8e88-1518">DocuemntDB</span></span>

* <span data-ttu-id="e8e88-1519">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1519">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="e8e88-1520">VM</span><span class="sxs-lookup"><span data-stu-id="e8e88-1520">VM</span></span>

* <span data-ttu-id="e8e88-1521">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1521">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="e8e88-1522">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1522">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="e8e88-1523">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1523">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="e8e88-1524">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1524">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="e8e88-1525">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1525">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="e8e88-1526">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1526">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="e8e88-1527">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="e8e88-1527">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="e8e88-1528">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="e8e88-1528">February 27, 2017</span></span>

<span data-ttu-id="e8e88-1529">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="e8e88-1529">Version 2.0.0</span></span>

<span data-ttu-id="e8e88-1530">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="e8e88-1530">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="e8e88-1531">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1531">Container Service (acs)</span></span>
- <span data-ttu-id="e8e88-1532">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1532">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="e8e88-1533">Rede</span><span class="sxs-lookup"><span data-stu-id="e8e88-1533">Networking</span></span>
- <span data-ttu-id="e8e88-1534">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e8e88-1534">Storage</span></span>

<span data-ttu-id="e8e88-1535">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1535">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="e8e88-1536">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="e8e88-1536">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="e8e88-1537">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="e8e88-1537">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="e8e88-1538">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="e8e88-1538">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="e8e88-1539">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1539">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="e8e88-1540">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="e8e88-1540">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="e8e88-1541">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1541">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="e8e88-1542">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="e8e88-1542">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="e8e88-1543">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="e8e88-1543">Provide feedback from the command line with the `az feedback` command</span></span>

