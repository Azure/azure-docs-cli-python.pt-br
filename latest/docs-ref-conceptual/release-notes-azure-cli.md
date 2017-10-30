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
ms.openlocfilehash: 429b099dabd27d9356e88791f955ec52acd2a5f9
ms.sourcegitcommit: 9b36c15dc0e10024e23b8018604f5ef63c025de1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/24/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="c38e2-104">Notas de versão da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="c38e2-104">Azure CLI 2.0 release notes</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="c38e2-105">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="c38e2-105">October 24, 2017</span></span>

<span data-ttu-id="c38e2-106">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="c38e2-106">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="c38e2-107">Núcleo</span><span class="sxs-lookup"><span data-stu-id="c38e2-107">Core</span></span>

* <span data-ttu-id="c38e2-108">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="c38e2-108">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="c38e2-109">ACR</span><span class="sxs-lookup"><span data-stu-id="c38e2-109">ACR</span></span>

* <span data-ttu-id="c38e2-110">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="c38e2-110">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="c38e2-111">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="c38e2-111">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="c38e2-112">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="c38e2-112">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="c38e2-113">ACS</span><span class="sxs-lookup"><span data-stu-id="c38e2-113">ACS</span></span>

* <span data-ttu-id="c38e2-114">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="c38e2-114">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="c38e2-115">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="c38e2-115">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="c38e2-116">AppService</span><span class="sxs-lookup"><span data-stu-id="c38e2-116">Appservice</span></span>

* <span data-ttu-id="c38e2-117">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="c38e2-117">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="c38e2-118">Componente</span><span class="sxs-lookup"><span data-stu-id="c38e2-118">Component</span></span>

* <span data-ttu-id="c38e2-119">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="c38e2-119">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="c38e2-120">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="c38e2-120">Monitor</span></span>

* <span data-ttu-id="c38e2-121">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="c38e2-121">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="c38e2-122">Recurso</span><span class="sxs-lookup"><span data-stu-id="c38e2-122">Resource</span></span>

* <span data-ttu-id="c38e2-123">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="c38e2-123">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="c38e2-124">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="c38e2-124">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="c38e2-125">VM</span><span class="sxs-lookup"><span data-stu-id="c38e2-125">VM</span></span>

* <span data-ttu-id="c38e2-126">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c38e2-126">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="c38e2-127">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="c38e2-127">October 9, 2017</span></span>

<span data-ttu-id="c38e2-128">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="c38e2-128">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="c38e2-129">Núcleo</span><span class="sxs-lookup"><span data-stu-id="c38e2-129">Core</span></span>

* <span data-ttu-id="c38e2-130">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c38e2-130">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="c38e2-131">AppService</span><span class="sxs-lookup"><span data-stu-id="c38e2-131">Appservice</span></span>

* <span data-ttu-id="c38e2-132">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="c38e2-132">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="c38e2-133">Batch</span><span class="sxs-lookup"><span data-stu-id="c38e2-133">Batch</span></span>

* <span data-ttu-id="c38e2-134">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="c38e2-134">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="c38e2-135">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="c38e2-135">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="c38e2-136">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="c38e2-136">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="c38e2-137">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="c38e2-137">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="c38e2-138">Batchai</span><span class="sxs-lookup"><span data-stu-id="c38e2-138">Batchai</span></span>

* <span data-ttu-id="c38e2-139">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="c38e2-139">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="c38e2-140">Keyvault</span><span class="sxs-lookup"><span data-stu-id="c38e2-140">Keyvault</span></span>

