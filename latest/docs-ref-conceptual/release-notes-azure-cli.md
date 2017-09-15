---
title: "Notas de versão da CLI do Azure 2.0"
description: "Saiba mais sobre as últimas atualizações da CLI do Azure 2.0"
keywords: "Notas da versão, CLI do Azure 2.0"
author: sptramer
ms.author: sttramer
manager: douge
ms.date: 04/03/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ce0428f7-0a59-4e72-9237-d907b171af51
ms.openlocfilehash: ad30efeb7efafcc5816160ee130665d37adb62c6
ms.sourcegitcommit: e866977985ba0286fa05f41729dd7e7d9ce86f8e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/13/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="0e54b-104">Notas de versão da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="0e54b-104">Azure CLI 2.0 release notes</span></span>

## <a name="september-11-2017"></a><span data-ttu-id="0e54b-105">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="0e54b-105">September 11, 2017</span></span>

<span data-ttu-id="0e54b-106">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="0e54b-106">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="0e54b-107">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0e54b-107">Core</span></span>

* <span data-ttu-id="0e54b-108">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="0e54b-108">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="0e54b-109">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="0e54b-109">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="0e54b-110">Acs</span><span class="sxs-lookup"><span data-stu-id="0e54b-110">Acs</span></span>

* <span data-ttu-id="0e54b-111">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="0e54b-111">Added `acs list-locations` command</span></span>
* <span data-ttu-id="0e54b-112">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="0e54b-112">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="0e54b-113">AppService</span><span class="sxs-lookup"><span data-stu-id="0e54b-113">Appservice</span></span>

* <span data-ttu-id="0e54b-114">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="0e54b-114">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="0e54b-115">CDN</span><span class="sxs-lookup"><span data-stu-id="0e54b-115">CDN</span></span>

* <span data-ttu-id="0e54b-116">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="0e54b-116">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="0e54b-117">Extensão</span><span class="sxs-lookup"><span data-stu-id="0e54b-117">Extension</span></span>

* <span data-ttu-id="0e54b-118">Versão Inicial.</span><span class="sxs-lookup"><span data-stu-id="0e54b-118">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="0e54b-119">Keyvault</span><span class="sxs-lookup"><span data-stu-id="0e54b-119">Keyvault</span></span>

* <span data-ttu-id="0e54b-120">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="0e54b-120">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="0e54b-121">Rede</span><span class="sxs-lookup"><span data-stu-id="0e54b-121">Network</span></span>

* <span data-ttu-id="0e54b-122">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="0e54b-122">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="0e54b-123">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="0e54b-123">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="0e54b-124">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="0e54b-124">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="0e54b-125">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="0e54b-125">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="0e54b-126">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="0e54b-126">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="0e54b-127">Recurso</span><span class="sxs-lookup"><span data-stu-id="0e54b-127">Resource</span></span>

* <span data-ttu-id="0e54b-128">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="0e54b-128">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="0e54b-129">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="0e54b-129">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="0e54b-130">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="0e54b-130">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="0e54b-131">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="0e54b-131">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="0e54b-132">SQL</span><span class="sxs-lookup"><span data-stu-id="0e54b-132">SQL</span></span>

* <span data-ttu-id="0e54b-133">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="0e54b-133">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="0e54b-134">VM</span><span class="sxs-lookup"><span data-stu-id="0e54b-134">VM</span></span>

* <span data-ttu-id="0e54b-135">Corrigido: Não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="0e54b-135">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="0e54b-136">Corrigido: Usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="0e54b-136">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="0e54b-137">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="0e54b-137">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="0e54b-138">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="0e54b-138">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="0e54b-139">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="0e54b-139">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="0e54b-140">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="0e54b-140">August 31, 2017</span></span>

<span data-ttu-id="0e54b-141">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="0e54b-141">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="0e54b-142">Keyvault</span><span class="sxs-lookup"><span data-stu-id="0e54b-142">Keyvault</span></span>

* <span data-ttu-id="0e54b-143">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="0e54b-143">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="0e54b-144">Sf</span><span class="sxs-lookup"><span data-stu-id="0e54b-144">Sf</span></span>

* <span data-ttu-id="0e54b-145">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="0e54b-145">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="0e54b-146">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="0e54b-146">Storage</span></span>

* <span data-ttu-id="0e54b-147">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="0e54b-147">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="0e54b-148">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="0e54b-148">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="0e54b-149">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="0e54b-149">August 28, 2017</span></span>

<span data-ttu-id="0e54b-150">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="0e54b-150">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="0e54b-151">CLI</span><span class="sxs-lookup"><span data-stu-id="0e54b-151">CLI</span></span>

* <span data-ttu-id="0e54b-152">Adicionada uma observação legal para `--version`.</span><span class="sxs-lookup"><span data-stu-id="0e54b-152">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="0e54b-153">ACS</span><span class="sxs-lookup"><span data-stu-id="0e54b-153">ACS</span></span>

