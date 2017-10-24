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
ms.openlocfilehash: 2ea9daa558200204750f19b5d22685587ff097ef
ms.sourcegitcommit: 376bc0601aba890630dadd55908c1a65ddf40f5a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/11/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="3565e-104">Notas de versão da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="3565e-104">Azure CLI 2.0 release notes</span></span>

## <a name="october-9-2017"></a><span data-ttu-id="3565e-105">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="3565e-105">October 9, 2017</span></span>

<span data-ttu-id="3565e-106">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="3565e-106">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="3565e-107">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3565e-107">Core</span></span>

* <span data-ttu-id="3565e-108">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="3565e-108">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="3565e-109">AppService</span><span class="sxs-lookup"><span data-stu-id="3565e-109">Appservice</span></span>

* <span data-ttu-id="3565e-110">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="3565e-110">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="3565e-111">Batch</span><span class="sxs-lookup"><span data-stu-id="3565e-111">Batch</span></span>

* <span data-ttu-id="3565e-112">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="3565e-112">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="3565e-113">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="3565e-113">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="3565e-114">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="3565e-114">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="3565e-115">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="3565e-115">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="3565e-116">Batchai</span><span class="sxs-lookup"><span data-stu-id="3565e-116">Batchai</span></span>

* <span data-ttu-id="3565e-117">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="3565e-117">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="3565e-118">Keyvault</span><span class="sxs-lookup"><span data-stu-id="3565e-118">Keyvault</span></span>

