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
ms.openlocfilehash: b44a387a144b9d7daca8d87309d8a5e1a47b078a
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967870"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="f2c97-103">Notas de versão da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="f2c97-103">Azure CLI 2.0 release notes</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="f2c97-104">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="f2c97-104">July 3, 2018</span></span>

<span data-ttu-id="f2c97-105">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="f2c97-105">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="f2c97-106">AKS</span><span class="sxs-lookup"><span data-stu-id="f2c97-106">AKS</span></span>

* <span data-ttu-id="f2c97-107">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="f2c97-107">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="f2c97-108">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="f2c97-108">July 3, 2018</span></span>

<span data-ttu-id="f2c97-109">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="f2c97-109">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="f2c97-110">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2c97-110">Core</span></span>

* <span data-ttu-id="f2c97-111">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="f2c97-111">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="f2c97-112">ACR</span><span class="sxs-lookup"><span data-stu-id="f2c97-112">ACR</span></span>

* <span data-ttu-id="f2c97-113">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="f2c97-113">Added polling build status</span></span>
* <span data-ttu-id="f2c97-114">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="f2c97-114">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="f2c97-115">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="f2c97-115">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-116">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-116">ACS</span></span>

* <span data-ttu-id="f2c97-117">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="f2c97-117">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="f2c97-118">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="f2c97-118">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="f2c97-119">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-119">Updated options for `aks browse` command.</span></span> <span data-ttu-id="f2c97-120">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="f2c97-120">Added `--listen-port` support</span></span>
* <span data-ttu-id="f2c97-121">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-121">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="f2c97-122">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="f2c97-122">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="f2c97-123">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="f2c97-123">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-124">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-124">AppService</span></span>

* <span data-ttu-id="f2c97-125">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="f2c97-125">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="f2c97-126">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="f2c97-126">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="f2c97-127">Backup</span><span class="sxs-lookup"><span data-stu-id="f2c97-127">Backup</span></span>

* <span data-ttu-id="f2c97-128">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="f2c97-128">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="f2c97-129">BatchAI</span><span class="sxs-lookup"><span data-stu-id="f2c97-129">BatchAI</span></span>

* <span data-ttu-id="f2c97-130">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="f2c97-130">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="f2c97-131">Nuvem</span><span class="sxs-lookup"><span data-stu-id="f2c97-131">Cloud</span></span>

* <span data-ttu-id="f2c97-132">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="f2c97-132">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="f2c97-133">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f2c97-133">Container</span></span>

* <span data-ttu-id="f2c97-134">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="f2c97-134">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="f2c97-135">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="f2c97-135">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="f2c97-136">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="f2c97-136">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="f2c97-137">Extensão</span><span class="sxs-lookup"><span data-stu-id="f2c97-137">Extension</span></span>

* <span data-ttu-id="f2c97-138">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="f2c97-138">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="f2c97-139">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-139">Network</span></span>

* <span data-ttu-id="f2c97-140">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="f2c97-140">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="f2c97-141">Rdbms</span><span class="sxs-lookup"><span data-stu-id="f2c97-141">Rdbms</span></span>

* <span data-ttu-id="f2c97-142">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="f2c97-142">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="f2c97-143">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2c97-143">Resource</span></span>

* <span data-ttu-id="f2c97-144">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="f2c97-144">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-145">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-145">VM</span></span>

* <span data-ttu-id="f2c97-146">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="f2c97-146">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="f2c97-147">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="f2c97-147">June 25, 2018</span></span>

<span data-ttu-id="f2c97-148">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="f2c97-148">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="f2c97-149">CLI</span><span class="sxs-lookup"><span data-stu-id="f2c97-149">CLI</span></span>

* <span data-ttu-id="f2c97-150">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="f2c97-150">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="f2c97-151">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="f2c97-151">June 19, 2018</span></span>

<span data-ttu-id="f2c97-152">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="f2c97-152">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="f2c97-153">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2c97-153">Core</span></span>

* <span data-ttu-id="f2c97-154">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="f2c97-154">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="f2c97-155">ACR</span><span class="sxs-lookup"><span data-stu-id="f2c97-155">ACR</span></span>

* <span data-ttu-id="f2c97-156">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="f2c97-156">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="f2c97-157">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="f2c97-157">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-158">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-158">ACS</span></span>

* <span data-ttu-id="f2c97-159">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="f2c97-159">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="f2c97-160">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="f2c97-160">Added `--update` support</span></span>
* <span data-ttu-id="f2c97-161">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="f2c97-161">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="f2c97-162">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="f2c97-162">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="f2c97-163">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="f2c97-163">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="f2c97-164">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="f2c97-164">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="f2c97-165">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="f2c97-165">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="f2c97-166">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="f2c97-166">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-167">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-167">AppService</span></span>

* <span data-ttu-id="f2c97-168">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="f2c97-168">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="f2c97-169">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="f2c97-169">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="f2c97-170">Lote</span><span class="sxs-lookup"><span data-stu-id="f2c97-170">Batch</span></span>

* <span data-ttu-id="f2c97-171">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="f2c97-171">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f2c97-172">Lote AI</span><span class="sxs-lookup"><span data-stu-id="f2c97-172">Batch AI</span></span>

* <span data-ttu-id="f2c97-173">Foi adicionado suporte aos espaços de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f2c97-173">Added support for workspaces.</span></span> <span data-ttu-id="f2c97-174">Os espaços de trabalho permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="f2c97-174">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="f2c97-175">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="f2c97-175">Added support for experiments.</span></span> <span data-ttu-id="f2c97-176">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="f2c97-176">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="f2c97-177">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="f2c97-177">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="f2c97-178">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-178">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="f2c97-179">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="f2c97-179">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="f2c97-180">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="f2c97-180">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="f2c97-181">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos espaços de trabalho</span><span class="sxs-lookup"><span data-stu-id="f2c97-181">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="f2c97-182">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="f2c97-182">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="f2c97-183">[ALTERAÇÃO SIGNIFICATIVA] `--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-183">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="f2c97-184">Para montar um NFS pertencente a outro espaço de trabalho/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="f2c97-184">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="f2c97-185">[ALTERAÇÃO SIGNIFICATIVA] `--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-185">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="f2c97-186">Para enviar um trabalho em um cluster pertencente a outro espaço de trabalho/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="f2c97-186">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="f2c97-187">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="f2c97-187">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="f2c97-188">Agora, o local é um atributo de um espaço de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f2c97-188">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="f2c97-189">[ALTERAÇÃO SIGNIFICATIVA] `--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-189">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="f2c97-190">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="f2c97-190">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="f2c97-191">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="f2c97-191">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="f2c97-192">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="f2c97-192">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="f2c97-193">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="f2c97-193">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="f2c97-194">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="f2c97-194">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="f2c97-195">Mapas</span><span class="sxs-lookup"><span data-stu-id="f2c97-195">Maps</span></span>

* <span data-ttu-id="f2c97-196">[ALTERAÇÃO SIGNIFICATIVA] `maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="f2c97-196">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="f2c97-197">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-197">Network</span></span>