* <span data-ttu-id="0e54b-154">Corrigidas as regiões de visualização.</span><span class="sxs-lookup"><span data-stu-id="0e54b-154">Corrected preview regions.</span></span>
* <span data-ttu-id="0e54b-155">Corrigida a formatação padrão de `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="0e54b-155">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="0e54b-156">Otimização de saída de comando do ACS.</span><span class="sxs-lookup"><span data-stu-id="0e54b-156">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="0e54b-157">AppService</span><span class="sxs-lookup"><span data-stu-id="0e54b-157">Appservice</span></span>

* <span data-ttu-id="0e54b-158">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="0e54b-158">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="0e54b-159">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="0e54b-159">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="0e54b-160">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="0e54b-160">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="0e54b-161">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e54b-161">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="0e54b-162">Correção: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="0e54b-162">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="0e54b-163">IoT</span><span class="sxs-lookup"><span data-stu-id="0e54b-163">IoT</span></span>

* <span data-ttu-id="0e54b-164">Correção #3934: Criação de política não limpa as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="0e54b-164">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="0e54b-165">Rede</span><span class="sxs-lookup"><span data-stu-id="0e54b-165">Network</span></span>

* <span data-ttu-id="0e54b-166">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="0e54b-166">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="0e54b-167">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0e54b-167">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="0e54b-168">Adicionado suporte para vários IP e intervalos de porta para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="0e54b-168">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="0e54b-169">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="0e54b-169">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="0e54b-170">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="0e54b-170">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="0e54b-171">Perfil</span><span class="sxs-lookup"><span data-stu-id="0e54b-171">Profile</span></span>

* <span data-ttu-id="0e54b-172">Exposto `--msi` e `--msi-port` para logon com a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="0e54b-172">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0e54b-173">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0e54b-173">Service Fabric</span></span>

* <span data-ttu-id="0e54b-174">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="0e54b-174">Preview release</span></span>
* <span data-ttu-id="0e54b-175">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="0e54b-175">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="0e54b-176">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="0e54b-176">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="0e54b-177">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="0e54b-177">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="0e54b-178">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="0e54b-178">Storage</span></span>

* <span data-ttu-id="0e54b-179">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="0e54b-179">Enabled setting blob tier</span></span>
* <span data-ttu-id="0e54b-180">Adicionados os argumentos `--bypass` e `--default-action` para `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="0e54b-180">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="0e54b-181">Comandos adicionados para adicionar as regras de rede virtual e com base em IP para `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="0e54b-181">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="0e54b-182">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="0e54b-182">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="0e54b-183">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="0e54b-183">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="0e54b-184">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="0e54b-184">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="0e54b-185">VM</span><span class="sxs-lookup"><span data-stu-id="0e54b-185">VM</span></span>

* <span data-ttu-id="0e54b-186">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="0e54b-186">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="0e54b-187">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="0e54b-187">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="0e54b-188">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="0e54b-188">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="0e54b-189">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="0e54b-189">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="0e54b-190">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="0e54b-190">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="0e54b-191">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="0e54b-191">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="0e54b-192">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="0e54b-192">August 15, 2017</span></span>

<span data-ttu-id="0e54b-193">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="0e54b-193">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="0e54b-194">ACS</span><span class="sxs-lookup"><span data-stu-id="0e54b-194">ACS</span></span>

* <span data-ttu-id="0e54b-195">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="0e54b-195">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="0e54b-196">AppService</span><span class="sxs-lookup"><span data-stu-id="0e54b-196">Appservice</span></span>

* <span data-ttu-id="0e54b-197">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="0e54b-197">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="0e54b-198">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="0e54b-198">Event Grid</span></span>

* <span data-ttu-id="0e54b-199">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="0e54b-199">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="0e54b-200">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="0e54b-200">August 11, 2017</span></span>

<span data-ttu-id="0e54b-201">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="0e54b-201">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="0e54b-202">ACS</span><span class="sxs-lookup"><span data-stu-id="0e54b-202">ACS</span></span>

* <span data-ttu-id="0e54b-203">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="0e54b-203">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="0e54b-204">Batch</span><span class="sxs-lookup"><span data-stu-id="0e54b-204">Batch</span></span>

* <span data-ttu-id="0e54b-205">Atualizado para o SDK 3.1.0 do Lote e SDK 4.1.0 do Gerenciamento de Lote</span><span class="sxs-lookup"><span data-stu-id="0e54b-205">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="0e54b-206">Adicionado um novo comando que mostra as contagens de tarefa de um trabalho</span><span class="sxs-lookup"><span data-stu-id="0e54b-206">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="0e54b-207">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="0e54b-207">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="0e54b-208">Ponto de extremidade de conta de lote agora dá suporte ao prefixo conta do Lote “https://” opcional</span><span class="sxs-lookup"><span data-stu-id="0e54b-208">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="0e54b-209">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="0e54b-209">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="0e54b-210">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="0e54b-210">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="0e54b-211">Componente</span><span class="sxs-lookup"><span data-stu-id="0e54b-211">Component</span></span>

* <span data-ttu-id="0e54b-212">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="0e54b-212">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="0e54b-213">Contêiner</span><span class="sxs-lookup"><span data-stu-id="0e54b-213">Container</span></span>

* <span data-ttu-id="0e54b-214">`create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="0e54b-214">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="0e54b-215">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0e54b-215">Data Lake Store</span></span>