* <span data-ttu-id="3565e-119">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="3565e-119">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="3565e-120">(#4448)</span><span class="sxs-lookup"><span data-stu-id="3565e-120">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="3565e-121">Rede</span><span class="sxs-lookup"><span data-stu-id="3565e-121">Network</span></span>

* <span data-ttu-id="3565e-122">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="3565e-122">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="3565e-123">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="3565e-123">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="3565e-124">Recurso</span><span class="sxs-lookup"><span data-stu-id="3565e-124">Resource</span></span>

* <span data-ttu-id="3565e-125">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="3565e-125">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="3565e-126">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="3565e-126">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="3565e-127">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="3565e-127">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="3565e-128">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="3565e-128">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="3565e-129">Sql</span><span class="sxs-lookup"><span data-stu-id="3565e-129">Sql</span></span>

* <span data-ttu-id="3565e-130">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="3565e-130">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="3565e-131">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="3565e-131">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="3565e-132">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="3565e-132">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="3565e-133">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3565e-133">Storage</span></span>

* <span data-ttu-id="3565e-134">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="3565e-134">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="3565e-135">VM</span><span class="sxs-lookup"><span data-stu-id="3565e-135">Vm</span></span>

* <span data-ttu-id="3565e-136">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="3565e-136">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="3565e-137">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="3565e-137">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="3565e-138">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="3565e-138">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="3565e-139">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="3565e-139">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="3565e-140">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="3565e-140">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="3565e-141">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="3565e-141">September 22, 2017</span></span>

<span data-ttu-id="3565e-142">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="3565e-142">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="3565e-143">Recurso</span><span class="sxs-lookup"><span data-stu-id="3565e-143">Resource</span></span>

* <span data-ttu-id="3565e-144">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="3565e-144">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="3565e-145">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="3565e-145">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="3565e-146">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="3565e-146">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="3565e-147">[ALTERAÇÃO SIGNIFICATIVA] O tipo de recurso `managedapp` foi alterado de `appliances` para `applications` e `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="3565e-147">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="3565e-148">Rede</span><span class="sxs-lookup"><span data-stu-id="3565e-148">Network</span></span>

* <span data-ttu-id="3565e-149">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="3565e-149">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="3565e-150">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="3565e-150">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="3565e-151">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="3565e-151">Added `asg` application security group commands</span></span>
* <span data-ttu-id="3565e-152">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="3565e-152">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="3565e-153">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3565e-153">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="3565e-154">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3565e-154">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="3565e-155">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="3565e-155">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="3565e-156">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3565e-156">Storage</span></span>

* <span data-ttu-id="3565e-157">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="3565e-157">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="3565e-158">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="3565e-158">Eventgrid</span></span>

* <span data-ttu-id="3565e-159">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="3565e-159">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="3565e-160">SQL</span><span class="sxs-lookup"><span data-stu-id="3565e-160">SQL</span></span>

* <span data-ttu-id="3565e-161">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="3565e-161">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="3565e-162">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="3565e-162">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="3565e-163">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3565e-163">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="3565e-164">Keyvault</span><span class="sxs-lookup"><span data-stu-id="3565e-164">Keyvault</span></span>

* <span data-ttu-id="3565e-165">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="3565e-165">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="3565e-166">VM</span><span class="sxs-lookup"><span data-stu-id="3565e-166">VM</span></span>

* <span data-ttu-id="3565e-167">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="3565e-167">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="3565e-168">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="3565e-168">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="3565e-169">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="3565e-169">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="3565e-170">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="3565e-170">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="3565e-171">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="3565e-171">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="3565e-172">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="3565e-172">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="3565e-173">ACS</span><span class="sxs-lookup"><span data-stu-id="3565e-173">ACS</span></span>

* <span data-ttu-id="3565e-174">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="3565e-174">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="3565e-175">AppService</span><span class="sxs-lookup"><span data-stu-id="3565e-175">Appservice</span></span>

* <span data-ttu-id="3565e-176">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="3565e-176">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="3565e-177">Backup</span><span class="sxs-lookup"><span data-stu-id="3565e-177">Backup</span></span>

* <span data-ttu-id="3565e-178">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="3565e-178">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="3565e-179">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="3565e-179">September 11, 2017</span></span>

<span data-ttu-id="3565e-180">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="3565e-180">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="3565e-181">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3565e-181">Core</span></span>

* <span data-ttu-id="3565e-182">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="3565e-182">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="3565e-183">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="3565e-183">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="3565e-184">Acs</span><span class="sxs-lookup"><span data-stu-id="3565e-184">Acs</span></span>

* <span data-ttu-id="3565e-185">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="3565e-185">Added `acs list-locations` command</span></span>
* <span data-ttu-id="3565e-186">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="3565e-186">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="3565e-187">AppService</span><span class="sxs-lookup"><span data-stu-id="3565e-187">Appservice</span></span>

* <span data-ttu-id="3565e-188">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="3565e-188">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="3565e-189">CDN</span><span class="sxs-lookup"><span data-stu-id="3565e-189">CDN</span></span>

* <span data-ttu-id="3565e-190">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="3565e-190">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="3565e-191">Extensão</span><span class="sxs-lookup"><span data-stu-id="3565e-191">Extension</span></span>

* <span data-ttu-id="3565e-192">Versão Inicial.</span><span class="sxs-lookup"><span data-stu-id="3565e-192">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="3565e-193">Keyvault</span><span class="sxs-lookup"><span data-stu-id="3565e-193">Keyvault</span></span>

* <span data-ttu-id="3565e-194">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="3565e-194">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="3565e-195">Rede</span><span class="sxs-lookup"><span data-stu-id="3565e-195">Network</span></span>

* <span data-ttu-id="3565e-196">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="3565e-196">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="3565e-197">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="3565e-197">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="3565e-198">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="3565e-198">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="3565e-199">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="3565e-199">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="3565e-200">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="3565e-200">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="3565e-201">Recurso</span><span class="sxs-lookup"><span data-stu-id="3565e-201">Resource</span></span>

* <span data-ttu-id="3565e-202">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="3565e-202">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="3565e-203">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="3565e-203">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="3565e-204">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="3565e-204">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="3565e-205">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="3565e-205">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="3565e-206">SQL</span><span class="sxs-lookup"><span data-stu-id="3565e-206">SQL</span></span>

* <span data-ttu-id="3565e-207">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="3565e-207">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="3565e-208">VM</span><span class="sxs-lookup"><span data-stu-id="3565e-208">VM</span></span>

* <span data-ttu-id="3565e-209">Corrigido: Não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="3565e-209">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="3565e-210">Corrigido: Usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="3565e-210">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="3565e-211">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="3565e-211">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="3565e-212">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="3565e-212">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="3565e-213">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="3565e-213">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="3565e-214">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="3565e-214">August 31, 2017</span></span>

<span data-ttu-id="3565e-215">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="3565e-215">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="3565e-216">Keyvault</span><span class="sxs-lookup"><span data-stu-id="3565e-216">Keyvault</span></span>

* <span data-ttu-id="3565e-217">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="3565e-217">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="3565e-218">Sf</span><span class="sxs-lookup"><span data-stu-id="3565e-218">Sf</span></span>

* <span data-ttu-id="3565e-219">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="3565e-219">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="3565e-220">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3565e-220">Storage</span></span>

* <span data-ttu-id="3565e-221">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="3565e-221">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="3565e-222">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="3565e-222">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="3565e-223">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="3565e-223">August 28, 2017</span></span>

<span data-ttu-id="3565e-224">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="3565e-224">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="3565e-225">CLI</span><span class="sxs-lookup"><span data-stu-id="3565e-225">CLI</span></span>

* <span data-ttu-id="3565e-226">Nota legal adicionada ao `--version`.</span><span class="sxs-lookup"><span data-stu-id="3565e-226">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="3565e-227">ACS</span><span class="sxs-lookup"><span data-stu-id="3565e-227">ACS</span></span>

* <span data-ttu-id="3565e-228">Corrigidas as regiões de visualização.</span><span class="sxs-lookup"><span data-stu-id="3565e-228">Corrected preview regions.</span></span>
* <span data-ttu-id="3565e-229">Corrigida a formatação padrão de `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="3565e-229">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="3565e-230">Saída de comando ACS otimizada.</span><span class="sxs-lookup"><span data-stu-id="3565e-230">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="3565e-231">AppService</span><span class="sxs-lookup"><span data-stu-id="3565e-231">Appservice</span></span>

* <span data-ttu-id="3565e-232">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="3565e-232">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="3565e-233">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="3565e-233">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="3565e-234">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="3565e-234">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="3565e-235">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="3565e-235">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="3565e-236">Correção: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="3565e-236">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="3565e-237">IoT</span><span class="sxs-lookup"><span data-stu-id="3565e-237">IoT</span></span>

* <span data-ttu-id="3565e-238">Correção #3934: Criação de política não limpa as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="3565e-238">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="3565e-239">Rede</span><span class="sxs-lookup"><span data-stu-id="3565e-239">Network</span></span>

* <span data-ttu-id="3565e-240">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="3565e-240">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="3565e-241">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3565e-241">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="3565e-242">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3565e-242">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="3565e-243">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="3565e-243">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="3565e-244">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="3565e-244">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="3565e-245">Perfil</span><span class="sxs-lookup"><span data-stu-id="3565e-245">Profile</span></span>

* <span data-ttu-id="3565e-246">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3565e-246">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="3565e-247">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="3565e-247">Service Fabric</span></span>

* <span data-ttu-id="3565e-248">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="3565e-248">Preview release</span></span>
* <span data-ttu-id="3565e-249">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="3565e-249">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="3565e-250">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="3565e-250">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="3565e-251">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="3565e-251">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="3565e-252">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3565e-252">Storage</span></span>

* <span data-ttu-id="3565e-253">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="3565e-253">Enabled setting blob tier</span></span>
* <span data-ttu-id="3565e-254">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="3565e-254">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="3565e-255">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="3565e-255">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="3565e-256">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="3565e-256">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="3565e-257">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="3565e-257">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="3565e-258">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="3565e-258">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="3565e-259">VM</span><span class="sxs-lookup"><span data-stu-id="3565e-259">VM</span></span>

* <span data-ttu-id="3565e-260">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="3565e-260">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="3565e-261">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="3565e-261">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="3565e-262">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="3565e-262">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="3565e-263">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="3565e-263">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="3565e-264">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="3565e-264">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="3565e-265">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="3565e-265">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="3565e-266">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="3565e-266">August 15, 2017</span></span>

<span data-ttu-id="3565e-267">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="3565e-267">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="3565e-268">ACS</span><span class="sxs-lookup"><span data-stu-id="3565e-268">ACS</span></span>

* <span data-ttu-id="3565e-269">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="3565e-269">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="3565e-270">AppService</span><span class="sxs-lookup"><span data-stu-id="3565e-270">Appservice</span></span>

* <span data-ttu-id="3565e-271">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="3565e-271">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="3565e-272">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="3565e-272">Event Grid</span></span>

* <span data-ttu-id="3565e-273">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="3565e-273">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="3565e-274">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="3565e-274">August 11, 2017</span></span>

<span data-ttu-id="3565e-275">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="3565e-275">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="3565e-276">ACS</span><span class="sxs-lookup"><span data-stu-id="3565e-276">ACS</span></span>

* <span data-ttu-id="3565e-277">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="3565e-277">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="3565e-278">Batch</span><span class="sxs-lookup"><span data-stu-id="3565e-278">Batch</span></span>

* <span data-ttu-id="3565e-279">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="3565e-279">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="3565e-280">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="3565e-280">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="3565e-281">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="3565e-281">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="3565e-282">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="3565e-282">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="3565e-283">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="3565e-283">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="3565e-284">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="3565e-284">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="3565e-285">Componente</span><span class="sxs-lookup"><span data-stu-id="3565e-285">Component</span></span>

* <span data-ttu-id="3565e-286">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="3565e-286">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="3565e-287">Contêiner</span><span class="sxs-lookup"><span data-stu-id="3565e-287">Container</span></span>

* <span data-ttu-id="3565e-288">`create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="3565e-288">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="3565e-289">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3565e-289">Data Lake Store</span></span>

* <span data-ttu-id="3565e-290">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="3565e-290">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="3565e-291">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="3565e-291">Event Grid</span></span>

* <span data-ttu-id="3565e-292">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="3565e-292">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="3565e-293">Rede</span><span class="sxs-lookup"><span data-stu-id="3565e-293">Network</span></span>

* <span data-ttu-id="3565e-294">`lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="3565e-294">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="3565e-295">`application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="3565e-295">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="3565e-296">`application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="3565e-296">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="3565e-297">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="3565e-297">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="3565e-298">Perfil</span><span class="sxs-lookup"><span data-stu-id="3565e-298">Profile</span></span>

* <span data-ttu-id="3565e-299">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="3565e-299">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="3565e-300">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3565e-300">Storage</span></span>

* <span data-ttu-id="3565e-301">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="3565e-301">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="3565e-302">VM</span><span class="sxs-lookup"><span data-stu-id="3565e-302">VM</span></span>

* <span data-ttu-id="3565e-303">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="3565e-303">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="3565e-304">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="3565e-304">Exposed `list-skus` command</span></span>
* <span data-ttu-id="3565e-305">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="3565e-305">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="3565e-306">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="3565e-306">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="3565e-307">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="3565e-307">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="3565e-308">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="3565e-308">July 28, 2017</span></span>

<span data-ttu-id="3565e-309">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="3565e-309">Version 2.0.12</span></span>

* <span data-ttu-id="3565e-310">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="3565e-310">Added container commands</span></span>
* <span data-ttu-id="3565e-311">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="3565e-311">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="3565e-312">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3565e-312">Core</span></span>

* <span data-ttu-id="3565e-313">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="3565e-313">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="3565e-314">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="3565e-314">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="3565e-315">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="3565e-315">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="3565e-316">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="3565e-316">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="3565e-317">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="3565e-317">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="3565e-318">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="3565e-318">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="3565e-319">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="3565e-319">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="3565e-320">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="3565e-320">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="3565e-321">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="3565e-321">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="3565e-322">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="3565e-322">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="3565e-323">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="3565e-323">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="3565e-324">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="3565e-324">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="3565e-325">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="3565e-325">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="3565e-326">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="3565e-326">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="3565e-327">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="3565e-327">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="3565e-328">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="3565e-328">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="3565e-329">ACR</span><span class="sxs-lookup"><span data-stu-id="3565e-329">ACR</span></span>

* <span data-ttu-id="3565e-330">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="3565e-330">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="3565e-331">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="3565e-331">Support SKU update for managed registries</span></span>
* <span data-ttu-id="3565e-332">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="3565e-332">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="3565e-333">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="3565e-333">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="3565e-334">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="3565e-334">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="3565e-335">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="3565e-335">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="3565e-336">ACS</span><span class="sxs-lookup"><span data-stu-id="3565e-336">ACS</span></span>

* <span data-ttu-id="3565e-337">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="3565e-337">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="3565e-338">AppService</span><span class="sxs-lookup"><span data-stu-id="3565e-338">Appservice</span></span>

* <span data-ttu-id="3565e-339">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="3565e-339">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="3565e-340">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="3565e-340">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="3565e-341">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="3565e-341">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="3565e-342">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="3565e-342">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="3565e-343">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="3565e-343">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="3565e-344">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="3565e-344">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="3565e-345">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="3565e-345">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="3565e-346">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="3565e-346">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="3565e-347">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="3565e-347">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="3565e-348">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="3565e-348">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="3565e-349">Batch</span><span class="sxs-lookup"><span data-stu-id="3565e-349">Batch</span></span>

* <span data-ttu-id="3565e-350">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="3565e-350">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="3565e-351">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="3565e-351">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="3565e-352">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="3565e-352">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="3565e-353">CDN</span><span class="sxs-lookup"><span data-stu-id="3565e-353">CDN</span></span>

* <span data-ttu-id="3565e-354">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir.</span><span class="sxs-lookup"><span data-stu-id="3565e-354">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="3565e-355">Nuvem</span><span class="sxs-lookup"><span data-stu-id="3565e-355">Cloud</span></span>

* <span data-ttu-id="3565e-356">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="3565e-356">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="3565e-357">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="3565e-357">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="3565e-358">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="3565e-358">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="3565e-359">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="3565e-359">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="3565e-360">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="3565e-360">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3565e-361">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3565e-361">CosmosDB</span></span>

* <span data-ttu-id="3565e-362">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="3565e-362">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="3565e-363">Adicionado suporte para o TTL padrão de coleção.</span><span class="sxs-lookup"><span data-stu-id="3565e-363">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="3565e-364">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="3565e-364">Data Lake Analytics</span></span>

* <span data-ttu-id="3565e-365">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="3565e-365">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="3565e-366">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="3565e-366">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="3565e-367">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="3565e-367">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="3565e-368">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3565e-368">Data Lake Store</span></span>

* <span data-ttu-id="3565e-369">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="3565e-369">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="3565e-370">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="3565e-370">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="3565e-371">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="3565e-371">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="3565e-372">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3565e-372">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="3565e-373">Interativo</span><span class="sxs-lookup"><span data-stu-id="3565e-373">Interactive</span></span>

* <span data-ttu-id="3565e-374">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="3565e-374">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="3565e-375">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="3565e-375">Increased test coverage</span></span>
* <span data-ttu-id="3565e-376">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="3565e-376">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="3565e-377">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="3565e-377">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="3565e-378">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="3565e-378">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="3565e-379">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="3565e-379">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="3565e-380">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="3565e-380">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="3565e-381">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="3565e-381">Added `--progress` flag</span></span>
* <span data-ttu-id="3565e-382">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="3565e-382">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="3565e-383">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="3565e-383">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="3565e-384">IoT</span><span class="sxs-lookup"><span data-stu-id="3565e-384">IoT</span></span>

* <span data-ttu-id="3565e-385">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="3565e-385">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="3565e-386">(#3934)</span><span class="sxs-lookup"><span data-stu-id="3565e-386">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="3565e-387">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="3565e-387">Key vault</span></span>

* <span data-ttu-id="3565e-388">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="3565e-388">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="3565e-389">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="3565e-389">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="3565e-390">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="3565e-390">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="3565e-391">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="3565e-391">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="3565e-392">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="3565e-392">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="3565e-393">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="3565e-393">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="3565e-394">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="3565e-394">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="3565e-395">(#3307)</span><span class="sxs-lookup"><span data-stu-id="3565e-395">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="3565e-396">Laboratório</span><span class="sxs-lookup"><span data-stu-id="3565e-396">Lab</span></span>

* <span data-ttu-id="3565e-397">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="3565e-397">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="3565e-398">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="3565e-398">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="3565e-399">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3565e-399">Monitor</span></span>

* <span data-ttu-id="3565e-400">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="3565e-400">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="3565e-401">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="3565e-401">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="3565e-402">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="3565e-402">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="3565e-403">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="3565e-403">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="3565e-404">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="3565e-404">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="3565e-405">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="3565e-405">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="3565e-406">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="3565e-406">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="3565e-407">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="3565e-407">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="3565e-408">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="3565e-408">`location` no longer required</span></span>
  * <span data-ttu-id="3565e-409">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="3565e-409">Add name and ID support for target</span></span>
  * <span data-ttu-id="3565e-410">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="3565e-410">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="3565e-411">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="3565e-411">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="3565e-412">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="3565e-412">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="3565e-413">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="3565e-413">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="3565e-414">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="3565e-414">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="3565e-415">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="3565e-415">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="3565e-416">Rede</span><span class="sxs-lookup"><span data-stu-id="3565e-416">Network</span></span>

* <span data-ttu-id="3565e-417">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="3565e-417">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="3565e-418">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="3565e-418">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="3565e-419">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="3565e-419">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="3565e-420">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="3565e-420">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="3565e-421">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="3565e-421">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="3565e-422">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="3565e-422">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="3565e-423">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="3565e-423">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="3565e-424">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="3565e-424">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="3565e-425">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="3565e-425">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="3565e-426">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="3565e-426">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="3565e-427">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="3565e-427">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="3565e-428">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="3565e-428">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="3565e-429">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="3565e-429">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="3565e-430">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="3565e-430">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="3565e-431">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="3565e-431">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="3565e-432">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="3565e-432">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="3565e-433">Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS</span><span class="sxs-lookup"><span data-stu-id="3565e-433">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="3565e-434">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="3565e-434">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="3565e-435">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="3565e-435">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="3565e-436">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="3565e-436">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="3565e-437">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="3565e-437">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="3565e-438">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="3565e-438">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="3565e-439">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="3565e-439">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="3565e-440">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="3565e-440">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="3565e-441">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="3565e-441">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="3565e-442">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="3565e-442">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="3565e-443">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="3565e-443">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="3565e-444">Perfil</span><span class="sxs-lookup"><span data-stu-id="3565e-444">Profile</span></span>

* <span data-ttu-id="3565e-445">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="3565e-445">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="3565e-446">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="3565e-446">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="3565e-447">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="3565e-447">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="3565e-448">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="3565e-448">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="3565e-449">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="3565e-449">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="3565e-450">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3565e-450">RDBMS</span></span>

* <span data-ttu-id="3565e-451">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="3565e-451">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="3565e-452">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="3565e-452">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="3565e-453">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="3565e-453">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="3565e-454">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="3565e-454">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="3565e-455">Recurso</span><span class="sxs-lookup"><span data-stu-id="3565e-455">Resource</span></span>

* <span data-ttu-id="3565e-456">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="3565e-456">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="3565e-457">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="3565e-457">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="3565e-458">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="3565e-458">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="3565e-459">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="3565e-459">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="3565e-460">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="3565e-460">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="3565e-461">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="3565e-461">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="3565e-462">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="3565e-462">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="3565e-463">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="3565e-463">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="3565e-464">Função</span><span class="sxs-lookup"><span data-stu-id="3565e-464">Role</span></span>

* <span data-ttu-id="3565e-465">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="3565e-465">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="3565e-466">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="3565e-466">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="3565e-467">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="3565e-467">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="3565e-468">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="3565e-468">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="3565e-469">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="3565e-469">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="3565e-470">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="3565e-470">Service Fabric</span></span>
* <span data-ttu-id="3565e-471">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="3565e-471">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="3565e-472">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="3565e-472">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="3565e-473">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="3565e-473">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="3565e-474">SQL</span><span class="sxs-lookup"><span data-stu-id="3565e-474">SQL</span></span>

* <span data-ttu-id="3565e-475">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="3565e-475">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="3565e-476">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="3565e-476">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="3565e-477">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="3565e-477">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="3565e-478">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3565e-478">Storage</span></span>

* <span data-ttu-id="3565e-479">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="3565e-479">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="3565e-480">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="3565e-480">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="3565e-481">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="3565e-481">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="3565e-482">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="3565e-482">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="3565e-483">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="3565e-483">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="3565e-484">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="3565e-484">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="3565e-485">VM</span><span class="sxs-lookup"><span data-stu-id="3565e-485">VM</span></span>

* <span data-ttu-id="3565e-486">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="3565e-486">Support configuring nsg</span></span>
* <span data-ttu-id="3565e-487">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="3565e-487">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="3565e-488">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="3565e-488">Support managed service identities</span></span>
* <span data-ttu-id="3565e-489">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="3565e-489">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="3565e-490">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="3565e-490">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="3565e-491">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="3565e-491">May 10, 2017</span></span>

<span data-ttu-id="3565e-492">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="3565e-492">Version 2.0.6</span></span>

* <span data-ttu-id="3565e-493">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3565e-493">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="3565e-494">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="3565e-494">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="3565e-495">Inclusão dos módulos Data Lake Analytics e Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="3565e-495">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="3565e-496">Inclusão do módulo Serviços Cognitivos.</span><span class="sxs-lookup"><span data-stu-id="3565e-496">Include Cognitive Services module.</span></span>
* <span data-ttu-id="3565e-497">Inclusão do módulo Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="3565e-497">Include Service Fabric module.</span></span>
* <span data-ttu-id="3565e-498">Inclusão do módulo Interativo (renomeação de az-shell).</span><span class="sxs-lookup"><span data-stu-id="3565e-498">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="3565e-499">Adição de suporte para comandos CDN.</span><span class="sxs-lookup"><span data-stu-id="3565e-499">Add support for CDN commands.</span></span>
* <span data-ttu-id="3565e-500">Remoção do módulo Contêiner.</span><span class="sxs-lookup"><span data-stu-id="3565e-500">Remove Container module.</span></span>
* <span data-ttu-id="3565e-501">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="3565e-501">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="3565e-502">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="3565e-502">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="3565e-503">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3565e-503">Core</span></span>

* <span data-ttu-id="3565e-504">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="3565e-504">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="3565e-505">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="3565e-505">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="3565e-506">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="3565e-506">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="3565e-507">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="3565e-507">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="3565e-508">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="3565e-508">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="3565e-509">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="3565e-509">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="3565e-510">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="3565e-510">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="3565e-511">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="3565e-511">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="3565e-512">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="3565e-512">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="3565e-513">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="3565e-513">core: Improved performance</span></span>
* <span data-ttu-id="3565e-514">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="3565e-514">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="3565e-515">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="3565e-515">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="3565e-516">ACS</span><span class="sxs-lookup"><span data-stu-id="3565e-516">ACS</span></span>

* <span data-ttu-id="3565e-517">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3565e-517">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="3565e-518">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="3565e-518">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="3565e-519">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="3565e-519">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="3565e-520">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="3565e-520">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="3565e-521">AppService</span><span class="sxs-lookup"><span data-stu-id="3565e-521">AppService</span></span>

* <span data-ttu-id="3565e-522">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="3565e-522">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="3565e-523">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="3565e-523">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="3565e-524">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="3565e-524">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="3565e-525">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="3565e-525">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="3565e-526">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="3565e-526">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="3565e-527">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="3565e-527">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="3565e-528">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="3565e-528">support slot swap with preview</span></span>
* <span data-ttu-id="3565e-529">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="3565e-529">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="3565e-530">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="3565e-530">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3565e-531">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3565e-531">CosmosDB</span></span>

* <span data-ttu-id="3565e-532">Renomeação do módulo DocumentDB para CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="3565e-532">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="3565e-533">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="3565e-533">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="3565e-534">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="3565e-534">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="3565e-535">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="3565e-535">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="3565e-536">Análises Data Lake</span><span class="sxs-lookup"><span data-stu-id="3565e-536">Data Lake Analytics</span></span>

* <span data-ttu-id="3565e-537">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro.</span><span class="sxs-lookup"><span data-stu-id="3565e-537">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="3565e-538">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="3565e-538">Add support for new catalog item type: package.</span></span> <span data-ttu-id="3565e-539">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="3565e-539">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="3565e-540">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="3565e-540">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="3565e-541">Tabela</span><span class="sxs-lookup"><span data-stu-id="3565e-541">Table</span></span>
  * <span data-ttu-id="3565e-542">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="3565e-542">Table valued function</span></span>
  * <span data-ttu-id="3565e-543">Visualizar</span><span class="sxs-lookup"><span data-stu-id="3565e-543">View</span></span>
  * <span data-ttu-id="3565e-544">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="3565e-544">Table Statistics.</span></span> <span data-ttu-id="3565e-545">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela.</span><span class="sxs-lookup"><span data-stu-id="3565e-545">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="3565e-546">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="3565e-546">Data Lake Store</span></span>

* <span data-ttu-id="3565e-547">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor.</span><span class="sxs-lookup"><span data-stu-id="3565e-547">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="3565e-548">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="3565e-548">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="3565e-549">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="3565e-549">missed help for access show.</span></span> <span data-ttu-id="3565e-550">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="3565e-550">adding it.</span></span> <span data-ttu-id="3565e-551">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="3565e-551">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="3565e-552">Localizar</span><span class="sxs-lookup"><span data-stu-id="3565e-552">Find</span></span>

* <span data-ttu-id="3565e-553">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="3565e-553">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="3565e-554">KeyVault</span><span class="sxs-lookup"><span data-stu-id="3565e-554">KeyVault</span></span>

* <span data-ttu-id="3565e-555">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="3565e-555">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="3565e-556">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço.</span><span class="sxs-lookup"><span data-stu-id="3565e-556">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="3565e-557">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="3565e-557">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="3565e-558">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”.</span><span class="sxs-lookup"><span data-stu-id="3565e-558">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="3565e-559">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="3565e-559">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="3565e-560">Laboratório</span><span class="sxs-lookup"><span data-stu-id="3565e-560">Lab</span></span>

* <span data-ttu-id="3565e-561">Adição dos comandos create, show, delete e list ao ambiente do laboratório.</span><span class="sxs-lookup"><span data-stu-id="3565e-561">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="3565e-562">Adição dos comandos show e list para exibir modelos ARM no laboratório.</span><span class="sxs-lookup"><span data-stu-id="3565e-562">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="3565e-563">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório.</span><span class="sxs-lookup"><span data-stu-id="3565e-563">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="3565e-564">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório.</span><span class="sxs-lookup"><span data-stu-id="3565e-564">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="3565e-565">Adição de comandos para gerenciar segredos em um Laboratório.</span><span class="sxs-lookup"><span data-stu-id="3565e-565">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="3565e-566">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="3565e-566">Monitor</span></span>

* <span data-ttu-id="3565e-567">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="3565e-567">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="3565e-568">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="3565e-568">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="3565e-569">Rede</span><span class="sxs-lookup"><span data-stu-id="3565e-569">Network</span></span>

* <span data-ttu-id="3565e-570">Adição do comando `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="3565e-570">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="3565e-571">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="3565e-571">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="3565e-572">Adição de suporte para drenagem de conexão do Gateway de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3565e-572">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="3565e-573">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3565e-573">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="3565e-574">Adição de suporte para filtros de rota e regras do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="3565e-574">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="3565e-575">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="3565e-575">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="3565e-576">Adição de suporte para seletores de tráfego baseados em política da conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="3565e-576">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="3565e-577">Adição de suporte para políticas IPsec da conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="3565e-577">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="3565e-578">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`.</span><span class="sxs-lookup"><span data-stu-id="3565e-578">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="3565e-579">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="3565e-579">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="3565e-580">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="3565e-580">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="3565e-581">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="3565e-581">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="3565e-582">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente.</span><span class="sxs-lookup"><span data-stu-id="3565e-582">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="3565e-583">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente.</span><span class="sxs-lookup"><span data-stu-id="3565e-583">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="3565e-584">Correção de um bug em que `traffic-manager endpoint update` não funciona.</span><span class="sxs-lookup"><span data-stu-id="3565e-584">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="3565e-585">Adição de comandos de visualização “network watcher”.</span><span class="sxs-lookup"><span data-stu-id="3565e-585">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="3565e-586">Perfil</span><span class="sxs-lookup"><span data-stu-id="3565e-586">Profile</span></span>

* <span data-ttu-id="3565e-587">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="3565e-587">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="3565e-588">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="3565e-588">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="3565e-589">Redis</span><span class="sxs-lookup"><span data-stu-id="3565e-589">Redis</span></span>

* <span data-ttu-id="3565e-590">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="3565e-590">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="3565e-591">Preterição do comando “update-settings”.</span><span class="sxs-lookup"><span data-stu-id="3565e-591">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="3565e-592">Recurso</span><span class="sxs-lookup"><span data-stu-id="3565e-592">Resource</span></span>

* <span data-ttu-id="3565e-593">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="3565e-593">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="3565e-594">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="3565e-594">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="3565e-595">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="3565e-595">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="3565e-596">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="3565e-596">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="3565e-597">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="3565e-597">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="3565e-598">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="3565e-598">Add docs for az lock update.</span></span> <span data-ttu-id="3565e-599">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="3565e-599">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="3565e-600">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="3565e-600">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="3565e-601">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="3565e-601">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="3565e-602">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="3565e-602">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="3565e-603">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="3565e-603">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="3565e-604">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="3565e-604">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="3565e-605">Função</span><span class="sxs-lookup"><span data-stu-id="3565e-605">Role</span></span>

* <span data-ttu-id="3565e-606">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="3565e-606">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="3565e-607">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="3565e-607">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="3565e-608">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="3565e-608">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="3565e-609">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="3565e-609">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="3565e-610">SQL</span><span class="sxs-lookup"><span data-stu-id="3565e-610">SQL</span></span>

* <span data-ttu-id="3565e-611">Adição dos comandos az sql server list-usages e az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="3565e-611">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="3565e-612">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="3565e-612">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="3565e-613">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3565e-613">Storage</span></span>

* <span data-ttu-id="3565e-614">Localização padrão da localização do grupo de recursos de `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="3565e-614">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="3565e-615">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="3565e-615">Add support for incremental blob copy</span></span>
* <span data-ttu-id="3565e-616">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="3565e-616">Add support for large block blob upload</span></span>
* <span data-ttu-id="3565e-617">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="3565e-617">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="3565e-618">VM</span><span class="sxs-lookup"><span data-stu-id="3565e-618">VM</span></span>

* <span data-ttu-id="3565e-619">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="3565e-619">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="3565e-620">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="3565e-620">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="3565e-621">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="3565e-621">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="3565e-622">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="3565e-622">az vm/vmss disk</span></span>
  3. <span data-ttu-id="3565e-623">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="3565e-623">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="3565e-624">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="3565e-624">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="3565e-625">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="3565e-625">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="3565e-626">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="3565e-626">April 3, 2017</span></span>

<span data-ttu-id="3565e-627">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="3565e-627">Version 2.0.2</span></span>

<span data-ttu-id="3565e-628">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão.</span><span class="sxs-lookup"><span data-stu-id="3565e-628">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="3565e-629">Núcleo</span><span class="sxs-lookup"><span data-stu-id="3565e-629">Core</span></span>

* <span data-ttu-id="3565e-630">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão.</span><span class="sxs-lookup"><span data-stu-id="3565e-630">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="3565e-631">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="3565e-631">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="3565e-632">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="3565e-632">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="3565e-633">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="3565e-633">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="3565e-634">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="3565e-634">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="3565e-635">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="3565e-635">Add prompting for missing template parameters.</span></span> <span data-ttu-id="3565e-636">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="3565e-636">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="3565e-637">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="3565e-637">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="3565e-638">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="3565e-638">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="3565e-639">ACS</span><span class="sxs-lookup"><span data-stu-id="3565e-639">ACS</span></span>

* <span data-ttu-id="3565e-640">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="3565e-640">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="3565e-641">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="3565e-641">Add support for ssh key password prompting.</span></span> <span data-ttu-id="3565e-642">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="3565e-642">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="3565e-643">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="3565e-643">Add support for windows clusters.</span></span> <span data-ttu-id="3565e-644">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="3565e-644">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="3565e-645">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="3565e-645">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="3565e-646">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="3565e-646">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="3565e-647">AppService</span><span class="sxs-lookup"><span data-stu-id="3565e-647">AppService</span></span>

* <span data-ttu-id="3565e-648">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="3565e-648">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="3565e-649">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="3565e-649">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="3565e-650">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="3565e-650">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="3565e-651">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="3565e-651">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="3565e-652">DataLake</span><span class="sxs-lookup"><span data-stu-id="3565e-652">DataLake</span></span>

* <span data-ttu-id="3565e-653">Versão inicial do módulo do Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="3565e-653">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="3565e-654">Versão inicial do módulo do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="3565e-654">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="3565e-655">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="3565e-655">DocuemntDB</span></span>

* <span data-ttu-id="3565e-656">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="3565e-656">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="3565e-657">VM</span><span class="sxs-lookup"><span data-stu-id="3565e-657">VM</span></span>

* <span data-ttu-id="3565e-658">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="3565e-658">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="3565e-659">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="3565e-659">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="3565e-660">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="3565e-660">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="3565e-661">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="3565e-661">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="3565e-662">Conjunto de dimensionamento de máquinas virtuais: suporte à * para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="3565e-662">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="3565e-663">Adicionar --secrets para o conjunto de dimensionamento de máquinas virtuais e VM ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="3565e-663">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="3565e-664">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="3565e-664">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="3565e-665">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="3565e-665">February 27, 2017</span></span>

<span data-ttu-id="3565e-666">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="3565e-666">Version 2.0.0</span></span>

<span data-ttu-id="3565e-667">Essa versão da CLI do Azure 2.0 é a primeira versão “Disponível”.</span><span class="sxs-lookup"><span data-stu-id="3565e-667">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="3565e-668">A disponibilidade se aplica a esses módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="3565e-668">General availability applies to these command modules:</span></span>
- <span data-ttu-id="3565e-669">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="3565e-669">Container Service (acs)</span></span>
- <span data-ttu-id="3565e-670">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="3565e-670">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="3565e-671">Rede</span><span class="sxs-lookup"><span data-stu-id="3565e-671">Networking</span></span>
- <span data-ttu-id="3565e-672">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3565e-672">Storage</span></span>

<span data-ttu-id="3565e-673">Esses módulos de comando podem ser usados na produção e são compatíveis com o SLA do Microsoft padrão.</span><span class="sxs-lookup"><span data-stu-id="3565e-673">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="3565e-674">Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="3565e-674">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="3565e-675">Você pode fazer perguntas sobre [StackOverflow usando a marcação azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) ou entrar em contato com a equipe do produto pelo endereço [ azfeedback@microsoft.com ](mailto:azfeedback@microsoft.com). Você pode fornecer comentários a partir da linha de comando com o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="3565e-675">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="3565e-676">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="3565e-676">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="3565e-677">Para verificar a versão da CLI, utilize `az --version`.</span><span class="sxs-lookup"><span data-stu-id="3565e-677">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="3565e-678">A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando.</span><span class="sxs-lookup"><span data-stu-id="3565e-678">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="3565e-679">Alguns dos módulos de comando têm um “b*n*” ou “rc*n*” pós-fixado.</span><span class="sxs-lookup"><span data-stu-id="3565e-679">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="3565e-680">Esses módulos de comando ainda estão em visualização e estarão disponíveis no futuro.</span><span class="sxs-lookup"><span data-stu-id="3565e-680">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="3565e-681">Também temos compilações de visualização diárias da CLI.</span><span class="sxs-lookup"><span data-stu-id="3565e-681">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="3565e-682">Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="3565e-682">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="3565e-683">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="3565e-683">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="3565e-684">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="3565e-684">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="3565e-685">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="3565e-685">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="3565e-686">Forneça comentários a partir da linha de comando com o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="3565e-686">Provide feedback from the command line with the `az feedback` command.</span></span>