* <span data-ttu-id="f2c97-198">Foi adicionado suporte a `https` para `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="f2c97-198">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="f2c97-199">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="f2c97-199">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="f2c97-200">#6502</span><span class="sxs-lookup"><span data-stu-id="f2c97-200">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="f2c97-201">Reservas</span><span class="sxs-lookup"><span data-stu-id="f2c97-201">Reservations</span></span>

* <span data-ttu-id="f2c97-202">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="f2c97-202">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="f2c97-203">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="f2c97-203">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="f2c97-204">[ALTERAÇÃO SIGNIFICATIVA] `kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="f2c97-204">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="f2c97-205">[ALTERAÇÃO SIGNIFICATIVA] `capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="f2c97-205">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="f2c97-206">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="f2c97-206">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="f2c97-207">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-207">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="f2c97-208">Função</span><span class="sxs-lookup"><span data-stu-id="f2c97-208">Role</span></span>

* <span data-ttu-id="f2c97-209">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="f2c97-209">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="f2c97-210">SQL</span><span class="sxs-lookup"><span data-stu-id="f2c97-210">SQL</span></span>

* <span data-ttu-id="f2c97-211">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="f2c97-211">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="f2c97-212">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-212">Storage</span></span>

* <span data-ttu-id="f2c97-213">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="f2c97-213">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-214">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-214">VM</span></span>

* <span data-ttu-id="f2c97-215">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-215">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="f2c97-216">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="f2c97-216">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="f2c97-217">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="f2c97-217">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="f2c97-218">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="f2c97-218">June 13, 2018</span></span>

<span data-ttu-id="f2c97-219">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="f2c97-219">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="f2c97-220">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2c97-220">Core</span></span>

* <span data-ttu-id="f2c97-221">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="f2c97-221">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="f2c97-222">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="f2c97-222">June 13, 2018</span></span>

<span data-ttu-id="f2c97-223">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="f2c97-223">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="f2c97-224">AKS</span><span class="sxs-lookup"><span data-stu-id="f2c97-224">AKS</span></span>

* <span data-ttu-id="f2c97-225">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-225">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="f2c97-226">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="f2c97-226">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="f2c97-227">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-227">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="f2c97-228">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-228">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="f2c97-229">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-229">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-230">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-230">AppService</span></span>

* <span data-ttu-id="f2c97-231">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="f2c97-231">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="f2c97-232">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="f2c97-232">June 5, 2018</span></span>

<span data-ttu-id="f2c97-233">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="f2c97-233">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="f2c97-234">Interativo</span><span class="sxs-lookup"><span data-stu-id="f2c97-234">Interactive</span></span>

* <span data-ttu-id="f2c97-235">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="f2c97-235">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="f2c97-236">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="f2c97-236">June 5, 2018</span></span>

<span data-ttu-id="f2c97-237">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="f2c97-237">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="f2c97-238">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2c97-238">Core</span></span>

* <span data-ttu-id="f2c97-239">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="f2c97-239">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="f2c97-240">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="f2c97-240">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="f2c97-241">ACR</span><span class="sxs-lookup"><span data-stu-id="f2c97-241">ACR</span></span>

* <span data-ttu-id="f2c97-242">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="f2c97-242">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="f2c97-243">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="f2c97-243">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="f2c97-244">AKS</span><span class="sxs-lookup"><span data-stu-id="f2c97-244">AKS</span></span>

* <span data-ttu-id="f2c97-245">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="f2c97-245">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="f2c97-246">Lote</span><span class="sxs-lookup"><span data-stu-id="f2c97-246">Batch</span></span>

* <span data-ttu-id="f2c97-247">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="f2c97-247">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="f2c97-248">IOT</span><span class="sxs-lookup"><span data-stu-id="f2c97-248">IOT</span></span>

* <span data-ttu-id="f2c97-249">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="f2c97-249">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="f2c97-250">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-250">Network</span></span>

* <span data-ttu-id="f2c97-251">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="f2c97-251">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="f2c97-252">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="f2c97-252">Policy Insights</span></span>

* <span data-ttu-id="f2c97-253">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="f2c97-253">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="f2c97-254">ARM</span><span class="sxs-lookup"><span data-stu-id="f2c97-254">ARM</span></span>

* <span data-ttu-id="f2c97-255">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="f2c97-255">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="f2c97-256">SQL</span><span class="sxs-lookup"><span data-stu-id="f2c97-256">SQL</span></span>

* <span data-ttu-id="f2c97-257">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="f2c97-257">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="f2c97-258">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="f2c97-258">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="f2c97-259">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-259">Storage</span></span>

* <span data-ttu-id="f2c97-260">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="f2c97-260">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-261">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-261">VM</span></span>

* <span data-ttu-id="f2c97-262">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="f2c97-262">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="f2c97-263">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-263">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="f2c97-264">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-264">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="f2c97-265">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="f2c97-265">May 22, 2018</span></span>

<span data-ttu-id="f2c97-266">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="f2c97-266">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="f2c97-267">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2c97-267">Core</span></span>

* <span data-ttu-id="f2c97-268">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="f2c97-268">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-269">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-269">ACS</span></span>

* <span data-ttu-id="f2c97-270">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="f2c97-270">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="f2c97-271">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="f2c97-271">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-272">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-272">AppService</span></span>

* <span data-ttu-id="f2c97-273">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="f2c97-273">Improved generic update commands</span></span>
* <span data-ttu-id="f2c97-274">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="f2c97-274">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="f2c97-275">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f2c97-275">Container</span></span>

* <span data-ttu-id="f2c97-276">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="f2c97-276">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="f2c97-277">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="f2c97-277">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="f2c97-278">Extensão</span><span class="sxs-lookup"><span data-stu-id="f2c97-278">Extension</span></span>

* <span data-ttu-id="f2c97-279">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="f2c97-279">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="f2c97-280">Interativo</span><span class="sxs-lookup"><span data-stu-id="f2c97-280">Interactive</span></span>

* <span data-ttu-id="f2c97-281">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="f2c97-281">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="f2c97-282">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="f2c97-282">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="f2c97-283">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f2c97-283">KeyVault</span></span>

* <span data-ttu-id="f2c97-284">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="f2c97-284">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="f2c97-285">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-285">Network</span></span>

* <span data-ttu-id="f2c97-286">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="f2c97-286">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="f2c97-287">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="f2c97-287">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="f2c97-288">SQL</span><span class="sxs-lookup"><span data-stu-id="f2c97-288">SQL</span></span>

* <span data-ttu-id="f2c97-289">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="f2c97-289">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="f2c97-290">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="f2c97-290">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="f2c97-291">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="f2c97-291">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="f2c97-292">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2c97-292">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="f2c97-293">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="f2c97-293">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="f2c97-294">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-294">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="f2c97-295">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="f2c97-295">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="f2c97-296">`edition`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-296">`edition`.</span></span> <span data-ttu-id="f2c97-297">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="f2c97-297">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="f2c97-298">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-298">`elasticPoolName`.</span></span> <span data-ttu-id="f2c97-299">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="f2c97-299">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="f2c97-300">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="f2c97-300">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="f2c97-301">`edition`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-301">`edition`.</span></span> <span data-ttu-id="f2c97-302">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="f2c97-302">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="f2c97-303">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-303">`dtu`.</span></span> <span data-ttu-id="f2c97-304">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="f2c97-304">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="f2c97-305">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-305">`databaseDtuMin`.</span></span> <span data-ttu-id="f2c97-306">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="f2c97-306">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="f2c97-307">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-307">`databaseDtuMax`.</span></span> <span data-ttu-id="f2c97-308">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="f2c97-308">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="f2c97-309">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-309">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="f2c97-310">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-310">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="f2c97-311">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-311">Storage</span></span>

* <span data-ttu-id="f2c97-312">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="f2c97-312">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="f2c97-313">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="f2c97-313">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-314">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-314">VM</span></span>

* <span data-ttu-id="f2c97-315">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-315">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="f2c97-316">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="f2c97-316">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="f2c97-317">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="f2c97-317">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="f2c97-318">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="f2c97-318">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="f2c97-319">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-319">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="f2c97-320">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="f2c97-320">May 7, 2018</span></span>

<span data-ttu-id="f2c97-321">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="f2c97-321">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="f2c97-322">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2c97-322">Core</span></span>

* <span data-ttu-id="f2c97-323">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="f2c97-323">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="f2c97-324">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="f2c97-324">Added limited support for positional arguments</span></span>
* <span data-ttu-id="f2c97-325">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-325">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="f2c97-326">#5591</span><span class="sxs-lookup"><span data-stu-id="f2c97-326">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="f2c97-327">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-327">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="f2c97-328">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="f2c97-328">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="f2c97-329">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="f2c97-329">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="f2c97-330">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="f2c97-330">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="f2c97-331">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="f2c97-331">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="f2c97-332">ACR</span><span class="sxs-lookup"><span data-stu-id="f2c97-332">ACR</span></span>

* <span data-ttu-id="f2c97-333">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="f2c97-333">Added ACR Build commands</span></span>
* <span data-ttu-id="f2c97-334">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="f2c97-334">Improved resource not found error messages</span></span>
* <span data-ttu-id="f2c97-335">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="f2c97-335">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="f2c97-336">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="f2c97-336">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="f2c97-337">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="f2c97-337">Improved repository commands error messages</span></span>
* <span data-ttu-id="f2c97-338">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="f2c97-338">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-339">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-339">ACS</span></span>

* <span data-ttu-id="f2c97-340">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="f2c97-340">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="f2c97-341">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="f2c97-341">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="f2c97-342">AMS</span><span class="sxs-lookup"><span data-stu-id="f2c97-342">AMS</span></span>

* <span data-ttu-id="f2c97-343">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="f2c97-343">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-344">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-344">Appservice</span></span>

* <span data-ttu-id="f2c97-345">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="f2c97-345">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="f2c97-346">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-346">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="f2c97-347">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="f2c97-347">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="f2c97-348">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="f2c97-348">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f2c97-349">Lote AI</span><span class="sxs-lookup"><span data-stu-id="f2c97-349">Batch AI</span></span>

* <span data-ttu-id="f2c97-350">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="f2c97-350">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f2c97-351">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="f2c97-351">Cognitive Services</span></span>

* <span data-ttu-id="f2c97-352">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="f2c97-352">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="f2c97-353">Consumo</span><span class="sxs-lookup"><span data-stu-id="f2c97-353">Consumption</span></span>

* <span data-ttu-id="f2c97-354">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-354">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="f2c97-355">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f2c97-355">Container</span></span>

* <span data-ttu-id="f2c97-356">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="f2c97-356">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="f2c97-357">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f2c97-357">Cosmos DB</span></span>

* <span data-ttu-id="f2c97-358">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f2c97-358">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="f2c97-359">DMS</span><span class="sxs-lookup"><span data-stu-id="f2c97-359">DMS</span></span>

* <span data-ttu-id="f2c97-360">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="f2c97-360">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="f2c97-361">Extensão</span><span class="sxs-lookup"><span data-stu-id="f2c97-361">Extension</span></span>

* <span data-ttu-id="f2c97-362">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="f2c97-362">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="f2c97-363">Interativo</span><span class="sxs-lookup"><span data-stu-id="f2c97-363">Interactive</span></span>

* <span data-ttu-id="f2c97-364">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="f2c97-364">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="f2c97-365">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="f2c97-365">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="f2c97-366">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="f2c97-366">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="f2c97-367">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="f2c97-367">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="f2c97-368">Laboratório</span><span class="sxs-lookup"><span data-stu-id="f2c97-368">Lab</span></span>

* <span data-ttu-id="f2c97-369">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="f2c97-369">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="f2c97-370">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-370">Network</span></span>

* <span data-ttu-id="f2c97-371">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="f2c97-371">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="f2c97-372">Perfil</span><span class="sxs-lookup"><span data-stu-id="f2c97-372">Profile</span></span>

* <span data-ttu-id="f2c97-373">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="f2c97-373">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="f2c97-374">[ALTERAÇÃO SIGNIFICATIVA] `--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="f2c97-374">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="f2c97-375">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="f2c97-375">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="f2c97-376">Redis</span><span class="sxs-lookup"><span data-stu-id="f2c97-376">Redis</span></span>

* <span data-ttu-id="f2c97-377">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="f2c97-377">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="f2c97-378">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="f2c97-378">Deprecated `redis list-all`.</span></span> <span data-ttu-id="f2c97-379">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="f2c97-379">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="f2c97-380">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="f2c97-380">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="f2c97-381">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="f2c97-381">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="f2c97-382">Função</span><span class="sxs-lookup"><span data-stu-id="f2c97-382">Role</span></span>

* <span data-ttu-id="f2c97-383">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="f2c97-383">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="f2c97-384">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-384">Storage</span></span>

* <span data-ttu-id="f2c97-385">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="f2c97-385">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="f2c97-386">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="f2c97-386">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="f2c97-387">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="f2c97-387">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="f2c97-388">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="f2c97-388">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="f2c97-389">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="f2c97-389">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-390">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-390">VM</span></span>

* <span data-ttu-id="f2c97-391">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="f2c97-391">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="f2c97-392">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="f2c97-392">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="f2c97-393">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="f2c97-393">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="f2c97-394">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="f2c97-394">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="f2c97-395">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="f2c97-395">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="f2c97-396">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="f2c97-396">Added write accelerator support</span></span>
* <span data-ttu-id="f2c97-397">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="f2c97-397">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="f2c97-398">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="f2c97-398">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="f2c97-399">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="f2c97-399">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="f2c97-400">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="f2c97-400">April 10, 2018</span></span>

<span data-ttu-id="f2c97-401">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="f2c97-401">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="f2c97-402">ACR</span><span class="sxs-lookup"><span data-stu-id="f2c97-402">ACR</span></span>

* <span data-ttu-id="f2c97-403">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="f2c97-403">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-404">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-404">ACS</span></span>

* <span data-ttu-id="f2c97-405">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="f2c97-405">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-406">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-406">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="f2c97-408">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="f2c97-408">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="f2c97-409">BatchAI</span><span class="sxs-lookup"><span data-stu-id="f2c97-409">BatchAI</span></span>

* <span data-ttu-id="f2c97-410">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="f2c97-410">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="f2c97-411">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="f2c97-411">Job level mounting</span></span>
 - <span data-ttu-id="f2c97-412">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="f2c97-412">Environment variables with secret values</span></span>
 - <span data-ttu-id="f2c97-413">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="f2c97-413">Performance counters settings</span></span>
 - <span data-ttu-id="f2c97-414">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="f2c97-414">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="f2c97-415">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="f2c97-415">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="f2c97-416">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="f2c97-416">Usage and limits reporting</span></span>
 - <span data-ttu-id="f2c97-417">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="f2c97-417">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="f2c97-418">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="f2c97-418">Support for custom images</span></span>
 - <span data-ttu-id="f2c97-419">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="f2c97-419">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="f2c97-420">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="f2c97-420">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="f2c97-421">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="f2c97-421">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="f2c97-422">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="f2c97-422">National clouds are supported</span></span>