* <span data-ttu-id="0e54b-216">Habilitado o controle de progresso</span><span class="sxs-lookup"><span data-stu-id="0e54b-216">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="0e54b-217">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="0e54b-217">Event Grid</span></span>

* <span data-ttu-id="0e54b-218">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="0e54b-218">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="0e54b-219">Rede</span><span class="sxs-lookup"><span data-stu-id="0e54b-219">Network</span></span>

* <span data-ttu-id="0e54b-220">`lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="0e54b-220">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="0e54b-221">`application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="0e54b-221">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="0e54b-222">`application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="0e54b-222">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="0e54b-223">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="0e54b-223">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="0e54b-224">Perfil</span><span class="sxs-lookup"><span data-stu-id="0e54b-224">Profile</span></span>

* <span data-ttu-id="0e54b-225">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="0e54b-225">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="0e54b-226">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="0e54b-226">Storage</span></span>

* <span data-ttu-id="0e54b-227">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="0e54b-227">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="0e54b-228">VM</span><span class="sxs-lookup"><span data-stu-id="0e54b-228">VM</span></span>

* <span data-ttu-id="0e54b-229">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="0e54b-229">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="0e54b-230">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="0e54b-230">Exposed `list-skus` command</span></span>
* <span data-ttu-id="0e54b-231">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="0e54b-231">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="0e54b-232">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="0e54b-232">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="0e54b-233">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="0e54b-233">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="0e54b-234">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="0e54b-234">July 28, 2017</span></span>

<span data-ttu-id="0e54b-235">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="0e54b-235">Version 2.0.12</span></span>

* <span data-ttu-id="0e54b-236">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="0e54b-236">Added container commands</span></span>
* <span data-ttu-id="0e54b-237">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="0e54b-237">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="0e54b-238">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0e54b-238">Core</span></span>

* <span data-ttu-id="0e54b-239">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="0e54b-239">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="0e54b-240">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="0e54b-240">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="0e54b-241">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="0e54b-241">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="0e54b-242">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="0e54b-242">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="0e54b-243">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="0e54b-243">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="0e54b-244">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="0e54b-244">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="0e54b-245">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="0e54b-245">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="0e54b-246">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="0e54b-246">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="0e54b-247">Aprimorado a desativação de áudio de argumentos de análise e acrescentar histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="0e54b-247">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="0e54b-248">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="0e54b-248">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="0e54b-249">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="0e54b-249">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="0e54b-250">Corrigida a idempotência fixa para criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="0e54b-250">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="0e54b-251">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="0e54b-251">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="0e54b-252">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="0e54b-252">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="0e54b-253">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="0e54b-253">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="0e54b-254">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="0e54b-254">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="0e54b-255">ACR</span><span class="sxs-lookup"><span data-stu-id="0e54b-255">ACR</span></span>

* <span data-ttu-id="0e54b-256">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="0e54b-256">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="0e54b-257">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="0e54b-257">Support SKU update for managed registries</span></span>
* <span data-ttu-id="0e54b-258">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="0e54b-258">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="0e54b-259">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="0e54b-259">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="0e54b-260">Adicionada autenticação do AAD adicionada com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="0e54b-260">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="0e54b-261">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="0e54b-261">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="0e54b-262">ACS</span><span class="sxs-lookup"><span data-stu-id="0e54b-262">ACS</span></span>

* <span data-ttu-id="0e54b-263">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="0e54b-263">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="0e54b-264">AppService</span><span class="sxs-lookup"><span data-stu-id="0e54b-264">Appservice</span></span>

* <span data-ttu-id="0e54b-265">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="0e54b-265">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="0e54b-266">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="0e54b-266">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="0e54b-267">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="0e54b-267">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="0e54b-268">Máscara de senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="0e54b-268">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="0e54b-269">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="0e54b-269">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="0e54b-270">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="0e54b-270">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="0e54b-271">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="0e54b-271">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="0e54b-272">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="0e54b-272">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="0e54b-273">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="0e54b-273">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="0e54b-274">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="0e54b-274">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="0e54b-275">Batch</span><span class="sxs-lookup"><span data-stu-id="0e54b-275">Batch</span></span>

* <span data-ttu-id="0e54b-276">Atualizado para o SDK 3.0.0 do Lote com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="0e54b-276">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="0e54b-277">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="0e54b-277">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="0e54b-278">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="0e54b-278">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="0e54b-279">CDN</span><span class="sxs-lookup"><span data-stu-id="0e54b-279">CDN</span></span>

* <span data-ttu-id="0e54b-280">Fornecida uma mensagem de erro mais adequada para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existe.</span><span class="sxs-lookup"><span data-stu-id="0e54b-280">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="0e54b-281">Nuvem</span><span class="sxs-lookup"><span data-stu-id="0e54b-281">Cloud</span></span>

* <span data-ttu-id="0e54b-282">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="0e54b-282">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="0e54b-283">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="0e54b-283">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="0e54b-284">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="0e54b-284">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="0e54b-285">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="0e54b-285">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="0e54b-286">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="0e54b-286">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0e54b-287">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0e54b-287">CosmosDB</span></span>

* <span data-ttu-id="0e54b-288">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="0e54b-288">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="0e54b-289">Adicionado suporte para o TTL padrão de coleção.</span><span class="sxs-lookup"><span data-stu-id="0e54b-289">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="0e54b-290">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="0e54b-290">Data Lake Analytics</span></span>

* <span data-ttu-id="0e54b-291">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="0e54b-291">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="0e54b-292">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="0e54b-292">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="0e54b-293">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="0e54b-293">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="0e54b-294">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0e54b-294">Data Lake Store</span></span>

* <span data-ttu-id="0e54b-295">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="0e54b-295">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="0e54b-296">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="0e54b-296">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="0e54b-297">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="0e54b-297">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="0e54b-298">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0e54b-298">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="0e54b-299">Interativo</span><span class="sxs-lookup"><span data-stu-id="0e54b-299">Interactive</span></span>

* <span data-ttu-id="0e54b-300">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="0e54b-300">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="0e54b-301">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="0e54b-301">Increased test coverage</span></span>
* <span data-ttu-id="0e54b-302">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="0e54b-302">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="0e54b-303">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="0e54b-303">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="0e54b-304">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="0e54b-304">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="0e54b-305">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="0e54b-305">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="0e54b-306">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="0e54b-306">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="0e54b-307">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="0e54b-307">Added `--progress` flag</span></span>
* <span data-ttu-id="0e54b-308">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="0e54b-308">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="0e54b-309">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="0e54b-309">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="0e54b-310">IoT</span><span class="sxs-lookup"><span data-stu-id="0e54b-310">IoT</span></span>

* <span data-ttu-id="0e54b-311">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="0e54b-311">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="0e54b-312">(#3934)</span><span class="sxs-lookup"><span data-stu-id="0e54b-312">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="0e54b-313">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="0e54b-313">Key vault</span></span>

* <span data-ttu-id="0e54b-314">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="0e54b-314">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="0e54b-315">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="0e54b-315">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="0e54b-316">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="0e54b-316">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="0e54b-317">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="0e54b-317">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="0e54b-318">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="0e54b-318">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="0e54b-319">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="0e54b-319">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="0e54b-320">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="0e54b-320">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="0e54b-321">(#3307)</span><span class="sxs-lookup"><span data-stu-id="0e54b-321">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="0e54b-322">Laboratório</span><span class="sxs-lookup"><span data-stu-id="0e54b-322">Lab</span></span>

* <span data-ttu-id="0e54b-323">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="0e54b-323">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="0e54b-324">Adicionada o formatador de tabela `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="0e54b-324">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="0e54b-325">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="0e54b-325">Monitor</span></span>