* <span data-ttu-id="c38e2-141">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="c38e2-141">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="c38e2-142">(#4448)</span><span class="sxs-lookup"><span data-stu-id="c38e2-142">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="c38e2-143">Rede</span><span class="sxs-lookup"><span data-stu-id="c38e2-143">Network</span></span>

* <span data-ttu-id="c38e2-144">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="c38e2-144">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="c38e2-145">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="c38e2-145">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="c38e2-146">Recurso</span><span class="sxs-lookup"><span data-stu-id="c38e2-146">Resource</span></span>

* <span data-ttu-id="c38e2-147">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="c38e2-147">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="c38e2-148">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="c38e2-148">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="c38e2-149">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="c38e2-149">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="c38e2-150">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="c38e2-150">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="c38e2-151">Sql</span><span class="sxs-lookup"><span data-stu-id="c38e2-151">Sql</span></span>

* <span data-ttu-id="c38e2-152">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="c38e2-152">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="c38e2-153">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="c38e2-153">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="c38e2-154">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="c38e2-154">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="c38e2-155">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="c38e2-155">Storage</span></span>

* <span data-ttu-id="c38e2-156">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="c38e2-156">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="c38e2-157">VM</span><span class="sxs-lookup"><span data-stu-id="c38e2-157">Vm</span></span>

* <span data-ttu-id="c38e2-158">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="c38e2-158">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="c38e2-159">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c38e2-159">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="c38e2-160">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="c38e2-160">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="c38e2-161">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="c38e2-161">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="c38e2-162">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c38e2-162">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="c38e2-163">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="c38e2-163">September 22, 2017</span></span>

<span data-ttu-id="c38e2-164">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="c38e2-164">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="c38e2-165">Recurso</span><span class="sxs-lookup"><span data-stu-id="c38e2-165">Resource</span></span>

* <span data-ttu-id="c38e2-166">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="c38e2-166">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="c38e2-167">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="c38e2-167">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="c38e2-168">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="c38e2-168">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="c38e2-169">[ALTERAÇÃO SIGNIFICATIVA] O tipo de recurso `managedapp` foi alterado de `appliances` para `applications` e `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="c38e2-169">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="c38e2-170">Rede</span><span class="sxs-lookup"><span data-stu-id="c38e2-170">Network</span></span>

* <span data-ttu-id="c38e2-171">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="c38e2-171">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="c38e2-172">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="c38e2-172">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="c38e2-173">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="c38e2-173">Added `asg` application security group commands</span></span>
* <span data-ttu-id="c38e2-174">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="c38e2-174">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="c38e2-175">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c38e2-175">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="c38e2-176">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c38e2-176">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="c38e2-177">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="c38e2-177">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="c38e2-178">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="c38e2-178">Storage</span></span>

* <span data-ttu-id="c38e2-179">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="c38e2-179">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="c38e2-180">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="c38e2-180">Eventgrid</span></span>

* <span data-ttu-id="c38e2-181">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="c38e2-181">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="c38e2-182">SQL</span><span class="sxs-lookup"><span data-stu-id="c38e2-182">SQL</span></span>

* <span data-ttu-id="c38e2-183">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="c38e2-183">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="c38e2-184">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="c38e2-184">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="c38e2-185">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c38e2-185">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="c38e2-186">Keyvault</span><span class="sxs-lookup"><span data-stu-id="c38e2-186">Keyvault</span></span>

* <span data-ttu-id="c38e2-187">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="c38e2-187">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="c38e2-188">VM</span><span class="sxs-lookup"><span data-stu-id="c38e2-188">VM</span></span>

* <span data-ttu-id="c38e2-189">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="c38e2-189">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="c38e2-190">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="c38e2-190">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="c38e2-191">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="c38e2-191">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="c38e2-192">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="c38e2-192">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="c38e2-193">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="c38e2-193">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="c38e2-194">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="c38e2-194">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="c38e2-195">ACS</span><span class="sxs-lookup"><span data-stu-id="c38e2-195">ACS</span></span>

* <span data-ttu-id="c38e2-196">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="c38e2-196">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="c38e2-197">AppService</span><span class="sxs-lookup"><span data-stu-id="c38e2-197">Appservice</span></span>

* <span data-ttu-id="c38e2-198">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="c38e2-198">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="c38e2-199">Backup</span><span class="sxs-lookup"><span data-stu-id="c38e2-199">Backup</span></span>

* <span data-ttu-id="c38e2-200">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="c38e2-200">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="c38e2-201">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="c38e2-201">September 11, 2017</span></span>

<span data-ttu-id="c38e2-202">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="c38e2-202">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="c38e2-203">Núcleo</span><span class="sxs-lookup"><span data-stu-id="c38e2-203">Core</span></span>

* <span data-ttu-id="c38e2-204">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="c38e2-204">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="c38e2-205">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="c38e2-205">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="c38e2-206">Acs</span><span class="sxs-lookup"><span data-stu-id="c38e2-206">Acs</span></span>

* <span data-ttu-id="c38e2-207">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="c38e2-207">Added `acs list-locations` command</span></span>
* <span data-ttu-id="c38e2-208">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="c38e2-208">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="c38e2-209">AppService</span><span class="sxs-lookup"><span data-stu-id="c38e2-209">Appservice</span></span>

* <span data-ttu-id="c38e2-210">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="c38e2-210">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="c38e2-211">CDN</span><span class="sxs-lookup"><span data-stu-id="c38e2-211">CDN</span></span>

* <span data-ttu-id="c38e2-212">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="c38e2-212">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="c38e2-213">Extensão</span><span class="sxs-lookup"><span data-stu-id="c38e2-213">Extension</span></span>

* <span data-ttu-id="c38e2-214">Versão Inicial.</span><span class="sxs-lookup"><span data-stu-id="c38e2-214">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="c38e2-215">Keyvault</span><span class="sxs-lookup"><span data-stu-id="c38e2-215">Keyvault</span></span>

* <span data-ttu-id="c38e2-216">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="c38e2-216">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="c38e2-217">Rede</span><span class="sxs-lookup"><span data-stu-id="c38e2-217">Network</span></span>

* <span data-ttu-id="c38e2-218">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="c38e2-218">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="c38e2-219">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="c38e2-219">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="c38e2-220">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="c38e2-220">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="c38e2-221">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="c38e2-221">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="c38e2-222">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="c38e2-222">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="c38e2-223">Recurso</span><span class="sxs-lookup"><span data-stu-id="c38e2-223">Resource</span></span>

* <span data-ttu-id="c38e2-224">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="c38e2-224">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="c38e2-225">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="c38e2-225">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="c38e2-226">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="c38e2-226">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="c38e2-227">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="c38e2-227">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="c38e2-228">SQL</span><span class="sxs-lookup"><span data-stu-id="c38e2-228">SQL</span></span>

* <span data-ttu-id="c38e2-229">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="c38e2-229">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="c38e2-230">VM</span><span class="sxs-lookup"><span data-stu-id="c38e2-230">VM</span></span>

* <span data-ttu-id="c38e2-231">Corrigido: Não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="c38e2-231">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="c38e2-232">Corrigido: Usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="c38e2-232">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="c38e2-233">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c38e2-233">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="c38e2-234">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="c38e2-234">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="c38e2-235">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="c38e2-235">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="c38e2-236">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="c38e2-236">August 31, 2017</span></span>

<span data-ttu-id="c38e2-237">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="c38e2-237">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="c38e2-238">Keyvault</span><span class="sxs-lookup"><span data-stu-id="c38e2-238">Keyvault</span></span>

* <span data-ttu-id="c38e2-239">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="c38e2-239">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="c38e2-240">Sf</span><span class="sxs-lookup"><span data-stu-id="c38e2-240">Sf</span></span>

* <span data-ttu-id="c38e2-241">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="c38e2-241">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="c38e2-242">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="c38e2-242">Storage</span></span>

* <span data-ttu-id="c38e2-243">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="c38e2-243">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="c38e2-244">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="c38e2-244">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="c38e2-245">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="c38e2-245">August 28, 2017</span></span>

<span data-ttu-id="c38e2-246">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="c38e2-246">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="c38e2-247">CLI</span><span class="sxs-lookup"><span data-stu-id="c38e2-247">CLI</span></span>

* <span data-ttu-id="c38e2-248">Nota legal adicionada ao `--version`.</span><span class="sxs-lookup"><span data-stu-id="c38e2-248">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="c38e2-249">ACS</span><span class="sxs-lookup"><span data-stu-id="c38e2-249">ACS</span></span>

* <span data-ttu-id="c38e2-250">Corrigidas as regiões de visualização.</span><span class="sxs-lookup"><span data-stu-id="c38e2-250">Corrected preview regions.</span></span>
* <span data-ttu-id="c38e2-251">Corrigida a formatação padrão de `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="c38e2-251">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="c38e2-252">Saída de comando ACS otimizada.</span><span class="sxs-lookup"><span data-stu-id="c38e2-252">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="c38e2-253">AppService</span><span class="sxs-lookup"><span data-stu-id="c38e2-253">Appservice</span></span>

* <span data-ttu-id="c38e2-254">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="c38e2-254">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="c38e2-255">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="c38e2-255">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="c38e2-256">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="c38e2-256">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="c38e2-257">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="c38e2-257">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="c38e2-258">Correção: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="c38e2-258">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="c38e2-259">IoT</span><span class="sxs-lookup"><span data-stu-id="c38e2-259">IoT</span></span>

* <span data-ttu-id="c38e2-260">Correção #3934: Criação de política não limpa as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="c38e2-260">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="c38e2-261">Rede</span><span class="sxs-lookup"><span data-stu-id="c38e2-261">Network</span></span>

* <span data-ttu-id="c38e2-262">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="c38e2-262">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="c38e2-263">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c38e2-263">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="c38e2-264">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c38e2-264">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="c38e2-265">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="c38e2-265">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="c38e2-266">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="c38e2-266">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="c38e2-267">Perfil</span><span class="sxs-lookup"><span data-stu-id="c38e2-267">Profile</span></span>

* <span data-ttu-id="c38e2-268">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="c38e2-268">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c38e2-269">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c38e2-269">Service Fabric</span></span>

* <span data-ttu-id="c38e2-270">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="c38e2-270">Preview release</span></span>
* <span data-ttu-id="c38e2-271">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="c38e2-271">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="c38e2-272">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="c38e2-272">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="c38e2-273">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="c38e2-273">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="c38e2-274">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="c38e2-274">Storage</span></span>

* <span data-ttu-id="c38e2-275">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="c38e2-275">Enabled setting blob tier</span></span>
* <span data-ttu-id="c38e2-276">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="c38e2-276">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="c38e2-277">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="c38e2-277">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="c38e2-278">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="c38e2-278">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="c38e2-279">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="c38e2-279">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="c38e2-280">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="c38e2-280">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="c38e2-281">VM</span><span class="sxs-lookup"><span data-stu-id="c38e2-281">VM</span></span>

* <span data-ttu-id="c38e2-282">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="c38e2-282">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="c38e2-283">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="c38e2-283">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="c38e2-284">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="c38e2-284">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="c38e2-285">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="c38e2-285">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="c38e2-286">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="c38e2-286">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="c38e2-287">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="c38e2-287">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="c38e2-288">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="c38e2-288">August 15, 2017</span></span>

<span data-ttu-id="c38e2-289">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="c38e2-289">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="c38e2-290">ACS</span><span class="sxs-lookup"><span data-stu-id="c38e2-290">ACS</span></span>

* <span data-ttu-id="c38e2-291">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="c38e2-291">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="c38e2-292">AppService</span><span class="sxs-lookup"><span data-stu-id="c38e2-292">Appservice</span></span>

* <span data-ttu-id="c38e2-293">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="c38e2-293">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="c38e2-294">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="c38e2-294">Event Grid</span></span>

* <span data-ttu-id="c38e2-295">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="c38e2-295">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="c38e2-296">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="c38e2-296">August 11, 2017</span></span>

<span data-ttu-id="c38e2-297">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="c38e2-297">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="c38e2-298">ACS</span><span class="sxs-lookup"><span data-stu-id="c38e2-298">ACS</span></span>

* <span data-ttu-id="c38e2-299">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="c38e2-299">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="c38e2-300">Batch</span><span class="sxs-lookup"><span data-stu-id="c38e2-300">Batch</span></span>

* <span data-ttu-id="c38e2-301">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="c38e2-301">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="c38e2-302">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="c38e2-302">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="c38e2-303">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="c38e2-303">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="c38e2-304">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="c38e2-304">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="c38e2-305">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="c38e2-305">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="c38e2-306">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="c38e2-306">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="c38e2-307">Componente</span><span class="sxs-lookup"><span data-stu-id="c38e2-307">Component</span></span>

* <span data-ttu-id="c38e2-308">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="c38e2-308">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="c38e2-309">Contêiner</span><span class="sxs-lookup"><span data-stu-id="c38e2-309">Container</span></span>

* <span data-ttu-id="c38e2-310">`create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="c38e2-310">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="c38e2-311">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c38e2-311">Data Lake Store</span></span>

* <span data-ttu-id="c38e2-312">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="c38e2-312">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="c38e2-313">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="c38e2-313">Event Grid</span></span>

* <span data-ttu-id="c38e2-314">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="c38e2-314">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="c38e2-315">Rede</span><span class="sxs-lookup"><span data-stu-id="c38e2-315">Network</span></span>

* <span data-ttu-id="c38e2-316">`lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="c38e2-316">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="c38e2-317">`application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="c38e2-317">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="c38e2-318">`application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="c38e2-318">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="c38e2-319">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="c38e2-319">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="c38e2-320">Perfil</span><span class="sxs-lookup"><span data-stu-id="c38e2-320">Profile</span></span>

* <span data-ttu-id="c38e2-321">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="c38e2-321">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="c38e2-322">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="c38e2-322">Storage</span></span>

* <span data-ttu-id="c38e2-323">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="c38e2-323">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="c38e2-324">VM</span><span class="sxs-lookup"><span data-stu-id="c38e2-324">VM</span></span>

* <span data-ttu-id="c38e2-325">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="c38e2-325">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="c38e2-326">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="c38e2-326">Exposed `list-skus` command</span></span>
* <span data-ttu-id="c38e2-327">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="c38e2-327">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="c38e2-328">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="c38e2-328">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="c38e2-329">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="c38e2-329">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="c38e2-330">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="c38e2-330">July 28, 2017</span></span>

<span data-ttu-id="c38e2-331">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="c38e2-331">Version 2.0.12</span></span>

* <span data-ttu-id="c38e2-332">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="c38e2-332">Added container commands</span></span>
* <span data-ttu-id="c38e2-333">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="c38e2-333">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="c38e2-334">Núcleo</span><span class="sxs-lookup"><span data-stu-id="c38e2-334">Core</span></span>

* <span data-ttu-id="c38e2-335">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="c38e2-335">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="c38e2-336">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="c38e2-336">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="c38e2-337">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="c38e2-337">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="c38e2-338">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="c38e2-338">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="c38e2-339">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="c38e2-339">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="c38e2-340">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="c38e2-340">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="c38e2-341">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="c38e2-341">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="c38e2-342">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="c38e2-342">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="c38e2-343">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="c38e2-343">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="c38e2-344">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="c38e2-344">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="c38e2-345">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="c38e2-345">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="c38e2-346">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="c38e2-346">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="c38e2-347">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="c38e2-347">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="c38e2-348">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="c38e2-348">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="c38e2-349">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="c38e2-349">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="c38e2-350">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="c38e2-350">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="c38e2-351">ACR</span><span class="sxs-lookup"><span data-stu-id="c38e2-351">ACR</span></span>

* <span data-ttu-id="c38e2-352">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="c38e2-352">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="c38e2-353">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="c38e2-353">Support SKU update for managed registries</span></span>
* <span data-ttu-id="c38e2-354">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="c38e2-354">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="c38e2-355">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="c38e2-355">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="c38e2-356">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="c38e2-356">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="c38e2-357">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="c38e2-357">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="c38e2-358">ACS</span><span class="sxs-lookup"><span data-stu-id="c38e2-358">ACS</span></span>

* <span data-ttu-id="c38e2-359">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="c38e2-359">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="c38e2-360">AppService</span><span class="sxs-lookup"><span data-stu-id="c38e2-360">Appservice</span></span>

* <span data-ttu-id="c38e2-361">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="c38e2-361">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="c38e2-362">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="c38e2-362">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="c38e2-363">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="c38e2-363">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="c38e2-364">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="c38e2-364">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="c38e2-365">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="c38e2-365">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="c38e2-366">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="c38e2-366">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="c38e2-367">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="c38e2-367">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="c38e2-368">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="c38e2-368">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="c38e2-369">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="c38e2-369">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="c38e2-370">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="c38e2-370">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="c38e2-371">Batch</span><span class="sxs-lookup"><span data-stu-id="c38e2-371">Batch</span></span>

* <span data-ttu-id="c38e2-372">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="c38e2-372">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="c38e2-373">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="c38e2-373">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="c38e2-374">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="c38e2-374">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="c38e2-375">CDN</span><span class="sxs-lookup"><span data-stu-id="c38e2-375">CDN</span></span>

* <span data-ttu-id="c38e2-376">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir.</span><span class="sxs-lookup"><span data-stu-id="c38e2-376">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="c38e2-377">Nuvem</span><span class="sxs-lookup"><span data-stu-id="c38e2-377">Cloud</span></span>

* <span data-ttu-id="c38e2-378">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="c38e2-378">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="c38e2-379">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="c38e2-379">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="c38e2-380">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="c38e2-380">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="c38e2-381">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="c38e2-381">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="c38e2-382">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="c38e2-382">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c38e2-383">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c38e2-383">CosmosDB</span></span>

* <span data-ttu-id="c38e2-384">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="c38e2-384">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="c38e2-385">Adicionado suporte para o TTL padrão de coleção.</span><span class="sxs-lookup"><span data-stu-id="c38e2-385">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c38e2-386">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c38e2-386">Data Lake Analytics</span></span>

* <span data-ttu-id="c38e2-387">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="c38e2-387">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="c38e2-388">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="c38e2-388">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="c38e2-389">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="c38e2-389">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c38e2-390">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c38e2-390">Data Lake Store</span></span>

* <span data-ttu-id="c38e2-391">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="c38e2-391">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="c38e2-392">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="c38e2-392">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="c38e2-393">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="c38e2-393">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="c38e2-394">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c38e2-394">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="c38e2-395">Interativo</span><span class="sxs-lookup"><span data-stu-id="c38e2-395">Interactive</span></span>

* <span data-ttu-id="c38e2-396">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="c38e2-396">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="c38e2-397">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="c38e2-397">Increased test coverage</span></span>
* <span data-ttu-id="c38e2-398">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="c38e2-398">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="c38e2-399">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="c38e2-399">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="c38e2-400">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="c38e2-400">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="c38e2-401">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="c38e2-401">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="c38e2-402">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="c38e2-402">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="c38e2-403">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="c38e2-403">Added `--progress` flag</span></span>
* <span data-ttu-id="c38e2-404">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="c38e2-404">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="c38e2-405">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="c38e2-405">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="c38e2-406">IoT</span><span class="sxs-lookup"><span data-stu-id="c38e2-406">IoT</span></span>

* <span data-ttu-id="c38e2-407">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="c38e2-407">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="c38e2-408">(#3934)</span><span class="sxs-lookup"><span data-stu-id="c38e2-408">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="c38e2-409">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="c38e2-409">Key vault</span></span>

* <span data-ttu-id="c38e2-410">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="c38e2-410">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="c38e2-411">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="c38e2-411">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="c38e2-412">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="c38e2-412">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="c38e2-413">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="c38e2-413">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="c38e2-414">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="c38e2-414">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="c38e2-415">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="c38e2-415">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="c38e2-416">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="c38e2-416">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="c38e2-417">(#3307)</span><span class="sxs-lookup"><span data-stu-id="c38e2-417">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="c38e2-418">Laboratório</span><span class="sxs-lookup"><span data-stu-id="c38e2-418">Lab</span></span>

* <span data-ttu-id="c38e2-419">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="c38e2-419">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="c38e2-420">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="c38e2-420">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="c38e2-421">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="c38e2-421">Monitor</span></span>

* <span data-ttu-id="c38e2-422">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="c38e2-422">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="c38e2-423">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="c38e2-423">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="c38e2-424">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="c38e2-424">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="c38e2-425">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="c38e2-425">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="c38e2-426">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="c38e2-426">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="c38e2-427">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="c38e2-427">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="c38e2-428">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="c38e2-428">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="c38e2-429">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="c38e2-429">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="c38e2-430">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="c38e2-430">`location` no longer required</span></span>
  * <span data-ttu-id="c38e2-431">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="c38e2-431">Add name and ID support for target</span></span>
  * <span data-ttu-id="c38e2-432">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="c38e2-432">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="c38e2-433">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="c38e2-433">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="c38e2-434">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="c38e2-434">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="c38e2-435">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="c38e2-435">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="c38e2-436">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="c38e2-436">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="c38e2-437">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="c38e2-437">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="c38e2-438">Rede</span><span class="sxs-lookup"><span data-stu-id="c38e2-438">Network</span></span>

* <span data-ttu-id="c38e2-439">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="c38e2-439">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="c38e2-440">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="c38e2-440">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="c38e2-441">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="c38e2-441">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="c38e2-442">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="c38e2-442">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="c38e2-443">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="c38e2-443">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="c38e2-444">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="c38e2-444">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="c38e2-445">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="c38e2-445">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="c38e2-446">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="c38e2-446">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="c38e2-447">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="c38e2-447">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="c38e2-448">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="c38e2-448">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="c38e2-449">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="c38e2-449">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="c38e2-450">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="c38e2-450">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="c38e2-451">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="c38e2-451">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="c38e2-452">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="c38e2-452">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="c38e2-453">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="c38e2-453">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="c38e2-454">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="c38e2-454">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="c38e2-455">Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS</span><span class="sxs-lookup"><span data-stu-id="c38e2-455">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="c38e2-456">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="c38e2-456">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="c38e2-457">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="c38e2-457">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="c38e2-458">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="c38e2-458">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="c38e2-459">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="c38e2-459">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="c38e2-460">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="c38e2-460">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="c38e2-461">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="c38e2-461">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="c38e2-462">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="c38e2-462">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="c38e2-463">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="c38e2-463">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="c38e2-464">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="c38e2-464">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="c38e2-465">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="c38e2-465">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="c38e2-466">Perfil</span><span class="sxs-lookup"><span data-stu-id="c38e2-466">Profile</span></span>

* <span data-ttu-id="c38e2-467">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="c38e2-467">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="c38e2-468">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="c38e2-468">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="c38e2-469">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="c38e2-469">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="c38e2-470">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="c38e2-470">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="c38e2-471">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="c38e2-471">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="c38e2-472">RDBMS</span><span class="sxs-lookup"><span data-stu-id="c38e2-472">RDBMS</span></span>

* <span data-ttu-id="c38e2-473">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="c38e2-473">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="c38e2-474">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="c38e2-474">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="c38e2-475">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="c38e2-475">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="c38e2-476">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="c38e2-476">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="c38e2-477">Recurso</span><span class="sxs-lookup"><span data-stu-id="c38e2-477">Resource</span></span>

* <span data-ttu-id="c38e2-478">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="c38e2-478">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="c38e2-479">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="c38e2-479">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="c38e2-480">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="c38e2-480">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="c38e2-481">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="c38e2-481">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="c38e2-482">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="c38e2-482">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="c38e2-483">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="c38e2-483">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="c38e2-484">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="c38e2-484">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="c38e2-485">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="c38e2-485">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="c38e2-486">Função</span><span class="sxs-lookup"><span data-stu-id="c38e2-486">Role</span></span>

* <span data-ttu-id="c38e2-487">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="c38e2-487">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="c38e2-488">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="c38e2-488">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="c38e2-489">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="c38e2-489">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="c38e2-490">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="c38e2-490">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="c38e2-491">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="c38e2-491">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c38e2-492">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c38e2-492">Service Fabric</span></span>
* <span data-ttu-id="c38e2-493">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="c38e2-493">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="c38e2-494">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="c38e2-494">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="c38e2-495">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="c38e2-495">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="c38e2-496">SQL</span><span class="sxs-lookup"><span data-stu-id="c38e2-496">SQL</span></span>

* <span data-ttu-id="c38e2-497">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="c38e2-497">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="c38e2-498">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="c38e2-498">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="c38e2-499">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="c38e2-499">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="c38e2-500">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="c38e2-500">Storage</span></span>

* <span data-ttu-id="c38e2-501">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="c38e2-501">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="c38e2-502">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="c38e2-502">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="c38e2-503">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="c38e2-503">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="c38e2-504">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="c38e2-504">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="c38e2-505">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="c38e2-505">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="c38e2-506">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="c38e2-506">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="c38e2-507">VM</span><span class="sxs-lookup"><span data-stu-id="c38e2-507">VM</span></span>

* <span data-ttu-id="c38e2-508">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="c38e2-508">Support configuring nsg</span></span>
* <span data-ttu-id="c38e2-509">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="c38e2-509">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="c38e2-510">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="c38e2-510">Support managed service identities</span></span>
* <span data-ttu-id="c38e2-511">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="c38e2-511">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="c38e2-512">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="c38e2-512">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="c38e2-513">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="c38e2-513">May 10, 2017</span></span>

<span data-ttu-id="c38e2-514">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="c38e2-514">Version 2.0.6</span></span>

* <span data-ttu-id="c38e2-515">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c38e2-515">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="c38e2-516">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="c38e2-516">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="c38e2-517">Inclusão dos módulos Data Lake Analytics e Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="c38e2-517">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="c38e2-518">Inclusão do módulo Serviços Cognitivos.</span><span class="sxs-lookup"><span data-stu-id="c38e2-518">Include Cognitive Services module.</span></span>
* <span data-ttu-id="c38e2-519">Inclusão do módulo Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="c38e2-519">Include Service Fabric module.</span></span>
* <span data-ttu-id="c38e2-520">Inclusão do módulo Interativo (renomeação de az-shell).</span><span class="sxs-lookup"><span data-stu-id="c38e2-520">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="c38e2-521">Adição de suporte para comandos CDN.</span><span class="sxs-lookup"><span data-stu-id="c38e2-521">Add support for CDN commands.</span></span>
* <span data-ttu-id="c38e2-522">Remoção do módulo Contêiner.</span><span class="sxs-lookup"><span data-stu-id="c38e2-522">Remove Container module.</span></span>
* <span data-ttu-id="c38e2-523">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="c38e2-523">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="c38e2-524">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="c38e2-524">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="c38e2-525">Núcleo</span><span class="sxs-lookup"><span data-stu-id="c38e2-525">Core</span></span>

* <span data-ttu-id="c38e2-526">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="c38e2-526">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="c38e2-527">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="c38e2-527">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="c38e2-528">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="c38e2-528">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="c38e2-529">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="c38e2-529">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="c38e2-530">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="c38e2-530">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="c38e2-531">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="c38e2-531">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="c38e2-532">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="c38e2-532">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="c38e2-533">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="c38e2-533">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="c38e2-534">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="c38e2-534">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="c38e2-535">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="c38e2-535">core: Improved performance</span></span>
* <span data-ttu-id="c38e2-536">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="c38e2-536">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="c38e2-537">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="c38e2-537">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="c38e2-538">ACS</span><span class="sxs-lookup"><span data-stu-id="c38e2-538">ACS</span></span>

* <span data-ttu-id="c38e2-539">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c38e2-539">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="c38e2-540">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="c38e2-540">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="c38e2-541">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="c38e2-541">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="c38e2-542">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="c38e2-542">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="c38e2-543">AppService</span><span class="sxs-lookup"><span data-stu-id="c38e2-543">AppService</span></span>

* <span data-ttu-id="c38e2-544">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="c38e2-544">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="c38e2-545">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="c38e2-545">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="c38e2-546">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="c38e2-546">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="c38e2-547">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="c38e2-547">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="c38e2-548">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="c38e2-548">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="c38e2-549">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="c38e2-549">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="c38e2-550">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="c38e2-550">support slot swap with preview</span></span>
* <span data-ttu-id="c38e2-551">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="c38e2-551">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="c38e2-552">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="c38e2-552">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c38e2-553">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="c38e2-553">CosmosDB</span></span>

* <span data-ttu-id="c38e2-554">Renomeação do módulo DocumentDB para CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="c38e2-554">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="c38e2-555">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="c38e2-555">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="c38e2-556">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="c38e2-556">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="c38e2-557">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="c38e2-557">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c38e2-558">Análises Data Lake</span><span class="sxs-lookup"><span data-stu-id="c38e2-558">Data Lake Analytics</span></span>

* <span data-ttu-id="c38e2-559">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro.</span><span class="sxs-lookup"><span data-stu-id="c38e2-559">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="c38e2-560">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="c38e2-560">Add support for new catalog item type: package.</span></span> <span data-ttu-id="c38e2-561">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="c38e2-561">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="c38e2-562">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="c38e2-562">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="c38e2-563">Tabela</span><span class="sxs-lookup"><span data-stu-id="c38e2-563">Table</span></span>
  * <span data-ttu-id="c38e2-564">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="c38e2-564">Table valued function</span></span>
  * <span data-ttu-id="c38e2-565">Visualizar</span><span class="sxs-lookup"><span data-stu-id="c38e2-565">View</span></span>
  * <span data-ttu-id="c38e2-566">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="c38e2-566">Table Statistics.</span></span> <span data-ttu-id="c38e2-567">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela.</span><span class="sxs-lookup"><span data-stu-id="c38e2-567">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c38e2-568">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="c38e2-568">Data Lake Store</span></span>

* <span data-ttu-id="c38e2-569">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor.</span><span class="sxs-lookup"><span data-stu-id="c38e2-569">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="c38e2-570">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="c38e2-570">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="c38e2-571">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="c38e2-571">missed help for access show.</span></span> <span data-ttu-id="c38e2-572">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="c38e2-572">adding it.</span></span> <span data-ttu-id="c38e2-573">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="c38e2-573">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="c38e2-574">Localizar</span><span class="sxs-lookup"><span data-stu-id="c38e2-574">Find</span></span>

* <span data-ttu-id="c38e2-575">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="c38e2-575">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="c38e2-576">KeyVault</span><span class="sxs-lookup"><span data-stu-id="c38e2-576">KeyVault</span></span>

* <span data-ttu-id="c38e2-577">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="c38e2-577">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="c38e2-578">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço.</span><span class="sxs-lookup"><span data-stu-id="c38e2-578">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="c38e2-579">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="c38e2-579">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="c38e2-580">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”.</span><span class="sxs-lookup"><span data-stu-id="c38e2-580">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="c38e2-581">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="c38e2-581">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="c38e2-582">Laboratório</span><span class="sxs-lookup"><span data-stu-id="c38e2-582">Lab</span></span>

* <span data-ttu-id="c38e2-583">Adição dos comandos create, show, delete e list ao ambiente do laboratório.</span><span class="sxs-lookup"><span data-stu-id="c38e2-583">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="c38e2-584">Adição dos comandos show e list para exibir modelos ARM no laboratório.</span><span class="sxs-lookup"><span data-stu-id="c38e2-584">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="c38e2-585">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório.</span><span class="sxs-lookup"><span data-stu-id="c38e2-585">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="c38e2-586">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório.</span><span class="sxs-lookup"><span data-stu-id="c38e2-586">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="c38e2-587">Adição de comandos para gerenciar segredos em um Laboratório.</span><span class="sxs-lookup"><span data-stu-id="c38e2-587">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="c38e2-588">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="c38e2-588">Monitor</span></span>

* <span data-ttu-id="c38e2-589">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="c38e2-589">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="c38e2-590">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="c38e2-590">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="c38e2-591">Rede</span><span class="sxs-lookup"><span data-stu-id="c38e2-591">Network</span></span>

* <span data-ttu-id="c38e2-592">Adição do comando `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="c38e2-592">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="c38e2-593">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="c38e2-593">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="c38e2-594">Adição de suporte para drenagem de conexão do Gateway de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c38e2-594">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="c38e2-595">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c38e2-595">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="c38e2-596">Adição de suporte para filtros de rota e regras do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="c38e2-596">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="c38e2-597">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="c38e2-597">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="c38e2-598">Adição de suporte para seletores de tráfego baseados em política da conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="c38e2-598">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="c38e2-599">Adição de suporte para políticas IPsec da conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="c38e2-599">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="c38e2-600">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`.</span><span class="sxs-lookup"><span data-stu-id="c38e2-600">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="c38e2-601">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="c38e2-601">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="c38e2-602">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="c38e2-602">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="c38e2-603">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="c38e2-603">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="c38e2-604">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente.</span><span class="sxs-lookup"><span data-stu-id="c38e2-604">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="c38e2-605">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente.</span><span class="sxs-lookup"><span data-stu-id="c38e2-605">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="c38e2-606">Correção de um bug em que `traffic-manager endpoint update` não funciona.</span><span class="sxs-lookup"><span data-stu-id="c38e2-606">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="c38e2-607">Adição de comandos de visualização “network watcher”.</span><span class="sxs-lookup"><span data-stu-id="c38e2-607">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="c38e2-608">Perfil</span><span class="sxs-lookup"><span data-stu-id="c38e2-608">Profile</span></span>

* <span data-ttu-id="c38e2-609">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="c38e2-609">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="c38e2-610">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="c38e2-610">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="c38e2-611">Redis</span><span class="sxs-lookup"><span data-stu-id="c38e2-611">Redis</span></span>

* <span data-ttu-id="c38e2-612">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="c38e2-612">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="c38e2-613">Preterição do comando “update-settings”.</span><span class="sxs-lookup"><span data-stu-id="c38e2-613">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="c38e2-614">Recurso</span><span class="sxs-lookup"><span data-stu-id="c38e2-614">Resource</span></span>

* <span data-ttu-id="c38e2-615">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="c38e2-615">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="c38e2-616">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="c38e2-616">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="c38e2-617">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="c38e2-617">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="c38e2-618">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="c38e2-618">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="c38e2-619">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="c38e2-619">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="c38e2-620">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="c38e2-620">Add docs for az lock update.</span></span> <span data-ttu-id="c38e2-621">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="c38e2-621">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="c38e2-622">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="c38e2-622">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="c38e2-623">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="c38e2-623">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="c38e2-624">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="c38e2-624">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="c38e2-625">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="c38e2-625">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="c38e2-626">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="c38e2-626">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="c38e2-627">Função</span><span class="sxs-lookup"><span data-stu-id="c38e2-627">Role</span></span>

* <span data-ttu-id="c38e2-628">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="c38e2-628">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="c38e2-629">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="c38e2-629">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="c38e2-630">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="c38e2-630">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="c38e2-631">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="c38e2-631">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="c38e2-632">SQL</span><span class="sxs-lookup"><span data-stu-id="c38e2-632">SQL</span></span>

* <span data-ttu-id="c38e2-633">Adição dos comandos az sql server list-usages e az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="c38e2-633">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="c38e2-634">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="c38e2-634">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="c38e2-635">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="c38e2-635">Storage</span></span>

* <span data-ttu-id="c38e2-636">Localização padrão da localização do grupo de recursos de `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="c38e2-636">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="c38e2-637">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="c38e2-637">Add support for incremental blob copy</span></span>
* <span data-ttu-id="c38e2-638">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="c38e2-638">Add support for large block blob upload</span></span>
* <span data-ttu-id="c38e2-639">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="c38e2-639">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="c38e2-640">VM</span><span class="sxs-lookup"><span data-stu-id="c38e2-640">VM</span></span>

* <span data-ttu-id="c38e2-641">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="c38e2-641">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="c38e2-642">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="c38e2-642">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="c38e2-643">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="c38e2-643">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="c38e2-644">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="c38e2-644">az vm/vmss disk</span></span>
  3. <span data-ttu-id="c38e2-645">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="c38e2-645">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="c38e2-646">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="c38e2-646">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="c38e2-647">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="c38e2-647">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="c38e2-648">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="c38e2-648">April 3, 2017</span></span>

<span data-ttu-id="c38e2-649">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="c38e2-649">Version 2.0.2</span></span>

<span data-ttu-id="c38e2-650">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão.</span><span class="sxs-lookup"><span data-stu-id="c38e2-650">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="c38e2-651">Núcleo</span><span class="sxs-lookup"><span data-stu-id="c38e2-651">Core</span></span>

* <span data-ttu-id="c38e2-652">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão.</span><span class="sxs-lookup"><span data-stu-id="c38e2-652">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="c38e2-653">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="c38e2-653">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="c38e2-654">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="c38e2-654">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="c38e2-655">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="c38e2-655">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="c38e2-656">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="c38e2-656">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="c38e2-657">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="c38e2-657">Add prompting for missing template parameters.</span></span> <span data-ttu-id="c38e2-658">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="c38e2-658">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="c38e2-659">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="c38e2-659">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="c38e2-660">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="c38e2-660">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="c38e2-661">ACS</span><span class="sxs-lookup"><span data-stu-id="c38e2-661">ACS</span></span>

* <span data-ttu-id="c38e2-662">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="c38e2-662">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="c38e2-663">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="c38e2-663">Add support for ssh key password prompting.</span></span> <span data-ttu-id="c38e2-664">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="c38e2-664">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="c38e2-665">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="c38e2-665">Add support for windows clusters.</span></span> <span data-ttu-id="c38e2-666">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="c38e2-666">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="c38e2-667">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="c38e2-667">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="c38e2-668">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="c38e2-668">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="c38e2-669">AppService</span><span class="sxs-lookup"><span data-stu-id="c38e2-669">AppService</span></span>

* <span data-ttu-id="c38e2-670">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="c38e2-670">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="c38e2-671">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="c38e2-671">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="c38e2-672">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="c38e2-672">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="c38e2-673">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="c38e2-673">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="c38e2-674">DataLake</span><span class="sxs-lookup"><span data-stu-id="c38e2-674">DataLake</span></span>

* <span data-ttu-id="c38e2-675">Versão inicial do módulo do Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="c38e2-675">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="c38e2-676">Versão inicial do módulo do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="c38e2-676">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="c38e2-677">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="c38e2-677">DocuemntDB</span></span>

* <span data-ttu-id="c38e2-678">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="c38e2-678">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="c38e2-679">VM</span><span class="sxs-lookup"><span data-stu-id="c38e2-679">VM</span></span>

* <span data-ttu-id="c38e2-680">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="c38e2-680">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="c38e2-681">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="c38e2-681">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="c38e2-682">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="c38e2-682">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="c38e2-683">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="c38e2-683">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="c38e2-684">Conjunto de dimensionamento de máquinas virtuais: suporte à * para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="c38e2-684">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="c38e2-685">Adicionar --secrets para o conjunto de dimensionamento de máquinas virtuais e VM ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="c38e2-685">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="c38e2-686">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="c38e2-686">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="c38e2-687">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="c38e2-687">February 27, 2017</span></span>

<span data-ttu-id="c38e2-688">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="c38e2-688">Version 2.0.0</span></span>

<span data-ttu-id="c38e2-689">Essa versão da CLI do Azure 2.0 é a primeira versão “Disponível”.</span><span class="sxs-lookup"><span data-stu-id="c38e2-689">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="c38e2-690">A disponibilidade se aplica a esses módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="c38e2-690">General availability applies to these command modules:</span></span>
- <span data-ttu-id="c38e2-691">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="c38e2-691">Container Service (acs)</span></span>
- <span data-ttu-id="c38e2-692">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="c38e2-692">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="c38e2-693">Rede</span><span class="sxs-lookup"><span data-stu-id="c38e2-693">Networking</span></span>
- <span data-ttu-id="c38e2-694">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="c38e2-694">Storage</span></span>

<span data-ttu-id="c38e2-695">Esses módulos de comando podem ser usados na produção e são compatíveis com o SLA do Microsoft padrão.</span><span class="sxs-lookup"><span data-stu-id="c38e2-695">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="c38e2-696">Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="c38e2-696">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="c38e2-697">Você pode fazer perguntas sobre [StackOverflow usando a marcação azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) ou entrar em contato com a equipe do produto pelo endereço [ azfeedback@microsoft.com ](mailto:azfeedback@microsoft.com). Você pode fornecer comentários a partir da linha de comando com o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="c38e2-697">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="c38e2-698">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="c38e2-698">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="c38e2-699">Para verificar a versão da CLI, utilize `az --version`.</span><span class="sxs-lookup"><span data-stu-id="c38e2-699">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="c38e2-700">A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando.</span><span class="sxs-lookup"><span data-stu-id="c38e2-700">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="c38e2-701">Alguns dos módulos de comando têm um “b*n*” ou “rc*n*” pós-fixado.</span><span class="sxs-lookup"><span data-stu-id="c38e2-701">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="c38e2-702">Esses módulos de comando ainda estão em visualização e estarão disponíveis no futuro.</span><span class="sxs-lookup"><span data-stu-id="c38e2-702">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="c38e2-703">Também temos compilações de visualização diárias da CLI.</span><span class="sxs-lookup"><span data-stu-id="c38e2-703">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="c38e2-704">Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="c38e2-704">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="c38e2-705">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="c38e2-705">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="c38e2-706">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="c38e2-706">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="c38e2-707">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="c38e2-707">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="c38e2-708">Forneça comentários a partir da linha de comando com o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="c38e2-708">Provide feedback from the command line with the `az feedback` command.</span></span>

