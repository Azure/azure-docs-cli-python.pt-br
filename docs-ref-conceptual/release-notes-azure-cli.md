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
ms.openlocfilehash: d0f8c01495cc95ecfbf6a41d510eb4bc54d47ba2
ms.sourcegitcommit: 8019690502e9f89c083839d83a0a245cc812e8b6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2018
ms.locfileid: "39392346"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="e00df-103">Notas de versão da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="e00df-103">Azure CLI 2.0 release notes</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="e00df-104">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="e00df-104">July 31, 2018</span></span>

<span data-ttu-id="e00df-105">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="e00df-105">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="e00df-106">ACR</span><span class="sxs-lookup"><span data-stu-id="e00df-106">ACR</span></span>

* <span data-ttu-id="e00df-107">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="e00df-107">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="e00df-108">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="e00df-108">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-109">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-109">ACS</span></span>

* <span data-ttu-id="e00df-110">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="e00df-110">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="e00df-111">Lote</span><span class="sxs-lookup"><span data-stu-id="e00df-111">Batch</span></span>

* <span data-ttu-id="e00df-112">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="e00df-112">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="e00df-113">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e00df-113">Container</span></span>

* <span data-ttu-id="e00df-114">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="e00df-114">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="e00df-115">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-115">Network</span></span>

* <span data-ttu-id="e00df-116">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="e00df-116">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="e00df-117">Recurso</span><span class="sxs-lookup"><span data-stu-id="e00df-117">Resource</span></span>

* <span data-ttu-id="e00df-118">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="e00df-118">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="e00df-119">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="e00df-119">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="e00df-120">Função</span><span class="sxs-lookup"><span data-stu-id="e00df-120">Role</span></span>

* <span data-ttu-id="e00df-121">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="e00df-121">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="e00df-122">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="e00df-122">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="e00df-123">Search</span><span class="sxs-lookup"><span data-stu-id="e00df-123">Search</span></span>

* <span data-ttu-id="e00df-124">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="e00df-124">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="e00df-125">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="e00df-125">Service Bus</span></span>

* <span data-ttu-id="e00df-126">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="e00df-126">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="e00df-127">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="e00df-127">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="e00df-128">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="e00df-128">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="e00df-129">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="e00df-129">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="e00df-130">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-130">Storage</span></span>

* <span data-ttu-id="e00df-131">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="e00df-131">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="e00df-132">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="e00df-132">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-133">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-133">VM</span></span>