* <span data-ttu-id="f2c97-423">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="f2c97-423">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="f2c97-424">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="f2c97-424">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="f2c97-425">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="f2c97-425">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="f2c97-426">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="f2c97-426">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="f2c97-427">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="f2c97-427">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="f2c97-428">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="f2c97-428">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="f2c97-429">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="f2c97-429">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="f2c97-430">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="f2c97-430">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="f2c97-431">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="f2c97-431">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="f2c97-432">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-432">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="f2c97-433">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="f2c97-433">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="f2c97-434">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="f2c97-434">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="f2c97-435">[ALTERAÇÃO SIGNIFICATIVA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-435">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="f2c97-436">Cobrança</span><span class="sxs-lookup"><span data-stu-id="f2c97-436">Billing</span></span>

* <span data-ttu-id="f2c97-437">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="f2c97-437">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="f2c97-438">Consumo</span><span class="sxs-lookup"><span data-stu-id="f2c97-438">Consumption</span></span>

* <span data-ttu-id="f2c97-439">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="f2c97-439">Added `marketplace` commands</span></span>
* <span data-ttu-id="f2c97-440">[ALTERAÇÃO SIGNIFICATIVA] `reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="f2c97-440">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="f2c97-441">[ALTERAÇÃO SIGNIFICATIVA] `reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="f2c97-441">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="f2c97-442">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="f2c97-442">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="f2c97-443">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="f2c97-443">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="f2c97-444">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="f2c97-444">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="f2c97-445">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f2c97-445">Container</span></span>

* <span data-ttu-id="f2c97-446">Adição dos parâmetros de montagem de volume de repositório git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="f2c97-446">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="f2c97-447">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="f2c97-447">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="f2c97-448">Extensão</span><span class="sxs-lookup"><span data-stu-id="f2c97-448">Extension</span></span>

* <span data-ttu-id="f2c97-449">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="f2c97-449">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="f2c97-450">Interativo</span><span class="sxs-lookup"><span data-stu-id="f2c97-450">Interactive</span></span>

* <span data-ttu-id="f2c97-451">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="f2c97-451">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="f2c97-452">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="f2c97-452">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="f2c97-453">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="f2c97-453">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="f2c97-454">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-454">Network</span></span>

* <span data-ttu-id="f2c97-455">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="f2c97-455">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="f2c97-456">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-456">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="f2c97-457">#4910</span><span class="sxs-lookup"><span data-stu-id="f2c97-457">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="f2c97-458">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="f2c97-458">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="f2c97-459">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="f2c97-459">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="f2c97-460">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-460">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="f2c97-461">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-461">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="f2c97-462">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="f2c97-462">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="f2c97-463">Perfil</span><span class="sxs-lookup"><span data-stu-id="f2c97-463">Profile</span></span>

* <span data-ttu-id="f2c97-464">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="f2c97-464">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="f2c97-465">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="f2c97-465">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="f2c97-466">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f2c97-466">RDBMS</span></span>

* <span data-ttu-id="f2c97-467">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="f2c97-467">Added `georestore` command</span></span>
* <span data-ttu-id="f2c97-468">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-468">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="f2c97-469">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2c97-469">Resource</span></span>

* <span data-ttu-id="f2c97-470">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-470">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="f2c97-471">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-471">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="f2c97-472">SQL</span><span class="sxs-lookup"><span data-stu-id="f2c97-472">SQL</span></span>

* <span data-ttu-id="f2c97-473">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="f2c97-473">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="f2c97-474">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-474">Storage</span></span>

* <span data-ttu-id="f2c97-475">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="f2c97-475">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-476">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-476">VM</span></span>

* <span data-ttu-id="f2c97-477">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-477">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="f2c97-478">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-478">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="f2c97-480">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-480">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="f2c97-481">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="f2c97-481">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="f2c97-482">#5718</span><span class="sxs-lookup"><span data-stu-id="f2c97-482">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="f2c97-483">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="f2c97-483">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="f2c97-484">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="f2c97-484">March 27, 2018</span></span>

<span data-ttu-id="f2c97-485">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="f2c97-485">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="f2c97-486">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2c97-486">Core</span></span>

* <span data-ttu-id="f2c97-487">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="f2c97-487">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-488">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-488">ACS</span></span>

* <span data-ttu-id="f2c97-489">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="f2c97-489">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-490">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-490">Appservice</span></span>

* <span data-ttu-id="f2c97-491">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-491">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="f2c97-492">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-492">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="f2c97-493">Backup</span><span class="sxs-lookup"><span data-stu-id="f2c97-493">Backup</span></span>

* <span data-ttu-id="f2c97-494">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-494">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="f2c97-495">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="f2c97-495">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="f2c97-496">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="f2c97-496">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="f2c97-497">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="f2c97-497">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="f2c97-498">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f2c97-498">Container</span></span>

* <span data-ttu-id="f2c97-499">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-499">Added `container exec` command.</span></span> <span data-ttu-id="f2c97-500">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="f2c97-500">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="f2c97-501">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="f2c97-501">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="f2c97-502">Extensão</span><span class="sxs-lookup"><span data-stu-id="f2c97-502">Extension</span></span>