* <span data-ttu-id="0e54b-326">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="0e54b-326">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="0e54b-327">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="0e54b-327">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="0e54b-328">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="0e54b-328">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="0e54b-329">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="0e54b-329">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="0e54b-330">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="0e54b-330">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="0e54b-331">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="0e54b-331">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="0e54b-332">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="0e54b-332">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="0e54b-333">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="0e54b-333">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="0e54b-334">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="0e54b-334">`location` no longer required</span></span>
  * <span data-ttu-id="0e54b-335">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="0e54b-335">Add name and ID support for target</span></span>
  * <span data-ttu-id="0e54b-336">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="0e54b-336">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="0e54b-337">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="0e54b-337">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="0e54b-338">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="0e54b-338">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="0e54b-339">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="0e54b-339">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="0e54b-340">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="0e54b-340">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="0e54b-341">Argumentos de conveniência adicional e exemplos para `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="0e54b-341">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="0e54b-342">Rede</span><span class="sxs-lookup"><span data-stu-id="0e54b-342">Network</span></span>

* <span data-ttu-id="0e54b-343">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="0e54b-343">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="0e54b-344">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="0e54b-344">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="0e54b-345">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="0e54b-345">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="0e54b-346">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="0e54b-346">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="0e54b-347">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="0e54b-347">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="0e54b-348">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="0e54b-348">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="0e54b-349">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="0e54b-349">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="0e54b-350">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="0e54b-350">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="0e54b-351">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="0e54b-351">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="0e54b-352">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="0e54b-352">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="0e54b-353">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="0e54b-353">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="0e54b-354">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="0e54b-354">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="0e54b-355">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="0e54b-355">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="0e54b-356">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="0e54b-356">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="0e54b-357">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="0e54b-357">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="0e54b-358">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="0e54b-358">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="0e54b-359">Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS</span><span class="sxs-lookup"><span data-stu-id="0e54b-359">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="0e54b-360">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="0e54b-360">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="0e54b-361">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="0e54b-361">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="0e54b-362">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="0e54b-362">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="0e54b-363">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="0e54b-363">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="0e54b-364">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="0e54b-364">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="0e54b-365">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="0e54b-365">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="0e54b-366">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="0e54b-366">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="0e54b-367">Usar o pool padrão de pool de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="0e54b-367">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="0e54b-368">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="0e54b-368">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="0e54b-369">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="0e54b-369">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="0e54b-370">Perfil</span><span class="sxs-lookup"><span data-stu-id="0e54b-370">Profile</span></span>

* <span data-ttu-id="0e54b-371">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="0e54b-371">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="0e54b-372">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="0e54b-372">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="0e54b-373">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="0e54b-373">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="0e54b-374">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="0e54b-374">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="0e54b-375">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="0e54b-375">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="0e54b-376">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0e54b-376">RDBMS</span></span>

* <span data-ttu-id="0e54b-377">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="0e54b-377">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="0e54b-378">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="0e54b-378">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="0e54b-379">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="0e54b-379">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="0e54b-380">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="0e54b-380">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="0e54b-381">Recurso</span><span class="sxs-lookup"><span data-stu-id="0e54b-381">Resource</span></span>

* <span data-ttu-id="0e54b-382">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="0e54b-382">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="0e54b-383">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="0e54b-383">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="0e54b-384">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="0e54b-384">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="0e54b-385">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="0e54b-385">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="0e54b-386">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="0e54b-386">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="0e54b-387">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="0e54b-387">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="0e54b-388">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="0e54b-388">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="0e54b-389">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="0e54b-389">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="0e54b-390">Função</span><span class="sxs-lookup"><span data-stu-id="0e54b-390">Role</span></span>

* <span data-ttu-id="0e54b-391">Suporte à saída para no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="0e54b-391">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="0e54b-392">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="0e54b-392">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="0e54b-393">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="0e54b-393">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="0e54b-394">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="0e54b-394">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="0e54b-395">Adicionada a integração do cofre da chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="0e54b-395">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0e54b-396">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0e54b-396">Service Fabric</span></span>
* <span data-ttu-id="0e54b-397">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="0e54b-397">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="0e54b-398">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="0e54b-398">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="0e54b-399">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="0e54b-399">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="0e54b-400">SQL</span><span class="sxs-lookup"><span data-stu-id="0e54b-400">SQL</span></span>

* <span data-ttu-id="0e54b-401">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="0e54b-401">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="0e54b-402">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="0e54b-402">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="0e54b-403">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="0e54b-403">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="0e54b-404">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="0e54b-404">Storage</span></span>

* <span data-ttu-id="0e54b-405">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="0e54b-405">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="0e54b-406">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="0e54b-406">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="0e54b-407">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="0e54b-407">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="0e54b-408">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="0e54b-408">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="0e54b-409">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="0e54b-409">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="0e54b-410">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="0e54b-410">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="0e54b-411">VM</span><span class="sxs-lookup"><span data-stu-id="0e54b-411">VM</span></span>

* <span data-ttu-id="0e54b-412">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="0e54b-412">Support configuring nsg</span></span>
* <span data-ttu-id="0e54b-413">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="0e54b-413">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="0e54b-414">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="0e54b-414">Support managed service identities</span></span>
* <span data-ttu-id="0e54b-415">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="0e54b-415">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="0e54b-416">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="0e54b-416">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="0e54b-417">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="0e54b-417">May 10, 2017</span></span>

<span data-ttu-id="0e54b-418">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="0e54b-418">Version 2.0.6</span></span>

* <span data-ttu-id="0e54b-419">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0e54b-419">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="0e54b-420">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="0e54b-420">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="0e54b-421">Inclusão dos módulos Data Lake Analytics e Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="0e54b-421">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="0e54b-422">Inclusão do módulo Serviços Cognitivos.</span><span class="sxs-lookup"><span data-stu-id="0e54b-422">Include Cognitive Services module.</span></span>
* <span data-ttu-id="0e54b-423">Inclusão do módulo Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="0e54b-423">Include Service Fabric module.</span></span>
* <span data-ttu-id="0e54b-424">Inclusão do módulo Interativo (renomeação de az-shell).</span><span class="sxs-lookup"><span data-stu-id="0e54b-424">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="0e54b-425">Adição de suporte para comandos CDN.</span><span class="sxs-lookup"><span data-stu-id="0e54b-425">Add support for CDN commands.</span></span>
* <span data-ttu-id="0e54b-426">Remoção do módulo Contêiner.</span><span class="sxs-lookup"><span data-stu-id="0e54b-426">Remove Container module.</span></span>
* <span data-ttu-id="0e54b-427">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="0e54b-427">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="0e54b-428">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="0e54b-428">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="0e54b-429">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0e54b-429">Core</span></span>

* <span data-ttu-id="0e54b-430">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="0e54b-430">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="0e54b-431">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="0e54b-431">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="0e54b-432">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="0e54b-432">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="0e54b-433">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="0e54b-433">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="0e54b-434">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="0e54b-434">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="0e54b-435">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="0e54b-435">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="0e54b-436">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="0e54b-436">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="0e54b-437">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="0e54b-437">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="0e54b-438">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="0e54b-438">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="0e54b-439">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="0e54b-439">core: Improved performance</span></span>
* <span data-ttu-id="0e54b-440">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="0e54b-440">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="0e54b-441">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="0e54b-441">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="0e54b-442">ACS</span><span class="sxs-lookup"><span data-stu-id="0e54b-442">ACS</span></span>

* <span data-ttu-id="0e54b-443">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e54b-443">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="0e54b-444">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="0e54b-444">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="0e54b-445">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="0e54b-445">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="0e54b-446">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="0e54b-446">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="0e54b-447">AppService</span><span class="sxs-lookup"><span data-stu-id="0e54b-447">AppService</span></span>

* <span data-ttu-id="0e54b-448">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="0e54b-448">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="0e54b-449">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="0e54b-449">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="0e54b-450">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="0e54b-450">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="0e54b-451">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="0e54b-451">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="0e54b-452">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="0e54b-452">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="0e54b-453">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="0e54b-453">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="0e54b-454">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="0e54b-454">support slot swap with preview</span></span>
* <span data-ttu-id="0e54b-455">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="0e54b-455">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="0e54b-456">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="0e54b-456">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0e54b-457">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0e54b-457">CosmosDB</span></span>

* <span data-ttu-id="0e54b-458">Renomeação do módulo DocumentDB para CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="0e54b-458">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="0e54b-459">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="0e54b-459">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="0e54b-460">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="0e54b-460">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="0e54b-461">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="0e54b-461">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="0e54b-462">Análises Data Lake</span><span class="sxs-lookup"><span data-stu-id="0e54b-462">Data Lake Analytics</span></span>

* <span data-ttu-id="0e54b-463">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro.</span><span class="sxs-lookup"><span data-stu-id="0e54b-463">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="0e54b-464">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="0e54b-464">Add support for new catalog item type: package.</span></span> <span data-ttu-id="0e54b-465">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="0e54b-465">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="0e54b-466">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="0e54b-466">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="0e54b-467">Tabela</span><span class="sxs-lookup"><span data-stu-id="0e54b-467">Table</span></span>
  * <span data-ttu-id="0e54b-468">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="0e54b-468">Table valued function</span></span>
  * <span data-ttu-id="0e54b-469">Visualizar</span><span class="sxs-lookup"><span data-stu-id="0e54b-469">View</span></span>
  * <span data-ttu-id="0e54b-470">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="0e54b-470">Table Statistics.</span></span> <span data-ttu-id="0e54b-471">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela.</span><span class="sxs-lookup"><span data-stu-id="0e54b-471">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="0e54b-472">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="0e54b-472">Data Lake Store</span></span>

* <span data-ttu-id="0e54b-473">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor.</span><span class="sxs-lookup"><span data-stu-id="0e54b-473">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="0e54b-474">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="0e54b-474">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="0e54b-475">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="0e54b-475">missed help for access show.</span></span> <span data-ttu-id="0e54b-476">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="0e54b-476">adding it.</span></span> <span data-ttu-id="0e54b-477">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="0e54b-477">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="0e54b-478">Localizar</span><span class="sxs-lookup"><span data-stu-id="0e54b-478">Find</span></span>

* <span data-ttu-id="0e54b-479">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="0e54b-479">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="0e54b-480">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0e54b-480">KeyVault</span></span>

* <span data-ttu-id="0e54b-481">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="0e54b-481">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="0e54b-482">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço.</span><span class="sxs-lookup"><span data-stu-id="0e54b-482">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="0e54b-483">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="0e54b-483">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="0e54b-484">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”.</span><span class="sxs-lookup"><span data-stu-id="0e54b-484">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="0e54b-485">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="0e54b-485">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="0e54b-486">Laboratório</span><span class="sxs-lookup"><span data-stu-id="0e54b-486">Lab</span></span>

* <span data-ttu-id="0e54b-487">Adição dos comandos create, show, delete e list ao ambiente do laboratório.</span><span class="sxs-lookup"><span data-stu-id="0e54b-487">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="0e54b-488">Adição dos comandos show e list para exibir modelos ARM no laboratório.</span><span class="sxs-lookup"><span data-stu-id="0e54b-488">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="0e54b-489">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório.</span><span class="sxs-lookup"><span data-stu-id="0e54b-489">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="0e54b-490">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório.</span><span class="sxs-lookup"><span data-stu-id="0e54b-490">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="0e54b-491">Adição de comandos para gerenciar segredos em um Laboratório.</span><span class="sxs-lookup"><span data-stu-id="0e54b-491">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="0e54b-492">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="0e54b-492">Monitor</span></span>

* <span data-ttu-id="0e54b-493">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="0e54b-493">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="0e54b-494">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="0e54b-494">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="0e54b-495">Rede</span><span class="sxs-lookup"><span data-stu-id="0e54b-495">Network</span></span>

* <span data-ttu-id="0e54b-496">Adição do comando `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="0e54b-496">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="0e54b-497">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="0e54b-497">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="0e54b-498">Adição de suporte para drenagem de conexão do Gateway de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0e54b-498">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="0e54b-499">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0e54b-499">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="0e54b-500">Adição de suporte para filtros de rota e regras do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="0e54b-500">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="0e54b-501">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="0e54b-501">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="0e54b-502">Adição de suporte para seletores de tráfego baseados em política da conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="0e54b-502">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="0e54b-503">Adição de suporte para políticas IPsec da conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="0e54b-503">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="0e54b-504">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`.</span><span class="sxs-lookup"><span data-stu-id="0e54b-504">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="0e54b-505">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="0e54b-505">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="0e54b-506">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="0e54b-506">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="0e54b-507">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="0e54b-507">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="0e54b-508">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente.</span><span class="sxs-lookup"><span data-stu-id="0e54b-508">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="0e54b-509">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente.</span><span class="sxs-lookup"><span data-stu-id="0e54b-509">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="0e54b-510">Correção de um bug em que `traffic-manager endpoint update` não funciona.</span><span class="sxs-lookup"><span data-stu-id="0e54b-510">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="0e54b-511">Adição de comandos de visualização “network watcher”.</span><span class="sxs-lookup"><span data-stu-id="0e54b-511">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="0e54b-512">Perfil</span><span class="sxs-lookup"><span data-stu-id="0e54b-512">Profile</span></span>

* <span data-ttu-id="0e54b-513">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="0e54b-513">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="0e54b-514">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="0e54b-514">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="0e54b-515">Redis</span><span class="sxs-lookup"><span data-stu-id="0e54b-515">Redis</span></span>

* <span data-ttu-id="0e54b-516">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="0e54b-516">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="0e54b-517">Preterição do comando “update-settings”.</span><span class="sxs-lookup"><span data-stu-id="0e54b-517">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="0e54b-518">Recurso</span><span class="sxs-lookup"><span data-stu-id="0e54b-518">Resource</span></span>

* <span data-ttu-id="0e54b-519">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="0e54b-519">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="0e54b-520">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="0e54b-520">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="0e54b-521">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="0e54b-521">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="0e54b-522">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="0e54b-522">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="0e54b-523">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="0e54b-523">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="0e54b-524">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="0e54b-524">Add docs for az lock update.</span></span> <span data-ttu-id="0e54b-525">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="0e54b-525">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="0e54b-526">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="0e54b-526">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="0e54b-527">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="0e54b-527">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="0e54b-528">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="0e54b-528">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="0e54b-529">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="0e54b-529">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="0e54b-530">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="0e54b-530">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="0e54b-531">Função</span><span class="sxs-lookup"><span data-stu-id="0e54b-531">Role</span></span>

* <span data-ttu-id="0e54b-532">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="0e54b-532">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="0e54b-533">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="0e54b-533">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="0e54b-534">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="0e54b-534">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="0e54b-535">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="0e54b-535">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="0e54b-536">SQL</span><span class="sxs-lookup"><span data-stu-id="0e54b-536">SQL</span></span>

* <span data-ttu-id="0e54b-537">Adição dos comandos az sql server list-usages e az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="0e54b-537">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="0e54b-538">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="0e54b-538">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="0e54b-539">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="0e54b-539">Storage</span></span>

* <span data-ttu-id="0e54b-540">Localização padrão da localização do grupo de recursos de `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="0e54b-540">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="0e54b-541">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="0e54b-541">Add support for incremental blob copy</span></span>
* <span data-ttu-id="0e54b-542">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="0e54b-542">Add support for large block blob upload</span></span>
* <span data-ttu-id="0e54b-543">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="0e54b-543">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="0e54b-544">VM</span><span class="sxs-lookup"><span data-stu-id="0e54b-544">VM</span></span>