* <span data-ttu-id="e00df-134">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="e00df-134">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="e00df-135">Suporte adicionado para o suporte `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="e00df-135">Added support for support `StandardSSD_LRS`</span></span>
* <span data-ttu-id="e00df-136">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="e00df-136">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="e00df-137">[ALTERAÇÃO SIGNIFICATIVA] `[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="e00df-137">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="e00df-138">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="e00df-138">July 18, 2018</span></span>

<span data-ttu-id="e00df-139">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="e00df-139">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="e00df-140">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e00df-140">Core</span></span>

* <span data-ttu-id="e00df-141">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="e00df-141">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="e00df-142">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="e00df-142">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="e00df-143">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="e00df-143">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="e00df-144">ACR</span><span class="sxs-lookup"><span data-stu-id="e00df-144">ACR</span></span>

* <span data-ttu-id="e00df-145">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="e00df-145">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="e00df-146">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="e00df-146">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="e00df-147">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="e00df-147">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="e00df-148">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="e00df-148">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-149">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-149">ACS</span></span>

* <span data-ttu-id="e00df-150">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="e00df-150">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-151">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-151">AppService</span></span>

* <span data-ttu-id="e00df-152">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="e00df-152">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="e00df-153">Lote</span><span class="sxs-lookup"><span data-stu-id="e00df-153">Batch</span></span>

* <span data-ttu-id="e00df-154">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e00df-154">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="e00df-155">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="e00df-155">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e00df-156">Lote AI</span><span class="sxs-lookup"><span data-stu-id="e00df-156">Batch AI</span></span>

* <span data-ttu-id="e00df-157">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="e00df-157">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="e00df-158">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e00df-158">Container</span></span>

* <span data-ttu-id="e00df-159">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="e00df-159">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="e00df-160">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="e00df-160">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="e00df-161">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-161">Network</span></span>

* <span data-ttu-id="e00df-162">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="e00df-162">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="e00df-163">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="e00df-163">Added `network nic wait`</span></span>
* <span data-ttu-id="e00df-164">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="e00df-164">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="e00df-165">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="e00df-165">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="e00df-166">Recurso</span><span class="sxs-lookup"><span data-stu-id="e00df-166">Resource</span></span>

* <span data-ttu-id="e00df-167">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="e00df-167">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="e00df-168">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="e00df-168">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="e00df-169">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="e00df-169">Added `deployment wait` command</span></span>
* <span data-ttu-id="e00df-170">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="e00df-170">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="e00df-171">SQL</span><span class="sxs-lookup"><span data-stu-id="e00df-171">SQL</span></span>

* <span data-ttu-id="e00df-172">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="e00df-172">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="e00df-173">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="e00df-173">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="e00df-174">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="e00df-174">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e00df-175">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-175">Storage</span></span>

* <span data-ttu-id="e00df-176">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="e00df-176">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-177">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-177">VM</span></span>

* <span data-ttu-id="e00df-178">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="e00df-178">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="e00df-179">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="e00df-179">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="e00df-180">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="e00df-180">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="e00df-181">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="e00df-181">July 3, 2018</span></span>

<span data-ttu-id="e00df-182">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="e00df-182">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="e00df-183">AKS</span><span class="sxs-lookup"><span data-stu-id="e00df-183">AKS</span></span>

* <span data-ttu-id="e00df-184">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="e00df-184">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="e00df-185">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="e00df-185">July 3, 2018</span></span>

<span data-ttu-id="e00df-186">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="e00df-186">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="e00df-187">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e00df-187">Core</span></span>

* <span data-ttu-id="e00df-188">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="e00df-188">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="e00df-189">ACR</span><span class="sxs-lookup"><span data-stu-id="e00df-189">ACR</span></span>

* <span data-ttu-id="e00df-190">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="e00df-190">Added polling build status</span></span>
* <span data-ttu-id="e00df-191">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="e00df-191">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="e00df-192">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="e00df-192">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-193">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-193">ACS</span></span>

* <span data-ttu-id="e00df-194">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="e00df-194">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="e00df-195">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="e00df-195">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="e00df-196">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="e00df-196">Updated options for `aks browse` command.</span></span> <span data-ttu-id="e00df-197">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="e00df-197">Added `--listen-port` support</span></span>
* <span data-ttu-id="e00df-198">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="e00df-198">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="e00df-199">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="e00df-199">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="e00df-200">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="e00df-200">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-201">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-201">AppService</span></span>

* <span data-ttu-id="e00df-202">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="e00df-202">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="e00df-203">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="e00df-203">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="e00df-204">Backup</span><span class="sxs-lookup"><span data-stu-id="e00df-204">Backup</span></span>

* <span data-ttu-id="e00df-205">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="e00df-205">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="e00df-206">BatchAI</span><span class="sxs-lookup"><span data-stu-id="e00df-206">BatchAI</span></span>

* <span data-ttu-id="e00df-207">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="e00df-207">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="e00df-208">Nuvem</span><span class="sxs-lookup"><span data-stu-id="e00df-208">Cloud</span></span>

* <span data-ttu-id="e00df-209">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="e00df-209">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="e00df-210">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e00df-210">Container</span></span>

* <span data-ttu-id="e00df-211">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="e00df-211">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="e00df-212">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="e00df-212">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="e00df-213">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="e00df-213">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="e00df-214">Extensão</span><span class="sxs-lookup"><span data-stu-id="e00df-214">Extension</span></span>

* <span data-ttu-id="e00df-215">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="e00df-215">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="e00df-216">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-216">Network</span></span>

* <span data-ttu-id="e00df-217">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="e00df-217">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="e00df-218">Rdbms</span><span class="sxs-lookup"><span data-stu-id="e00df-218">Rdbms</span></span>

* <span data-ttu-id="e00df-219">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="e00df-219">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="e00df-220">Recurso</span><span class="sxs-lookup"><span data-stu-id="e00df-220">Resource</span></span>

* <span data-ttu-id="e00df-221">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="e00df-221">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-222">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-222">VM</span></span>

* <span data-ttu-id="e00df-223">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="e00df-223">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="e00df-224">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="e00df-224">June 25, 2018</span></span>

<span data-ttu-id="e00df-225">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="e00df-225">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="e00df-226">CLI</span><span class="sxs-lookup"><span data-stu-id="e00df-226">CLI</span></span>

* <span data-ttu-id="e00df-227">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="e00df-227">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="e00df-228">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="e00df-228">June 19, 2018</span></span>

<span data-ttu-id="e00df-229">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="e00df-229">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="e00df-230">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e00df-230">Core</span></span>

* <span data-ttu-id="e00df-231">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="e00df-231">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="e00df-232">ACR</span><span class="sxs-lookup"><span data-stu-id="e00df-232">ACR</span></span>

* <span data-ttu-id="e00df-233">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="e00df-233">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="e00df-234">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="e00df-234">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-235">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-235">ACS</span></span>

* <span data-ttu-id="e00df-236">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="e00df-236">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="e00df-237">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="e00df-237">Added `--update` support</span></span>
* <span data-ttu-id="e00df-238">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="e00df-238">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="e00df-239">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="e00df-239">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="e00df-240">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="e00df-240">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="e00df-241">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="e00df-241">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="e00df-242">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="e00df-242">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="e00df-243">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="e00df-243">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-244">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-244">AppService</span></span>

* <span data-ttu-id="e00df-245">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="e00df-245">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="e00df-246">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="e00df-246">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="e00df-247">Lote</span><span class="sxs-lookup"><span data-stu-id="e00df-247">Batch</span></span>

* <span data-ttu-id="e00df-248">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="e00df-248">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e00df-249">Lote AI</span><span class="sxs-lookup"><span data-stu-id="e00df-249">Batch AI</span></span>

* <span data-ttu-id="e00df-250">Foi adicionado suporte aos espaços de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e00df-250">Added support for workspaces.</span></span> <span data-ttu-id="e00df-251">Os espaços de trabalho permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="e00df-251">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="e00df-252">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="e00df-252">Added support for experiments.</span></span> <span data-ttu-id="e00df-253">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="e00df-253">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="e00df-254">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="e00df-254">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="e00df-255">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="e00df-255">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="e00df-256">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="e00df-256">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="e00df-257">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="e00df-257">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="e00df-258">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos espaços de trabalho</span><span class="sxs-lookup"><span data-stu-id="e00df-258">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="e00df-259">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="e00df-259">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="e00df-260">[ALTERAÇÃO SIGNIFICATIVA] `--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="e00df-260">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="e00df-261">Para montar um NFS pertencente a outro espaço de trabalho/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="e00df-261">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="e00df-262">[ALTERAÇÃO SIGNIFICATIVA] `--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="e00df-262">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="e00df-263">Para enviar um trabalho em um cluster pertencente a outro espaço de trabalho/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="e00df-263">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="e00df-264">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="e00df-264">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="e00df-265">Agora, o local é um atributo de um espaço de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e00df-265">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="e00df-266">[ALTERAÇÃO SIGNIFICATIVA] `--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="e00df-266">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="e00df-267">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="e00df-267">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="e00df-268">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="e00df-268">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="e00df-269">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="e00df-269">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="e00df-270">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="e00df-270">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="e00df-271">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="e00df-271">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="e00df-272">Mapas</span><span class="sxs-lookup"><span data-stu-id="e00df-272">Maps</span></span>

* <span data-ttu-id="e00df-273">[ALTERAÇÃO SIGNIFICATIVA] `maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="e00df-273">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="e00df-274">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-274">Network</span></span>

* <span data-ttu-id="e00df-275">Foi adicionado suporte a `https` para `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="e00df-275">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="e00df-276">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="e00df-276">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="e00df-277">#6502</span><span class="sxs-lookup"><span data-stu-id="e00df-277">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="e00df-278">Reservas</span><span class="sxs-lookup"><span data-stu-id="e00df-278">Reservations</span></span>

* <span data-ttu-id="e00df-279">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="e00df-279">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="e00df-280">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="e00df-280">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="e00df-281">[ALTERAÇÃO SIGNIFICATIVA] `kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="e00df-281">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="e00df-282">[ALTERAÇÃO SIGNIFICATIVA] `capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="e00df-282">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="e00df-283">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="e00df-283">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="e00df-284">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="e00df-284">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="e00df-285">Função</span><span class="sxs-lookup"><span data-stu-id="e00df-285">Role</span></span>

* <span data-ttu-id="e00df-286">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="e00df-286">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="e00df-287">SQL</span><span class="sxs-lookup"><span data-stu-id="e00df-287">SQL</span></span>

* <span data-ttu-id="e00df-288">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="e00df-288">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="e00df-289">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-289">Storage</span></span>

* <span data-ttu-id="e00df-290">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="e00df-290">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-291">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-291">VM</span></span>

* <span data-ttu-id="e00df-292">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="e00df-292">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="e00df-293">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="e00df-293">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="e00df-294">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="e00df-294">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="e00df-295">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="e00df-295">June 13, 2018</span></span>

<span data-ttu-id="e00df-296">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="e00df-296">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="e00df-297">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e00df-297">Core</span></span>

* <span data-ttu-id="e00df-298">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="e00df-298">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="e00df-299">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="e00df-299">June 13, 2018</span></span>

<span data-ttu-id="e00df-300">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="e00df-300">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="e00df-301">AKS</span><span class="sxs-lookup"><span data-stu-id="e00df-301">AKS</span></span>

* <span data-ttu-id="e00df-302">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="e00df-302">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="e00df-303">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="e00df-303">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="e00df-304">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="e00df-304">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="e00df-305">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="e00df-305">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="e00df-306">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="e00df-306">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-307">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-307">AppService</span></span>

* <span data-ttu-id="e00df-308">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="e00df-308">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="e00df-309">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="e00df-309">June 5, 2018</span></span>

<span data-ttu-id="e00df-310">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="e00df-310">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="e00df-311">Interativo</span><span class="sxs-lookup"><span data-stu-id="e00df-311">Interactive</span></span>

* <span data-ttu-id="e00df-312">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="e00df-312">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="e00df-313">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="e00df-313">June 5, 2018</span></span>

<span data-ttu-id="e00df-314">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="e00df-314">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="e00df-315">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e00df-315">Core</span></span>

* <span data-ttu-id="e00df-316">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="e00df-316">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="e00df-317">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="e00df-317">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="e00df-318">ACR</span><span class="sxs-lookup"><span data-stu-id="e00df-318">ACR</span></span>

* <span data-ttu-id="e00df-319">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="e00df-319">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="e00df-320">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="e00df-320">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="e00df-321">AKS</span><span class="sxs-lookup"><span data-stu-id="e00df-321">AKS</span></span>

* <span data-ttu-id="e00df-322">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="e00df-322">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="e00df-323">Lote</span><span class="sxs-lookup"><span data-stu-id="e00df-323">Batch</span></span>

* <span data-ttu-id="e00df-324">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="e00df-324">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="e00df-325">IOT</span><span class="sxs-lookup"><span data-stu-id="e00df-325">IOT</span></span>

* <span data-ttu-id="e00df-326">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="e00df-326">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="e00df-327">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-327">Network</span></span>

* <span data-ttu-id="e00df-328">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="e00df-328">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="e00df-329">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="e00df-329">Policy Insights</span></span>

* <span data-ttu-id="e00df-330">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="e00df-330">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="e00df-331">ARM</span><span class="sxs-lookup"><span data-stu-id="e00df-331">ARM</span></span>

* <span data-ttu-id="e00df-332">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="e00df-332">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="e00df-333">SQL</span><span class="sxs-lookup"><span data-stu-id="e00df-333">SQL</span></span>

* <span data-ttu-id="e00df-334">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="e00df-334">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="e00df-335">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="e00df-335">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="e00df-336">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-336">Storage</span></span>

* <span data-ttu-id="e00df-337">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="e00df-337">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-338">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-338">VM</span></span>

* <span data-ttu-id="e00df-339">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="e00df-339">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="e00df-340">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="e00df-340">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="e00df-341">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="e00df-341">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="e00df-342">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="e00df-342">May 22, 2018</span></span>

<span data-ttu-id="e00df-343">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="e00df-343">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="e00df-344">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e00df-344">Core</span></span>

* <span data-ttu-id="e00df-345">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="e00df-345">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-346">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-346">ACS</span></span>

* <span data-ttu-id="e00df-347">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="e00df-347">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="e00df-348">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="e00df-348">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-349">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-349">AppService</span></span>

* <span data-ttu-id="e00df-350">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="e00df-350">Improved generic update commands</span></span>
* <span data-ttu-id="e00df-351">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="e00df-351">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="e00df-352">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e00df-352">Container</span></span>

* <span data-ttu-id="e00df-353">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="e00df-353">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="e00df-354">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="e00df-354">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="e00df-355">Extensão</span><span class="sxs-lookup"><span data-stu-id="e00df-355">Extension</span></span>

* <span data-ttu-id="e00df-356">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="e00df-356">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="e00df-357">Interativo</span><span class="sxs-lookup"><span data-stu-id="e00df-357">Interactive</span></span>

* <span data-ttu-id="e00df-358">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="e00df-358">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="e00df-359">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="e00df-359">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="e00df-360">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e00df-360">KeyVault</span></span>

* <span data-ttu-id="e00df-361">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="e00df-361">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="e00df-362">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-362">Network</span></span>

* <span data-ttu-id="e00df-363">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="e00df-363">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="e00df-364">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="e00df-364">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="e00df-365">SQL</span><span class="sxs-lookup"><span data-stu-id="e00df-365">SQL</span></span>

* <span data-ttu-id="e00df-366">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="e00df-366">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="e00df-367">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="e00df-367">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="e00df-368">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="e00df-368">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="e00df-369">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e00df-369">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="e00df-370">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="e00df-370">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="e00df-371">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="e00df-371">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="e00df-372">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="e00df-372">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="e00df-373">`edition`.</span><span class="sxs-lookup"><span data-stu-id="e00df-373">`edition`.</span></span> <span data-ttu-id="e00df-374">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="e00df-374">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="e00df-375">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="e00df-375">`elasticPoolName`.</span></span> <span data-ttu-id="e00df-376">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="e00df-376">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="e00df-377">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="e00df-377">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="e00df-378">`edition`.</span><span class="sxs-lookup"><span data-stu-id="e00df-378">`edition`.</span></span> <span data-ttu-id="e00df-379">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="e00df-379">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="e00df-380">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="e00df-380">`dtu`.</span></span> <span data-ttu-id="e00df-381">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="e00df-381">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="e00df-382">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="e00df-382">`databaseDtuMin`.</span></span> <span data-ttu-id="e00df-383">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="e00df-383">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="e00df-384">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="e00df-384">`databaseDtuMax`.</span></span> <span data-ttu-id="e00df-385">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="e00df-385">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="e00df-386">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="e00df-386">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="e00df-387">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="e00df-387">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="e00df-388">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-388">Storage</span></span>

* <span data-ttu-id="e00df-389">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="e00df-389">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="e00df-390">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="e00df-390">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-391">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-391">VM</span></span>

* <span data-ttu-id="e00df-392">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="e00df-392">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="e00df-393">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="e00df-393">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="e00df-394">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="e00df-394">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="e00df-395">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="e00df-395">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="e00df-396">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="e00df-396">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="e00df-397">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="e00df-397">May 7, 2018</span></span>

<span data-ttu-id="e00df-398">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="e00df-398">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="e00df-399">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e00df-399">Core</span></span>

* <span data-ttu-id="e00df-400">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="e00df-400">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="e00df-401">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="e00df-401">Added limited support for positional arguments</span></span>
* <span data-ttu-id="e00df-402">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="e00df-402">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="e00df-403">#5591</span><span class="sxs-lookup"><span data-stu-id="e00df-403">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="e00df-404">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="e00df-404">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="e00df-405">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="e00df-405">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="e00df-406">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="e00df-406">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="e00df-407">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="e00df-407">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="e00df-408">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="e00df-408">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="e00df-409">ACR</span><span class="sxs-lookup"><span data-stu-id="e00df-409">ACR</span></span>

* <span data-ttu-id="e00df-410">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="e00df-410">Added ACR Build commands</span></span>
* <span data-ttu-id="e00df-411">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="e00df-411">Improved resource not found error messages</span></span>
* <span data-ttu-id="e00df-412">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="e00df-412">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="e00df-413">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="e00df-413">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="e00df-414">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="e00df-414">Improved repository commands error messages</span></span>
* <span data-ttu-id="e00df-415">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="e00df-415">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-416">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-416">ACS</span></span>

* <span data-ttu-id="e00df-417">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="e00df-417">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="e00df-418">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="e00df-418">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="e00df-419">AMS</span><span class="sxs-lookup"><span data-stu-id="e00df-419">AMS</span></span>

* <span data-ttu-id="e00df-420">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="e00df-420">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-421">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-421">Appservice</span></span>

* <span data-ttu-id="e00df-422">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="e00df-422">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="e00df-423">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="e00df-423">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="e00df-424">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="e00df-424">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="e00df-425">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="e00df-425">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e00df-426">Lote AI</span><span class="sxs-lookup"><span data-stu-id="e00df-426">Batch AI</span></span>

* <span data-ttu-id="e00df-427">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="e00df-427">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e00df-428">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="e00df-428">Cognitive Services</span></span>

* <span data-ttu-id="e00df-429">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="e00df-429">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="e00df-430">Consumo</span><span class="sxs-lookup"><span data-stu-id="e00df-430">Consumption</span></span>

* <span data-ttu-id="e00df-431">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="e00df-431">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="e00df-432">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e00df-432">Container</span></span>

* <span data-ttu-id="e00df-433">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="e00df-433">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="e00df-434">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e00df-434">Cosmos DB</span></span>

* <span data-ttu-id="e00df-435">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e00df-435">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="e00df-436">DMS</span><span class="sxs-lookup"><span data-stu-id="e00df-436">DMS</span></span>

* <span data-ttu-id="e00df-437">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="e00df-437">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="e00df-438">Extensão</span><span class="sxs-lookup"><span data-stu-id="e00df-438">Extension</span></span>

* <span data-ttu-id="e00df-439">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="e00df-439">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="e00df-440">Interativo</span><span class="sxs-lookup"><span data-stu-id="e00df-440">Interactive</span></span>

* <span data-ttu-id="e00df-441">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="e00df-441">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="e00df-442">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="e00df-442">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="e00df-443">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="e00df-443">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="e00df-444">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="e00df-444">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="e00df-445">Laboratório</span><span class="sxs-lookup"><span data-stu-id="e00df-445">Lab</span></span>

* <span data-ttu-id="e00df-446">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="e00df-446">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="e00df-447">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-447">Network</span></span>

* <span data-ttu-id="e00df-448">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="e00df-448">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="e00df-449">Perfil</span><span class="sxs-lookup"><span data-stu-id="e00df-449">Profile</span></span>

* <span data-ttu-id="e00df-450">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="e00df-450">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="e00df-451">[ALTERAÇÃO SIGNIFICATIVA] `--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="e00df-451">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="e00df-452">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="e00df-452">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="e00df-453">Redis</span><span class="sxs-lookup"><span data-stu-id="e00df-453">Redis</span></span>

* <span data-ttu-id="e00df-454">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="e00df-454">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="e00df-455">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="e00df-455">Deprecated `redis list-all`.</span></span> <span data-ttu-id="e00df-456">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="e00df-456">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="e00df-457">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="e00df-457">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="e00df-458">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="e00df-458">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="e00df-459">Função</span><span class="sxs-lookup"><span data-stu-id="e00df-459">Role</span></span>

* <span data-ttu-id="e00df-460">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="e00df-460">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="e00df-461">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-461">Storage</span></span>

* <span data-ttu-id="e00df-462">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="e00df-462">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="e00df-463">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="e00df-463">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="e00df-464">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="e00df-464">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="e00df-465">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="e00df-465">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="e00df-466">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="e00df-466">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-467">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-467">VM</span></span>

* <span data-ttu-id="e00df-468">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="e00df-468">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="e00df-469">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="e00df-469">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="e00df-470">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="e00df-470">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="e00df-471">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="e00df-471">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="e00df-472">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="e00df-472">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="e00df-473">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="e00df-473">Added write accelerator support</span></span>
* <span data-ttu-id="e00df-474">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="e00df-474">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="e00df-475">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="e00df-475">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="e00df-476">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="e00df-476">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="e00df-477">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="e00df-477">April 10, 2018</span></span>

<span data-ttu-id="e00df-478">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="e00df-478">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="e00df-479">ACR</span><span class="sxs-lookup"><span data-stu-id="e00df-479">ACR</span></span>

* <span data-ttu-id="e00df-480">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="e00df-480">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-481">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-481">ACS</span></span>

* <span data-ttu-id="e00df-482">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="e00df-482">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-483">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-483">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="e00df-485">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="e00df-485">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="e00df-486">BatchAI</span><span class="sxs-lookup"><span data-stu-id="e00df-486">BatchAI</span></span>

* <span data-ttu-id="e00df-487">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="e00df-487">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="e00df-488">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="e00df-488">Job level mounting</span></span>
 - <span data-ttu-id="e00df-489">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="e00df-489">Environment variables with secret values</span></span>
 - <span data-ttu-id="e00df-490">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="e00df-490">Performance counters settings</span></span>
 - <span data-ttu-id="e00df-491">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="e00df-491">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="e00df-492">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="e00df-492">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="e00df-493">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="e00df-493">Usage and limits reporting</span></span>
 - <span data-ttu-id="e00df-494">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="e00df-494">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="e00df-495">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="e00df-495">Support for custom images</span></span>
 - <span data-ttu-id="e00df-496">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="e00df-496">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="e00df-497">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="e00df-497">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="e00df-498">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="e00df-498">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="e00df-499">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="e00df-499">National clouds are supported</span></span>
* <span data-ttu-id="e00df-500">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="e00df-500">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="e00df-501">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="e00df-501">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="e00df-502">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="e00df-502">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="e00df-503">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="e00df-503">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="e00df-504">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="e00df-504">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="e00df-505">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="e00df-505">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="e00df-506">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="e00df-506">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="e00df-507">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="e00df-507">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="e00df-508">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="e00df-508">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="e00df-509">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="e00df-509">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="e00df-510">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="e00df-510">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="e00df-511">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="e00df-511">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="e00df-512">[ALTERAÇÃO SIGNIFICATIVA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="e00df-512">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="e00df-513">Cobrança</span><span class="sxs-lookup"><span data-stu-id="e00df-513">Billing</span></span>

* <span data-ttu-id="e00df-514">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="e00df-514">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="e00df-515">Consumo</span><span class="sxs-lookup"><span data-stu-id="e00df-515">Consumption</span></span>

* <span data-ttu-id="e00df-516">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="e00df-516">Added `marketplace` commands</span></span>
* <span data-ttu-id="e00df-517">[ALTERAÇÃO SIGNIFICATIVA] `reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="e00df-517">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="e00df-518">[ALTERAÇÃO SIGNIFICATIVA] `reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="e00df-518">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="e00df-519">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="e00df-519">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="e00df-520">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="e00df-520">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="e00df-521">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="e00df-521">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="e00df-522">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e00df-522">Container</span></span>

* <span data-ttu-id="e00df-523">Adição dos parâmetros de montagem de volume de repositório git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="e00df-523">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="e00df-524">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="e00df-524">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="e00df-525">Extensão</span><span class="sxs-lookup"><span data-stu-id="e00df-525">Extension</span></span>

* <span data-ttu-id="e00df-526">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="e00df-526">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="e00df-527">Interativo</span><span class="sxs-lookup"><span data-stu-id="e00df-527">Interactive</span></span>

* <span data-ttu-id="e00df-528">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="e00df-528">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="e00df-529">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="e00df-529">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="e00df-530">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="e00df-530">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="e00df-531">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-531">Network</span></span>

* <span data-ttu-id="e00df-532">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="e00df-532">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="e00df-533">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="e00df-533">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="e00df-534">#4910</span><span class="sxs-lookup"><span data-stu-id="e00df-534">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="e00df-535">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="e00df-535">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="e00df-536">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="e00df-536">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="e00df-537">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e00df-537">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="e00df-538">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e00df-538">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="e00df-539">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="e00df-539">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="e00df-540">Perfil</span><span class="sxs-lookup"><span data-stu-id="e00df-540">Profile</span></span>

* <span data-ttu-id="e00df-541">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="e00df-541">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="e00df-542">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="e00df-542">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="e00df-543">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e00df-543">RDBMS</span></span>

* <span data-ttu-id="e00df-544">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="e00df-544">Added `georestore` command</span></span>
* <span data-ttu-id="e00df-545">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="e00df-545">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="e00df-546">Recurso</span><span class="sxs-lookup"><span data-stu-id="e00df-546">Resource</span></span>

* <span data-ttu-id="e00df-547">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="e00df-547">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="e00df-548">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="e00df-548">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="e00df-549">SQL</span><span class="sxs-lookup"><span data-stu-id="e00df-549">SQL</span></span>

* <span data-ttu-id="e00df-550">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="e00df-550">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="e00df-551">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-551">Storage</span></span>

* <span data-ttu-id="e00df-552">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="e00df-552">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-553">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-553">VM</span></span>

* <span data-ttu-id="e00df-554">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e00df-554">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="e00df-555">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="e00df-555">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="e00df-557">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="e00df-557">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="e00df-558">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="e00df-558">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="e00df-559">#5718</span><span class="sxs-lookup"><span data-stu-id="e00df-559">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="e00df-560">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="e00df-560">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="e00df-561">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="e00df-561">March 27, 2018</span></span>

<span data-ttu-id="e00df-562">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="e00df-562">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="e00df-563">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e00df-563">Core</span></span>

* <span data-ttu-id="e00df-564">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="e00df-564">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-565">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-565">ACS</span></span>

* <span data-ttu-id="e00df-566">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e00df-566">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-567">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-567">Appservice</span></span>

* <span data-ttu-id="e00df-568">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="e00df-568">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="e00df-569">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="e00df-569">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="e00df-570">Backup</span><span class="sxs-lookup"><span data-stu-id="e00df-570">Backup</span></span>

* <span data-ttu-id="e00df-571">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="e00df-571">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="e00df-572">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="e00df-572">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="e00df-573">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="e00df-573">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="e00df-574">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="e00df-574">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="e00df-575">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e00df-575">Container</span></span>

* <span data-ttu-id="e00df-576">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="e00df-576">Added `container exec` command.</span></span> <span data-ttu-id="e00df-577">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="e00df-577">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="e00df-578">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="e00df-578">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="e00df-579">Extensão</span><span class="sxs-lookup"><span data-stu-id="e00df-579">Extension</span></span>

* <span data-ttu-id="e00df-580">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="e00df-580">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="e00df-581">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="e00df-581">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="e00df-582">[ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="e00df-582">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="e00df-583">Interativo</span><span class="sxs-lookup"><span data-stu-id="e00df-583">Interactive</span></span>

* <span data-ttu-id="e00df-584">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="e00df-584">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="e00df-585">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="e00df-585">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="e00df-586">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="e00df-586">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="e00df-587">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="e00df-587">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="e00df-588">Laboratório</span><span class="sxs-lookup"><span data-stu-id="e00df-588">Lab</span></span>

* <span data-ttu-id="e00df-589">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="e00df-589">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="e00df-590">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e00df-590">Monitor</span></span>

* <span data-ttu-id="e00df-591">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="e00df-591">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="e00df-592">[#4529](https://github.com/Azure/azure-cli/issues/5785) corrigido: `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="e00df-592">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="e00df-593">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="e00df-593">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="e00df-594">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-594">Network</span></span>

* <span data-ttu-id="e00df-595">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="e00df-595">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="e00df-596">Perfil</span><span class="sxs-lookup"><span data-stu-id="e00df-596">Profile</span></span>

* <span data-ttu-id="e00df-597">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="e00df-597">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e00df-598">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e00df-598">RDBMS</span></span>

* <span data-ttu-id="e00df-599">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="e00df-599">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="e00df-600">Recurso</span><span class="sxs-lookup"><span data-stu-id="e00df-600">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="e00df-602">Função</span><span class="sxs-lookup"><span data-stu-id="e00df-602">Role</span></span>

* <span data-ttu-id="e00df-603">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="e00df-603">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="e00df-604">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="e00df-604">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="e00df-605">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="e00df-605">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="e00df-606">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="e00df-606">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="e00df-607">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="e00df-607">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="e00df-608">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-608">Storage</span></span>

* <span data-ttu-id="e00df-609">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="e00df-609">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="e00df-610">[4049#](https://github.com/Azure/azure-cli/issues/4049) corrigido: problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="e00df-610">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-611">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-611">VM</span></span>

* <span data-ttu-id="e00df-612">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="e00df-612">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="e00df-613">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="e00df-613">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="e00df-614">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="e00df-614">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="e00df-615">[ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="e00df-615">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="e00df-616">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="e00df-616">March 13, 2018</span></span>

<span data-ttu-id="e00df-617">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="e00df-617">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="e00df-618">ACR</span><span class="sxs-lookup"><span data-stu-id="e00df-618">ACR</span></span>

* <span data-ttu-id="e00df-619">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="e00df-619">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="e00df-620">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="e00df-620">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="e00df-621">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="e00df-621">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-622">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-622">ACS</span></span>

* <span data-ttu-id="e00df-623">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="e00df-623">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="e00df-624">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="e00df-624">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="e00df-625">Supervisor</span><span class="sxs-lookup"><span data-stu-id="e00df-625">Advisor</span></span>

* <span data-ttu-id="e00df-626">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="e00df-626">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="e00df-627">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="e00df-627">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="e00df-628">[ALTERAÇÃO SIGNIFICATIVA] `advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="e00df-628">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="e00df-629">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="e00df-629">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="e00df-630">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="e00df-630">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-631">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-631">Appservice</span></span>

* <span data-ttu-id="e00df-632">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="e00df-632">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="e00df-633">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="e00df-633">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="e00df-634">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="e00df-634">Eventhubs</span></span>

* <span data-ttu-id="e00df-635">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e00df-635">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="e00df-636">Extensão</span><span class="sxs-lookup"><span data-stu-id="e00df-636">Extension</span></span>

* <span data-ttu-id="e00df-637">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="e00df-637">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="e00df-638">Interativo</span><span class="sxs-lookup"><span data-stu-id="e00df-638">Interactive</span></span>

* <span data-ttu-id="e00df-639">[5625](https://github.com/Azure/azure-cli/issues/5625) corrigido: manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="e00df-639">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="e00df-640">[3016](https://github.com/Azure/azure-cli/issues/3016) corrigido: histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="e00df-640">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="e00df-641">[5688](https://github.com/Azure/azure-cli/issues/5688) corrigido: as conclusões não aparecerão se o carregamento da tabela de comando encontrou uma exceção</span><span class="sxs-lookup"><span data-stu-id="e00df-641">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="e00df-642">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="e00df-642">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="e00df-643">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e00df-643">Monitor</span></span>

* <span data-ttu-id="e00df-644">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="e00df-644">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="e00df-645">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="e00df-645">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="e00df-646">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="e00df-646">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="e00df-647">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="e00df-647">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="e00df-648">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-648">Network</span></span>

* <span data-ttu-id="e00df-649">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="e00df-649">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="e00df-650">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="e00df-650">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="e00df-651">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="e00df-651">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="e00df-652">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="e00df-652">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="e00df-653">Perfil</span><span class="sxs-lookup"><span data-stu-id="e00df-653">Profile</span></span>

* <span data-ttu-id="e00df-654">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="e00df-654">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="e00df-655">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="e00df-655">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e00df-656">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e00df-656">RDBMS</span></span>

* <span data-ttu-id="e00df-657">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="e00df-657">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="e00df-658">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="e00df-658">Service Bus</span></span>

* <span data-ttu-id="e00df-659">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e00df-659">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="e00df-660">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-660">Storage</span></span>

* <span data-ttu-id="e00df-661">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="e00df-661">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="e00df-662">[5286](https://github.com/Azure/azure-cli/issues/5286) corrigido: os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="e00df-662">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-663">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-663">VM</span></span>

* <span data-ttu-id="e00df-664">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="e00df-664">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="e00df-665">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="e00df-665">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="e00df-666">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="e00df-666">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="e00df-667">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="e00df-667">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="e00df-668">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="e00df-668">February 27, 2018</span></span>

<span data-ttu-id="e00df-669">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="e00df-669">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="e00df-670">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e00df-670">Core</span></span>

* <span data-ttu-id="e00df-671">Correção [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="e00df-671">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="e00df-672">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="e00df-672">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="e00df-673">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="e00df-673">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-674">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-674">ACS</span></span>

* <span data-ttu-id="e00df-675">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="e00df-675">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="e00df-676">Correção do problema de permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="e00df-676">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="e00df-677">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="e00df-677">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="e00df-678">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="e00df-678">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-679">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-679">Appservice</span></span>

* <span data-ttu-id="e00df-680">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="e00df-680">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="e00df-681">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="e00df-681">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e00df-682">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="e00df-682">Cognitive Services</span></span>

* <span data-ttu-id="e00df-683">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="e00df-683">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="e00df-684">Consumo</span><span class="sxs-lookup"><span data-stu-id="e00df-684">Consumption</span></span>

* <span data-ttu-id="e00df-685">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="e00df-685">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="e00df-686">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="e00df-686">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="e00df-687">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e00df-687">Container</span></span>

* <span data-ttu-id="e00df-688">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="e00df-688">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="e00df-689">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-689">Network</span></span>

* <span data-ttu-id="e00df-690">Correção [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="e00df-690">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="e00df-691">Recurso</span><span class="sxs-lookup"><span data-stu-id="e00df-691">Resource</span></span>

* <span data-ttu-id="e00df-692">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="e00df-692">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="e00df-693">Função</span><span class="sxs-lookup"><span data-stu-id="e00df-693">Role</span></span>

* <span data-ttu-id="e00df-694">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="e00df-694">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="e00df-695">SQL</span><span class="sxs-lookup"><span data-stu-id="e00df-695">SQL</span></span>

* <span data-ttu-id="e00df-696">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="e00df-696">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="e00df-697">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-697">Storage</span></span>

* <span data-ttu-id="e00df-698">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="e00df-698">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-699">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-699">VM</span></span>

* <span data-ttu-id="e00df-700">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="e00df-700">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="e00df-701">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="e00df-701">February 13, 2018</span></span>

<span data-ttu-id="e00df-702">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="e00df-702">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="e00df-703">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e00df-703">Core</span></span>

* <span data-ttu-id="e00df-704">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="e00df-704">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-705">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-705">ACS</span></span>

* <span data-ttu-id="e00df-706">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="e00df-706">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="e00df-707">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="e00df-707">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="e00df-708">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="e00df-708">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="e00df-709">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="e00df-709">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="e00df-710">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="e00df-710">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="e00df-711">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="e00df-711">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="e00df-712">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="e00df-712">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="e00df-713">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="e00df-713">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-714">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-714">Appservice</span></span>

* <span data-ttu-id="e00df-715">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="e00df-715">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="e00df-716">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="e00df-716">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="e00df-717">CDN</span><span class="sxs-lookup"><span data-stu-id="e00df-717">CDN</span></span>

* <span data-ttu-id="e00df-718">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="e00df-718">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="e00df-719">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e00df-719">Container</span></span>

* <span data-ttu-id="e00df-720">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="e00df-720">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="e00df-721">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="e00df-721">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e00df-722">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e00df-722">CosmosDB</span></span>

* <span data-ttu-id="e00df-723">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="e00df-723">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="e00df-724">Extensão</span><span class="sxs-lookup"><span data-stu-id="e00df-724">Extension</span></span>

* <span data-ttu-id="e00df-725">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="e00df-725">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="e00df-726">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="e00df-726">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="e00df-727">Comentários</span><span class="sxs-lookup"><span data-stu-id="e00df-727">Feedback</span></span>

* <span data-ttu-id="e00df-728">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="e00df-728">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="e00df-729">Interativo</span><span class="sxs-lookup"><span data-stu-id="e00df-729">Interactive</span></span>

* <span data-ttu-id="e00df-730">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e00df-730">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="e00df-731">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="e00df-731">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="e00df-732">IoT</span><span class="sxs-lookup"><span data-stu-id="e00df-732">IoT</span></span>

* <span data-ttu-id="e00df-733">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="e00df-733">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="e00df-734">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="e00df-734">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="e00df-735">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e00df-735">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="e00df-736">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="e00df-736">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="e00df-737">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e00df-737">Monitor</span></span>

* <span data-ttu-id="e00df-738">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="e00df-738">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="e00df-739">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-739">Network</span></span>

* <span data-ttu-id="e00df-740">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="e00df-740">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="e00df-741">Perfil</span><span class="sxs-lookup"><span data-stu-id="e00df-741">Profile</span></span>

* <span data-ttu-id="e00df-742">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="e00df-742">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="e00df-743">Recurso</span><span class="sxs-lookup"><span data-stu-id="e00df-743">Resource</span></span>

* <span data-ttu-id="e00df-744">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="e00df-744">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="e00df-745">Função</span><span class="sxs-lookup"><span data-stu-id="e00df-745">Role</span></span>

* <span data-ttu-id="e00df-746">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="e00df-746">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="e00df-747">SQL</span><span class="sxs-lookup"><span data-stu-id="e00df-747">SQL</span></span>

* <span data-ttu-id="e00df-748">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="e00df-748">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="e00df-749">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="e00df-749">Added `sql db rename`</span></span>
* <span data-ttu-id="e00df-750">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="e00df-750">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="e00df-751">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-751">Storage</span></span>

* <span data-ttu-id="e00df-752">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="e00df-752">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-753">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-753">VM</span></span>

* <span data-ttu-id="e00df-754">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="e00df-754">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="e00df-755">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="e00df-755">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="e00df-756">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="e00df-756">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="e00df-757">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="e00df-757">January 31, 2018</span></span>

<span data-ttu-id="e00df-758">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="e00df-758">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="e00df-759">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e00df-759">Core</span></span>

* <span data-ttu-id="e00df-760">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="e00df-760">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="e00df-761">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="e00df-761">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="e00df-762">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="e00df-762">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="e00df-763">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="e00df-763">Use `--verbose` to see</span></span>
* <span data-ttu-id="e00df-764">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="e00df-764">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-765">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-765">ACS</span></span>

* <span data-ttu-id="e00df-766">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="e00df-766">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="e00df-767">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="e00df-767">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-768">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-768">Appservice</span></span>

* <span data-ttu-id="e00df-769">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="e00df-769">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="e00df-770">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="e00df-770">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="e00df-771">CDN</span><span class="sxs-lookup"><span data-stu-id="e00df-771">CDN</span></span>

* <span data-ttu-id="e00df-772">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="e00df-772">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e00df-773">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e00df-773">CosmosDB</span></span>

* <span data-ttu-id="e00df-774">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="e00df-774">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="e00df-775">Interativo</span><span class="sxs-lookup"><span data-stu-id="e00df-775">Interactive</span></span>

* <span data-ttu-id="e00df-776">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="e00df-776">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="e00df-777">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-777">Network</span></span>

* <span data-ttu-id="e00df-778">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="e00df-778">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="e00df-779">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="e00df-779">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="e00df-780">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="e00df-780">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="e00df-781">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="e00df-781">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="e00df-782">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="e00df-782">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="e00df-783">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="e00df-783">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="e00df-784">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="e00df-784">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="e00df-785">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="e00df-785">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="e00df-786">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="e00df-786">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="e00df-787">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="e00df-787">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="e00df-788">Perfil</span><span class="sxs-lookup"><span data-stu-id="e00df-788">Profile</span></span>

* <span data-ttu-id="e00df-789">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="e00df-789">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="e00df-790">Recurso</span><span class="sxs-lookup"><span data-stu-id="e00df-790">Resource</span></span>

* <span data-ttu-id="e00df-791">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="e00df-791">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="e00df-792">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-792">Storage</span></span>

* <span data-ttu-id="e00df-793">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="e00df-793">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="e00df-794">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="e00df-794">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="e00df-795">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="e00df-795">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="e00df-796">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="e00df-796">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="e00df-797">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="e00df-797">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-798">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-798">VM</span></span>

* <span data-ttu-id="e00df-799">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="e00df-799">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="e00df-800">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="e00df-800">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="e00df-801">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="e00df-801">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="e00df-802">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e00df-802">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="e00df-803">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="e00df-803">January 17, 2018</span></span>

<span data-ttu-id="e00df-804">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="e00df-804">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="e00df-805">ACR</span><span class="sxs-lookup"><span data-stu-id="e00df-805">ACR</span></span>

* <span data-ttu-id="e00df-806">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="e00df-806">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="e00df-807">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="e00df-807">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-808">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-808">ACS</span></span>

* <span data-ttu-id="e00df-809">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="e00df-809">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="e00df-810">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="e00df-810">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-811">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-811">Appservice</span></span>

* <span data-ttu-id="e00df-812">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="e00df-812">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="e00df-813">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="e00df-813">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="e00df-814">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="e00df-814">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="e00df-815">Backup</span><span class="sxs-lookup"><span data-stu-id="e00df-815">Backup</span></span>

* <span data-ttu-id="e00df-816">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="e00df-816">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="e00df-817">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="e00df-817">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="e00df-818">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="e00df-818">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="e00df-819">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="e00df-819">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="e00df-820">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="e00df-820">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="e00df-821">Lote</span><span class="sxs-lookup"><span data-stu-id="e00df-821">Batch</span></span>

* <span data-ttu-id="e00df-822">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="e00df-822">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="e00df-823">Nuvem</span><span class="sxs-lookup"><span data-stu-id="e00df-823">Cloud</span></span>

* <span data-ttu-id="e00df-824">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="e00df-824">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="e00df-825">Consumo</span><span class="sxs-lookup"><span data-stu-id="e00df-825">Consumption</span></span>

* <span data-ttu-id="e00df-826">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="e00df-826">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="e00df-827">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="e00df-827">Event Grid</span></span>

* <span data-ttu-id="e00df-828">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="e00df-828">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="e00df-829">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="e00df-829">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="e00df-830">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="e00df-830">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="e00df-831">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="e00df-831">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="e00df-832">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="e00df-832">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="e00df-833">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="e00df-833">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="e00df-834">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="e00df-834">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="e00df-835">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="e00df-835">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="e00df-836">Interativo</span><span class="sxs-lookup"><span data-stu-id="e00df-836">Interactive</span></span>

* <span data-ttu-id="e00df-837">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="e00df-837">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="e00df-838">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="e00df-838">Fixed errors on startup</span></span>
* <span data-ttu-id="e00df-839">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="e00df-839">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="e00df-840">IoT</span><span class="sxs-lookup"><span data-stu-id="e00df-840">IoT</span></span>

* <span data-ttu-id="e00df-841">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="e00df-841">Added support for device provisioning service</span></span>
* <span data-ttu-id="e00df-842">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="e00df-842">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="e00df-843">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="e00df-843">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="e00df-844">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e00df-844">Monitor</span></span>

* <span data-ttu-id="e00df-845">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="e00df-845">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="e00df-846">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="e00df-846">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="e00df-847">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="e00df-847">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="e00df-848">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-848">Network</span></span>

* <span data-ttu-id="e00df-849">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="e00df-849">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="e00df-850">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e00df-850">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="e00df-851">Perfil</span><span class="sxs-lookup"><span data-stu-id="e00df-851">Profile</span></span>

* <span data-ttu-id="e00df-852">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="e00df-852">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="e00df-853">Função</span><span class="sxs-lookup"><span data-stu-id="e00df-853">Role</span></span>

* <span data-ttu-id="e00df-854">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="e00df-854">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e00df-855">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e00df-855">Service Fabric</span></span>

* <span data-ttu-id="e00df-856">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="e00df-856">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="e00df-857">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="e00df-857">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-858">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-858">VM</span></span>

* <span data-ttu-id="e00df-859">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="e00df-859">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="e00df-860">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="e00df-860">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="e00df-861">[ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="e00df-861">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="e00df-862">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="e00df-862">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="e00df-863">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="e00df-863">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="e00df-864">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e00df-864">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="e00df-865">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e00df-865">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="e00df-866">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="e00df-866">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="e00df-867">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="e00df-867">December 19, 2017</span></span>

<span data-ttu-id="e00df-868">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="e00df-868">Version 2.0.23</span></span>

* <span data-ttu-id="e00df-869">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="e00df-869">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="e00df-870">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e00df-870">Container</span></span>

* <span data-ttu-id="e00df-871">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="e00df-871">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="e00df-872">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-872">Network</span></span>

* <span data-ttu-id="e00df-873">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e00df-873">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="e00df-874">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e00df-874">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="e00df-875">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-875">Storage</span></span>

* <span data-ttu-id="e00df-876">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="e00df-876">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-877">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-877">VM</span></span>

* <span data-ttu-id="e00df-878">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="e00df-878">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="e00df-879">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="e00df-879">December 5, 2017</span></span>

<span data-ttu-id="e00df-880">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="e00df-880">Version 2.0.22</span></span>

* <span data-ttu-id="e00df-881">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="e00df-881">Removed `az component` commands.</span></span> <span data-ttu-id="e00df-882">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="e00df-882">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="e00df-883">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e00df-883">Core</span></span>
* <span data-ttu-id="e00df-884">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="e00df-884">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="e00df-885">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="e00df-885">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-886">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-886">ACS</span></span>

* <span data-ttu-id="e00df-887">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="e00df-887">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="e00df-888">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="e00df-888">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="e00df-889">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="e00df-889">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="e00df-890">Supervisor</span><span class="sxs-lookup"><span data-stu-id="e00df-890">Advisor</span></span>

* <span data-ttu-id="e00df-891">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e00df-891">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-892">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-892">Appservice</span></span>

* <span data-ttu-id="e00df-893">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="e00df-893">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="e00df-894">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="e00df-894">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="e00df-895">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="e00df-895">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="e00df-896">Consumo</span><span class="sxs-lookup"><span data-stu-id="e00df-896">Consumption</span></span>

* <span data-ttu-id="e00df-897">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="e00df-897">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="e00df-898">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e00df-898">Container</span></span>

* <span data-ttu-id="e00df-899">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="e00df-899">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="e00df-900">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e00df-900">Monitor</span></span>

* <span data-ttu-id="e00df-901">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="e00df-901">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="e00df-902">Recurso</span><span class="sxs-lookup"><span data-stu-id="e00df-902">Resource</span></span>

* <span data-ttu-id="e00df-903">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="e00df-903">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="e00df-904">Função</span><span class="sxs-lookup"><span data-stu-id="e00df-904">Role</span></span>

* <span data-ttu-id="e00df-905">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="e00df-905">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="e00df-906">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="e00df-906">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="e00df-907">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="e00df-907">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="e00df-908">SQL</span><span class="sxs-lookup"><span data-stu-id="e00df-908">SQL</span></span>

* <span data-ttu-id="e00df-909">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="e00df-909">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="e00df-910">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="e00df-910">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-911">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-911">VM</span></span>

* <span data-ttu-id="e00df-912">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="e00df-912">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="e00df-913">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="e00df-913">November 14, 2017</span></span>

<span data-ttu-id="e00df-914">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="e00df-914">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="e00df-915">ACR</span><span class="sxs-lookup"><span data-stu-id="e00df-915">ACR</span></span>

* <span data-ttu-id="e00df-916">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="e00df-916">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="e00df-917">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-917">ACS</span></span>

* <span data-ttu-id="e00df-918">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="e00df-918">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="e00df-919">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="e00df-919">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="e00df-920">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="e00df-920">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="e00df-921">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="e00df-921">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="e00df-922">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="e00df-922">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-923">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-923">Appservice</span></span>

* <span data-ttu-id="e00df-924">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="e00df-924">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="e00df-925">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="e00df-925">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="e00df-926">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="e00df-926">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="e00df-927">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="e00df-927">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="e00df-928">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="e00df-928">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="e00df-929">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="e00df-929">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="e00df-930">Lote</span><span class="sxs-lookup"><span data-stu-id="e00df-930">Batch</span></span>

* <span data-ttu-id="e00df-931">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="e00df-931">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="e00df-932">Batchai</span><span class="sxs-lookup"><span data-stu-id="e00df-932">Batchai</span></span>

* <span data-ttu-id="e00df-933">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="e00df-933">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="e00df-934">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="e00df-934">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="e00df-935">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="e00df-935">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="e00df-936">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="e00df-936">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="e00df-937">Nuvem</span><span class="sxs-lookup"><span data-stu-id="e00df-937">Cloud</span></span>

* <span data-ttu-id="e00df-938">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="e00df-938">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="e00df-939">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e00df-939">Container</span></span>

* <span data-ttu-id="e00df-940">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="e00df-940">Added support to open multiple ports</span></span>
* <span data-ttu-id="e00df-941">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="e00df-941">Added container group restart policy</span></span>
* <span data-ttu-id="e00df-942">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="e00df-942">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="e00df-943">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="e00df-943">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e00df-944">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e00df-944">Data Lake Analytics</span></span>

* <span data-ttu-id="e00df-945">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="e00df-945">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e00df-946">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e00df-946">Data Lake Store</span></span>

* <span data-ttu-id="e00df-947">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="e00df-947">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="e00df-948">Extensão</span><span class="sxs-lookup"><span data-stu-id="e00df-948">Extension</span></span>

* <span data-ttu-id="e00df-949">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="e00df-949">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="e00df-950">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="e00df-950">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="e00df-951">IoT</span><span class="sxs-lookup"><span data-stu-id="e00df-951">IoT</span></span>

* <span data-ttu-id="e00df-952">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="e00df-952">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="e00df-953">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e00df-953">Monitor</span></span>

* <span data-ttu-id="e00df-954">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="e00df-954">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="e00df-955">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-955">Network</span></span>

* <span data-ttu-id="e00df-956">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="e00df-956">Added support for CAA DNS records</span></span>
* <span data-ttu-id="e00df-957">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="e00df-957">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="e00df-958">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="e00df-958">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="e00df-959">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="e00df-959">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="e00df-960">Reservas</span><span class="sxs-lookup"><span data-stu-id="e00df-960">Reservations</span></span>

* <span data-ttu-id="e00df-961">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="e00df-961">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="e00df-962">Recurso</span><span class="sxs-lookup"><span data-stu-id="e00df-962">Resource</span></span>

* <span data-ttu-id="e00df-963">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="e00df-963">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="e00df-964">SQL</span><span class="sxs-lookup"><span data-stu-id="e00df-964">SQL</span></span>

* <span data-ttu-id="e00df-965">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e00df-965">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="e00df-966">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-966">Storage</span></span>

* <span data-ttu-id="e00df-967">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="e00df-967">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="e00df-968">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="e00df-968">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="e00df-969">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="e00df-969">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="e00df-970">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="e00df-970">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="e00df-971">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="e00df-971">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="e00df-972">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="e00df-972">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="e00df-973">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e00df-973">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-974">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-974">VM</span></span>

* <span data-ttu-id="e00df-975">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="e00df-975">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="e00df-976">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="e00df-976">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="e00df-977">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="e00df-977">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="e00df-978">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="e00df-978">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="e00df-979">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="e00df-979">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="e00df-980">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="e00df-980">October 24, 2017</span></span>

<span data-ttu-id="e00df-981">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="e00df-981">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="e00df-982">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e00df-982">Core</span></span>

* <span data-ttu-id="e00df-983">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="e00df-983">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="e00df-984">ACR</span><span class="sxs-lookup"><span data-stu-id="e00df-984">ACR</span></span>

* <span data-ttu-id="e00df-985">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="e00df-985">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="e00df-986">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="e00df-986">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="e00df-987">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="e00df-987">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-988">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-988">ACS</span></span>

* <span data-ttu-id="e00df-989">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="e00df-989">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="e00df-990">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="e00df-990">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-991">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-991">Appservice</span></span>

* <span data-ttu-id="e00df-992">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="e00df-992">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="e00df-993">Componente</span><span class="sxs-lookup"><span data-stu-id="e00df-993">Component</span></span>

* <span data-ttu-id="e00df-994">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="e00df-994">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="e00df-995">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e00df-995">Monitor</span></span>

* <span data-ttu-id="e00df-996">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="e00df-996">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="e00df-997">Recurso</span><span class="sxs-lookup"><span data-stu-id="e00df-997">Resource</span></span>

* <span data-ttu-id="e00df-998">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="e00df-998">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="e00df-999">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="e00df-999">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-1000">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-1000">VM</span></span>

* <span data-ttu-id="e00df-1001">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1001">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="e00df-1002">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="e00df-1002">October 9, 2017</span></span>

<span data-ttu-id="e00df-1003">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="e00df-1003">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="e00df-1004">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e00df-1004">Core</span></span>

* <span data-ttu-id="e00df-1005">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="e00df-1005">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-1006">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-1006">Appservice</span></span>

* <span data-ttu-id="e00df-1007">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="e00df-1007">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="e00df-1008">Lote</span><span class="sxs-lookup"><span data-stu-id="e00df-1008">Batch</span></span>

* <span data-ttu-id="e00df-1009">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="e00df-1009">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="e00df-1010">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="e00df-1010">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="e00df-1011">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="e00df-1011">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="e00df-1012">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="e00df-1012">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="e00df-1013">Batchai</span><span class="sxs-lookup"><span data-stu-id="e00df-1013">Batchai</span></span>

* <span data-ttu-id="e00df-1014">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="e00df-1014">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="e00df-1015">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e00df-1015">Keyvault</span></span>

* <span data-ttu-id="e00df-1016">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="e00df-1016">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="e00df-1017">(#4448)</span><span class="sxs-lookup"><span data-stu-id="e00df-1017">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="e00df-1018">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-1018">Network</span></span>

* <span data-ttu-id="e00df-1019">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="e00df-1019">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="e00df-1020">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="e00df-1020">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="e00df-1021">Recurso</span><span class="sxs-lookup"><span data-stu-id="e00df-1021">Resource</span></span>

* <span data-ttu-id="e00df-1022">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="e00df-1022">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="e00df-1023">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="e00df-1023">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="e00df-1024">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="e00df-1024">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="e00df-1025">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="e00df-1025">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="e00df-1026">Sql</span><span class="sxs-lookup"><span data-stu-id="e00df-1026">Sql</span></span>

* <span data-ttu-id="e00df-1027">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="e00df-1027">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="e00df-1028">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="e00df-1028">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="e00df-1029">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="e00df-1029">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="e00df-1030">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-1030">Storage</span></span>

* <span data-ttu-id="e00df-1031">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="e00df-1031">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-1032">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-1032">Vm</span></span>

* <span data-ttu-id="e00df-1033">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="e00df-1033">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="e00df-1034">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1034">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="e00df-1035">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="e00df-1035">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="e00df-1036">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1036">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="e00df-1037">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1037">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="e00df-1038">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="e00df-1038">September 22, 2017</span></span>

<span data-ttu-id="e00df-1039">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="e00df-1039">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="e00df-1040">Recurso</span><span class="sxs-lookup"><span data-stu-id="e00df-1040">Resource</span></span>

* <span data-ttu-id="e00df-1041">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="e00df-1041">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="e00df-1042">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="e00df-1042">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="e00df-1043">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1043">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="e00df-1044">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="e00df-1044">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="e00df-1045">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-1045">Network</span></span>

* <span data-ttu-id="e00df-1046">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="e00df-1046">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="e00df-1047">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="e00df-1047">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="e00df-1048">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e00df-1048">Added `asg` application security group commands</span></span>
* <span data-ttu-id="e00df-1049">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="e00df-1049">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="e00df-1050">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e00df-1050">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="e00df-1051">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e00df-1051">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="e00df-1052">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="e00df-1052">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e00df-1053">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-1053">Storage</span></span>

* <span data-ttu-id="e00df-1054">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="e00df-1054">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="e00df-1055">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="e00df-1055">Eventgrid</span></span>

* <span data-ttu-id="e00df-1056">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="e00df-1056">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="e00df-1057">SQL</span><span class="sxs-lookup"><span data-stu-id="e00df-1057">SQL</span></span>

* <span data-ttu-id="e00df-1058">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="e00df-1058">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="e00df-1059">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="e00df-1059">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="e00df-1060">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e00df-1060">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="e00df-1061">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e00df-1061">Keyvault</span></span>

* <span data-ttu-id="e00df-1062">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="e00df-1062">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-1063">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-1063">VM</span></span>

* <span data-ttu-id="e00df-1064">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1064">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="e00df-1065">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="e00df-1065">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="e00df-1066">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1066">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="e00df-1067">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="e00df-1067">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="e00df-1068">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="e00df-1068">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="e00df-1069">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="e00df-1069">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-1070">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-1070">ACS</span></span>

* <span data-ttu-id="e00df-1071">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-1071">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-1072">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-1072">Appservice</span></span>

* <span data-ttu-id="e00df-1073">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="e00df-1073">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="e00df-1074">Backup</span><span class="sxs-lookup"><span data-stu-id="e00df-1074">Backup</span></span>

* <span data-ttu-id="e00df-1075">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="e00df-1075">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="e00df-1076">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="e00df-1076">September 11, 2017</span></span>

<span data-ttu-id="e00df-1077">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="e00df-1077">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="e00df-1078">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e00df-1078">Core</span></span>

* <span data-ttu-id="e00df-1079">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="e00df-1079">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="e00df-1080">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="e00df-1080">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-1081">Acs</span><span class="sxs-lookup"><span data-stu-id="e00df-1081">Acs</span></span>

* <span data-ttu-id="e00df-1082">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="e00df-1082">Added `acs list-locations` command</span></span>
* <span data-ttu-id="e00df-1083">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="e00df-1083">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-1084">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-1084">Appservice</span></span>

* <span data-ttu-id="e00df-1085">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="e00df-1085">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="e00df-1086">CDN</span><span class="sxs-lookup"><span data-stu-id="e00df-1086">CDN</span></span>

* <span data-ttu-id="e00df-1087">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1087">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="e00df-1088">Extensão</span><span class="sxs-lookup"><span data-stu-id="e00df-1088">Extension</span></span>

* <span data-ttu-id="e00df-1089">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="e00df-1089">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="e00df-1090">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e00df-1090">Keyvault</span></span>

* <span data-ttu-id="e00df-1091">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="e00df-1091">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="e00df-1092">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-1092">Network</span></span>

* <span data-ttu-id="e00df-1093">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="e00df-1093">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="e00df-1094">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="e00df-1094">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="e00df-1095">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="e00df-1095">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="e00df-1096">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1096">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="e00df-1097">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1097">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="e00df-1098">Recurso</span><span class="sxs-lookup"><span data-stu-id="e00df-1098">Resource</span></span>

* <span data-ttu-id="e00df-1099">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="e00df-1099">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="e00df-1100">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1100">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="e00df-1101">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="e00df-1101">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="e00df-1102">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="e00df-1102">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="e00df-1103">SQL</span><span class="sxs-lookup"><span data-stu-id="e00df-1103">SQL</span></span>

* <span data-ttu-id="e00df-1104">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="e00df-1104">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-1105">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-1105">VM</span></span>

* <span data-ttu-id="e00df-1106">Corrigido: Não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="e00df-1106">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="e00df-1107">Corrigido: Usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="e00df-1107">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="e00df-1108">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1108">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="e00df-1109">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="e00df-1109">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="e00df-1110">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="e00df-1110">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="e00df-1111">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="e00df-1111">August 31, 2017</span></span>

<span data-ttu-id="e00df-1112">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="e00df-1112">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="e00df-1113">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e00df-1113">Keyvault</span></span>

* <span data-ttu-id="e00df-1114">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="e00df-1114">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="e00df-1115">Sf</span><span class="sxs-lookup"><span data-stu-id="e00df-1115">Sf</span></span>

* <span data-ttu-id="e00df-1116">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="e00df-1116">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="e00df-1117">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-1117">Storage</span></span>

* <span data-ttu-id="e00df-1118">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="e00df-1118">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="e00df-1119">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="e00df-1119">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="e00df-1120">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="e00df-1120">August 28, 2017</span></span>

<span data-ttu-id="e00df-1121">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="e00df-1121">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="e00df-1122">CLI</span><span class="sxs-lookup"><span data-stu-id="e00df-1122">CLI</span></span>

* <span data-ttu-id="e00df-1123">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="e00df-1123">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-1124">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-1124">ACS</span></span>

* <span data-ttu-id="e00df-1125">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="e00df-1125">Corrected preview regions</span></span>
* <span data-ttu-id="e00df-1126">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="e00df-1126">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="e00df-1127">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="e00df-1127">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-1128">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-1128">Appservice</span></span>

* <span data-ttu-id="e00df-1129">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="e00df-1129">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="e00df-1130">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="e00df-1130">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="e00df-1131">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="e00df-1131">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="e00df-1132">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="e00df-1132">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="e00df-1133">Correção: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="e00df-1133">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="e00df-1134">IoT</span><span class="sxs-lookup"><span data-stu-id="e00df-1134">IoT</span></span>

* <span data-ttu-id="e00df-1135">Correção #3934: Criação de política não limpa as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="e00df-1135">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="e00df-1136">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-1136">Network</span></span>

* <span data-ttu-id="e00df-1137">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="e00df-1137">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="e00df-1138">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e00df-1138">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="e00df-1139">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e00df-1139">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="e00df-1140">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1140">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="e00df-1141">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1141">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="e00df-1142">Perfil</span><span class="sxs-lookup"><span data-stu-id="e00df-1142">Profile</span></span>

* <span data-ttu-id="e00df-1143">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="e00df-1143">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e00df-1144">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e00df-1144">Service Fabric</span></span>

* <span data-ttu-id="e00df-1145">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="e00df-1145">Preview release</span></span>
* <span data-ttu-id="e00df-1146">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="e00df-1146">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="e00df-1147">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="e00df-1147">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="e00df-1148">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="e00df-1148">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="e00df-1149">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-1149">Storage</span></span>

* <span data-ttu-id="e00df-1150">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="e00df-1150">Enabled setting blob tier</span></span>
* <span data-ttu-id="e00df-1151">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="e00df-1151">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="e00df-1152">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="e00df-1152">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="e00df-1153">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="e00df-1153">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="e00df-1154">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="e00df-1154">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="e00df-1155">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="e00df-1155">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-1156">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-1156">VM</span></span>

* <span data-ttu-id="e00df-1157">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="e00df-1157">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="e00df-1158">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="e00df-1158">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="e00df-1159">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1159">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="e00df-1160">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="e00df-1160">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="e00df-1161">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="e00df-1161">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="e00df-1162">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1162">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="e00df-1163">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="e00df-1163">August 15, 2017</span></span>

<span data-ttu-id="e00df-1164">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="e00df-1164">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-1165">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-1165">ACS</span></span>

* <span data-ttu-id="e00df-1166">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="e00df-1166">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-1167">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-1167">Appservice</span></span>

* <span data-ttu-id="e00df-1168">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="e00df-1168">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="e00df-1169">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="e00df-1169">Event Grid</span></span>

* <span data-ttu-id="e00df-1170">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="e00df-1170">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="e00df-1171">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="e00df-1171">August 11, 2017</span></span>

<span data-ttu-id="e00df-1172">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="e00df-1172">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-1173">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-1173">ACS</span></span>

* <span data-ttu-id="e00df-1174">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="e00df-1174">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="e00df-1175">Lote</span><span class="sxs-lookup"><span data-stu-id="e00df-1175">Batch</span></span>

* <span data-ttu-id="e00df-1176">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="e00df-1176">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="e00df-1177">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="e00df-1177">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="e00df-1178">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="e00df-1178">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="e00df-1179">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="e00df-1179">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="e00df-1180">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="e00df-1180">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="e00df-1181">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="e00df-1181">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="e00df-1182">Componente</span><span class="sxs-lookup"><span data-stu-id="e00df-1182">Component</span></span>

* <span data-ttu-id="e00df-1183">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="e00df-1183">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="e00df-1184">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e00df-1184">Container</span></span>

* <span data-ttu-id="e00df-1185">`create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="e00df-1185">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="e00df-1186">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e00df-1186">Data Lake Store</span></span>

* <span data-ttu-id="e00df-1187">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="e00df-1187">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="e00df-1188">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="e00df-1188">Event Grid</span></span>

* <span data-ttu-id="e00df-1189">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e00df-1189">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="e00df-1190">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-1190">Network</span></span>

* <span data-ttu-id="e00df-1191">`lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="e00df-1191">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="e00df-1192">`application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="e00df-1192">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="e00df-1193">`application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="e00df-1193">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="e00df-1194">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="e00df-1194">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="e00df-1195">Perfil</span><span class="sxs-lookup"><span data-stu-id="e00df-1195">Profile</span></span>

* <span data-ttu-id="e00df-1196">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="e00df-1196">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="e00df-1197">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-1197">Storage</span></span>

* <span data-ttu-id="e00df-1198">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="e00df-1198">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-1199">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-1199">VM</span></span>

* <span data-ttu-id="e00df-1200">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="e00df-1200">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="e00df-1201">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="e00df-1201">Exposed `list-skus` command</span></span>
* <span data-ttu-id="e00df-1202">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="e00df-1202">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="e00df-1203">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="e00df-1203">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="e00df-1204">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="e00df-1204">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="e00df-1205">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="e00df-1205">July 28, 2017</span></span>

<span data-ttu-id="e00df-1206">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="e00df-1206">Version 2.0.12</span></span>

* <span data-ttu-id="e00df-1207">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="e00df-1207">Added container commands</span></span>
* <span data-ttu-id="e00df-1208">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="e00df-1208">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="e00df-1209">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e00df-1209">Core</span></span>

* <span data-ttu-id="e00df-1210">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="e00df-1210">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="e00df-1211">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="e00df-1211">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="e00df-1212">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="e00df-1212">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="e00df-1213">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="e00df-1213">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="e00df-1214">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="e00df-1214">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="e00df-1215">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="e00df-1215">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="e00df-1216">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="e00df-1216">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="e00df-1217">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="e00df-1217">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="e00df-1218">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="e00df-1218">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="e00df-1219">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="e00df-1219">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="e00df-1220">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="e00df-1220">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="e00df-1221">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="e00df-1221">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="e00df-1222">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="e00df-1222">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="e00df-1223">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="e00df-1223">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="e00df-1224">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="e00df-1224">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="e00df-1225">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="e00df-1225">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="e00df-1226">ACR</span><span class="sxs-lookup"><span data-stu-id="e00df-1226">ACR</span></span>

* <span data-ttu-id="e00df-1227">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="e00df-1227">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="e00df-1228">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="e00df-1228">Support SKU update for managed registries</span></span>
* <span data-ttu-id="e00df-1229">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="e00df-1229">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="e00df-1230">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="e00df-1230">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="e00df-1231">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="e00df-1231">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="e00df-1232">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="e00df-1232">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-1233">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-1233">ACS</span></span>

* <span data-ttu-id="e00df-1234">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="e00df-1234">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-1235">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-1235">Appservice</span></span>

* <span data-ttu-id="e00df-1236">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="e00df-1236">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="e00df-1237">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="e00df-1237">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="e00df-1238">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="e00df-1238">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="e00df-1239">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="e00df-1239">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="e00df-1240">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="e00df-1240">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="e00df-1241">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="e00df-1241">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="e00df-1242">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="e00df-1242">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="e00df-1243">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="e00df-1243">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="e00df-1244">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="e00df-1244">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="e00df-1245">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="e00df-1245">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="e00df-1246">Lote</span><span class="sxs-lookup"><span data-stu-id="e00df-1246">Batch</span></span>

* <span data-ttu-id="e00df-1247">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="e00df-1247">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="e00df-1248">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="e00df-1248">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="e00df-1249">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="e00df-1249">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="e00df-1250">CDN</span><span class="sxs-lookup"><span data-stu-id="e00df-1250">CDN</span></span>

* <span data-ttu-id="e00df-1251">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="e00df-1251">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="e00df-1252">Nuvem</span><span class="sxs-lookup"><span data-stu-id="e00df-1252">Cloud</span></span>

* <span data-ttu-id="e00df-1253">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="e00df-1253">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="e00df-1254">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="e00df-1254">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="e00df-1255">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="e00df-1255">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="e00df-1256">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="e00df-1256">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="e00df-1257">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="e00df-1257">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e00df-1258">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e00df-1258">CosmosDB</span></span>

* <span data-ttu-id="e00df-1259">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="e00df-1259">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="e00df-1260">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="e00df-1260">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e00df-1261">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e00df-1261">Data Lake Analytics</span></span>

* <span data-ttu-id="e00df-1262">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="e00df-1262">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="e00df-1263">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="e00df-1263">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="e00df-1264">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="e00df-1264">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e00df-1265">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e00df-1265">Data Lake Store</span></span>

* <span data-ttu-id="e00df-1266">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="e00df-1266">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="e00df-1267">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="e00df-1267">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="e00df-1268">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="e00df-1268">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="e00df-1269">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e00df-1269">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="e00df-1270">Interativo</span><span class="sxs-lookup"><span data-stu-id="e00df-1270">Interactive</span></span>

* <span data-ttu-id="e00df-1271">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="e00df-1271">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="e00df-1272">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="e00df-1272">Increased test coverage</span></span>
* <span data-ttu-id="e00df-1273">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="e00df-1273">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="e00df-1274">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="e00df-1274">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="e00df-1275">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="e00df-1275">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="e00df-1276">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="e00df-1276">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="e00df-1277">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="e00df-1277">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="e00df-1278">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="e00df-1278">Added `--progress` flag</span></span>
* <span data-ttu-id="e00df-1279">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="e00df-1279">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="e00df-1280">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="e00df-1280">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="e00df-1281">IoT</span><span class="sxs-lookup"><span data-stu-id="e00df-1281">IoT</span></span>

* <span data-ttu-id="e00df-1282">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="e00df-1282">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="e00df-1283">(#3934)</span><span class="sxs-lookup"><span data-stu-id="e00df-1283">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="e00df-1284">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="e00df-1284">Key vault</span></span>

* <span data-ttu-id="e00df-1285">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="e00df-1285">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="e00df-1286">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="e00df-1286">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="e00df-1287">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="e00df-1287">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="e00df-1288">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="e00df-1288">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="e00df-1289">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="e00df-1289">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="e00df-1290">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="e00df-1290">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="e00df-1291">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="e00df-1291">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="e00df-1292">(#3307)</span><span class="sxs-lookup"><span data-stu-id="e00df-1292">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="e00df-1293">Laboratório</span><span class="sxs-lookup"><span data-stu-id="e00df-1293">Lab</span></span>

* <span data-ttu-id="e00df-1294">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="e00df-1294">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="e00df-1295">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="e00df-1295">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="e00df-1296">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e00df-1296">Monitor</span></span>

* <span data-ttu-id="e00df-1297">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="e00df-1297">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="e00df-1298">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="e00df-1298">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="e00df-1299">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="e00df-1299">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="e00df-1300">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="e00df-1300">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="e00df-1301">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="e00df-1301">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="e00df-1302">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="e00df-1302">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="e00df-1303">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="e00df-1303">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="e00df-1304">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="e00df-1304">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="e00df-1305">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="e00df-1305">`location` no longer required</span></span>
  * <span data-ttu-id="e00df-1306">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="e00df-1306">Add name and ID support for target</span></span>
  * <span data-ttu-id="e00df-1307">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="e00df-1307">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="e00df-1308">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="e00df-1308">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="e00df-1309">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="e00df-1309">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="e00df-1310">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="e00df-1310">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="e00df-1311">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="e00df-1311">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="e00df-1312">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="e00df-1312">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="e00df-1313">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-1313">Network</span></span>

* <span data-ttu-id="e00df-1314">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="e00df-1314">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="e00df-1315">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="e00df-1315">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="e00df-1316">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="e00df-1316">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="e00df-1317">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="e00df-1317">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="e00df-1318">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="e00df-1318">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="e00df-1319">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="e00df-1319">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="e00df-1320">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="e00df-1320">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="e00df-1321">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="e00df-1321">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="e00df-1322">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="e00df-1322">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="e00df-1323">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="e00df-1323">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="e00df-1324">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1324">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="e00df-1325">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="e00df-1325">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="e00df-1326">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="e00df-1326">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="e00df-1327">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="e00df-1327">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="e00df-1328">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="e00df-1328">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="e00df-1329">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1329">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="e00df-1330">Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS</span><span class="sxs-lookup"><span data-stu-id="e00df-1330">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="e00df-1331">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="e00df-1331">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="e00df-1332">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="e00df-1332">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="e00df-1333">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1333">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="e00df-1334">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="e00df-1334">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="e00df-1335">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="e00df-1335">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="e00df-1336">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="e00df-1336">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="e00df-1337">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="e00df-1337">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="e00df-1338">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="e00df-1338">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="e00df-1339">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="e00df-1339">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="e00df-1340">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="e00df-1340">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="e00df-1341">Perfil</span><span class="sxs-lookup"><span data-stu-id="e00df-1341">Profile</span></span>

* <span data-ttu-id="e00df-1342">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="e00df-1342">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="e00df-1343">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="e00df-1343">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="e00df-1344">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="e00df-1344">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="e00df-1345">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="e00df-1345">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="e00df-1346">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="e00df-1346">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="e00df-1347">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e00df-1347">RDBMS</span></span>

* <span data-ttu-id="e00df-1348">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="e00df-1348">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="e00df-1349">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="e00df-1349">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="e00df-1350">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="e00df-1350">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="e00df-1351">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="e00df-1351">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="e00df-1352">Recurso</span><span class="sxs-lookup"><span data-stu-id="e00df-1352">Resource</span></span>

* <span data-ttu-id="e00df-1353">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1353">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="e00df-1354">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="e00df-1354">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="e00df-1355">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="e00df-1355">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="e00df-1356">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="e00df-1356">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="e00df-1357">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="e00df-1357">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="e00df-1358">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="e00df-1358">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="e00df-1359">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="e00df-1359">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="e00df-1360">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="e00df-1360">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="e00df-1361">Função</span><span class="sxs-lookup"><span data-stu-id="e00df-1361">Role</span></span>

* <span data-ttu-id="e00df-1362">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="e00df-1362">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="e00df-1363">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="e00df-1363">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="e00df-1364">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="e00df-1364">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="e00df-1365">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="e00df-1365">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="e00df-1366">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="e00df-1366">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e00df-1367">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e00df-1367">Service Fabric</span></span>
* <span data-ttu-id="e00df-1368">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="e00df-1368">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="e00df-1369">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="e00df-1369">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="e00df-1370">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="e00df-1370">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="e00df-1371">SQL</span><span class="sxs-lookup"><span data-stu-id="e00df-1371">SQL</span></span>

* <span data-ttu-id="e00df-1372">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="e00df-1372">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="e00df-1373">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="e00df-1373">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="e00df-1374">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="e00df-1374">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="e00df-1375">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-1375">Storage</span></span>

* <span data-ttu-id="e00df-1376">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="e00df-1376">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="e00df-1377">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="e00df-1377">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="e00df-1378">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="e00df-1378">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="e00df-1379">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="e00df-1379">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="e00df-1380">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="e00df-1380">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="e00df-1381">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="e00df-1381">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-1382">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-1382">VM</span></span>

* <span data-ttu-id="e00df-1383">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="e00df-1383">Support configuring nsg</span></span>
* <span data-ttu-id="e00df-1384">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="e00df-1384">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="e00df-1385">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="e00df-1385">Support managed service identities</span></span>
* <span data-ttu-id="e00df-1386">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="e00df-1386">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="e00df-1387">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="e00df-1387">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="e00df-1388">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="e00df-1388">May 10, 2017</span></span>

<span data-ttu-id="e00df-1389">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="e00df-1389">Version 2.0.6</span></span>

* <span data-ttu-id="e00df-1390">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e00df-1390">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="e00df-1391">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="e00df-1391">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="e00df-1392">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e00df-1392">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="e00df-1393">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="e00df-1393">Include Cognitive Services module</span></span>
* <span data-ttu-id="e00df-1394">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e00df-1394">Include Service Fabric module</span></span>
* <span data-ttu-id="e00df-1395">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="e00df-1395">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="e00df-1396">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="e00df-1396">Add support for CDN commands</span></span>
* <span data-ttu-id="e00df-1397">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="e00df-1397">Remove Container module</span></span>
* <span data-ttu-id="e00df-1398">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="e00df-1398">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="e00df-1399">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="e00df-1399">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="e00df-1400">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e00df-1400">Core</span></span>

* <span data-ttu-id="e00df-1401">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="e00df-1401">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="e00df-1402">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="e00df-1402">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="e00df-1403">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="e00df-1403">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="e00df-1404">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="e00df-1404">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="e00df-1405">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="e00df-1405">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="e00df-1406">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="e00df-1406">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="e00df-1407">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="e00df-1407">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="e00df-1408">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="e00df-1408">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="e00df-1409">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="e00df-1409">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="e00df-1410">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="e00df-1410">core: Improved performance</span></span>
* <span data-ttu-id="e00df-1411">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="e00df-1411">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="e00df-1412">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="e00df-1412">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-1413">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-1413">ACS</span></span>

* <span data-ttu-id="e00df-1414">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e00df-1414">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="e00df-1415">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="e00df-1415">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="e00df-1416">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="e00df-1416">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="e00df-1417">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="e00df-1417">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-1418">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-1418">AppService</span></span>

* <span data-ttu-id="e00df-1419">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="e00df-1419">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="e00df-1420">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="e00df-1420">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="e00df-1421">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="e00df-1421">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="e00df-1422">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="e00df-1422">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="e00df-1423">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="e00df-1423">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="e00df-1424">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="e00df-1424">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="e00df-1425">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="e00df-1425">support slot swap with preview</span></span>
* <span data-ttu-id="e00df-1426">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="e00df-1426">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="e00df-1427">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="e00df-1427">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e00df-1428">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e00df-1428">CosmosDB</span></span>

* <span data-ttu-id="e00df-1429">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e00df-1429">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="e00df-1430">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="e00df-1430">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="e00df-1431">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="e00df-1431">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="e00df-1432">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="e00df-1432">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e00df-1433">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e00df-1433">Data Lake Analytics</span></span>

* <span data-ttu-id="e00df-1434">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="e00df-1434">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="e00df-1435">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="e00df-1435">Add support for new catalog item type: package.</span></span> <span data-ttu-id="e00df-1436">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="e00df-1436">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="e00df-1437">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="e00df-1437">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="e00df-1438">Tabela</span><span class="sxs-lookup"><span data-stu-id="e00df-1438">Table</span></span>
  * <span data-ttu-id="e00df-1439">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="e00df-1439">Table valued function</span></span>
  * <span data-ttu-id="e00df-1440">Visualizar</span><span class="sxs-lookup"><span data-stu-id="e00df-1440">View</span></span>
  * <span data-ttu-id="e00df-1441">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="e00df-1441">Table Statistics.</span></span> <span data-ttu-id="e00df-1442">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="e00df-1442">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e00df-1443">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e00df-1443">Data Lake Store</span></span>

* <span data-ttu-id="e00df-1444">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="e00df-1444">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="e00df-1445">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="e00df-1445">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="e00df-1446">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="e00df-1446">missed help for access show.</span></span> <span data-ttu-id="e00df-1447">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="e00df-1447">adding it.</span></span> <span data-ttu-id="e00df-1448">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="e00df-1448">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="e00df-1449">Localizar</span><span class="sxs-lookup"><span data-stu-id="e00df-1449">Find</span></span>

* <span data-ttu-id="e00df-1450">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="e00df-1450">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="e00df-1451">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e00df-1451">KeyVault</span></span>

* <span data-ttu-id="e00df-1452">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="e00df-1452">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="e00df-1453">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="e00df-1453">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="e00df-1454">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="e00df-1454">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="e00df-1455">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="e00df-1455">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="e00df-1456">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="e00df-1456">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="e00df-1457">Laboratório</span><span class="sxs-lookup"><span data-stu-id="e00df-1457">Lab</span></span>

* <span data-ttu-id="e00df-1458">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="e00df-1458">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="e00df-1459">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="e00df-1459">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="e00df-1460">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="e00df-1460">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="e00df-1461">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="e00df-1461">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="e00df-1462">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="e00df-1462">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="e00df-1463">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e00df-1463">Monitor</span></span>

* <span data-ttu-id="e00df-1464">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="e00df-1464">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="e00df-1465">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="e00df-1465">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="e00df-1466">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-1466">Network</span></span>

* <span data-ttu-id="e00df-1467">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="e00df-1467">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="e00df-1468">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1468">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="e00df-1469">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e00df-1469">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="e00df-1470">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e00df-1470">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="e00df-1471">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="e00df-1471">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="e00df-1472">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="e00df-1472">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="e00df-1473">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="e00df-1473">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="e00df-1474">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="e00df-1474">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="e00df-1475">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="e00df-1475">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="e00df-1476">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="e00df-1476">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="e00df-1477">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="e00df-1477">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="e00df-1478">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1478">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="e00df-1479">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="e00df-1479">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="e00df-1480">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="e00df-1480">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="e00df-1481">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="e00df-1481">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="e00df-1482">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="e00df-1482">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="e00df-1483">Perfil</span><span class="sxs-lookup"><span data-stu-id="e00df-1483">Profile</span></span>

* <span data-ttu-id="e00df-1484">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="e00df-1484">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="e00df-1485">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="e00df-1485">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="e00df-1486">Redis</span><span class="sxs-lookup"><span data-stu-id="e00df-1486">Redis</span></span>

* <span data-ttu-id="e00df-1487">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="e00df-1487">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="e00df-1488">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="e00df-1488">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="e00df-1489">Recurso</span><span class="sxs-lookup"><span data-stu-id="e00df-1489">Resource</span></span>

* <span data-ttu-id="e00df-1490">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="e00df-1490">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="e00df-1491">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="e00df-1491">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="e00df-1492">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="e00df-1492">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="e00df-1493">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="e00df-1493">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="e00df-1494">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="e00df-1494">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="e00df-1495">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="e00df-1495">Add docs for az lock update.</span></span> <span data-ttu-id="e00df-1496">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="e00df-1496">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="e00df-1497">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="e00df-1497">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="e00df-1498">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="e00df-1498">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="e00df-1499">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="e00df-1499">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="e00df-1500">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="e00df-1500">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="e00df-1501">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="e00df-1501">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="e00df-1502">Função</span><span class="sxs-lookup"><span data-stu-id="e00df-1502">Role</span></span>

* <span data-ttu-id="e00df-1503">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="e00df-1503">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="e00df-1504">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="e00df-1504">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="e00df-1505">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="e00df-1505">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="e00df-1506">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="e00df-1506">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="e00df-1507">SQL</span><span class="sxs-lookup"><span data-stu-id="e00df-1507">SQL</span></span>

* <span data-ttu-id="e00df-1508">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="e00df-1508">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="e00df-1509">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="e00df-1509">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="e00df-1510">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-1510">Storage</span></span>

* <span data-ttu-id="e00df-1511">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="e00df-1511">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="e00df-1512">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="e00df-1512">Add support for incremental blob copy</span></span>
* <span data-ttu-id="e00df-1513">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="e00df-1513">Add support for large block blob upload</span></span>
* <span data-ttu-id="e00df-1514">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="e00df-1514">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-1515">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-1515">VM</span></span>

* <span data-ttu-id="e00df-1516">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="e00df-1516">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="e00df-1517">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="e00df-1517">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="e00df-1518">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="e00df-1518">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="e00df-1519">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="e00df-1519">az vm/vmss disk</span></span>
  3. <span data-ttu-id="e00df-1520">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="e00df-1520">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="e00df-1521">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="e00df-1521">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="e00df-1522">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="e00df-1522">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="e00df-1523">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="e00df-1523">April 3, 2017</span></span>

<span data-ttu-id="e00df-1524">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="e00df-1524">Version 2.0.2</span></span>

<span data-ttu-id="e00df-1525">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="e00df-1525">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="e00df-1526">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e00df-1526">Core</span></span>

* <span data-ttu-id="e00df-1527">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="e00df-1527">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="e00df-1528">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="e00df-1528">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="e00df-1529">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="e00df-1529">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="e00df-1530">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="e00df-1530">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="e00df-1531">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="e00df-1531">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="e00df-1532">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="e00df-1532">Add prompting for missing template parameters.</span></span> <span data-ttu-id="e00df-1533">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="e00df-1533">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="e00df-1534">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="e00df-1534">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="e00df-1535">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="e00df-1535">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="e00df-1536">ACS</span><span class="sxs-lookup"><span data-stu-id="e00df-1536">ACS</span></span>

* <span data-ttu-id="e00df-1537">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="e00df-1537">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="e00df-1538">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="e00df-1538">Add support for ssh key password prompting.</span></span> <span data-ttu-id="e00df-1539">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="e00df-1539">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="e00df-1540">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="e00df-1540">Add support for windows clusters.</span></span> <span data-ttu-id="e00df-1541">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="e00df-1541">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="e00df-1542">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="e00df-1542">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="e00df-1543">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="e00df-1543">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="e00df-1544">AppService</span><span class="sxs-lookup"><span data-stu-id="e00df-1544">AppService</span></span>

* <span data-ttu-id="e00df-1545">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="e00df-1545">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="e00df-1546">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="e00df-1546">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="e00df-1547">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="e00df-1547">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="e00df-1548">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="e00df-1548">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="e00df-1549">DataLake</span><span class="sxs-lookup"><span data-stu-id="e00df-1549">DataLake</span></span>

* <span data-ttu-id="e00df-1550">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e00df-1550">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="e00df-1551">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e00df-1551">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="e00df-1552">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="e00df-1552">DocuemntDB</span></span>

* <span data-ttu-id="e00df-1553">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="e00df-1553">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="e00df-1554">VM</span><span class="sxs-lookup"><span data-stu-id="e00df-1554">VM</span></span>

* <span data-ttu-id="e00df-1555">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="e00df-1555">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="e00df-1556">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="e00df-1556">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="e00df-1557">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="e00df-1557">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="e00df-1558">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="e00df-1558">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="e00df-1559">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="e00df-1559">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="e00df-1560">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="e00df-1560">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="e00df-1561">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="e00df-1561">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="e00df-1562">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="e00df-1562">February 27, 2017</span></span>

<span data-ttu-id="e00df-1563">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="e00df-1563">Version 2.0.0</span></span>

<span data-ttu-id="e00df-1564">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="e00df-1564">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="e00df-1565">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="e00df-1565">Container Service (acs)</span></span>
- <span data-ttu-id="e00df-1566">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="e00df-1566">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="e00df-1567">Rede</span><span class="sxs-lookup"><span data-stu-id="e00df-1567">Networking</span></span>
- <span data-ttu-id="e00df-1568">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e00df-1568">Storage</span></span>

<span data-ttu-id="e00df-1569">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="e00df-1569">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="e00df-1570">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="e00df-1570">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="e00df-1571">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="e00df-1571">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="e00df-1572">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="e00df-1572">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="e00df-1573">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="e00df-1573">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="e00df-1574">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="e00df-1574">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="e00df-1575">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="e00df-1575">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="e00df-1576">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="e00df-1576">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="e00df-1577">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="e00df-1577">Provide feedback from the command line with the `az feedback` command</span></span>