* <span data-ttu-id="f2c97-503">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="f2c97-503">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="f2c97-504">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="f2c97-504">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="f2c97-505">[ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="f2c97-505">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="f2c97-506">Interativo</span><span class="sxs-lookup"><span data-stu-id="f2c97-506">Interactive</span></span>

* <span data-ttu-id="f2c97-507">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="f2c97-507">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="f2c97-508">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="f2c97-508">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="f2c97-509">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="f2c97-509">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="f2c97-510">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="f2c97-510">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="f2c97-511">Laboratório</span><span class="sxs-lookup"><span data-stu-id="f2c97-511">Lab</span></span>

* <span data-ttu-id="f2c97-512">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="f2c97-512">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="f2c97-513">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f2c97-513">Monitor</span></span>

* <span data-ttu-id="f2c97-514">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="f2c97-514">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="f2c97-515">[#4529](https://github.com/Azure/azure-cli/issues/5785) corrigido: `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="f2c97-515">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="f2c97-516">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="f2c97-516">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="f2c97-517">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-517">Network</span></span>

* <span data-ttu-id="f2c97-518">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="f2c97-518">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="f2c97-519">Perfil</span><span class="sxs-lookup"><span data-stu-id="f2c97-519">Profile</span></span>

* <span data-ttu-id="f2c97-520">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="f2c97-520">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f2c97-521">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f2c97-521">RDBMS</span></span>

* <span data-ttu-id="f2c97-522">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="f2c97-522">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="f2c97-523">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2c97-523">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="f2c97-525">Função</span><span class="sxs-lookup"><span data-stu-id="f2c97-525">Role</span></span>

* <span data-ttu-id="f2c97-526">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-526">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="f2c97-527">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="f2c97-527">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="f2c97-528">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-528">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="f2c97-529">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-529">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="f2c97-530">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="f2c97-530">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="f2c97-531">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-531">Storage</span></span>

* <span data-ttu-id="f2c97-532">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="f2c97-532">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="f2c97-533">[4049#](https://github.com/Azure/azure-cli/issues/4049) corrigido: problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="f2c97-533">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-534">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-534">VM</span></span>

* <span data-ttu-id="f2c97-535">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="f2c97-535">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="f2c97-536">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-536">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="f2c97-537">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="f2c97-537">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="f2c97-538">[ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="f2c97-538">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="f2c97-539">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="f2c97-539">March 13, 2018</span></span>

<span data-ttu-id="f2c97-540">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="f2c97-540">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="f2c97-541">ACR</span><span class="sxs-lookup"><span data-stu-id="f2c97-541">ACR</span></span>

* <span data-ttu-id="f2c97-542">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="f2c97-542">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="f2c97-543">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="f2c97-543">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="f2c97-544">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="f2c97-544">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-545">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-545">ACS</span></span>

* <span data-ttu-id="f2c97-546">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="f2c97-546">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="f2c97-547">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="f2c97-547">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="f2c97-548">Supervisor</span><span class="sxs-lookup"><span data-stu-id="f2c97-548">Advisor</span></span>

* <span data-ttu-id="f2c97-549">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="f2c97-549">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="f2c97-550">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-550">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="f2c97-551">[ALTERAÇÃO SIGNIFICATIVA] `advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="f2c97-551">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="f2c97-552">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="f2c97-552">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="f2c97-553">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="f2c97-553">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-554">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-554">Appservice</span></span>

* <span data-ttu-id="f2c97-555">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="f2c97-555">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="f2c97-556">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="f2c97-556">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="f2c97-557">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="f2c97-557">Eventhubs</span></span>

* <span data-ttu-id="f2c97-558">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="f2c97-558">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="f2c97-559">Extensão</span><span class="sxs-lookup"><span data-stu-id="f2c97-559">Extension</span></span>

* <span data-ttu-id="f2c97-560">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="f2c97-560">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="f2c97-561">Interativo</span><span class="sxs-lookup"><span data-stu-id="f2c97-561">Interactive</span></span>

* <span data-ttu-id="f2c97-562">[5625](https://github.com/Azure/azure-cli/issues/5625) corrigido: manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="f2c97-562">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="f2c97-563">[3016](https://github.com/Azure/azure-cli/issues/3016) corrigido: histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="f2c97-563">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="f2c97-564">[5688](https://github.com/Azure/azure-cli/issues/5688) corrigido: as conclusões não aparecerão se o carregamento da tabela de comando encontrou uma exceção</span><span class="sxs-lookup"><span data-stu-id="f2c97-564">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="f2c97-565">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="f2c97-565">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="f2c97-566">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f2c97-566">Monitor</span></span>

* <span data-ttu-id="f2c97-567">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="f2c97-567">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="f2c97-568">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="f2c97-568">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="f2c97-569">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="f2c97-569">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="f2c97-570">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="f2c97-570">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="f2c97-571">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-571">Network</span></span>

* <span data-ttu-id="f2c97-572">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-572">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="f2c97-573">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="f2c97-573">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="f2c97-574">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="f2c97-574">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="f2c97-575">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="f2c97-575">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="f2c97-576">Perfil</span><span class="sxs-lookup"><span data-stu-id="f2c97-576">Profile</span></span>

* <span data-ttu-id="f2c97-577">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="f2c97-577">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="f2c97-578">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="f2c97-578">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f2c97-579">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f2c97-579">RDBMS</span></span>

* <span data-ttu-id="f2c97-580">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="f2c97-580">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="f2c97-581">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="f2c97-581">Service Bus</span></span>

* <span data-ttu-id="f2c97-582">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="f2c97-582">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="f2c97-583">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-583">Storage</span></span>

* <span data-ttu-id="f2c97-584">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="f2c97-584">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="f2c97-585">[5286](https://github.com/Azure/azure-cli/issues/5286) corrigido: os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="f2c97-585">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-586">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-586">VM</span></span>

* <span data-ttu-id="f2c97-587">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="f2c97-587">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="f2c97-588">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="f2c97-588">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="f2c97-589">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="f2c97-589">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="f2c97-590">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="f2c97-590">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="f2c97-591">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="f2c97-591">February 27, 2018</span></span>

<span data-ttu-id="f2c97-592">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="f2c97-592">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="f2c97-593">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2c97-593">Core</span></span>

* <span data-ttu-id="f2c97-594">Correção [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="f2c97-594">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="f2c97-595">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="f2c97-595">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="f2c97-596">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="f2c97-596">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-597">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-597">ACS</span></span>

* <span data-ttu-id="f2c97-598">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="f2c97-598">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="f2c97-599">Correção do problema de permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="f2c97-599">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="f2c97-600">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="f2c97-600">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="f2c97-601">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="f2c97-601">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-602">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-602">Appservice</span></span>

* <span data-ttu-id="f2c97-603">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="f2c97-603">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="f2c97-604">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="f2c97-604">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f2c97-605">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="f2c97-605">Cognitive Services</span></span>

* <span data-ttu-id="f2c97-606">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="f2c97-606">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="f2c97-607">Consumo</span><span class="sxs-lookup"><span data-stu-id="f2c97-607">Consumption</span></span>

* <span data-ttu-id="f2c97-608">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="f2c97-608">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="f2c97-609">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="f2c97-609">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="f2c97-610">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f2c97-610">Container</span></span>

* <span data-ttu-id="f2c97-611">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="f2c97-611">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="f2c97-612">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-612">Network</span></span>

* <span data-ttu-id="f2c97-613">Correção [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="f2c97-613">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="f2c97-614">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2c97-614">Resource</span></span>

* <span data-ttu-id="f2c97-615">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="f2c97-615">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="f2c97-616">Função</span><span class="sxs-lookup"><span data-stu-id="f2c97-616">Role</span></span>

* <span data-ttu-id="f2c97-617">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="f2c97-617">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="f2c97-618">SQL</span><span class="sxs-lookup"><span data-stu-id="f2c97-618">SQL</span></span>

* <span data-ttu-id="f2c97-619">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="f2c97-619">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="f2c97-620">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-620">Storage</span></span>

* <span data-ttu-id="f2c97-621">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-621">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-622">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-622">VM</span></span>

* <span data-ttu-id="f2c97-623">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="f2c97-623">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="f2c97-624">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="f2c97-624">February 13, 2018</span></span>

<span data-ttu-id="f2c97-625">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="f2c97-625">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="f2c97-626">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2c97-626">Core</span></span>

* <span data-ttu-id="f2c97-627">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="f2c97-627">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-628">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-628">ACS</span></span>

* <span data-ttu-id="f2c97-629">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="f2c97-629">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="f2c97-630">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-630">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="f2c97-631">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="f2c97-631">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="f2c97-632">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="f2c97-632">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="f2c97-633">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="f2c97-633">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="f2c97-634">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="f2c97-634">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="f2c97-635">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="f2c97-635">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="f2c97-636">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="f2c97-636">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-637">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-637">Appservice</span></span>

* <span data-ttu-id="f2c97-638">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="f2c97-638">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="f2c97-639">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="f2c97-639">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="f2c97-640">CDN</span><span class="sxs-lookup"><span data-stu-id="f2c97-640">CDN</span></span>

* <span data-ttu-id="f2c97-641">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-641">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="f2c97-642">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f2c97-642">Container</span></span>

* <span data-ttu-id="f2c97-643">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="f2c97-643">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="f2c97-644">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="f2c97-644">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f2c97-645">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f2c97-645">CosmosDB</span></span>

* <span data-ttu-id="f2c97-646">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="f2c97-646">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="f2c97-647">Extensão</span><span class="sxs-lookup"><span data-stu-id="f2c97-647">Extension</span></span>

* <span data-ttu-id="f2c97-648">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-648">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="f2c97-649">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-649">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="f2c97-650">Comentários</span><span class="sxs-lookup"><span data-stu-id="f2c97-650">Feedback</span></span>

* <span data-ttu-id="f2c97-651">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="f2c97-651">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="f2c97-652">Interativo</span><span class="sxs-lookup"><span data-stu-id="f2c97-652">Interactive</span></span>

* <span data-ttu-id="f2c97-653">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="f2c97-653">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="f2c97-654">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="f2c97-654">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="f2c97-655">IoT</span><span class="sxs-lookup"><span data-stu-id="f2c97-655">IoT</span></span>

* <span data-ttu-id="f2c97-656">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="f2c97-656">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="f2c97-657">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="f2c97-657">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="f2c97-658">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-658">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="f2c97-659">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="f2c97-659">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="f2c97-660">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f2c97-660">Monitor</span></span>

* <span data-ttu-id="f2c97-661">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-661">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="f2c97-662">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-662">Network</span></span>

* <span data-ttu-id="f2c97-663">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="f2c97-663">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="f2c97-664">Perfil</span><span class="sxs-lookup"><span data-stu-id="f2c97-664">Profile</span></span>

* <span data-ttu-id="f2c97-665">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="f2c97-665">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="f2c97-666">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2c97-666">Resource</span></span>

* <span data-ttu-id="f2c97-667">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="f2c97-667">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="f2c97-668">Função</span><span class="sxs-lookup"><span data-stu-id="f2c97-668">Role</span></span>

* <span data-ttu-id="f2c97-669">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-669">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="f2c97-670">SQL</span><span class="sxs-lookup"><span data-stu-id="f2c97-670">SQL</span></span>

* <span data-ttu-id="f2c97-671">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="f2c97-671">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="f2c97-672">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="f2c97-672">Added `sql db rename`</span></span>
* <span data-ttu-id="f2c97-673">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="f2c97-673">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="f2c97-674">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-674">Storage</span></span>

* <span data-ttu-id="f2c97-675">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="f2c97-675">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-676">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-676">VM</span></span>

* <span data-ttu-id="f2c97-677">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="f2c97-677">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="f2c97-678">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="f2c97-678">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="f2c97-679">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="f2c97-679">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="f2c97-680">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="f2c97-680">January 31, 2018</span></span>

<span data-ttu-id="f2c97-681">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="f2c97-681">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="f2c97-682">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2c97-682">Core</span></span>

* <span data-ttu-id="f2c97-683">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="f2c97-683">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="f2c97-684">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="f2c97-684">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="f2c97-685">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="f2c97-685">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="f2c97-686">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="f2c97-686">Use `--verbose` to see</span></span>
* <span data-ttu-id="f2c97-687">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="f2c97-687">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-688">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-688">ACS</span></span>

* <span data-ttu-id="f2c97-689">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="f2c97-689">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="f2c97-690">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="f2c97-690">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-691">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-691">Appservice</span></span>

* <span data-ttu-id="f2c97-692">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="f2c97-692">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="f2c97-693">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="f2c97-693">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="f2c97-694">CDN</span><span class="sxs-lookup"><span data-stu-id="f2c97-694">CDN</span></span>

* <span data-ttu-id="f2c97-695">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-695">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f2c97-696">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f2c97-696">CosmosDB</span></span>

* <span data-ttu-id="f2c97-697">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="f2c97-697">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="f2c97-698">Interativo</span><span class="sxs-lookup"><span data-stu-id="f2c97-698">Interactive</span></span>

* <span data-ttu-id="f2c97-699">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="f2c97-699">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="f2c97-700">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-700">Network</span></span>

* <span data-ttu-id="f2c97-701">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-701">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="f2c97-702">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="f2c97-702">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="f2c97-703">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-703">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="f2c97-704">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-704">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="f2c97-705">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="f2c97-705">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="f2c97-706">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="f2c97-706">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="f2c97-707">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="f2c97-707">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="f2c97-708">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="f2c97-708">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="f2c97-709">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="f2c97-709">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="f2c97-710">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="f2c97-710">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="f2c97-711">Perfil</span><span class="sxs-lookup"><span data-stu-id="f2c97-711">Profile</span></span>

* <span data-ttu-id="f2c97-712">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="f2c97-712">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="f2c97-713">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2c97-713">Resource</span></span>

* <span data-ttu-id="f2c97-714">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="f2c97-714">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="f2c97-715">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-715">Storage</span></span>

* <span data-ttu-id="f2c97-716">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="f2c97-716">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="f2c97-717">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="f2c97-717">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="f2c97-718">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="f2c97-718">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="f2c97-719">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-719">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="f2c97-720">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="f2c97-720">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-721">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-721">VM</span></span>

* <span data-ttu-id="f2c97-722">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="f2c97-722">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="f2c97-723">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="f2c97-723">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="f2c97-724">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="f2c97-724">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="f2c97-725">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-725">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="f2c97-726">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="f2c97-726">January 17, 2018</span></span>

<span data-ttu-id="f2c97-727">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="f2c97-727">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="f2c97-728">ACR</span><span class="sxs-lookup"><span data-stu-id="f2c97-728">ACR</span></span>

* <span data-ttu-id="f2c97-729">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="f2c97-729">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="f2c97-730">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="f2c97-730">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-731">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-731">ACS</span></span>

* <span data-ttu-id="f2c97-732">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="f2c97-732">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="f2c97-733">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="f2c97-733">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-734">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-734">Appservice</span></span>

* <span data-ttu-id="f2c97-735">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="f2c97-735">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="f2c97-736">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="f2c97-736">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="f2c97-737">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="f2c97-737">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="f2c97-738">Backup</span><span class="sxs-lookup"><span data-stu-id="f2c97-738">Backup</span></span>

* <span data-ttu-id="f2c97-739">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="f2c97-739">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="f2c97-740">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="f2c97-740">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="f2c97-741">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="f2c97-741">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="f2c97-742">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="f2c97-742">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="f2c97-743">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="f2c97-743">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="f2c97-744">Lote</span><span class="sxs-lookup"><span data-stu-id="f2c97-744">Batch</span></span>

* <span data-ttu-id="f2c97-745">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="f2c97-745">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="f2c97-746">Nuvem</span><span class="sxs-lookup"><span data-stu-id="f2c97-746">Cloud</span></span>

* <span data-ttu-id="f2c97-747">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="f2c97-747">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="f2c97-748">Consumo</span><span class="sxs-lookup"><span data-stu-id="f2c97-748">Consumption</span></span>

* <span data-ttu-id="f2c97-749">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="f2c97-749">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="f2c97-750">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="f2c97-750">Event Grid</span></span>

* <span data-ttu-id="f2c97-751">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="f2c97-751">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="f2c97-752">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="f2c97-752">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="f2c97-753">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="f2c97-753">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="f2c97-754">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="f2c97-754">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="f2c97-755">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-755">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="f2c97-756">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-756">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="f2c97-757">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="f2c97-757">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="f2c97-758">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="f2c97-758">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="f2c97-759">Interativo</span><span class="sxs-lookup"><span data-stu-id="f2c97-759">Interactive</span></span>

* <span data-ttu-id="f2c97-760">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="f2c97-760">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="f2c97-761">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="f2c97-761">Fixed errors on startup</span></span>
* <span data-ttu-id="f2c97-762">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="f2c97-762">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="f2c97-763">IoT</span><span class="sxs-lookup"><span data-stu-id="f2c97-763">IoT</span></span>

* <span data-ttu-id="f2c97-764">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="f2c97-764">Added support for device provisioning service</span></span>
* <span data-ttu-id="f2c97-765">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="f2c97-765">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="f2c97-766">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="f2c97-766">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="f2c97-767">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f2c97-767">Monitor</span></span>

* <span data-ttu-id="f2c97-768">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="f2c97-768">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="f2c97-769">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-769">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="f2c97-770">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="f2c97-770">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="f2c97-771">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-771">Network</span></span>

* <span data-ttu-id="f2c97-772">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-772">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="f2c97-773">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-773">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="f2c97-774">Perfil</span><span class="sxs-lookup"><span data-stu-id="f2c97-774">Profile</span></span>

* <span data-ttu-id="f2c97-775">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="f2c97-775">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="f2c97-776">Função</span><span class="sxs-lookup"><span data-stu-id="f2c97-776">Role</span></span>

* <span data-ttu-id="f2c97-777">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="f2c97-777">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f2c97-778">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f2c97-778">Service Fabric</span></span>

* <span data-ttu-id="f2c97-779">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="f2c97-779">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="f2c97-780">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="f2c97-780">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-781">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-781">VM</span></span>

* <span data-ttu-id="f2c97-782">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="f2c97-782">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="f2c97-783">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="f2c97-783">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="f2c97-784">[ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="f2c97-784">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="f2c97-785">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="f2c97-785">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="f2c97-786">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="f2c97-786">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="f2c97-787">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-787">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="f2c97-788">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-788">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="f2c97-789">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="f2c97-789">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="f2c97-790">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="f2c97-790">December 19, 2017</span></span>

<span data-ttu-id="f2c97-791">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="f2c97-791">Version 2.0.23</span></span>

* <span data-ttu-id="f2c97-792">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="f2c97-792">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="f2c97-793">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f2c97-793">Container</span></span>

* <span data-ttu-id="f2c97-794">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="f2c97-794">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="f2c97-795">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-795">Network</span></span>

* <span data-ttu-id="f2c97-796">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-796">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="f2c97-797">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-797">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="f2c97-798">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-798">Storage</span></span>

* <span data-ttu-id="f2c97-799">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="f2c97-799">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-800">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-800">VM</span></span>

* <span data-ttu-id="f2c97-801">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="f2c97-801">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="f2c97-802">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="f2c97-802">December 5, 2017</span></span>

<span data-ttu-id="f2c97-803">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="f2c97-803">Version 2.0.22</span></span>

* <span data-ttu-id="f2c97-804">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="f2c97-804">Removed `az component` commands.</span></span> <span data-ttu-id="f2c97-805">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="f2c97-805">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="f2c97-806">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2c97-806">Core</span></span>
* <span data-ttu-id="f2c97-807">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="f2c97-807">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="f2c97-808">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="f2c97-808">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-809">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-809">ACS</span></span>

* <span data-ttu-id="f2c97-810">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="f2c97-810">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="f2c97-811">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-811">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="f2c97-812">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="f2c97-812">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="f2c97-813">Supervisor</span><span class="sxs-lookup"><span data-stu-id="f2c97-813">Advisor</span></span>

* <span data-ttu-id="f2c97-814">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="f2c97-814">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-815">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-815">Appservice</span></span>

* <span data-ttu-id="f2c97-816">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="f2c97-816">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="f2c97-817">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="f2c97-817">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="f2c97-818">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="f2c97-818">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="f2c97-819">Consumo</span><span class="sxs-lookup"><span data-stu-id="f2c97-819">Consumption</span></span>

* <span data-ttu-id="f2c97-820">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="f2c97-820">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="f2c97-821">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f2c97-821">Container</span></span>

* <span data-ttu-id="f2c97-822">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="f2c97-822">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="f2c97-823">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f2c97-823">Monitor</span></span>

* <span data-ttu-id="f2c97-824">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="f2c97-824">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="f2c97-825">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2c97-825">Resource</span></span>

* <span data-ttu-id="f2c97-826">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="f2c97-826">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="f2c97-827">Função</span><span class="sxs-lookup"><span data-stu-id="f2c97-827">Role</span></span>

* <span data-ttu-id="f2c97-828">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="f2c97-828">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="f2c97-829">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="f2c97-829">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="f2c97-830">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="f2c97-830">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="f2c97-831">SQL</span><span class="sxs-lookup"><span data-stu-id="f2c97-831">SQL</span></span>

* <span data-ttu-id="f2c97-832">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="f2c97-832">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="f2c97-833">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="f2c97-833">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-834">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-834">VM</span></span>

* <span data-ttu-id="f2c97-835">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="f2c97-835">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="f2c97-836">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="f2c97-836">November 14, 2017</span></span>

<span data-ttu-id="f2c97-837">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="f2c97-837">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="f2c97-838">ACR</span><span class="sxs-lookup"><span data-stu-id="f2c97-838">ACR</span></span>

* <span data-ttu-id="f2c97-839">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="f2c97-839">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="f2c97-840">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-840">ACS</span></span>

* <span data-ttu-id="f2c97-841">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="f2c97-841">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="f2c97-842">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-842">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="f2c97-843">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="f2c97-843">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="f2c97-844">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="f2c97-844">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="f2c97-845">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="f2c97-845">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-846">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-846">Appservice</span></span>

* <span data-ttu-id="f2c97-847">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="f2c97-847">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="f2c97-848">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="f2c97-848">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="f2c97-849">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="f2c97-849">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="f2c97-850">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="f2c97-850">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="f2c97-851">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="f2c97-851">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="f2c97-852">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="f2c97-852">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="f2c97-853">Lote</span><span class="sxs-lookup"><span data-stu-id="f2c97-853">Batch</span></span>

* <span data-ttu-id="f2c97-854">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="f2c97-854">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="f2c97-855">Batchai</span><span class="sxs-lookup"><span data-stu-id="f2c97-855">Batchai</span></span>

* <span data-ttu-id="f2c97-856">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-856">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="f2c97-857">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-857">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="f2c97-858">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="f2c97-858">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="f2c97-859">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-859">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="f2c97-860">Nuvem</span><span class="sxs-lookup"><span data-stu-id="f2c97-860">Cloud</span></span>

* <span data-ttu-id="f2c97-861">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="f2c97-861">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="f2c97-862">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f2c97-862">Container</span></span>

* <span data-ttu-id="f2c97-863">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="f2c97-863">Added support to open multiple ports</span></span>
* <span data-ttu-id="f2c97-864">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="f2c97-864">Added container group restart policy</span></span>
* <span data-ttu-id="f2c97-865">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="f2c97-865">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="f2c97-866">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="f2c97-866">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f2c97-867">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f2c97-867">Data Lake Analytics</span></span>

* <span data-ttu-id="f2c97-868">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="f2c97-868">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f2c97-869">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f2c97-869">Data Lake Store</span></span>

* <span data-ttu-id="f2c97-870">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="f2c97-870">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="f2c97-871">Extensão</span><span class="sxs-lookup"><span data-stu-id="f2c97-871">Extension</span></span>

* <span data-ttu-id="f2c97-872">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="f2c97-872">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="f2c97-873">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="f2c97-873">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="f2c97-874">IoT</span><span class="sxs-lookup"><span data-stu-id="f2c97-874">IoT</span></span>

* <span data-ttu-id="f2c97-875">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="f2c97-875">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="f2c97-876">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f2c97-876">Monitor</span></span>

* <span data-ttu-id="f2c97-877">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="f2c97-877">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="f2c97-878">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-878">Network</span></span>

* <span data-ttu-id="f2c97-879">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="f2c97-879">Added support for CAA DNS records</span></span>
* <span data-ttu-id="f2c97-880">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-880">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="f2c97-881">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="f2c97-881">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="f2c97-882">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="f2c97-882">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="f2c97-883">Reservas</span><span class="sxs-lookup"><span data-stu-id="f2c97-883">Reservations</span></span>

* <span data-ttu-id="f2c97-884">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="f2c97-884">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="f2c97-885">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2c97-885">Resource</span></span>

* <span data-ttu-id="f2c97-886">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="f2c97-886">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="f2c97-887">SQL</span><span class="sxs-lookup"><span data-stu-id="f2c97-887">SQL</span></span>

* <span data-ttu-id="f2c97-888">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-888">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="f2c97-889">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-889">Storage</span></span>

* <span data-ttu-id="f2c97-890">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="f2c97-890">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="f2c97-891">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="f2c97-891">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="f2c97-892">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="f2c97-892">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="f2c97-893">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="f2c97-893">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="f2c97-894">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-894">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="f2c97-895">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="f2c97-895">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="f2c97-896">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-896">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-897">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-897">VM</span></span>

* <span data-ttu-id="f2c97-898">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="f2c97-898">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="f2c97-899">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="f2c97-899">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="f2c97-900">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="f2c97-900">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="f2c97-901">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="f2c97-901">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="f2c97-902">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="f2c97-902">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="f2c97-903">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="f2c97-903">October 24, 2017</span></span>

<span data-ttu-id="f2c97-904">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="f2c97-904">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="f2c97-905">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2c97-905">Core</span></span>

* <span data-ttu-id="f2c97-906">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="f2c97-906">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="f2c97-907">ACR</span><span class="sxs-lookup"><span data-stu-id="f2c97-907">ACR</span></span>

* <span data-ttu-id="f2c97-908">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="f2c97-908">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="f2c97-909">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="f2c97-909">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="f2c97-910">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="f2c97-910">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-911">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-911">ACS</span></span>

* <span data-ttu-id="f2c97-912">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="f2c97-912">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="f2c97-913">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="f2c97-913">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-914">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-914">Appservice</span></span>

* <span data-ttu-id="f2c97-915">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="f2c97-915">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="f2c97-916">Componente</span><span class="sxs-lookup"><span data-stu-id="f2c97-916">Component</span></span>

* <span data-ttu-id="f2c97-917">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="f2c97-917">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="f2c97-918">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f2c97-918">Monitor</span></span>

* <span data-ttu-id="f2c97-919">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="f2c97-919">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="f2c97-920">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2c97-920">Resource</span></span>

* <span data-ttu-id="f2c97-921">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="f2c97-921">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="f2c97-922">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="f2c97-922">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-923">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-923">VM</span></span>

* <span data-ttu-id="f2c97-924">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-924">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="f2c97-925">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="f2c97-925">October 9, 2017</span></span>

<span data-ttu-id="f2c97-926">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="f2c97-926">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="f2c97-927">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2c97-927">Core</span></span>

* <span data-ttu-id="f2c97-928">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="f2c97-928">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-929">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-929">Appservice</span></span>

* <span data-ttu-id="f2c97-930">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-930">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="f2c97-931">Lote</span><span class="sxs-lookup"><span data-stu-id="f2c97-931">Batch</span></span>

* <span data-ttu-id="f2c97-932">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="f2c97-932">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="f2c97-933">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="f2c97-933">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="f2c97-934">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="f2c97-934">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="f2c97-935">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="f2c97-935">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="f2c97-936">Batchai</span><span class="sxs-lookup"><span data-stu-id="f2c97-936">Batchai</span></span>

* <span data-ttu-id="f2c97-937">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="f2c97-937">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="f2c97-938">Keyvault</span><span class="sxs-lookup"><span data-stu-id="f2c97-938">Keyvault</span></span>

* <span data-ttu-id="f2c97-939">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="f2c97-939">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="f2c97-940">(#4448)</span><span class="sxs-lookup"><span data-stu-id="f2c97-940">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="f2c97-941">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-941">Network</span></span>

* <span data-ttu-id="f2c97-942">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="f2c97-942">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="f2c97-943">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="f2c97-943">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="f2c97-944">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2c97-944">Resource</span></span>

* <span data-ttu-id="f2c97-945">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="f2c97-945">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="f2c97-946">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="f2c97-946">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="f2c97-947">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="f2c97-947">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="f2c97-948">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="f2c97-948">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="f2c97-949">Sql</span><span class="sxs-lookup"><span data-stu-id="f2c97-949">Sql</span></span>

* <span data-ttu-id="f2c97-950">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="f2c97-950">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="f2c97-951">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="f2c97-951">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="f2c97-952">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="f2c97-952">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="f2c97-953">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-953">Storage</span></span>

* <span data-ttu-id="f2c97-954">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="f2c97-954">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-955">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-955">Vm</span></span>

* <span data-ttu-id="f2c97-956">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="f2c97-956">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="f2c97-957">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-957">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="f2c97-958">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="f2c97-958">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="f2c97-959">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-959">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="f2c97-960">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-960">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="f2c97-961">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="f2c97-961">September 22, 2017</span></span>

<span data-ttu-id="f2c97-962">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="f2c97-962">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="f2c97-963">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2c97-963">Resource</span></span>

* <span data-ttu-id="f2c97-964">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="f2c97-964">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="f2c97-965">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="f2c97-965">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="f2c97-966">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-966">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="f2c97-967">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="f2c97-967">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="f2c97-968">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-968">Network</span></span>

* <span data-ttu-id="f2c97-969">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="f2c97-969">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="f2c97-970">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="f2c97-970">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="f2c97-971">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2c97-971">Added `asg` application security group commands</span></span>
* <span data-ttu-id="f2c97-972">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-972">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="f2c97-973">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-973">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="f2c97-974">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-974">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="f2c97-975">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-975">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f2c97-976">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-976">Storage</span></span>

* <span data-ttu-id="f2c97-977">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="f2c97-977">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="f2c97-978">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="f2c97-978">Eventgrid</span></span>

* <span data-ttu-id="f2c97-979">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="f2c97-979">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="f2c97-980">SQL</span><span class="sxs-lookup"><span data-stu-id="f2c97-980">SQL</span></span>

* <span data-ttu-id="f2c97-981">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="f2c97-981">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="f2c97-982">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="f2c97-982">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="f2c97-983">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-983">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="f2c97-984">Keyvault</span><span class="sxs-lookup"><span data-stu-id="f2c97-984">Keyvault</span></span>

* <span data-ttu-id="f2c97-985">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="f2c97-985">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-986">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-986">VM</span></span>

* <span data-ttu-id="f2c97-987">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-987">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="f2c97-988">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="f2c97-988">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="f2c97-989">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-989">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="f2c97-990">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="f2c97-990">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="f2c97-991">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="f2c97-991">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="f2c97-992">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="f2c97-992">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-993">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-993">ACS</span></span>

* <span data-ttu-id="f2c97-994">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-994">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-995">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-995">Appservice</span></span>

* <span data-ttu-id="f2c97-996">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-996">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="f2c97-997">Backup</span><span class="sxs-lookup"><span data-stu-id="f2c97-997">Backup</span></span>

* <span data-ttu-id="f2c97-998">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="f2c97-998">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="f2c97-999">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="f2c97-999">September 11, 2017</span></span>

<span data-ttu-id="f2c97-1000">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="f2c97-1000">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="f2c97-1001">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2c97-1001">Core</span></span>

* <span data-ttu-id="f2c97-1002">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="f2c97-1002">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="f2c97-1003">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="f2c97-1003">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-1004">Acs</span><span class="sxs-lookup"><span data-stu-id="f2c97-1004">Acs</span></span>

* <span data-ttu-id="f2c97-1005">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1005">Added `acs list-locations` command</span></span>
* <span data-ttu-id="f2c97-1006">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="f2c97-1006">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-1007">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-1007">Appservice</span></span>

* <span data-ttu-id="f2c97-1008">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="f2c97-1008">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="f2c97-1009">CDN</span><span class="sxs-lookup"><span data-stu-id="f2c97-1009">CDN</span></span>

* <span data-ttu-id="f2c97-1010">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1010">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="f2c97-1011">Extensão</span><span class="sxs-lookup"><span data-stu-id="f2c97-1011">Extension</span></span>

* <span data-ttu-id="f2c97-1012">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="f2c97-1012">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="f2c97-1013">Keyvault</span><span class="sxs-lookup"><span data-stu-id="f2c97-1013">Keyvault</span></span>

* <span data-ttu-id="f2c97-1014">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1014">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="f2c97-1015">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-1015">Network</span></span>

* <span data-ttu-id="f2c97-1016">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1016">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="f2c97-1017">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1017">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="f2c97-1018">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1018">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="f2c97-1019">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1019">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="f2c97-1020">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1020">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="f2c97-1021">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2c97-1021">Resource</span></span>

* <span data-ttu-id="f2c97-1022">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1022">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="f2c97-1023">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1023">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="f2c97-1024">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="f2c97-1024">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="f2c97-1025">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="f2c97-1025">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="f2c97-1026">SQL</span><span class="sxs-lookup"><span data-stu-id="f2c97-1026">SQL</span></span>

* <span data-ttu-id="f2c97-1027">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1027">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-1028">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-1028">VM</span></span>

* <span data-ttu-id="f2c97-1029">Corrigido: Não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="f2c97-1029">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="f2c97-1030">Corrigido: Usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="f2c97-1030">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="f2c97-1031">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1031">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="f2c97-1032">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="f2c97-1032">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="f2c97-1033">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="f2c97-1033">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="f2c97-1034">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="f2c97-1034">August 31, 2017</span></span>

<span data-ttu-id="f2c97-1035">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="f2c97-1035">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="f2c97-1036">Keyvault</span><span class="sxs-lookup"><span data-stu-id="f2c97-1036">Keyvault</span></span>

* <span data-ttu-id="f2c97-1037">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1037">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="f2c97-1038">Sf</span><span class="sxs-lookup"><span data-stu-id="f2c97-1038">Sf</span></span>

* <span data-ttu-id="f2c97-1039">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1039">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="f2c97-1040">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-1040">Storage</span></span>

* <span data-ttu-id="f2c97-1041">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="f2c97-1041">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="f2c97-1042">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="f2c97-1042">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="f2c97-1043">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="f2c97-1043">August 28, 2017</span></span>

<span data-ttu-id="f2c97-1044">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="f2c97-1044">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="f2c97-1045">CLI</span><span class="sxs-lookup"><span data-stu-id="f2c97-1045">CLI</span></span>

* <span data-ttu-id="f2c97-1046">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1046">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-1047">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-1047">ACS</span></span>

* <span data-ttu-id="f2c97-1048">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="f2c97-1048">Corrected preview regions</span></span>
* <span data-ttu-id="f2c97-1049">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1049">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="f2c97-1050">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="f2c97-1050">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-1051">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-1051">Appservice</span></span>

* <span data-ttu-id="f2c97-1052">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1052">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="f2c97-1053">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1053">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="f2c97-1054">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1054">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="f2c97-1055">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2c97-1055">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="f2c97-1056">Correção: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="f2c97-1056">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="f2c97-1057">IoT</span><span class="sxs-lookup"><span data-stu-id="f2c97-1057">IoT</span></span>

* <span data-ttu-id="f2c97-1058">Correção #3934: Criação de política não limpa as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="f2c97-1058">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="f2c97-1059">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-1059">Network</span></span>

* <span data-ttu-id="f2c97-1060">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1060">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="f2c97-1061">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1061">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="f2c97-1062">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1062">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="f2c97-1063">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1063">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="f2c97-1064">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1064">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="f2c97-1065">Perfil</span><span class="sxs-lookup"><span data-stu-id="f2c97-1065">Profile</span></span>

* <span data-ttu-id="f2c97-1066">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="f2c97-1066">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f2c97-1067">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f2c97-1067">Service Fabric</span></span>

* <span data-ttu-id="f2c97-1068">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="f2c97-1068">Preview release</span></span>
* <span data-ttu-id="f2c97-1069">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="f2c97-1069">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="f2c97-1070">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="f2c97-1070">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="f2c97-1071">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="f2c97-1071">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="f2c97-1072">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-1072">Storage</span></span>

* <span data-ttu-id="f2c97-1073">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="f2c97-1073">Enabled setting blob tier</span></span>
* <span data-ttu-id="f2c97-1074">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="f2c97-1074">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="f2c97-1075">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="f2c97-1075">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="f2c97-1076">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="f2c97-1076">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="f2c97-1077">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1077">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="f2c97-1078">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="f2c97-1078">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-1079">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-1079">VM</span></span>

* <span data-ttu-id="f2c97-1080">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1080">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="f2c97-1081">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="f2c97-1081">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="f2c97-1082">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1082">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="f2c97-1083">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="f2c97-1083">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="f2c97-1084">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="f2c97-1084">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="f2c97-1085">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1085">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="f2c97-1086">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="f2c97-1086">August 15, 2017</span></span>

<span data-ttu-id="f2c97-1087">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="f2c97-1087">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-1088">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-1088">ACS</span></span>

* <span data-ttu-id="f2c97-1089">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="f2c97-1089">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-1090">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-1090">Appservice</span></span>

* <span data-ttu-id="f2c97-1091">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="f2c97-1091">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="f2c97-1092">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="f2c97-1092">Event Grid</span></span>

* <span data-ttu-id="f2c97-1093">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="f2c97-1093">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="f2c97-1094">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="f2c97-1094">August 11, 2017</span></span>

<span data-ttu-id="f2c97-1095">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="f2c97-1095">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-1096">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-1096">ACS</span></span>

* <span data-ttu-id="f2c97-1097">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="f2c97-1097">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="f2c97-1098">Lote</span><span class="sxs-lookup"><span data-stu-id="f2c97-1098">Batch</span></span>

* <span data-ttu-id="f2c97-1099">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="f2c97-1099">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="f2c97-1100">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="f2c97-1100">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="f2c97-1101">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="f2c97-1101">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="f2c97-1102">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="f2c97-1102">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="f2c97-1103">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="f2c97-1103">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="f2c97-1104">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="f2c97-1104">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="f2c97-1105">Componente</span><span class="sxs-lookup"><span data-stu-id="f2c97-1105">Component</span></span>

* <span data-ttu-id="f2c97-1106">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="f2c97-1106">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="f2c97-1107">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f2c97-1107">Container</span></span>

* <span data-ttu-id="f2c97-1108">`create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="f2c97-1108">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="f2c97-1109">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f2c97-1109">Data Lake Store</span></span>

* <span data-ttu-id="f2c97-1110">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-1110">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="f2c97-1111">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="f2c97-1111">Event Grid</span></span>

* <span data-ttu-id="f2c97-1112">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="f2c97-1112">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="f2c97-1113">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-1113">Network</span></span>

* <span data-ttu-id="f2c97-1114">`lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="f2c97-1114">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="f2c97-1115">`application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="f2c97-1115">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="f2c97-1116">`application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="f2c97-1116">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="f2c97-1117">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1117">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="f2c97-1118">Perfil</span><span class="sxs-lookup"><span data-stu-id="f2c97-1118">Profile</span></span>

* <span data-ttu-id="f2c97-1119">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="f2c97-1119">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="f2c97-1120">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-1120">Storage</span></span>

* <span data-ttu-id="f2c97-1121">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="f2c97-1121">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-1122">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-1122">VM</span></span>

* <span data-ttu-id="f2c97-1123">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="f2c97-1123">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="f2c97-1124">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1124">Exposed `list-skus` command</span></span>
* <span data-ttu-id="f2c97-1125">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="f2c97-1125">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="f2c97-1126">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="f2c97-1126">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="f2c97-1127">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="f2c97-1127">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="f2c97-1128">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="f2c97-1128">July 28, 2017</span></span>

<span data-ttu-id="f2c97-1129">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="f2c97-1129">Version 2.0.12</span></span>

* <span data-ttu-id="f2c97-1130">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="f2c97-1130">Added container commands</span></span>
* <span data-ttu-id="f2c97-1131">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="f2c97-1131">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="f2c97-1132">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2c97-1132">Core</span></span>

* <span data-ttu-id="f2c97-1133">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="f2c97-1133">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="f2c97-1134">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="f2c97-1134">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="f2c97-1135">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="f2c97-1135">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="f2c97-1136">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1136">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="f2c97-1137">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="f2c97-1137">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="f2c97-1138">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1138">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="f2c97-1139">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1139">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="f2c97-1140">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1140">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="f2c97-1141">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1141">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="f2c97-1142">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="f2c97-1142">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="f2c97-1143">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="f2c97-1143">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="f2c97-1144">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1144">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="f2c97-1145">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="f2c97-1145">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="f2c97-1146">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="f2c97-1146">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="f2c97-1147">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="f2c97-1147">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="f2c97-1148">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1148">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="f2c97-1149">ACR</span><span class="sxs-lookup"><span data-stu-id="f2c97-1149">ACR</span></span>

* <span data-ttu-id="f2c97-1150">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="f2c97-1150">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="f2c97-1151">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="f2c97-1151">Support SKU update for managed registries</span></span>
* <span data-ttu-id="f2c97-1152">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="f2c97-1152">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="f2c97-1153">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="f2c97-1153">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="f2c97-1154">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="f2c97-1154">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="f2c97-1155">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="f2c97-1155">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-1156">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-1156">ACS</span></span>

* <span data-ttu-id="f2c97-1157">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="f2c97-1157">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-1158">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-1158">Appservice</span></span>

* <span data-ttu-id="f2c97-1159">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="f2c97-1159">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="f2c97-1160">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="f2c97-1160">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="f2c97-1161">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1161">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="f2c97-1162">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1162">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="f2c97-1163">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1163">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="f2c97-1164">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1164">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="f2c97-1165">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1165">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="f2c97-1166">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1166">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="f2c97-1167">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="f2c97-1167">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="f2c97-1168">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1168">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="f2c97-1169">Lote</span><span class="sxs-lookup"><span data-stu-id="f2c97-1169">Batch</span></span>

* <span data-ttu-id="f2c97-1170">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="f2c97-1170">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="f2c97-1171">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1171">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="f2c97-1172">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1172">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="f2c97-1173">CDN</span><span class="sxs-lookup"><span data-stu-id="f2c97-1173">CDN</span></span>

* <span data-ttu-id="f2c97-1174">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="f2c97-1174">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="f2c97-1175">Nuvem</span><span class="sxs-lookup"><span data-stu-id="f2c97-1175">Cloud</span></span>

* <span data-ttu-id="f2c97-1176">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="f2c97-1176">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="f2c97-1177">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="f2c97-1177">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="f2c97-1178">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="f2c97-1178">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="f2c97-1179">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="f2c97-1179">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="f2c97-1180">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1180">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f2c97-1181">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f2c97-1181">CosmosDB</span></span>

* <span data-ttu-id="f2c97-1182">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="f2c97-1182">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="f2c97-1183">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="f2c97-1183">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f2c97-1184">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f2c97-1184">Data Lake Analytics</span></span>

* <span data-ttu-id="f2c97-1185">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1185">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="f2c97-1186">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1186">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="f2c97-1187">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1187">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f2c97-1188">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f2c97-1188">Data Lake Store</span></span>

* <span data-ttu-id="f2c97-1189">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1189">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="f2c97-1190">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="f2c97-1190">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="f2c97-1191">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="f2c97-1191">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="f2c97-1192">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f2c97-1192">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="f2c97-1193">Interativo</span><span class="sxs-lookup"><span data-stu-id="f2c97-1193">Interactive</span></span>

* <span data-ttu-id="f2c97-1194">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="f2c97-1194">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="f2c97-1195">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="f2c97-1195">Increased test coverage</span></span>
* <span data-ttu-id="f2c97-1196">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="f2c97-1196">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="f2c97-1197">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1197">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="f2c97-1198">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1198">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="f2c97-1199">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1199">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="f2c97-1200">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1200">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="f2c97-1201">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1201">Added `--progress` flag</span></span>
* <span data-ttu-id="f2c97-1202">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="f2c97-1202">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="f2c97-1203">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1203">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="f2c97-1204">IoT</span><span class="sxs-lookup"><span data-stu-id="f2c97-1204">IoT</span></span>

* <span data-ttu-id="f2c97-1205">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="f2c97-1205">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="f2c97-1206">(#3934)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1206">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="f2c97-1207">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="f2c97-1207">Key vault</span></span>

* <span data-ttu-id="f2c97-1208">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="f2c97-1208">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="f2c97-1209">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1209">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="f2c97-1210">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1210">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="f2c97-1211">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1211">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="f2c97-1212">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1212">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="f2c97-1213">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1213">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="f2c97-1214">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="f2c97-1214">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="f2c97-1215">(#3307)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1215">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="f2c97-1216">Laboratório</span><span class="sxs-lookup"><span data-stu-id="f2c97-1216">Lab</span></span>

* <span data-ttu-id="f2c97-1217">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1217">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="f2c97-1218">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1218">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="f2c97-1219">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f2c97-1219">Monitor</span></span>

* <span data-ttu-id="f2c97-1220">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1220">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="f2c97-1221">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1221">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="f2c97-1222">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1222">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="f2c97-1223">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1223">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="f2c97-1224">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1224">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="f2c97-1225">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="f2c97-1225">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="f2c97-1226">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="f2c97-1226">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="f2c97-1227">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="f2c97-1227">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="f2c97-1228">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="f2c97-1228">`location` no longer required</span></span>
  * <span data-ttu-id="f2c97-1229">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="f2c97-1229">Add name and ID support for target</span></span>
  * <span data-ttu-id="f2c97-1230">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1230">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="f2c97-1231">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="f2c97-1231">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="f2c97-1232">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="f2c97-1232">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="f2c97-1233">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="f2c97-1233">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="f2c97-1234">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1234">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="f2c97-1235">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1235">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="f2c97-1236">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-1236">Network</span></span>

* <span data-ttu-id="f2c97-1237">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1237">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="f2c97-1238">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1238">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="f2c97-1239">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="f2c97-1239">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="f2c97-1240">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="f2c97-1240">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="f2c97-1241">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1241">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="f2c97-1242">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1242">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="f2c97-1243">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1243">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="f2c97-1244">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1244">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="f2c97-1245">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1245">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="f2c97-1246">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1246">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="f2c97-1247">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1247">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="f2c97-1248">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1248">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="f2c97-1249">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1249">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="f2c97-1250">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1250">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="f2c97-1251">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1251">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="f2c97-1252">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1252">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="f2c97-1253">Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS</span><span class="sxs-lookup"><span data-stu-id="f2c97-1253">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="f2c97-1254">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1254">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="f2c97-1255">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1255">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="f2c97-1256">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1256">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="f2c97-1257">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1257">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="f2c97-1258">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1258">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="f2c97-1259">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1259">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="f2c97-1260">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="f2c97-1260">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="f2c97-1261">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="f2c97-1261">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="f2c97-1262">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="f2c97-1262">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="f2c97-1263">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="f2c97-1263">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="f2c97-1264">Perfil</span><span class="sxs-lookup"><span data-stu-id="f2c97-1264">Profile</span></span>

* <span data-ttu-id="f2c97-1265">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="f2c97-1265">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="f2c97-1266">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="f2c97-1266">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="f2c97-1267">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="f2c97-1267">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="f2c97-1268">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="f2c97-1268">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="f2c97-1269">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="f2c97-1269">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="f2c97-1270">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f2c97-1270">RDBMS</span></span>

* <span data-ttu-id="f2c97-1271">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1271">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="f2c97-1272">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1272">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="f2c97-1273">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1273">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="f2c97-1274">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1274">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="f2c97-1275">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2c97-1275">Resource</span></span>

* <span data-ttu-id="f2c97-1276">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1276">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="f2c97-1277">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1277">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="f2c97-1278">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1278">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="f2c97-1279">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1279">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="f2c97-1280">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1280">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="f2c97-1281">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1281">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="f2c97-1282">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1282">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="f2c97-1283">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1283">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="f2c97-1284">Função</span><span class="sxs-lookup"><span data-stu-id="f2c97-1284">Role</span></span>

* <span data-ttu-id="f2c97-1285">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1285">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="f2c97-1286">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1286">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="f2c97-1287">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1287">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="f2c97-1288">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1288">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="f2c97-1289">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1289">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f2c97-1290">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f2c97-1290">Service Fabric</span></span>
* <span data-ttu-id="f2c97-1291">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1291">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="f2c97-1292">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1292">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="f2c97-1293">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1293">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="f2c97-1294">SQL</span><span class="sxs-lookup"><span data-stu-id="f2c97-1294">SQL</span></span>

* <span data-ttu-id="f2c97-1295">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1295">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="f2c97-1296">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1296">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="f2c97-1297">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1297">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="f2c97-1298">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-1298">Storage</span></span>

* <span data-ttu-id="f2c97-1299">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1299">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="f2c97-1300">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="f2c97-1300">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="f2c97-1301">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1301">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="f2c97-1302">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1302">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="f2c97-1303">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1303">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="f2c97-1304">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1304">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-1305">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-1305">VM</span></span>

* <span data-ttu-id="f2c97-1306">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="f2c97-1306">Support configuring nsg</span></span>
* <span data-ttu-id="f2c97-1307">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="f2c97-1307">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="f2c97-1308">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="f2c97-1308">Support managed service identities</span></span>
* <span data-ttu-id="f2c97-1309">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1309">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="f2c97-1310">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="f2c97-1310">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="f2c97-1311">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="f2c97-1311">May 10, 2017</span></span>

<span data-ttu-id="f2c97-1312">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="f2c97-1312">Version 2.0.6</span></span>

* <span data-ttu-id="f2c97-1313">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f2c97-1313">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="f2c97-1314">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1314">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="f2c97-1315">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f2c97-1315">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="f2c97-1316">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="f2c97-1316">Include Cognitive Services module</span></span>
* <span data-ttu-id="f2c97-1317">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f2c97-1317">Include Service Fabric module</span></span>
* <span data-ttu-id="f2c97-1318">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1318">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="f2c97-1319">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="f2c97-1319">Add support for CDN commands</span></span>
* <span data-ttu-id="f2c97-1320">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="f2c97-1320">Remove Container module</span></span>
* <span data-ttu-id="f2c97-1321">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1321">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="f2c97-1322">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1322">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="f2c97-1323">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2c97-1323">Core</span></span>

* <span data-ttu-id="f2c97-1324">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="f2c97-1324">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="f2c97-1325">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1325">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="f2c97-1326">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1326">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="f2c97-1327">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1327">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="f2c97-1328">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1328">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="f2c97-1329">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1329">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="f2c97-1330">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1330">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="f2c97-1331">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1331">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="f2c97-1332">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1332">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="f2c97-1333">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="f2c97-1333">core: Improved performance</span></span>
* <span data-ttu-id="f2c97-1334">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="f2c97-1334">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="f2c97-1335">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="f2c97-1335">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-1336">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-1336">ACS</span></span>

* <span data-ttu-id="f2c97-1337">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2c97-1337">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="f2c97-1338">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="f2c97-1338">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="f2c97-1339">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="f2c97-1339">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="f2c97-1340">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1340">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-1341">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-1341">AppService</span></span>

* <span data-ttu-id="f2c97-1342">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="f2c97-1342">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="f2c97-1343">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="f2c97-1343">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="f2c97-1344">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1344">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="f2c97-1345">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="f2c97-1345">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="f2c97-1346">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="f2c97-1346">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="f2c97-1347">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1347">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="f2c97-1348">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="f2c97-1348">support slot swap with preview</span></span>
* <span data-ttu-id="f2c97-1349">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1349">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="f2c97-1350">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1350">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f2c97-1351">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f2c97-1351">CosmosDB</span></span>

* <span data-ttu-id="f2c97-1352">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f2c97-1352">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="f2c97-1353">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="f2c97-1353">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="f2c97-1354">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="f2c97-1354">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="f2c97-1355">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="f2c97-1355">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f2c97-1356">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f2c97-1356">Data Lake Analytics</span></span>

* <span data-ttu-id="f2c97-1357">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="f2c97-1357">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="f2c97-1358">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="f2c97-1358">Add support for new catalog item type: package.</span></span> <span data-ttu-id="f2c97-1359">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1359">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="f2c97-1360">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="f2c97-1360">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="f2c97-1361">Tabela</span><span class="sxs-lookup"><span data-stu-id="f2c97-1361">Table</span></span>
  * <span data-ttu-id="f2c97-1362">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="f2c97-1362">Table valued function</span></span>
  * <span data-ttu-id="f2c97-1363">Visualizar</span><span class="sxs-lookup"><span data-stu-id="f2c97-1363">View</span></span>
  * <span data-ttu-id="f2c97-1364">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="f2c97-1364">Table Statistics.</span></span> <span data-ttu-id="f2c97-1365">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="f2c97-1365">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f2c97-1366">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f2c97-1366">Data Lake Store</span></span>

* <span data-ttu-id="f2c97-1367">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="f2c97-1367">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="f2c97-1368">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1368">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="f2c97-1369">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="f2c97-1369">missed help for access show.</span></span> <span data-ttu-id="f2c97-1370">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="f2c97-1370">adding it.</span></span> <span data-ttu-id="f2c97-1371">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1371">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="f2c97-1372">Localizar</span><span class="sxs-lookup"><span data-stu-id="f2c97-1372">Find</span></span>

* <span data-ttu-id="f2c97-1373">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="f2c97-1373">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="f2c97-1374">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f2c97-1374">KeyVault</span></span>

* <span data-ttu-id="f2c97-1375">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="f2c97-1375">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="f2c97-1376">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="f2c97-1376">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="f2c97-1377">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="f2c97-1377">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="f2c97-1378">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="f2c97-1378">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="f2c97-1379">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1379">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="f2c97-1380">Laboratório</span><span class="sxs-lookup"><span data-stu-id="f2c97-1380">Lab</span></span>

* <span data-ttu-id="f2c97-1381">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="f2c97-1381">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="f2c97-1382">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="f2c97-1382">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="f2c97-1383">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="f2c97-1383">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="f2c97-1384">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="f2c97-1384">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="f2c97-1385">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="f2c97-1385">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="f2c97-1386">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f2c97-1386">Monitor</span></span>

* <span data-ttu-id="f2c97-1387">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1387">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="f2c97-1388">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1388">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="f2c97-1389">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-1389">Network</span></span>

* <span data-ttu-id="f2c97-1390">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1390">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="f2c97-1391">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1391">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="f2c97-1392">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2c97-1392">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="f2c97-1393">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2c97-1393">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="f2c97-1394">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="f2c97-1394">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="f2c97-1395">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="f2c97-1395">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="f2c97-1396">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="f2c97-1396">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="f2c97-1397">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="f2c97-1397">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="f2c97-1398">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1398">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="f2c97-1399">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="f2c97-1399">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="f2c97-1400">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1400">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="f2c97-1401">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1401">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="f2c97-1402">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="f2c97-1402">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="f2c97-1403">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="f2c97-1403">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="f2c97-1404">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="f2c97-1404">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="f2c97-1405">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="f2c97-1405">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="f2c97-1406">Perfil</span><span class="sxs-lookup"><span data-stu-id="f2c97-1406">Profile</span></span>

* <span data-ttu-id="f2c97-1407">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1407">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="f2c97-1408">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1408">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="f2c97-1409">Redis</span><span class="sxs-lookup"><span data-stu-id="f2c97-1409">Redis</span></span>

* <span data-ttu-id="f2c97-1410">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="f2c97-1410">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="f2c97-1411">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="f2c97-1411">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="f2c97-1412">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2c97-1412">Resource</span></span>

* <span data-ttu-id="f2c97-1413">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1413">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="f2c97-1414">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1414">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="f2c97-1415">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1415">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="f2c97-1416">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="f2c97-1416">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="f2c97-1417">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1417">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="f2c97-1418">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="f2c97-1418">Add docs for az lock update.</span></span> <span data-ttu-id="f2c97-1419">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1419">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="f2c97-1420">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="f2c97-1420">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="f2c97-1421">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1421">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="f2c97-1422">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="f2c97-1422">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="f2c97-1423">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1423">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="f2c97-1424">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1424">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="f2c97-1425">Função</span><span class="sxs-lookup"><span data-stu-id="f2c97-1425">Role</span></span>

* <span data-ttu-id="f2c97-1426">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1426">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="f2c97-1427">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1427">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="f2c97-1428">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1428">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="f2c97-1429">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="f2c97-1429">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="f2c97-1430">SQL</span><span class="sxs-lookup"><span data-stu-id="f2c97-1430">SQL</span></span>

* <span data-ttu-id="f2c97-1431">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="f2c97-1431">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="f2c97-1432">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1432">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="f2c97-1433">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-1433">Storage</span></span>

* <span data-ttu-id="f2c97-1434">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1434">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="f2c97-1435">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="f2c97-1435">Add support for incremental blob copy</span></span>
* <span data-ttu-id="f2c97-1436">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="f2c97-1436">Add support for large block blob upload</span></span>
* <span data-ttu-id="f2c97-1437">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="f2c97-1437">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-1438">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-1438">VM</span></span>

* <span data-ttu-id="f2c97-1439">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="f2c97-1439">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="f2c97-1440">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="f2c97-1440">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="f2c97-1441">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="f2c97-1441">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="f2c97-1442">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="f2c97-1442">az vm/vmss disk</span></span>
  3. <span data-ttu-id="f2c97-1443">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="f2c97-1443">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="f2c97-1444">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="f2c97-1444">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="f2c97-1445">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1445">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="f2c97-1446">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="f2c97-1446">April 3, 2017</span></span>

<span data-ttu-id="f2c97-1447">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="f2c97-1447">Version 2.0.2</span></span>

<span data-ttu-id="f2c97-1448">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="f2c97-1448">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="f2c97-1449">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2c97-1449">Core</span></span>

* <span data-ttu-id="f2c97-1450">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="f2c97-1450">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="f2c97-1451">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1451">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="f2c97-1452">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1452">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="f2c97-1453">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1453">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="f2c97-1454">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1454">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="f2c97-1455">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="f2c97-1455">Add prompting for missing template parameters.</span></span> <span data-ttu-id="f2c97-1456">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1456">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="f2c97-1457">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="f2c97-1457">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="f2c97-1458">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="f2c97-1458">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="f2c97-1459">ACS</span><span class="sxs-lookup"><span data-stu-id="f2c97-1459">ACS</span></span>

* <span data-ttu-id="f2c97-1460">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1460">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="f2c97-1461">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="f2c97-1461">Add support for ssh key password prompting.</span></span> <span data-ttu-id="f2c97-1462">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1462">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="f2c97-1463">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="f2c97-1463">Add support for windows clusters.</span></span> <span data-ttu-id="f2c97-1464">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1464">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="f2c97-1465">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="f2c97-1465">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="f2c97-1466">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1466">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="f2c97-1467">AppService</span><span class="sxs-lookup"><span data-stu-id="f2c97-1467">AppService</span></span>

* <span data-ttu-id="f2c97-1468">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1468">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="f2c97-1469">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1469">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="f2c97-1470">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1470">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="f2c97-1471">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1471">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="f2c97-1472">DataLake</span><span class="sxs-lookup"><span data-stu-id="f2c97-1472">DataLake</span></span>

* <span data-ttu-id="f2c97-1473">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f2c97-1473">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="f2c97-1474">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f2c97-1474">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="f2c97-1475">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="f2c97-1475">DocuemntDB</span></span>

* <span data-ttu-id="f2c97-1476">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1476">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="f2c97-1477">VM</span><span class="sxs-lookup"><span data-stu-id="f2c97-1477">VM</span></span>

* <span data-ttu-id="f2c97-1478">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1478">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="f2c97-1479">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1479">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="f2c97-1480">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1480">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="f2c97-1481">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1481">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="f2c97-1482">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1482">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="f2c97-1483">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1483">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="f2c97-1484">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="f2c97-1484">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="f2c97-1485">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="f2c97-1485">February 27, 2017</span></span>

<span data-ttu-id="f2c97-1486">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="f2c97-1486">Version 2.0.0</span></span>

<span data-ttu-id="f2c97-1487">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="f2c97-1487">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="f2c97-1488">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1488">Container Service (acs)</span></span>
- <span data-ttu-id="f2c97-1489">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1489">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="f2c97-1490">Rede</span><span class="sxs-lookup"><span data-stu-id="f2c97-1490">Networking</span></span>
- <span data-ttu-id="f2c97-1491">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2c97-1491">Storage</span></span>

<span data-ttu-id="f2c97-1492">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1492">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="f2c97-1493">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="f2c97-1493">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="f2c97-1494">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="f2c97-1494">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="f2c97-1495">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="f2c97-1495">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="f2c97-1496">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1496">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="f2c97-1497">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="f2c97-1497">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="f2c97-1498">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1498">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="f2c97-1499">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="f2c97-1499">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="f2c97-1500">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="f2c97-1500">Provide feedback from the command line with the `az feedback` command</span></span>