* <span data-ttu-id="0e54b-545">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="0e54b-545">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="0e54b-546">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="0e54b-546">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="0e54b-547">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="0e54b-547">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="0e54b-548">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="0e54b-548">az vm/vmss disk</span></span>
  3. <span data-ttu-id="0e54b-549">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="0e54b-549">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="0e54b-550">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="0e54b-550">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="0e54b-551">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="0e54b-551">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="0e54b-552">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="0e54b-552">April 3, 2017</span></span>

<span data-ttu-id="0e54b-553">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="0e54b-553">Version 2.0.2</span></span>

<span data-ttu-id="0e54b-554">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão.</span><span class="sxs-lookup"><span data-stu-id="0e54b-554">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="0e54b-555">Núcleo</span><span class="sxs-lookup"><span data-stu-id="0e54b-555">Core</span></span>

* <span data-ttu-id="0e54b-556">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão.</span><span class="sxs-lookup"><span data-stu-id="0e54b-556">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="0e54b-557">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="0e54b-557">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="0e54b-558">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="0e54b-558">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="0e54b-559">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="0e54b-559">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="0e54b-560">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="0e54b-560">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="0e54b-561">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="0e54b-561">Add prompting for missing template parameters.</span></span> <span data-ttu-id="0e54b-562">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="0e54b-562">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="0e54b-563">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="0e54b-563">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="0e54b-564">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="0e54b-564">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="0e54b-565">ACS</span><span class="sxs-lookup"><span data-stu-id="0e54b-565">ACS</span></span>

* <span data-ttu-id="0e54b-566">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([&#2554;](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="0e54b-566">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="0e54b-567">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="0e54b-567">Add support for ssh key password prompting.</span></span> <span data-ttu-id="0e54b-568">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="0e54b-568">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="0e54b-569">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="0e54b-569">Add support for windows clusters.</span></span> <span data-ttu-id="0e54b-570">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="0e54b-570">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="0e54b-571">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="0e54b-571">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="0e54b-572">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="0e54b-572">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="0e54b-573">AppService</span><span class="sxs-lookup"><span data-stu-id="0e54b-573">AppService</span></span>

* <span data-ttu-id="0e54b-574">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="0e54b-574">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="0e54b-575">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="0e54b-575">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="0e54b-576">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="0e54b-576">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="0e54b-577">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="0e54b-577">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="0e54b-578">DataLake</span><span class="sxs-lookup"><span data-stu-id="0e54b-578">DataLake</span></span>

* <span data-ttu-id="0e54b-579">Versão inicial do módulo do Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="0e54b-579">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="0e54b-580">Versão inicial do módulo do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="0e54b-580">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="0e54b-581">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="0e54b-581">DocuemntDB</span></span>

* <span data-ttu-id="0e54b-582">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="0e54b-582">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="0e54b-583">VM</span><span class="sxs-lookup"><span data-stu-id="0e54b-583">VM</span></span>

* <span data-ttu-id="0e54b-584">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="0e54b-584">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="0e54b-585">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="0e54b-585">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="0e54b-586">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="0e54b-586">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="0e54b-587">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="0e54b-587">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="0e54b-588">Conjunto de dimensionamento de máquinas virtuais: suporte à * para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="0e54b-588">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="0e54b-589">Adicionar --secrets para o conjunto de dimensionamento de máquinas virtuais e VM ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="0e54b-589">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="0e54b-590">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="0e54b-590">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="0e54b-591">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="0e54b-591">February 27, 2017</span></span>

<span data-ttu-id="0e54b-592">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="0e54b-592">Version 2.0.0</span></span>

<span data-ttu-id="0e54b-593">Essa versão da CLI do Azure 2.0 é a primeira versão “Disponível”.</span><span class="sxs-lookup"><span data-stu-id="0e54b-593">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="0e54b-594">A disponibilidade se aplica a esses módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="0e54b-594">General availability applies to these command modules:</span></span>
- <span data-ttu-id="0e54b-595">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="0e54b-595">Container Service (acs)</span></span>
- <span data-ttu-id="0e54b-596">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="0e54b-596">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="0e54b-597">Rede</span><span class="sxs-lookup"><span data-stu-id="0e54b-597">Networking</span></span>
- <span data-ttu-id="0e54b-598">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="0e54b-598">Storage</span></span>

<span data-ttu-id="0e54b-599">Esses módulos de comando podem ser usados na produção e são compatíveis com o SLA do Microsoft padrão.</span><span class="sxs-lookup"><span data-stu-id="0e54b-599">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="0e54b-600">Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="0e54b-600">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="0e54b-601">Você pode fazer perguntas sobre [StackOverflow usando a marcação azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) ou entrar em contato com a equipe do produto pelo endereço [ azfeedback@microsoft.com ](mailto:azfeedback@microsoft.com). Você pode fornecer comentários a partir da linha de comando com o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="0e54b-601">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="0e54b-602">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="0e54b-602">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="0e54b-603">Para verificar a versão da CLI, utilize `az --version`.</span><span class="sxs-lookup"><span data-stu-id="0e54b-603">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="0e54b-604">A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando.</span><span class="sxs-lookup"><span data-stu-id="0e54b-604">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="0e54b-605">Alguns dos módulos de comando têm um “b*n*” ou “rc*n*” pós-fixado.</span><span class="sxs-lookup"><span data-stu-id="0e54b-605">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="0e54b-606">Esses módulos de comando ainda estão em visualização e estarão disponíveis no futuro.</span><span class="sxs-lookup"><span data-stu-id="0e54b-606">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="0e54b-607">Também temos compilações de visualização diárias da CLI.</span><span class="sxs-lookup"><span data-stu-id="0e54b-607">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="0e54b-608">Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="0e54b-608">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="0e54b-609">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="0e54b-609">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="0e54b-610">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="0e54b-610">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="0e54b-611">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="0e54b-611">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="0e54b-612">Forneça comentários a partir da linha de comando com o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="0e54b-612">Provide feedback from the command line with the `az feedback` command.</span></span>

