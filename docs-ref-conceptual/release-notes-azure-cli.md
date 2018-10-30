---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/23/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 65e34ab6014c47ae92a6d4bae8cdc30d4a1413dc
ms.sourcegitcommit: aec89531c938781b4724f43b5bb4b878e106a26a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2018
ms.locfileid: "49952478"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="05b9c-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="05b9c-103">Azure CLI release notes</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="05b9c-104">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-104">October 23, 2018</span></span>

<span data-ttu-id="05b9c-105">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="05b9c-105">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="05b9c-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-106">Core</span></span>
* <span data-ttu-id="05b9c-107">Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`</span><span class="sxs-lookup"><span data-stu-id="05b9c-107">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="05b9c-108">Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="05b9c-108">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="05b9c-109">ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-109">ACR</span></span>
* <span data-ttu-id="05b9c-110">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="05b9c-110">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="05b9c-111">CDN</span><span class="sxs-lookup"><span data-stu-id="05b9c-111">CDN</span></span>
* <span data-ttu-id="05b9c-112">[ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="05b9c-112">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="05b9c-113">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="05b9c-113">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="05b9c-114">Contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-114">Container</span></span>
* <span data-ttu-id="05b9c-115">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="05b9c-115">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="05b9c-116">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="05b9c-116">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="05b9c-117">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="05b9c-117">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="05b9c-118">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="05b9c-118">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="05b9c-119">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="05b9c-119">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="05b9c-120">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="05b9c-120">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="05b9c-121">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="05b9c-121">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="05b9c-122">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="05b9c-122">CosmosDB</span></span>
* <span data-ttu-id="05b9c-123">Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-123">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="05b9c-124">Interativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-124">Interactive</span></span>
* <span data-ttu-id="05b9c-125">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="05b9c-125">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="05b9c-126">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="05b9c-126">IoT Central</span></span>
* <span data-ttu-id="05b9c-127">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="05b9c-127">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="05b9c-128">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="05b9c-128">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="05b9c-129">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="05b9c-129">Monitor</span></span>
* <span data-ttu-id="05b9c-130">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="05b9c-130">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="05b9c-131">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="05b9c-131">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="05b9c-132">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="05b9c-132">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="05b9c-133">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="05b9c-133">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="05b9c-134">Adicionado `--namespace` como alias para a opção preterida `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="05b9c-134">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="05b9c-135">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="05b9c-135">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="05b9c-136">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="05b9c-136">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="05b9c-137">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="05b9c-137">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="05b9c-138">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="05b9c-138">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="05b9c-139">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-139">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-140">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-140">Network</span></span>
* <span data-ttu-id="05b9c-141">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="05b9c-141">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="05b9c-142">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="05b9c-142">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="05b9c-143">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="05b9c-143">ServiceBus</span></span>
* <span data-ttu-id="05b9c-144">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="05b9c-144">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="05b9c-145">SQL</span><span class="sxs-lookup"><span data-stu-id="05b9c-145">SQL</span></span>
* <span data-ttu-id="05b9c-146">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="05b9c-146">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-147">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-147">Storage</span></span>
* <span data-ttu-id="05b9c-148">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="05b9c-148">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="05b9c-149">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="05b9c-149">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-150">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-150">VM</span></span>
* <span data-ttu-id="05b9c-151">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-151">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="05b9c-152">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-152">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="05b9c-153">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-153">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="05b9c-154">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-154">October 16, 2018</span></span>

<span data-ttu-id="05b9c-155">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="05b9c-155">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-156">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-156">VM</span></span>
* <span data-ttu-id="05b9c-157">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="05b9c-157">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="05b9c-158">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-158">October 9, 2018</span></span>

<span data-ttu-id="05b9c-159">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="05b9c-159">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="05b9c-160">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-160">Core</span></span>
* <span data-ttu-id="05b9c-161">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="05b9c-161">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="05b9c-162">ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-162">ACR</span></span>
* <span data-ttu-id="05b9c-163">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="05b9c-163">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-164">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-164">ACS</span></span>
* <span data-ttu-id="05b9c-165">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="05b9c-165">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="05b9c-166">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="05b9c-166">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="05b9c-167">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="05b9c-167">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="05b9c-168">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="05b9c-168">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="05b9c-169">Contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-169">Container</span></span>
* <span data-ttu-id="05b9c-170">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um tempo de execução específico</span><span class="sxs-lookup"><span data-stu-id="05b9c-170">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="05b9c-171">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="05b9c-171">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="05b9c-172">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="05b9c-172">Event Hub</span></span>
* <span data-ttu-id="05b9c-173">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-173">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="05b9c-174">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="05b9c-174">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="05b9c-175">Extensões</span><span class="sxs-lookup"><span data-stu-id="05b9c-175">Extensions</span></span>
* <span data-ttu-id="05b9c-176">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="05b9c-176">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="05b9c-177">HDInsight</span><span class="sxs-lookup"><span data-stu-id="05b9c-177">HDInsight</span></span>
* <span data-ttu-id="05b9c-178">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="05b9c-178">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="05b9c-179">IoT</span><span class="sxs-lookup"><span data-stu-id="05b9c-179">IoT</span></span>
* <span data-ttu-id="05b9c-180">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="05b9c-180">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="05b9c-181">KeyVault</span><span class="sxs-lookup"><span data-stu-id="05b9c-181">KeyVault</span></span>
* <span data-ttu-id="05b9c-182">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="05b9c-182">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-183">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-183">Network</span></span>
* <span data-ttu-id="05b9c-184">`network dns zone create` corrigido: o comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="05b9c-184">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="05b9c-185">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="05b9c-185">See #6052</span></span>
* <span data-ttu-id="05b9c-186">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-186">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="05b9c-187">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="05b9c-187">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="05b9c-188">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="05b9c-188">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="05b9c-189">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="05b9c-189">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="05b9c-190">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="05b9c-190">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="05b9c-191">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-191">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="05b9c-192">Função</span><span class="sxs-lookup"><span data-stu-id="05b9c-192">Role</span></span>
* <span data-ttu-id="05b9c-193">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="05b9c-193">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="05b9c-194">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="05b9c-194">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="05b9c-195">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="05b9c-195">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="05b9c-196">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="05b9c-196">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="05b9c-197">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="05b9c-197">Service Bus</span></span>
* <span data-ttu-id="05b9c-198">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="05b9c-198">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-199">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-199">VM</span></span>
* <span data-ttu-id="05b9c-200">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="05b9c-200">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="05b9c-201">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-201">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="05b9c-202">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="05b9c-202">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="05b9c-203">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="05b9c-203">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="05b9c-204">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="05b9c-204">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="05b9c-205">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="05b9c-205">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="05b9c-206">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-206">September 21, 2018</span></span>

<span data-ttu-id="05b9c-207">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="05b9c-207">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="05b9c-208">ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-208">ACR</span></span>
* <span data-ttu-id="05b9c-209">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-209">Added ACR Task commands</span></span>
* <span data-ttu-id="05b9c-210">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="05b9c-210">Added quick run command</span></span>
* <span data-ttu-id="05b9c-211">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="05b9c-211">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="05b9c-212">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-212">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="05b9c-213">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="05b9c-213">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="05b9c-214">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="05b9c-214">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-215">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-215">ACS</span></span>
* <span data-ttu-id="05b9c-216">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="05b9c-216">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="05b9c-217">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="05b9c-217">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-218">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-218">AppService</span></span>

* <span data-ttu-id="05b9c-219">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="05b9c-219">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="05b9c-220">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="05b9c-220">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="05b9c-221">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="05b9c-221">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="05b9c-222">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="05b9c-222">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="05b9c-223">Lote</span><span class="sxs-lookup"><span data-stu-id="05b9c-223">Batch</span></span>
* <span data-ttu-id="05b9c-224">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="05b9c-224">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="05b9c-225">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="05b9c-225">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="05b9c-226">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-226">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="05b9c-227">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="05b9c-227">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="05b9c-228">Lote AI</span><span class="sxs-lookup"><span data-stu-id="05b9c-228">Batch AI</span></span> 
* <span data-ttu-id="05b9c-229">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-229">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="05b9c-230">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="05b9c-230">Cognitive Services</span></span>
* <span data-ttu-id="05b9c-231">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="05b9c-231">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="05b9c-232">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="05b9c-232">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="05b9c-233">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="05b9c-233">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="05b9c-234">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="05b9c-234">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="05b9c-235">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="05b9c-235">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="05b9c-236">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="05b9c-236">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="05b9c-237">Contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-237">Container</span></span>
* <span data-ttu-id="05b9c-238">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="05b9c-238">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="05b9c-239">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-239">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="05b9c-240">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="05b9c-240">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="05b9c-241">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="05b9c-241">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="05b9c-242">DataLake</span><span class="sxs-lookup"><span data-stu-id="05b9c-242">Datalake</span></span>
* <span data-ttu-id="05b9c-243">Comandos adicionados para regras de rede virtual</span><span class="sxs-lookup"><span data-stu-id="05b9c-243">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="05b9c-244">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-244">Interactive Shell</span></span>
* <span data-ttu-id="05b9c-245">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="05b9c-245">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="05b9c-246">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="05b9c-246">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="05b9c-247">IoT</span><span class="sxs-lookup"><span data-stu-id="05b9c-247">IoT</span></span>
* <span data-ttu-id="05b9c-248">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="05b9c-248">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="05b9c-249">Key Vault</span><span class="sxs-lookup"><span data-stu-id="05b9c-249">Key Vault</span></span>
* <span data-ttu-id="05b9c-250">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="05b9c-250">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-251">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-251">Network</span></span>
* <span data-ttu-id="05b9c-252">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="05b9c-252">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="05b9c-253">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="05b9c-253">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="05b9c-254">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="05b9c-254">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="05b9c-255">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="05b9c-255">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="05b9c-256">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-256">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="05b9c-257">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-257">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="05b9c-258">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="05b9c-258">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="05b9c-259">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="05b9c-259">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="05b9c-260">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="05b9c-260">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="05b9c-261">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="05b9c-261">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="05b9c-262">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="05b9c-262">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="05b9c-263">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="05b9c-263">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="05b9c-264">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="05b9c-264">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="05b9c-265">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="05b9c-265">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="05b9c-266">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="05b9c-266">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="05b9c-267">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="05b9c-267">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="05b9c-268">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-268">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="05b9c-269">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="05b9c-269">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="05b9c-270">RDBMS</span><span class="sxs-lookup"><span data-stu-id="05b9c-270">RDBMS</span></span>
* <span data-ttu-id="05b9c-271">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="05b9c-271">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="05b9c-272">Reserva</span><span class="sxs-lookup"><span data-stu-id="05b9c-272">Reservation</span></span>
* <span data-ttu-id="05b9c-273">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="05b9c-273">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="05b9c-274">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="05b9c-274">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="05b9c-275">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-275">Manage App</span></span>
* <span data-ttu-id="05b9c-276">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="05b9c-276">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="05b9c-277">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="05b9c-277">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="05b9c-278">Função</span><span class="sxs-lookup"><span data-stu-id="05b9c-278">Role</span></span>
* <span data-ttu-id="05b9c-279">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="05b9c-279">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="05b9c-280">SignalR</span><span class="sxs-lookup"><span data-stu-id="05b9c-280">SignalR</span></span>
* <span data-ttu-id="05b9c-281">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="05b9c-281">First release</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-282">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-282">Storage</span></span>
* <span data-ttu-id="05b9c-283">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="05b9c-283">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="05b9c-284">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="05b9c-284">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-285">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-285">VM</span></span>
* <span data-ttu-id="05b9c-286">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="05b9c-286">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="05b9c-287">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="05b9c-287">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="05b9c-288">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-288">August 28, 2018</span></span>

<span data-ttu-id="05b9c-289">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="05b9c-289">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="05b9c-290">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-290">Core</span></span>

* <span data-ttu-id="05b9c-291">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="05b9c-291">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="05b9c-292">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="05b9c-292">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="05b9c-293">ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-293">ACR</span></span>

* <span data-ttu-id="05b9c-294">Adicionada uma solução alternativa para operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="05b9c-294">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="05b9c-295">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="05b9c-295">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-296">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-296">ACS</span></span>

* <span data-ttu-id="05b9c-297">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="05b9c-297">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="05b9c-298">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="05b9c-298">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-299">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-299">AppService</span></span>

* <span data-ttu-id="05b9c-300">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="05b9c-300">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="05b9c-301">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="05b9c-301">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="05b9c-302">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="05b9c-302">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="05b9c-303">Backup</span><span class="sxs-lookup"><span data-stu-id="05b9c-303">Backup</span></span>

* <span data-ttu-id="05b9c-304">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="05b9c-304">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="05b9c-305">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="05b9c-305">Bot Service</span></span>

* <span data-ttu-id="05b9c-306">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="05b9c-306">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="05b9c-307">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="05b9c-307">Cognitive Services</span></span>

* <span data-ttu-id="05b9c-308">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="05b9c-308">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="05b9c-309">IoT</span><span class="sxs-lookup"><span data-stu-id="05b9c-309">IoT</span></span>

* <span data-ttu-id="05b9c-310">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="05b9c-310">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="05b9c-311">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="05b9c-311">Monitor</span></span>

* <span data-ttu-id="05b9c-312">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="05b9c-312">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="05b9c-313">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="05b9c-313">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-314">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-314">Network</span></span>

* <span data-ttu-id="05b9c-315">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="05b9c-315">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="05b9c-316">Recurso</span><span class="sxs-lookup"><span data-stu-id="05b9c-316">Resource</span></span>

* <span data-ttu-id="05b9c-317">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="05b9c-317">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-318">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-318">Storage</span></span>

* <span data-ttu-id="05b9c-319">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="05b9c-319">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-320">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-320">VM</span></span>

* <span data-ttu-id="05b9c-321">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="05b9c-321">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="05b9c-322">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-322">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="05b9c-323">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-323">Auguest 14, 2018</span></span>

<span data-ttu-id="05b9c-324">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="05b9c-324">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="05b9c-325">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-325">Core</span></span>

* <span data-ttu-id="05b9c-326">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="05b9c-326">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="05b9c-327">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="05b9c-327">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="05b9c-328">Telemetria</span><span class="sxs-lookup"><span data-stu-id="05b9c-328">Telemetry</span></span>

* <span data-ttu-id="05b9c-329">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="05b9c-329">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="05b9c-330">ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-330">ACR</span></span>

* <span data-ttu-id="05b9c-331">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="05b9c-331">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="05b9c-332">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="05b9c-332">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-333">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-333">ACS</span></span>

* <span data-ttu-id="05b9c-334">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="05b9c-334">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="05b9c-335">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="05b9c-335">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="05b9c-336">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="05b9c-336">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="05b9c-337">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="05b9c-337">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="05b9c-338">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="05b9c-338">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="05b9c-339">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-339">AppService</span></span>

* <span data-ttu-id="05b9c-340">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="05b9c-340">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="05b9c-341">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="05b9c-341">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="05b9c-342">BatchAI</span><span class="sxs-lookup"><span data-stu-id="05b9c-342">BatchAI</span></span>

* <span data-ttu-id="05b9c-343">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="05b9c-343">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="05b9c-344">Contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-344">Container</span></span>

* <span data-ttu-id="05b9c-345">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-345">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="05b9c-346">IoT</span><span class="sxs-lookup"><span data-stu-id="05b9c-346">IoT</span></span>

* <span data-ttu-id="05b9c-347">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="05b9c-347">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="05b9c-348">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="05b9c-348">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="05b9c-349">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="05b9c-349">Iot Central</span></span>

* <span data-ttu-id="05b9c-350">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="05b9c-350">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="05b9c-351">KeyVault</span><span class="sxs-lookup"><span data-stu-id="05b9c-351">KeyVault</span></span>


* <span data-ttu-id="05b9c-352">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="05b9c-352">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="05b9c-353">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-353">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="05b9c-354">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="05b9c-354">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="05b9c-355">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="05b9c-355">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="05b9c-356">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="05b9c-356">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="05b9c-357">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="05b9c-357">Relay</span></span>

* <span data-ttu-id="05b9c-358">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="05b9c-358">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="05b9c-359">Sql</span><span class="sxs-lookup"><span data-stu-id="05b9c-359">Sql</span></span>

* <span data-ttu-id="05b9c-360">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="05b9c-360">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-361">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-361">Storage</span></span>

* <span data-ttu-id="05b9c-362">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="05b9c-362">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="05b9c-363">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="05b9c-363">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="05b9c-364">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="05b9c-364">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="05b9c-365">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="05b9c-365">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="05b9c-366">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-366">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-367">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-367">VM</span></span>

* <span data-ttu-id="05b9c-368">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="05b9c-368">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="05b9c-369">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-369">July 31, 2018</span></span>

<span data-ttu-id="05b9c-370">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="05b9c-370">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="05b9c-371">ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-371">ACR</span></span>

* <span data-ttu-id="05b9c-372">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="05b9c-372">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="05b9c-373">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="05b9c-373">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-374">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-374">ACS</span></span>

* <span data-ttu-id="05b9c-375">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="05b9c-375">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="05b9c-376">Lote</span><span class="sxs-lookup"><span data-stu-id="05b9c-376">Batch</span></span>

* <span data-ttu-id="05b9c-377">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="05b9c-377">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="05b9c-378">Contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-378">Container</span></span>

* <span data-ttu-id="05b9c-379">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="05b9c-379">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-380">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-380">Network</span></span>

* <span data-ttu-id="05b9c-381">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="05b9c-381">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="05b9c-382">Recurso</span><span class="sxs-lookup"><span data-stu-id="05b9c-382">Resource</span></span>

* <span data-ttu-id="05b9c-383">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="05b9c-383">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="05b9c-384">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="05b9c-384">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="05b9c-385">Função</span><span class="sxs-lookup"><span data-stu-id="05b9c-385">Role</span></span>

* <span data-ttu-id="05b9c-386">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="05b9c-386">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="05b9c-387">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="05b9c-387">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="05b9c-388">Search</span><span class="sxs-lookup"><span data-stu-id="05b9c-388">Search</span></span>

* <span data-ttu-id="05b9c-389">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="05b9c-389">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="05b9c-390">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="05b9c-390">Service Bus</span></span>

* <span data-ttu-id="05b9c-391">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="05b9c-391">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="05b9c-392">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="05b9c-392">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="05b9c-393">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="05b9c-393">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="05b9c-394">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="05b9c-394">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-395">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-395">Storage</span></span>

* <span data-ttu-id="05b9c-396">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="05b9c-396">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="05b9c-397">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="05b9c-397">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-398">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-398">VM</span></span>

* <span data-ttu-id="05b9c-399">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="05b9c-399">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="05b9c-400">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="05b9c-400">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="05b9c-401">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-401">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="05b9c-402">[ALTERAÇÃO SIGNIFICATIVA] `[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="05b9c-402">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="05b9c-403">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-403">July 18, 2018</span></span>

<span data-ttu-id="05b9c-404">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="05b9c-404">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="05b9c-405">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-405">Core</span></span>

* <span data-ttu-id="05b9c-406">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="05b9c-406">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="05b9c-407">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="05b9c-407">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="05b9c-408">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="05b9c-408">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="05b9c-409">ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-409">ACR</span></span>

* <span data-ttu-id="05b9c-410">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="05b9c-410">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="05b9c-411">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="05b9c-411">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="05b9c-412">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="05b9c-412">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="05b9c-413">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="05b9c-413">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-414">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-414">ACS</span></span>

* <span data-ttu-id="05b9c-415">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="05b9c-415">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-416">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-416">AppService</span></span>

* <span data-ttu-id="05b9c-417">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="05b9c-417">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="05b9c-418">Lote</span><span class="sxs-lookup"><span data-stu-id="05b9c-418">Batch</span></span>

* <span data-ttu-id="05b9c-419">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="05b9c-419">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="05b9c-420">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="05b9c-420">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="05b9c-421">Lote AI</span><span class="sxs-lookup"><span data-stu-id="05b9c-421">Batch AI</span></span>

* <span data-ttu-id="05b9c-422">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="05b9c-422">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="05b9c-423">Contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-423">Container</span></span>

* <span data-ttu-id="05b9c-424">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="05b9c-424">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="05b9c-425">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="05b9c-425">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-426">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-426">Network</span></span>

* <span data-ttu-id="05b9c-427">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-427">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="05b9c-428">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="05b9c-428">Added `network nic wait`</span></span>
* <span data-ttu-id="05b9c-429">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="05b9c-429">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="05b9c-430">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="05b9c-430">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="05b9c-431">Recurso</span><span class="sxs-lookup"><span data-stu-id="05b9c-431">Resource</span></span>

* <span data-ttu-id="05b9c-432">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="05b9c-432">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="05b9c-433">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="05b9c-433">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="05b9c-434">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="05b9c-434">Added `deployment wait` command</span></span>
* <span data-ttu-id="05b9c-435">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="05b9c-435">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="05b9c-436">SQL</span><span class="sxs-lookup"><span data-stu-id="05b9c-436">SQL</span></span>

* <span data-ttu-id="05b9c-437">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-437">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="05b9c-438">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="05b9c-438">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="05b9c-439">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="05b9c-439">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-440">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-440">Storage</span></span>

* <span data-ttu-id="05b9c-441">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="05b9c-441">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-442">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-442">VM</span></span>

* <span data-ttu-id="05b9c-443">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="05b9c-443">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="05b9c-444">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-444">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="05b9c-445">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="05b9c-445">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="05b9c-446">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-446">July 3, 2018</span></span>

<span data-ttu-id="05b9c-447">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="05b9c-447">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="05b9c-448">AKS</span><span class="sxs-lookup"><span data-stu-id="05b9c-448">AKS</span></span>

* <span data-ttu-id="05b9c-449">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="05b9c-449">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="05b9c-450">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-450">July 3, 2018</span></span>

<span data-ttu-id="05b9c-451">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="05b9c-451">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="05b9c-452">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-452">Core</span></span>

* <span data-ttu-id="05b9c-453">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-453">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="05b9c-454">ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-454">ACR</span></span>

* <span data-ttu-id="05b9c-455">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="05b9c-455">Added polling build status</span></span>
* <span data-ttu-id="05b9c-456">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="05b9c-456">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="05b9c-457">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="05b9c-457">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-458">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-458">ACS</span></span>

* <span data-ttu-id="05b9c-459">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="05b9c-459">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="05b9c-460">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="05b9c-460">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="05b9c-461">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-461">Updated options for `aks browse` command.</span></span> <span data-ttu-id="05b9c-462">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="05b9c-462">Added `--listen-port` support</span></span>
* <span data-ttu-id="05b9c-463">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-463">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="05b9c-464">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="05b9c-464">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="05b9c-465">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="05b9c-465">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-466">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-466">AppService</span></span>

* <span data-ttu-id="05b9c-467">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="05b9c-467">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="05b9c-468">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="05b9c-468">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="05b9c-469">Backup</span><span class="sxs-lookup"><span data-stu-id="05b9c-469">Backup</span></span>

* <span data-ttu-id="05b9c-470">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="05b9c-470">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="05b9c-471">BatchAI</span><span class="sxs-lookup"><span data-stu-id="05b9c-471">BatchAI</span></span>

* <span data-ttu-id="05b9c-472">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="05b9c-472">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="05b9c-473">Nuvem</span><span class="sxs-lookup"><span data-stu-id="05b9c-473">Cloud</span></span>

* <span data-ttu-id="05b9c-474">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="05b9c-474">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="05b9c-475">Contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-475">Container</span></span>

* <span data-ttu-id="05b9c-476">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="05b9c-476">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="05b9c-477">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="05b9c-477">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="05b9c-478">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="05b9c-478">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="05b9c-479">Extensão</span><span class="sxs-lookup"><span data-stu-id="05b9c-479">Extension</span></span>

* <span data-ttu-id="05b9c-480">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="05b9c-480">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-481">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-481">Network</span></span>

* <span data-ttu-id="05b9c-482">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="05b9c-482">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="05b9c-483">Rdbms</span><span class="sxs-lookup"><span data-stu-id="05b9c-483">Rdbms</span></span>

* <span data-ttu-id="05b9c-484">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="05b9c-484">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="05b9c-485">Recurso</span><span class="sxs-lookup"><span data-stu-id="05b9c-485">Resource</span></span>

* <span data-ttu-id="05b9c-486">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="05b9c-486">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-487">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-487">VM</span></span>

* <span data-ttu-id="05b9c-488">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="05b9c-488">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="05b9c-489">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-489">June 25, 2018</span></span>

<span data-ttu-id="05b9c-490">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="05b9c-490">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="05b9c-491">CLI</span><span class="sxs-lookup"><span data-stu-id="05b9c-491">CLI</span></span>

* <span data-ttu-id="05b9c-492">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="05b9c-492">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="05b9c-493">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-493">June 19, 2018</span></span>

<span data-ttu-id="05b9c-494">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="05b9c-494">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="05b9c-495">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-495">Core</span></span>

* <span data-ttu-id="05b9c-496">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="05b9c-496">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="05b9c-497">ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-497">ACR</span></span>

* <span data-ttu-id="05b9c-498">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="05b9c-498">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="05b9c-499">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="05b9c-499">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-500">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-500">ACS</span></span>

* <span data-ttu-id="05b9c-501">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="05b9c-501">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="05b9c-502">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="05b9c-502">Added `--update` support</span></span>
* <span data-ttu-id="05b9c-503">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="05b9c-503">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="05b9c-504">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="05b9c-504">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="05b9c-505">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="05b9c-505">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="05b9c-506">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="05b9c-506">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="05b9c-507">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="05b9c-507">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="05b9c-508">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="05b9c-508">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-509">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-509">AppService</span></span>

* <span data-ttu-id="05b9c-510">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="05b9c-510">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="05b9c-511">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="05b9c-511">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="05b9c-512">Lote</span><span class="sxs-lookup"><span data-stu-id="05b9c-512">Batch</span></span>

* <span data-ttu-id="05b9c-513">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="05b9c-513">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="05b9c-514">Lote AI</span><span class="sxs-lookup"><span data-stu-id="05b9c-514">Batch AI</span></span>

* <span data-ttu-id="05b9c-515">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="05b9c-515">Added support for workspaces.</span></span> <span data-ttu-id="05b9c-516">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="05b9c-516">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="05b9c-517">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="05b9c-517">Added support for experiments.</span></span> <span data-ttu-id="05b9c-518">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="05b9c-518">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="05b9c-519">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="05b9c-519">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="05b9c-520">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-520">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="05b9c-521">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="05b9c-521">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="05b9c-522">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="05b9c-522">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="05b9c-523">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="05b9c-523">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="05b9c-524">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="05b9c-524">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="05b9c-525">[ALTERAÇÃO SIGNIFICATIVA] `--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-525">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="05b9c-526">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="05b9c-526">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="05b9c-527">[ALTERAÇÃO SIGNIFICATIVA] `--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-527">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="05b9c-528">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="05b9c-528">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="05b9c-529">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="05b9c-529">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="05b9c-530">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="05b9c-530">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="05b9c-531">[ALTERAÇÃO SIGNIFICATIVA] `--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-531">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="05b9c-532">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="05b9c-532">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="05b9c-533">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="05b9c-533">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="05b9c-534">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="05b9c-534">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="05b9c-535">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="05b9c-535">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="05b9c-536">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="05b9c-536">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="05b9c-537">Mapas</span><span class="sxs-lookup"><span data-stu-id="05b9c-537">Maps</span></span>

* <span data-ttu-id="05b9c-538">[ALTERAÇÃO SIGNIFICATIVA] `maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="05b9c-538">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-539">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-539">Network</span></span>

* <span data-ttu-id="05b9c-540">Foi adicionado suporte a `https` para `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="05b9c-540">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="05b9c-541">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="05b9c-541">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="05b9c-542">#6502</span><span class="sxs-lookup"><span data-stu-id="05b9c-542">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="05b9c-543">Reservas</span><span class="sxs-lookup"><span data-stu-id="05b9c-543">Reservations</span></span>

* <span data-ttu-id="05b9c-544">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="05b9c-544">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="05b9c-545">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="05b9c-545">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="05b9c-546">[ALTERAÇÃO SIGNIFICATIVA] `kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="05b9c-546">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="05b9c-547">[ALTERAÇÃO SIGNIFICATIVA] `capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="05b9c-547">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="05b9c-548">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="05b9c-548">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="05b9c-549">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-549">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="05b9c-550">Função</span><span class="sxs-lookup"><span data-stu-id="05b9c-550">Role</span></span>

* <span data-ttu-id="05b9c-551">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="05b9c-551">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="05b9c-552">SQL</span><span class="sxs-lookup"><span data-stu-id="05b9c-552">SQL</span></span>

* <span data-ttu-id="05b9c-553">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="05b9c-553">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-554">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-554">Storage</span></span>

* <span data-ttu-id="05b9c-555">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="05b9c-555">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-556">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-556">VM</span></span>

* <span data-ttu-id="05b9c-557">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-557">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="05b9c-558">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="05b9c-558">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="05b9c-559">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="05b9c-559">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="05b9c-560">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-560">June 13, 2018</span></span>

<span data-ttu-id="05b9c-561">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="05b9c-561">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="05b9c-562">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-562">Core</span></span>

* <span data-ttu-id="05b9c-563">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="05b9c-563">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="05b9c-564">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-564">June 13, 2018</span></span>

<span data-ttu-id="05b9c-565">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="05b9c-565">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="05b9c-566">AKS</span><span class="sxs-lookup"><span data-stu-id="05b9c-566">AKS</span></span>

* <span data-ttu-id="05b9c-567">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-567">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="05b9c-568">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="05b9c-568">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="05b9c-569">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-569">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="05b9c-570">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-570">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="05b9c-571">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-571">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-572">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-572">AppService</span></span>

* <span data-ttu-id="05b9c-573">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="05b9c-573">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="05b9c-574">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-574">June 5, 2018</span></span>

<span data-ttu-id="05b9c-575">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="05b9c-575">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="05b9c-576">Interativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-576">Interactive</span></span>

* <span data-ttu-id="05b9c-577">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-577">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="05b9c-578">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-578">June 5, 2018</span></span>

<span data-ttu-id="05b9c-579">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="05b9c-579">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="05b9c-580">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-580">Core</span></span>

* <span data-ttu-id="05b9c-581">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="05b9c-581">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="05b9c-582">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="05b9c-582">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="05b9c-583">ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-583">ACR</span></span>

* <span data-ttu-id="05b9c-584">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="05b9c-584">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="05b9c-585">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="05b9c-585">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="05b9c-586">AKS</span><span class="sxs-lookup"><span data-stu-id="05b9c-586">AKS</span></span>

* <span data-ttu-id="05b9c-587">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="05b9c-587">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="05b9c-588">Lote</span><span class="sxs-lookup"><span data-stu-id="05b9c-588">Batch</span></span>

* <span data-ttu-id="05b9c-589">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="05b9c-589">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="05b9c-590">IOT</span><span class="sxs-lookup"><span data-stu-id="05b9c-590">IOT</span></span>

* <span data-ttu-id="05b9c-591">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="05b9c-591">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-592">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-592">Network</span></span>

* <span data-ttu-id="05b9c-593">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="05b9c-593">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="05b9c-594">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="05b9c-594">Policy Insights</span></span>

* <span data-ttu-id="05b9c-595">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="05b9c-595">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="05b9c-596">ARM</span><span class="sxs-lookup"><span data-stu-id="05b9c-596">ARM</span></span>

* <span data-ttu-id="05b9c-597">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="05b9c-597">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="05b9c-598">SQL</span><span class="sxs-lookup"><span data-stu-id="05b9c-598">SQL</span></span>

* <span data-ttu-id="05b9c-599">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="05b9c-599">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="05b9c-600">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="05b9c-600">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="05b9c-601">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-601">Storage</span></span>

* <span data-ttu-id="05b9c-602">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="05b9c-602">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-603">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-603">VM</span></span>

* <span data-ttu-id="05b9c-604">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="05b9c-604">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="05b9c-605">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-605">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="05b9c-606">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-606">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="05b9c-607">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-607">May 22, 2018</span></span>

<span data-ttu-id="05b9c-608">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="05b9c-608">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="05b9c-609">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-609">Core</span></span>

* <span data-ttu-id="05b9c-610">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="05b9c-610">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-611">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-611">ACS</span></span>

* <span data-ttu-id="05b9c-612">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="05b9c-612">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="05b9c-613">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="05b9c-613">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-614">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-614">AppService</span></span>

* <span data-ttu-id="05b9c-615">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="05b9c-615">Improved generic update commands</span></span>
* <span data-ttu-id="05b9c-616">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="05b9c-616">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="05b9c-617">Contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-617">Container</span></span>

* <span data-ttu-id="05b9c-618">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="05b9c-618">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="05b9c-619">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-619">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="05b9c-620">Extensão</span><span class="sxs-lookup"><span data-stu-id="05b9c-620">Extension</span></span>

* <span data-ttu-id="05b9c-621">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="05b9c-621">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="05b9c-622">Interativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-622">Interactive</span></span>

* <span data-ttu-id="05b9c-623">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="05b9c-623">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="05b9c-624">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="05b9c-624">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="05b9c-625">KeyVault</span><span class="sxs-lookup"><span data-stu-id="05b9c-625">KeyVault</span></span>

* <span data-ttu-id="05b9c-626">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="05b9c-626">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-627">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-627">Network</span></span>

* <span data-ttu-id="05b9c-628">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="05b9c-628">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="05b9c-629">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="05b9c-629">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="05b9c-630">SQL</span><span class="sxs-lookup"><span data-stu-id="05b9c-630">SQL</span></span>

* <span data-ttu-id="05b9c-631">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="05b9c-631">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="05b9c-632">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="05b9c-632">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="05b9c-633">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="05b9c-633">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="05b9c-634">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05b9c-634">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="05b9c-635">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="05b9c-635">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="05b9c-636">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-636">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="05b9c-637">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="05b9c-637">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="05b9c-638">`edition`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-638">`edition`.</span></span> <span data-ttu-id="05b9c-639">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="05b9c-639">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="05b9c-640">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-640">`elasticPoolName`.</span></span> <span data-ttu-id="05b9c-641">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="05b9c-641">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="05b9c-642">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="05b9c-642">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="05b9c-643">`edition`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-643">`edition`.</span></span> <span data-ttu-id="05b9c-644">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="05b9c-644">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="05b9c-645">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-645">`dtu`.</span></span> <span data-ttu-id="05b9c-646">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="05b9c-646">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="05b9c-647">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-647">`databaseDtuMin`.</span></span> <span data-ttu-id="05b9c-648">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="05b9c-648">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="05b9c-649">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-649">`databaseDtuMax`.</span></span> <span data-ttu-id="05b9c-650">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="05b9c-650">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="05b9c-651">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-651">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="05b9c-652">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-652">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-653">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-653">Storage</span></span>

* <span data-ttu-id="05b9c-654">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="05b9c-654">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="05b9c-655">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="05b9c-655">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-656">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-656">VM</span></span>

* <span data-ttu-id="05b9c-657">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-657">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="05b9c-658">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="05b9c-658">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="05b9c-659">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="05b9c-659">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="05b9c-660">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="05b9c-660">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="05b9c-661">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-661">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="05b9c-662">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-662">May 7, 2018</span></span>

<span data-ttu-id="05b9c-663">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="05b9c-663">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="05b9c-664">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-664">Core</span></span>

* <span data-ttu-id="05b9c-665">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="05b9c-665">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="05b9c-666">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="05b9c-666">Added limited support for positional arguments</span></span>
* <span data-ttu-id="05b9c-667">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-667">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="05b9c-668">#5591</span><span class="sxs-lookup"><span data-stu-id="05b9c-668">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="05b9c-669">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-669">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="05b9c-670">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="05b9c-670">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="05b9c-671">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="05b9c-671">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="05b9c-672">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="05b9c-672">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="05b9c-673">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="05b9c-673">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="05b9c-674">ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-674">ACR</span></span>

* <span data-ttu-id="05b9c-675">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-675">Added ACR Build commands</span></span>
* <span data-ttu-id="05b9c-676">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="05b9c-676">Improved resource not found error messages</span></span>
* <span data-ttu-id="05b9c-677">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="05b9c-677">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="05b9c-678">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="05b9c-678">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="05b9c-679">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="05b9c-679">Improved repository commands error messages</span></span>
* <span data-ttu-id="05b9c-680">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="05b9c-680">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-681">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-681">ACS</span></span>

* <span data-ttu-id="05b9c-682">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="05b9c-682">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="05b9c-683">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="05b9c-683">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="05b9c-684">AMS</span><span class="sxs-lookup"><span data-stu-id="05b9c-684">AMS</span></span>

* <span data-ttu-id="05b9c-685">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="05b9c-685">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-686">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-686">Appservice</span></span>

* <span data-ttu-id="05b9c-687">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="05b9c-687">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="05b9c-688">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-688">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="05b9c-689">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="05b9c-689">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="05b9c-690">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="05b9c-690">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="05b9c-691">Lote AI</span><span class="sxs-lookup"><span data-stu-id="05b9c-691">Batch AI</span></span>

* <span data-ttu-id="05b9c-692">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="05b9c-692">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="05b9c-693">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="05b9c-693">Cognitive Services</span></span>

* <span data-ttu-id="05b9c-694">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="05b9c-694">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="05b9c-695">Consumo</span><span class="sxs-lookup"><span data-stu-id="05b9c-695">Consumption</span></span>

* <span data-ttu-id="05b9c-696">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-696">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="05b9c-697">Contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-697">Container</span></span>

* <span data-ttu-id="05b9c-698">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="05b9c-698">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="05b9c-699">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="05b9c-699">Cosmos DB</span></span>

* <span data-ttu-id="05b9c-700">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="05b9c-700">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="05b9c-701">DMS</span><span class="sxs-lookup"><span data-stu-id="05b9c-701">DMS</span></span>

* <span data-ttu-id="05b9c-702">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="05b9c-702">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="05b9c-703">Extensão</span><span class="sxs-lookup"><span data-stu-id="05b9c-703">Extension</span></span>

* <span data-ttu-id="05b9c-704">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="05b9c-704">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="05b9c-705">Interativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-705">Interactive</span></span>

* <span data-ttu-id="05b9c-706">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="05b9c-706">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="05b9c-707">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="05b9c-707">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="05b9c-708">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="05b9c-708">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="05b9c-709">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="05b9c-709">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="05b9c-710">Laboratório</span><span class="sxs-lookup"><span data-stu-id="05b9c-710">Lab</span></span>

* <span data-ttu-id="05b9c-711">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="05b9c-711">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-712">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-712">Network</span></span>

* <span data-ttu-id="05b9c-713">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="05b9c-713">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="05b9c-714">Perfil</span><span class="sxs-lookup"><span data-stu-id="05b9c-714">Profile</span></span>

* <span data-ttu-id="05b9c-715">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="05b9c-715">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="05b9c-716">[ALTERAÇÃO SIGNIFICATIVA] `--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="05b9c-716">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="05b9c-717">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="05b9c-717">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="05b9c-718">Redis</span><span class="sxs-lookup"><span data-stu-id="05b9c-718">Redis</span></span>

* <span data-ttu-id="05b9c-719">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="05b9c-719">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="05b9c-720">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="05b9c-720">Deprecated `redis list-all`.</span></span> <span data-ttu-id="05b9c-721">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="05b9c-721">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="05b9c-722">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="05b9c-722">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="05b9c-723">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="05b9c-723">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="05b9c-724">Função</span><span class="sxs-lookup"><span data-stu-id="05b9c-724">Role</span></span>

* <span data-ttu-id="05b9c-725">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="05b9c-725">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-726">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-726">Storage</span></span>

* <span data-ttu-id="05b9c-727">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="05b9c-727">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="05b9c-728">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="05b9c-728">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="05b9c-729">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="05b9c-729">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="05b9c-730">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="05b9c-730">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="05b9c-731">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="05b9c-731">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-732">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-732">VM</span></span>

* <span data-ttu-id="05b9c-733">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="05b9c-733">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="05b9c-734">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="05b9c-734">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="05b9c-735">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="05b9c-735">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="05b9c-736">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="05b9c-736">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="05b9c-737">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="05b9c-737">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="05b9c-738">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="05b9c-738">Added write accelerator support</span></span>
* <span data-ttu-id="05b9c-739">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="05b9c-739">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="05b9c-740">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="05b9c-740">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="05b9c-741">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="05b9c-741">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="05b9c-742">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-742">April 10, 2018</span></span>

<span data-ttu-id="05b9c-743">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="05b9c-743">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="05b9c-744">ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-744">ACR</span></span>

* <span data-ttu-id="05b9c-745">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="05b9c-745">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-746">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-746">ACS</span></span>

* <span data-ttu-id="05b9c-747">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="05b9c-747">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-748">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-748">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="05b9c-750">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="05b9c-750">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="05b9c-751">BatchAI</span><span class="sxs-lookup"><span data-stu-id="05b9c-751">BatchAI</span></span>

* <span data-ttu-id="05b9c-752">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="05b9c-752">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="05b9c-753">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="05b9c-753">Job level mounting</span></span>
  - <span data-ttu-id="05b9c-754">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="05b9c-754">Environment variables with secret values</span></span>
  - <span data-ttu-id="05b9c-755">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="05b9c-755">Performance counters settings</span></span>
  - <span data-ttu-id="05b9c-756">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="05b9c-756">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="05b9c-757">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="05b9c-757">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="05b9c-758">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="05b9c-758">Usage and limits reporting</span></span>
  - <span data-ttu-id="05b9c-759">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="05b9c-759">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="05b9c-760">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="05b9c-760">Support for custom images</span></span>
  - <span data-ttu-id="05b9c-761">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="05b9c-761">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="05b9c-762">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="05b9c-762">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="05b9c-763">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="05b9c-763">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="05b9c-764">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="05b9c-764">National clouds are supported</span></span>
* <span data-ttu-id="05b9c-765">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="05b9c-765">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="05b9c-766">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="05b9c-766">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="05b9c-767">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="05b9c-767">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="05b9c-768">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="05b9c-768">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="05b9c-769">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="05b9c-769">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="05b9c-770">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="05b9c-770">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="05b9c-771">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="05b9c-771">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="05b9c-772">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="05b9c-772">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="05b9c-773">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="05b9c-773">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="05b9c-774">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-774">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="05b9c-775">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="05b9c-775">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="05b9c-776">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="05b9c-776">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="05b9c-777">[ALTERAÇÃO SIGNIFICATIVA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-777">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="05b9c-778">Cobrança</span><span class="sxs-lookup"><span data-stu-id="05b9c-778">Billing</span></span>

* <span data-ttu-id="05b9c-779">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="05b9c-779">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="05b9c-780">Consumo</span><span class="sxs-lookup"><span data-stu-id="05b9c-780">Consumption</span></span>

* <span data-ttu-id="05b9c-781">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="05b9c-781">Added `marketplace` commands</span></span>
* <span data-ttu-id="05b9c-782">[ALTERAÇÃO SIGNIFICATIVA] `reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="05b9c-782">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="05b9c-783">[ALTERAÇÃO SIGNIFICATIVA] `reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="05b9c-783">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="05b9c-784">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="05b9c-784">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="05b9c-785">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="05b9c-785">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="05b9c-786">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="05b9c-786">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="05b9c-787">Contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-787">Container</span></span>

* <span data-ttu-id="05b9c-788">Adição dos parâmetros de montagem de volume de repositório git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="05b9c-788">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="05b9c-789">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="05b9c-789">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="05b9c-790">Extensão</span><span class="sxs-lookup"><span data-stu-id="05b9c-790">Extension</span></span>

* <span data-ttu-id="05b9c-791">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="05b9c-791">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="05b9c-792">Interativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-792">Interactive</span></span>

* <span data-ttu-id="05b9c-793">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="05b9c-793">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="05b9c-794">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="05b9c-794">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="05b9c-795">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="05b9c-795">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-796">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-796">Network</span></span>

* <span data-ttu-id="05b9c-797">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="05b9c-797">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="05b9c-798">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-798">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="05b9c-799">#4910</span><span class="sxs-lookup"><span data-stu-id="05b9c-799">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="05b9c-800">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="05b9c-800">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="05b9c-801">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="05b9c-801">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="05b9c-802">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-802">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="05b9c-803">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-803">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="05b9c-804">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="05b9c-804">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="05b9c-805">Perfil</span><span class="sxs-lookup"><span data-stu-id="05b9c-805">Profile</span></span>

* <span data-ttu-id="05b9c-806">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="05b9c-806">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="05b9c-807">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="05b9c-807">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="05b9c-808">RDBMS</span><span class="sxs-lookup"><span data-stu-id="05b9c-808">RDBMS</span></span>

* <span data-ttu-id="05b9c-809">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="05b9c-809">Added `georestore` command</span></span>
* <span data-ttu-id="05b9c-810">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-810">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="05b9c-811">Recurso</span><span class="sxs-lookup"><span data-stu-id="05b9c-811">Resource</span></span>

* <span data-ttu-id="05b9c-812">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-812">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="05b9c-813">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-813">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="05b9c-814">SQL</span><span class="sxs-lookup"><span data-stu-id="05b9c-814">SQL</span></span>

* <span data-ttu-id="05b9c-815">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="05b9c-815">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-816">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-816">Storage</span></span>

* <span data-ttu-id="05b9c-817">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="05b9c-817">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-818">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-818">VM</span></span>

* <span data-ttu-id="05b9c-819">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-819">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="05b9c-820">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-820">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="05b9c-822">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-822">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="05b9c-823">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="05b9c-823">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="05b9c-824">#5718</span><span class="sxs-lookup"><span data-stu-id="05b9c-824">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="05b9c-825">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="05b9c-825">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="05b9c-826">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-826">March 27, 2018</span></span>

<span data-ttu-id="05b9c-827">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="05b9c-827">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="05b9c-828">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-828">Core</span></span>

* <span data-ttu-id="05b9c-829">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="05b9c-829">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-830">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-830">ACS</span></span>

* <span data-ttu-id="05b9c-831">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="05b9c-831">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-832">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-832">Appservice</span></span>

* <span data-ttu-id="05b9c-833">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-833">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="05b9c-834">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-834">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="05b9c-835">Backup</span><span class="sxs-lookup"><span data-stu-id="05b9c-835">Backup</span></span>

* <span data-ttu-id="05b9c-836">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-836">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="05b9c-837">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="05b9c-837">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="05b9c-838">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="05b9c-838">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="05b9c-839">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="05b9c-839">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="05b9c-840">Contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-840">Container</span></span>

* <span data-ttu-id="05b9c-841">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-841">Added `container exec` command.</span></span> <span data-ttu-id="05b9c-842">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="05b9c-842">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="05b9c-843">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-843">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="05b9c-844">Extensão</span><span class="sxs-lookup"><span data-stu-id="05b9c-844">Extension</span></span>

* <span data-ttu-id="05b9c-845">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="05b9c-845">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="05b9c-846">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="05b9c-846">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="05b9c-847">[ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="05b9c-847">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="05b9c-848">Interativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-848">Interactive</span></span>

* <span data-ttu-id="05b9c-849">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="05b9c-849">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="05b9c-850">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="05b9c-850">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="05b9c-851">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="05b9c-851">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="05b9c-852">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="05b9c-852">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="05b9c-853">Laboratório</span><span class="sxs-lookup"><span data-stu-id="05b9c-853">Lab</span></span>

* <span data-ttu-id="05b9c-854">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="05b9c-854">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="05b9c-855">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="05b9c-855">Monitor</span></span>

* <span data-ttu-id="05b9c-856">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="05b9c-856">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="05b9c-857">[#4529](https://github.com/Azure/azure-cli/issues/5785) corrigido: `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="05b9c-857">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="05b9c-858">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="05b9c-858">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-859">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-859">Network</span></span>

* <span data-ttu-id="05b9c-860">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="05b9c-860">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="05b9c-861">Perfil</span><span class="sxs-lookup"><span data-stu-id="05b9c-861">Profile</span></span>

* <span data-ttu-id="05b9c-862">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="05b9c-862">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="05b9c-863">RDBMS</span><span class="sxs-lookup"><span data-stu-id="05b9c-863">RDBMS</span></span>

* <span data-ttu-id="05b9c-864">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="05b9c-864">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="05b9c-865">Recurso</span><span class="sxs-lookup"><span data-stu-id="05b9c-865">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="05b9c-867">Função</span><span class="sxs-lookup"><span data-stu-id="05b9c-867">Role</span></span>

* <span data-ttu-id="05b9c-868">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-868">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="05b9c-869">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="05b9c-869">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="05b9c-870">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-870">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="05b9c-871">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-871">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="05b9c-872">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="05b9c-872">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-873">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-873">Storage</span></span>

* <span data-ttu-id="05b9c-874">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="05b9c-874">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="05b9c-875">[4049#](https://github.com/Azure/azure-cli/issues/4049) corrigido: problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="05b9c-875">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-876">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-876">VM</span></span>

* <span data-ttu-id="05b9c-877">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="05b9c-877">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="05b9c-878">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-878">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="05b9c-879">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="05b9c-879">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="05b9c-880">[ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="05b9c-880">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="05b9c-881">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-881">March 13, 2018</span></span>

<span data-ttu-id="05b9c-882">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="05b9c-882">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="05b9c-883">ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-883">ACR</span></span>

* <span data-ttu-id="05b9c-884">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="05b9c-884">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="05b9c-885">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="05b9c-885">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="05b9c-886">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="05b9c-886">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-887">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-887">ACS</span></span>

* <span data-ttu-id="05b9c-888">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="05b9c-888">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="05b9c-889">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="05b9c-889">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="05b9c-890">Supervisor</span><span class="sxs-lookup"><span data-stu-id="05b9c-890">Advisor</span></span>

* <span data-ttu-id="05b9c-891">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="05b9c-891">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="05b9c-892">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-892">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="05b9c-893">[ALTERAÇÃO SIGNIFICATIVA] `advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="05b9c-893">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="05b9c-894">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="05b9c-894">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="05b9c-895">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="05b9c-895">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-896">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-896">Appservice</span></span>

* <span data-ttu-id="05b9c-897">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="05b9c-897">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="05b9c-898">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="05b9c-898">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="05b9c-899">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="05b9c-899">Eventhubs</span></span>

* <span data-ttu-id="05b9c-900">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="05b9c-900">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="05b9c-901">Extensão</span><span class="sxs-lookup"><span data-stu-id="05b9c-901">Extension</span></span>

* <span data-ttu-id="05b9c-902">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="05b9c-902">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="05b9c-903">Interativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-903">Interactive</span></span>

* <span data-ttu-id="05b9c-904">[5625](https://github.com/Azure/azure-cli/issues/5625) corrigido: manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="05b9c-904">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="05b9c-905">[3016](https://github.com/Azure/azure-cli/issues/3016) corrigido: histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="05b9c-905">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="05b9c-906">[5688](https://github.com/Azure/azure-cli/issues/5688) corrigido: as conclusões não aparecerão se o carregamento da tabela de comando encontrou uma exceção</span><span class="sxs-lookup"><span data-stu-id="05b9c-906">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="05b9c-907">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="05b9c-907">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="05b9c-908">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="05b9c-908">Monitor</span></span>

* <span data-ttu-id="05b9c-909">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="05b9c-909">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="05b9c-910">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="05b9c-910">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="05b9c-911">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="05b9c-911">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="05b9c-912">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="05b9c-912">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-913">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-913">Network</span></span>

* <span data-ttu-id="05b9c-914">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-914">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="05b9c-915">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="05b9c-915">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="05b9c-916">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="05b9c-916">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="05b9c-917">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="05b9c-917">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="05b9c-918">Perfil</span><span class="sxs-lookup"><span data-stu-id="05b9c-918">Profile</span></span>

* <span data-ttu-id="05b9c-919">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="05b9c-919">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="05b9c-920">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="05b9c-920">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="05b9c-921">RDBMS</span><span class="sxs-lookup"><span data-stu-id="05b9c-921">RDBMS</span></span>

* <span data-ttu-id="05b9c-922">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="05b9c-922">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="05b9c-923">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="05b9c-923">Service Bus</span></span>

* <span data-ttu-id="05b9c-924">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="05b9c-924">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-925">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-925">Storage</span></span>

* <span data-ttu-id="05b9c-926">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="05b9c-926">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="05b9c-927">[5286](https://github.com/Azure/azure-cli/issues/5286) corrigido: os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="05b9c-927">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-928">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-928">VM</span></span>

* <span data-ttu-id="05b9c-929">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="05b9c-929">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="05b9c-930">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="05b9c-930">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="05b9c-931">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="05b9c-931">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="05b9c-932">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="05b9c-932">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="05b9c-933">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-933">February 27, 2018</span></span>

<span data-ttu-id="05b9c-934">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="05b9c-934">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="05b9c-935">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-935">Core</span></span>

* <span data-ttu-id="05b9c-936">Correção [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="05b9c-936">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="05b9c-937">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="05b9c-937">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="05b9c-938">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="05b9c-938">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-939">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-939">ACS</span></span>

* <span data-ttu-id="05b9c-940">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="05b9c-940">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="05b9c-941">Correção do problema de permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="05b9c-941">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="05b9c-942">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="05b9c-942">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="05b9c-943">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="05b9c-943">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-944">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-944">Appservice</span></span>

* <span data-ttu-id="05b9c-945">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="05b9c-945">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="05b9c-946">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="05b9c-946">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="05b9c-947">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="05b9c-947">Cognitive Services</span></span>

* <span data-ttu-id="05b9c-948">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="05b9c-948">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="05b9c-949">Consumo</span><span class="sxs-lookup"><span data-stu-id="05b9c-949">Consumption</span></span>

* <span data-ttu-id="05b9c-950">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="05b9c-950">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="05b9c-951">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="05b9c-951">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="05b9c-952">Contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-952">Container</span></span>

* <span data-ttu-id="05b9c-953">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="05b9c-953">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-954">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-954">Network</span></span>

* <span data-ttu-id="05b9c-955">Correção [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="05b9c-955">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="05b9c-956">Recurso</span><span class="sxs-lookup"><span data-stu-id="05b9c-956">Resource</span></span>

* <span data-ttu-id="05b9c-957">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="05b9c-957">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="05b9c-958">Função</span><span class="sxs-lookup"><span data-stu-id="05b9c-958">Role</span></span>

* <span data-ttu-id="05b9c-959">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="05b9c-959">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="05b9c-960">SQL</span><span class="sxs-lookup"><span data-stu-id="05b9c-960">SQL</span></span>

* <span data-ttu-id="05b9c-961">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="05b9c-961">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-962">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-962">Storage</span></span>

* <span data-ttu-id="05b9c-963">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-963">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-964">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-964">VM</span></span>

* <span data-ttu-id="05b9c-965">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="05b9c-965">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="05b9c-966">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-966">February 13, 2018</span></span>

<span data-ttu-id="05b9c-967">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="05b9c-967">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="05b9c-968">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-968">Core</span></span>

* <span data-ttu-id="05b9c-969">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="05b9c-969">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-970">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-970">ACS</span></span>

* <span data-ttu-id="05b9c-971">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="05b9c-971">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="05b9c-972">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-972">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="05b9c-973">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="05b9c-973">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="05b9c-974">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="05b9c-974">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="05b9c-975">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="05b9c-975">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="05b9c-976">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="05b9c-976">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="05b9c-977">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="05b9c-977">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="05b9c-978">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="05b9c-978">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-979">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-979">Appservice</span></span>

* <span data-ttu-id="05b9c-980">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="05b9c-980">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="05b9c-981">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="05b9c-981">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="05b9c-982">CDN</span><span class="sxs-lookup"><span data-stu-id="05b9c-982">CDN</span></span>

* <span data-ttu-id="05b9c-983">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-983">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="05b9c-984">Contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-984">Container</span></span>

* <span data-ttu-id="05b9c-985">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="05b9c-985">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="05b9c-986">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-986">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="05b9c-987">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="05b9c-987">CosmosDB</span></span>

* <span data-ttu-id="05b9c-988">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="05b9c-988">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="05b9c-989">Extensão</span><span class="sxs-lookup"><span data-stu-id="05b9c-989">Extension</span></span>

* <span data-ttu-id="05b9c-990">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-990">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="05b9c-991">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-991">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="05b9c-992">Comentários</span><span class="sxs-lookup"><span data-stu-id="05b9c-992">Feedback</span></span>

* <span data-ttu-id="05b9c-993">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="05b9c-993">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="05b9c-994">Interativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-994">Interactive</span></span>

* <span data-ttu-id="05b9c-995">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="05b9c-995">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="05b9c-996">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="05b9c-996">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="05b9c-997">IoT</span><span class="sxs-lookup"><span data-stu-id="05b9c-997">IoT</span></span>

* <span data-ttu-id="05b9c-998">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="05b9c-998">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="05b9c-999">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="05b9c-999">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="05b9c-1000">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1000">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="05b9c-1001">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="05b9c-1001">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="05b9c-1002">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="05b9c-1002">Monitor</span></span>

* <span data-ttu-id="05b9c-1003">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1003">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-1004">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-1004">Network</span></span>

* <span data-ttu-id="05b9c-1005">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="05b9c-1005">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="05b9c-1006">Perfil</span><span class="sxs-lookup"><span data-stu-id="05b9c-1006">Profile</span></span>

* <span data-ttu-id="05b9c-1007">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1007">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="05b9c-1008">Recurso</span><span class="sxs-lookup"><span data-stu-id="05b9c-1008">Resource</span></span>

* <span data-ttu-id="05b9c-1009">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="05b9c-1009">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="05b9c-1010">Função</span><span class="sxs-lookup"><span data-stu-id="05b9c-1010">Role</span></span>

* <span data-ttu-id="05b9c-1011">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1011">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="05b9c-1012">SQL</span><span class="sxs-lookup"><span data-stu-id="05b9c-1012">SQL</span></span>

* <span data-ttu-id="05b9c-1013">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1013">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="05b9c-1014">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1014">Added `sql db rename`</span></span>
* <span data-ttu-id="05b9c-1015">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="05b9c-1015">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-1016">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-1016">Storage</span></span>

* <span data-ttu-id="05b9c-1017">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="05b9c-1017">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-1018">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-1018">VM</span></span>

* <span data-ttu-id="05b9c-1019">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="05b9c-1019">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="05b9c-1020">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="05b9c-1020">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="05b9c-1021">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1021">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="05b9c-1022">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-1022">January 31, 2018</span></span>

<span data-ttu-id="05b9c-1023">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="05b9c-1023">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="05b9c-1024">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1024">Core</span></span>

* <span data-ttu-id="05b9c-1025">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="05b9c-1025">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="05b9c-1026">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="05b9c-1026">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="05b9c-1027">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1027">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="05b9c-1028">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="05b9c-1028">Use `--verbose` to see</span></span>
* <span data-ttu-id="05b9c-1029">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="05b9c-1029">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-1030">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-1030">ACS</span></span>

* <span data-ttu-id="05b9c-1031">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="05b9c-1031">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="05b9c-1032">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1032">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-1033">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-1033">Appservice</span></span>

* <span data-ttu-id="05b9c-1034">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1034">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="05b9c-1035">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="05b9c-1035">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="05b9c-1036">CDN</span><span class="sxs-lookup"><span data-stu-id="05b9c-1036">CDN</span></span>

* <span data-ttu-id="05b9c-1037">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1037">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="05b9c-1038">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="05b9c-1038">CosmosDB</span></span>

* <span data-ttu-id="05b9c-1039">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="05b9c-1039">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="05b9c-1040">Interativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1040">Interactive</span></span>

* <span data-ttu-id="05b9c-1041">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="05b9c-1041">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-1042">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-1042">Network</span></span>

* <span data-ttu-id="05b9c-1043">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1043">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="05b9c-1044">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="05b9c-1044">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="05b9c-1045">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1045">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="05b9c-1046">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1046">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="05b9c-1047">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1047">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="05b9c-1048">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="05b9c-1048">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="05b9c-1049">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="05b9c-1049">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="05b9c-1050">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="05b9c-1050">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="05b9c-1051">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1051">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="05b9c-1052">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1052">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="05b9c-1053">Perfil</span><span class="sxs-lookup"><span data-stu-id="05b9c-1053">Profile</span></span>

* <span data-ttu-id="05b9c-1054">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="05b9c-1054">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="05b9c-1055">Recurso</span><span class="sxs-lookup"><span data-stu-id="05b9c-1055">Resource</span></span>

* <span data-ttu-id="05b9c-1056">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="05b9c-1056">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-1057">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-1057">Storage</span></span>

* <span data-ttu-id="05b9c-1058">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="05b9c-1058">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="05b9c-1059">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="05b9c-1059">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="05b9c-1060">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1060">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="05b9c-1061">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1061">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="05b9c-1062">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="05b9c-1062">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-1063">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-1063">VM</span></span>

* <span data-ttu-id="05b9c-1064">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="05b9c-1064">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="05b9c-1065">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="05b9c-1065">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="05b9c-1066">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="05b9c-1066">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="05b9c-1067">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1067">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="05b9c-1068">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="05b9c-1068">January 17, 2018</span></span>

<span data-ttu-id="05b9c-1069">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="05b9c-1069">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="05b9c-1070">ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-1070">ACR</span></span>

* <span data-ttu-id="05b9c-1071">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="05b9c-1071">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="05b9c-1072">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="05b9c-1072">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-1073">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-1073">ACS</span></span>

* <span data-ttu-id="05b9c-1074">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1074">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="05b9c-1075">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="05b9c-1075">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-1076">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-1076">Appservice</span></span>

* <span data-ttu-id="05b9c-1077">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1077">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="05b9c-1078">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1078">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="05b9c-1079">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1079">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="05b9c-1080">Backup</span><span class="sxs-lookup"><span data-stu-id="05b9c-1080">Backup</span></span>

* <span data-ttu-id="05b9c-1081">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="05b9c-1081">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="05b9c-1082">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1082">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="05b9c-1083">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="05b9c-1083">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="05b9c-1084">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="05b9c-1084">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="05b9c-1085">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="05b9c-1085">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="05b9c-1086">Lote</span><span class="sxs-lookup"><span data-stu-id="05b9c-1086">Batch</span></span>

* <span data-ttu-id="05b9c-1087">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="05b9c-1087">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="05b9c-1088">Nuvem</span><span class="sxs-lookup"><span data-stu-id="05b9c-1088">Cloud</span></span>

* <span data-ttu-id="05b9c-1089">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="05b9c-1089">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="05b9c-1090">Consumo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1090">Consumption</span></span>

* <span data-ttu-id="05b9c-1091">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1091">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="05b9c-1092">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="05b9c-1092">Event Grid</span></span>

* <span data-ttu-id="05b9c-1093">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1093">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="05b9c-1094">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1094">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="05b9c-1095">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1095">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="05b9c-1096">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1096">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="05b9c-1097">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1097">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="05b9c-1098">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1098">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="05b9c-1099">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1099">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="05b9c-1100">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="05b9c-1100">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="05b9c-1101">Interativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1101">Interactive</span></span>

* <span data-ttu-id="05b9c-1102">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="05b9c-1102">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="05b9c-1103">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="05b9c-1103">Fixed errors on startup</span></span>
* <span data-ttu-id="05b9c-1104">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1104">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="05b9c-1105">IoT</span><span class="sxs-lookup"><span data-stu-id="05b9c-1105">IoT</span></span>

* <span data-ttu-id="05b9c-1106">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="05b9c-1106">Added support for device provisioning service</span></span>
* <span data-ttu-id="05b9c-1107">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="05b9c-1107">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="05b9c-1108">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="05b9c-1108">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="05b9c-1109">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="05b9c-1109">Monitor</span></span>

* <span data-ttu-id="05b9c-1110">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1110">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="05b9c-1111">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1111">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="05b9c-1112">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="05b9c-1112">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-1113">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-1113">Network</span></span>

* <span data-ttu-id="05b9c-1114">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1114">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="05b9c-1115">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1115">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="05b9c-1116">Perfil</span><span class="sxs-lookup"><span data-stu-id="05b9c-1116">Profile</span></span>

* <span data-ttu-id="05b9c-1117">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="05b9c-1117">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="05b9c-1118">Função</span><span class="sxs-lookup"><span data-stu-id="05b9c-1118">Role</span></span>

* <span data-ttu-id="05b9c-1119">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="05b9c-1119">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="05b9c-1120">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="05b9c-1120">Service Fabric</span></span>

* <span data-ttu-id="05b9c-1121">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="05b9c-1121">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="05b9c-1122">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="05b9c-1122">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-1123">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-1123">VM</span></span>

* <span data-ttu-id="05b9c-1124">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1124">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="05b9c-1125">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="05b9c-1125">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="05b9c-1126">[ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="05b9c-1126">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="05b9c-1127">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="05b9c-1127">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="05b9c-1128">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="05b9c-1128">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="05b9c-1129">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1129">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="05b9c-1130">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1130">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="05b9c-1131">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1131">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="05b9c-1132">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="05b9c-1132">December 19, 2017</span></span>

<span data-ttu-id="05b9c-1133">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="05b9c-1133">Version 2.0.23</span></span>

* <span data-ttu-id="05b9c-1134">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="05b9c-1134">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="05b9c-1135">Contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-1135">Container</span></span>

* <span data-ttu-id="05b9c-1136">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-1136">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-1137">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-1137">Network</span></span>

* <span data-ttu-id="05b9c-1138">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1138">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="05b9c-1139">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1139">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-1140">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-1140">Storage</span></span>

* <span data-ttu-id="05b9c-1141">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="05b9c-1141">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-1142">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-1142">VM</span></span>

* <span data-ttu-id="05b9c-1143">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="05b9c-1143">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="05b9c-1144">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="05b9c-1144">December 5, 2017</span></span>

<span data-ttu-id="05b9c-1145">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="05b9c-1145">Version 2.0.22</span></span>

* <span data-ttu-id="05b9c-1146">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1146">Removed `az component` commands.</span></span> <span data-ttu-id="05b9c-1147">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1147">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="05b9c-1148">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1148">Core</span></span>
* <span data-ttu-id="05b9c-1149">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="05b9c-1149">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="05b9c-1150">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="05b9c-1150">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-1151">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-1151">ACS</span></span>

* <span data-ttu-id="05b9c-1152">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="05b9c-1152">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="05b9c-1153">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1153">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="05b9c-1154">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="05b9c-1154">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="05b9c-1155">Supervisor</span><span class="sxs-lookup"><span data-stu-id="05b9c-1155">Advisor</span></span>

* <span data-ttu-id="05b9c-1156">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="05b9c-1156">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-1157">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-1157">Appservice</span></span>

* <span data-ttu-id="05b9c-1158">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1158">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="05b9c-1159">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="05b9c-1159">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="05b9c-1160">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1160">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="05b9c-1161">Consumo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1161">Consumption</span></span>

* <span data-ttu-id="05b9c-1162">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="05b9c-1162">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="05b9c-1163">Contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-1163">Container</span></span>

* <span data-ttu-id="05b9c-1164">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="05b9c-1164">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="05b9c-1165">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="05b9c-1165">Monitor</span></span>

* <span data-ttu-id="05b9c-1166">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="05b9c-1166">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="05b9c-1167">Recurso</span><span class="sxs-lookup"><span data-stu-id="05b9c-1167">Resource</span></span>

* <span data-ttu-id="05b9c-1168">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1168">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="05b9c-1169">Função</span><span class="sxs-lookup"><span data-stu-id="05b9c-1169">Role</span></span>

* <span data-ttu-id="05b9c-1170">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1170">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="05b9c-1171">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="05b9c-1171">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="05b9c-1172">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1172">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="05b9c-1173">SQL</span><span class="sxs-lookup"><span data-stu-id="05b9c-1173">SQL</span></span>

* <span data-ttu-id="05b9c-1174">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="05b9c-1174">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="05b9c-1175">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="05b9c-1175">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-1176">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-1176">VM</span></span>

* <span data-ttu-id="05b9c-1177">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1177">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="05b9c-1178">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="05b9c-1178">November 14, 2017</span></span>

<span data-ttu-id="05b9c-1179">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="05b9c-1179">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="05b9c-1180">ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-1180">ACR</span></span>

* <span data-ttu-id="05b9c-1181">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="05b9c-1181">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="05b9c-1182">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-1182">ACS</span></span>

* <span data-ttu-id="05b9c-1183">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="05b9c-1183">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="05b9c-1184">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1184">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="05b9c-1185">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1185">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="05b9c-1186">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="05b9c-1186">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="05b9c-1187">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="05b9c-1187">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-1188">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-1188">Appservice</span></span>

* <span data-ttu-id="05b9c-1189">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="05b9c-1189">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="05b9c-1190">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1190">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="05b9c-1191">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1191">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="05b9c-1192">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1192">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="05b9c-1193">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="05b9c-1193">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="05b9c-1194">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1194">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="05b9c-1195">Lote</span><span class="sxs-lookup"><span data-stu-id="05b9c-1195">Batch</span></span>

* <span data-ttu-id="05b9c-1196">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1196">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="05b9c-1197">Batchai</span><span class="sxs-lookup"><span data-stu-id="05b9c-1197">Batchai</span></span>

* <span data-ttu-id="05b9c-1198">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1198">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="05b9c-1199">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1199">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="05b9c-1200">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1200">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="05b9c-1201">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1201">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="05b9c-1202">Nuvem</span><span class="sxs-lookup"><span data-stu-id="05b9c-1202">Cloud</span></span>

* <span data-ttu-id="05b9c-1203">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="05b9c-1203">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="05b9c-1204">Contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-1204">Container</span></span>

* <span data-ttu-id="05b9c-1205">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="05b9c-1205">Added support to open multiple ports</span></span>
* <span data-ttu-id="05b9c-1206">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="05b9c-1206">Added container group restart policy</span></span>
* <span data-ttu-id="05b9c-1207">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="05b9c-1207">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="05b9c-1208">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="05b9c-1208">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="05b9c-1209">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="05b9c-1209">Data Lake Analytics</span></span>

* <span data-ttu-id="05b9c-1210">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="05b9c-1210">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="05b9c-1211">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="05b9c-1211">Data Lake Store</span></span>

* <span data-ttu-id="05b9c-1212">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="05b9c-1212">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="05b9c-1213">Extensão</span><span class="sxs-lookup"><span data-stu-id="05b9c-1213">Extension</span></span>

* <span data-ttu-id="05b9c-1214">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="05b9c-1214">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="05b9c-1215">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="05b9c-1215">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="05b9c-1216">IoT</span><span class="sxs-lookup"><span data-stu-id="05b9c-1216">IoT</span></span>

* <span data-ttu-id="05b9c-1217">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="05b9c-1217">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="05b9c-1218">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="05b9c-1218">Monitor</span></span>

* <span data-ttu-id="05b9c-1219">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1219">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-1220">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-1220">Network</span></span>

* <span data-ttu-id="05b9c-1221">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="05b9c-1221">Added support for CAA DNS records</span></span>
* <span data-ttu-id="05b9c-1222">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1222">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="05b9c-1223">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="05b9c-1223">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="05b9c-1224">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1224">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="05b9c-1225">Reservas</span><span class="sxs-lookup"><span data-stu-id="05b9c-1225">Reservations</span></span>

* <span data-ttu-id="05b9c-1226">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="05b9c-1226">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="05b9c-1227">Recurso</span><span class="sxs-lookup"><span data-stu-id="05b9c-1227">Resource</span></span>

* <span data-ttu-id="05b9c-1228">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="05b9c-1228">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="05b9c-1229">SQL</span><span class="sxs-lookup"><span data-stu-id="05b9c-1229">SQL</span></span>

* <span data-ttu-id="05b9c-1230">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1230">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-1231">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-1231">Storage</span></span>

* <span data-ttu-id="05b9c-1232">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="05b9c-1232">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="05b9c-1233">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="05b9c-1233">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="05b9c-1234">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1234">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="05b9c-1235">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1235">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="05b9c-1236">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1236">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="05b9c-1237">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1237">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="05b9c-1238">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1238">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-1239">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-1239">VM</span></span>

* <span data-ttu-id="05b9c-1240">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1240">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="05b9c-1241">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="05b9c-1241">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="05b9c-1242">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="05b9c-1242">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="05b9c-1243">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1243">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="05b9c-1244">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1244">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="05b9c-1245">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="05b9c-1245">October 24, 2017</span></span>

<span data-ttu-id="05b9c-1246">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="05b9c-1246">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="05b9c-1247">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1247">Core</span></span>

* <span data-ttu-id="05b9c-1248">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1248">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="05b9c-1249">ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-1249">ACR</span></span>

* <span data-ttu-id="05b9c-1250">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1250">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="05b9c-1251">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="05b9c-1251">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="05b9c-1252">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="05b9c-1252">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-1253">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-1253">ACS</span></span>

* <span data-ttu-id="05b9c-1254">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="05b9c-1254">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="05b9c-1255">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="05b9c-1255">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-1256">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-1256">Appservice</span></span>

* <span data-ttu-id="05b9c-1257">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="05b9c-1257">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="05b9c-1258">Componente</span><span class="sxs-lookup"><span data-stu-id="05b9c-1258">Component</span></span>

* <span data-ttu-id="05b9c-1259">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="05b9c-1259">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="05b9c-1260">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="05b9c-1260">Monitor</span></span>

* <span data-ttu-id="05b9c-1261">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1261">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="05b9c-1262">Recurso</span><span class="sxs-lookup"><span data-stu-id="05b9c-1262">Resource</span></span>

* <span data-ttu-id="05b9c-1263">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1263">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="05b9c-1264">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="05b9c-1264">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-1265">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-1265">VM</span></span>

* <span data-ttu-id="05b9c-1266">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1266">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="05b9c-1267">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="05b9c-1267">October 9, 2017</span></span>

<span data-ttu-id="05b9c-1268">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="05b9c-1268">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="05b9c-1269">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1269">Core</span></span>

* <span data-ttu-id="05b9c-1270">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="05b9c-1270">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-1271">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-1271">Appservice</span></span>

* <span data-ttu-id="05b9c-1272">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1272">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="05b9c-1273">Lote</span><span class="sxs-lookup"><span data-stu-id="05b9c-1273">Batch</span></span>

* <span data-ttu-id="05b9c-1274">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="05b9c-1274">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="05b9c-1275">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="05b9c-1275">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="05b9c-1276">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="05b9c-1276">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="05b9c-1277">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="05b9c-1277">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="05b9c-1278">Batchai</span><span class="sxs-lookup"><span data-stu-id="05b9c-1278">Batchai</span></span>

* <span data-ttu-id="05b9c-1279">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="05b9c-1279">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="05b9c-1280">Keyvault</span><span class="sxs-lookup"><span data-stu-id="05b9c-1280">Keyvault</span></span>

* <span data-ttu-id="05b9c-1281">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1281">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="05b9c-1282">(#4448)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1282">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="05b9c-1283">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-1283">Network</span></span>

* <span data-ttu-id="05b9c-1284">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="05b9c-1284">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="05b9c-1285">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="05b9c-1285">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="05b9c-1286">Recurso</span><span class="sxs-lookup"><span data-stu-id="05b9c-1286">Resource</span></span>

* <span data-ttu-id="05b9c-1287">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1287">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="05b9c-1288">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="05b9c-1288">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="05b9c-1289">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1289">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="05b9c-1290">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="05b9c-1290">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="05b9c-1291">Sql</span><span class="sxs-lookup"><span data-stu-id="05b9c-1291">Sql</span></span>

* <span data-ttu-id="05b9c-1292">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="05b9c-1292">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="05b9c-1293">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="05b9c-1293">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="05b9c-1294">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="05b9c-1294">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-1295">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-1295">Storage</span></span>

* <span data-ttu-id="05b9c-1296">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="05b9c-1296">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-1297">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-1297">Vm</span></span>

* <span data-ttu-id="05b9c-1298">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="05b9c-1298">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="05b9c-1299">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1299">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="05b9c-1300">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1300">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="05b9c-1301">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1301">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="05b9c-1302">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1302">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="05b9c-1303">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="05b9c-1303">September 22, 2017</span></span>

<span data-ttu-id="05b9c-1304">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="05b9c-1304">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="05b9c-1305">Recurso</span><span class="sxs-lookup"><span data-stu-id="05b9c-1305">Resource</span></span>

* <span data-ttu-id="05b9c-1306">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="05b9c-1306">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="05b9c-1307">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="05b9c-1307">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="05b9c-1308">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1308">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="05b9c-1309">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1309">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-1310">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-1310">Network</span></span>

* <span data-ttu-id="05b9c-1311">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1311">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="05b9c-1312">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1312">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="05b9c-1313">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1313">Added `asg` application security group commands</span></span>
* <span data-ttu-id="05b9c-1314">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1314">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="05b9c-1315">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1315">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="05b9c-1316">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1316">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="05b9c-1317">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1317">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-1318">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-1318">Storage</span></span>

* <span data-ttu-id="05b9c-1319">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="05b9c-1319">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="05b9c-1320">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="05b9c-1320">Eventgrid</span></span>

* <span data-ttu-id="05b9c-1321">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="05b9c-1321">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="05b9c-1322">SQL</span><span class="sxs-lookup"><span data-stu-id="05b9c-1322">SQL</span></span>

* <span data-ttu-id="05b9c-1323">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1323">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="05b9c-1324">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="05b9c-1324">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="05b9c-1325">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1325">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="05b9c-1326">Keyvault</span><span class="sxs-lookup"><span data-stu-id="05b9c-1326">Keyvault</span></span>

* <span data-ttu-id="05b9c-1327">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="05b9c-1327">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-1328">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-1328">VM</span></span>

* <span data-ttu-id="05b9c-1329">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1329">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="05b9c-1330">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="05b9c-1330">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="05b9c-1331">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1331">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="05b9c-1332">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1332">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="05b9c-1333">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1333">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="05b9c-1334">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1334">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-1335">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-1335">ACS</span></span>

* <span data-ttu-id="05b9c-1336">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-1336">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-1337">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-1337">Appservice</span></span>

* <span data-ttu-id="05b9c-1338">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1338">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="05b9c-1339">Backup</span><span class="sxs-lookup"><span data-stu-id="05b9c-1339">Backup</span></span>

* <span data-ttu-id="05b9c-1340">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="05b9c-1340">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="05b9c-1341">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="05b9c-1341">September 11, 2017</span></span>

<span data-ttu-id="05b9c-1342">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="05b9c-1342">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="05b9c-1343">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1343">Core</span></span>

* <span data-ttu-id="05b9c-1344">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="05b9c-1344">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="05b9c-1345">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="05b9c-1345">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-1346">Acs</span><span class="sxs-lookup"><span data-stu-id="05b9c-1346">Acs</span></span>

* <span data-ttu-id="05b9c-1347">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1347">Added `acs list-locations` command</span></span>
* <span data-ttu-id="05b9c-1348">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="05b9c-1348">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-1349">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-1349">Appservice</span></span>

* <span data-ttu-id="05b9c-1350">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1350">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="05b9c-1351">CDN</span><span class="sxs-lookup"><span data-stu-id="05b9c-1351">CDN</span></span>

* <span data-ttu-id="05b9c-1352">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1352">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="05b9c-1353">Extensão</span><span class="sxs-lookup"><span data-stu-id="05b9c-1353">Extension</span></span>

* <span data-ttu-id="05b9c-1354">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="05b9c-1354">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="05b9c-1355">Keyvault</span><span class="sxs-lookup"><span data-stu-id="05b9c-1355">Keyvault</span></span>

* <span data-ttu-id="05b9c-1356">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1356">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-1357">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-1357">Network</span></span>

* <span data-ttu-id="05b9c-1358">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1358">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="05b9c-1359">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1359">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="05b9c-1360">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1360">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="05b9c-1361">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1361">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="05b9c-1362">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1362">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="05b9c-1363">Recurso</span><span class="sxs-lookup"><span data-stu-id="05b9c-1363">Resource</span></span>

* <span data-ttu-id="05b9c-1364">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1364">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="05b9c-1365">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1365">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="05b9c-1366">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="05b9c-1366">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="05b9c-1367">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="05b9c-1367">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="05b9c-1368">SQL</span><span class="sxs-lookup"><span data-stu-id="05b9c-1368">SQL</span></span>

* <span data-ttu-id="05b9c-1369">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1369">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-1370">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-1370">VM</span></span>

* <span data-ttu-id="05b9c-1371">Corrigido: Não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="05b9c-1371">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="05b9c-1372">Corrigido: Usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="05b9c-1372">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="05b9c-1373">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1373">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="05b9c-1374">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="05b9c-1374">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="05b9c-1375">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="05b9c-1375">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="05b9c-1376">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="05b9c-1376">August 31, 2017</span></span>

<span data-ttu-id="05b9c-1377">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="05b9c-1377">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="05b9c-1378">Keyvault</span><span class="sxs-lookup"><span data-stu-id="05b9c-1378">Keyvault</span></span>

* <span data-ttu-id="05b9c-1379">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1379">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="05b9c-1380">Sf</span><span class="sxs-lookup"><span data-stu-id="05b9c-1380">Sf</span></span>

* <span data-ttu-id="05b9c-1381">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1381">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-1382">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-1382">Storage</span></span>

* <span data-ttu-id="05b9c-1383">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="05b9c-1383">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="05b9c-1384">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="05b9c-1384">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="05b9c-1385">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="05b9c-1385">August 28, 2017</span></span>

<span data-ttu-id="05b9c-1386">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="05b9c-1386">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="05b9c-1387">CLI</span><span class="sxs-lookup"><span data-stu-id="05b9c-1387">CLI</span></span>

* <span data-ttu-id="05b9c-1388">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1388">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-1389">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-1389">ACS</span></span>

* <span data-ttu-id="05b9c-1390">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="05b9c-1390">Corrected preview regions</span></span>
* <span data-ttu-id="05b9c-1391">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1391">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="05b9c-1392">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="05b9c-1392">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-1393">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-1393">Appservice</span></span>

* <span data-ttu-id="05b9c-1394">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1394">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="05b9c-1395">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1395">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="05b9c-1396">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1396">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="05b9c-1397">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1397">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="05b9c-1398">Correção: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="05b9c-1398">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="05b9c-1399">IoT</span><span class="sxs-lookup"><span data-stu-id="05b9c-1399">IoT</span></span>

* <span data-ttu-id="05b9c-1400">Correção #3934: Criação de política não limpa as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="05b9c-1400">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-1401">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-1401">Network</span></span>

* <span data-ttu-id="05b9c-1402">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1402">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="05b9c-1403">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1403">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="05b9c-1404">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1404">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="05b9c-1405">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1405">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="05b9c-1406">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1406">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="05b9c-1407">Perfil</span><span class="sxs-lookup"><span data-stu-id="05b9c-1407">Profile</span></span>

* <span data-ttu-id="05b9c-1408">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="05b9c-1408">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="05b9c-1409">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="05b9c-1409">Service Fabric</span></span>

* <span data-ttu-id="05b9c-1410">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="05b9c-1410">Preview release</span></span>
* <span data-ttu-id="05b9c-1411">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="05b9c-1411">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="05b9c-1412">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="05b9c-1412">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="05b9c-1413">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="05b9c-1413">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-1414">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-1414">Storage</span></span>

* <span data-ttu-id="05b9c-1415">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="05b9c-1415">Enabled setting blob tier</span></span>
* <span data-ttu-id="05b9c-1416">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="05b9c-1416">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="05b9c-1417">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="05b9c-1417">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="05b9c-1418">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="05b9c-1418">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="05b9c-1419">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1419">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="05b9c-1420">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="05b9c-1420">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-1421">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-1421">VM</span></span>

* <span data-ttu-id="05b9c-1422">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1422">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="05b9c-1423">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="05b9c-1423">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="05b9c-1424">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1424">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="05b9c-1425">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="05b9c-1425">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="05b9c-1426">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="05b9c-1426">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="05b9c-1427">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1427">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="05b9c-1428">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="05b9c-1428">August 15, 2017</span></span>

<span data-ttu-id="05b9c-1429">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="05b9c-1429">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-1430">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-1430">ACS</span></span>

* <span data-ttu-id="05b9c-1431">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="05b9c-1431">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-1432">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-1432">Appservice</span></span>

* <span data-ttu-id="05b9c-1433">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="05b9c-1433">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="05b9c-1434">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="05b9c-1434">Event Grid</span></span>

* <span data-ttu-id="05b9c-1435">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="05b9c-1435">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="05b9c-1436">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="05b9c-1436">August 11, 2017</span></span>

<span data-ttu-id="05b9c-1437">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="05b9c-1437">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-1438">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-1438">ACS</span></span>

* <span data-ttu-id="05b9c-1439">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="05b9c-1439">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="05b9c-1440">Lote</span><span class="sxs-lookup"><span data-stu-id="05b9c-1440">Batch</span></span>

* <span data-ttu-id="05b9c-1441">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="05b9c-1441">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="05b9c-1442">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="05b9c-1442">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="05b9c-1443">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="05b9c-1443">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="05b9c-1444">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="05b9c-1444">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="05b9c-1445">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="05b9c-1445">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="05b9c-1446">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="05b9c-1446">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="05b9c-1447">Componente</span><span class="sxs-lookup"><span data-stu-id="05b9c-1447">Component</span></span>

* <span data-ttu-id="05b9c-1448">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="05b9c-1448">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="05b9c-1449">Contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-1449">Container</span></span>

* <span data-ttu-id="05b9c-1450">`create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="05b9c-1450">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="05b9c-1451">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="05b9c-1451">Data Lake Store</span></span>

* <span data-ttu-id="05b9c-1452">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-1452">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="05b9c-1453">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="05b9c-1453">Event Grid</span></span>

* <span data-ttu-id="05b9c-1454">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="05b9c-1454">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-1455">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-1455">Network</span></span>

* <span data-ttu-id="05b9c-1456">`lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="05b9c-1456">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="05b9c-1457">`application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="05b9c-1457">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="05b9c-1458">`application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="05b9c-1458">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="05b9c-1459">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1459">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="05b9c-1460">Perfil</span><span class="sxs-lookup"><span data-stu-id="05b9c-1460">Profile</span></span>

* <span data-ttu-id="05b9c-1461">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="05b9c-1461">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-1462">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-1462">Storage</span></span>

* <span data-ttu-id="05b9c-1463">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="05b9c-1463">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-1464">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-1464">VM</span></span>

* <span data-ttu-id="05b9c-1465">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="05b9c-1465">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="05b9c-1466">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1466">Exposed `list-skus` command</span></span>
* <span data-ttu-id="05b9c-1467">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="05b9c-1467">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="05b9c-1468">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="05b9c-1468">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="05b9c-1469">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="05b9c-1469">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="05b9c-1470">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="05b9c-1470">July 28, 2017</span></span>

<span data-ttu-id="05b9c-1471">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="05b9c-1471">Version 2.0.12</span></span>

* <span data-ttu-id="05b9c-1472">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-1472">Added container commands</span></span>
* <span data-ttu-id="05b9c-1473">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1473">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="05b9c-1474">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1474">Core</span></span>

* <span data-ttu-id="05b9c-1475">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="05b9c-1475">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="05b9c-1476">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="05b9c-1476">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="05b9c-1477">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="05b9c-1477">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="05b9c-1478">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1478">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="05b9c-1479">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="05b9c-1479">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="05b9c-1480">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1480">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="05b9c-1481">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1481">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="05b9c-1482">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1482">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="05b9c-1483">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1483">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="05b9c-1484">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="05b9c-1484">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="05b9c-1485">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="05b9c-1485">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="05b9c-1486">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1486">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="05b9c-1487">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="05b9c-1487">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="05b9c-1488">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="05b9c-1488">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="05b9c-1489">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="05b9c-1489">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="05b9c-1490">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1490">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="05b9c-1491">ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-1491">ACR</span></span>

* <span data-ttu-id="05b9c-1492">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="05b9c-1492">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="05b9c-1493">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="05b9c-1493">Support SKU update for managed registries</span></span>
* <span data-ttu-id="05b9c-1494">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="05b9c-1494">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="05b9c-1495">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-1495">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="05b9c-1496">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-1496">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="05b9c-1497">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="05b9c-1497">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-1498">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-1498">ACS</span></span>

* <span data-ttu-id="05b9c-1499">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="05b9c-1499">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-1500">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-1500">Appservice</span></span>

* <span data-ttu-id="05b9c-1501">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="05b9c-1501">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="05b9c-1502">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="05b9c-1502">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="05b9c-1503">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1503">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="05b9c-1504">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1504">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="05b9c-1505">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1505">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="05b9c-1506">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1506">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="05b9c-1507">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1507">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="05b9c-1508">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1508">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="05b9c-1509">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1509">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="05b9c-1510">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1510">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="05b9c-1511">Lote</span><span class="sxs-lookup"><span data-stu-id="05b9c-1511">Batch</span></span>

* <span data-ttu-id="05b9c-1512">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="05b9c-1512">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="05b9c-1513">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1513">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="05b9c-1514">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1514">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="05b9c-1515">CDN</span><span class="sxs-lookup"><span data-stu-id="05b9c-1515">CDN</span></span>

* <span data-ttu-id="05b9c-1516">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="05b9c-1516">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="05b9c-1517">Nuvem</span><span class="sxs-lookup"><span data-stu-id="05b9c-1517">Cloud</span></span>

* <span data-ttu-id="05b9c-1518">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="05b9c-1518">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="05b9c-1519">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="05b9c-1519">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="05b9c-1520">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="05b9c-1520">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="05b9c-1521">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="05b9c-1521">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="05b9c-1522">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1522">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="05b9c-1523">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="05b9c-1523">CosmosDB</span></span>

* <span data-ttu-id="05b9c-1524">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="05b9c-1524">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="05b9c-1525">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="05b9c-1525">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="05b9c-1526">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="05b9c-1526">Data Lake Analytics</span></span>

* <span data-ttu-id="05b9c-1527">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1527">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="05b9c-1528">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1528">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="05b9c-1529">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1529">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="05b9c-1530">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="05b9c-1530">Data Lake Store</span></span>

* <span data-ttu-id="05b9c-1531">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1531">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="05b9c-1532">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="05b9c-1532">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="05b9c-1533">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1533">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="05b9c-1534">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="05b9c-1534">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="05b9c-1535">Interativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1535">Interactive</span></span>

* <span data-ttu-id="05b9c-1536">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="05b9c-1536">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="05b9c-1537">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="05b9c-1537">Increased test coverage</span></span>
* <span data-ttu-id="05b9c-1538">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="05b9c-1538">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="05b9c-1539">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1539">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="05b9c-1540">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1540">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="05b9c-1541">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1541">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="05b9c-1542">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1542">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="05b9c-1543">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1543">Added `--progress` flag</span></span>
* <span data-ttu-id="05b9c-1544">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="05b9c-1544">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="05b9c-1545">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1545">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="05b9c-1546">IoT</span><span class="sxs-lookup"><span data-stu-id="05b9c-1546">IoT</span></span>

* <span data-ttu-id="05b9c-1547">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1547">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="05b9c-1548">(#3934)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1548">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="05b9c-1549">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="05b9c-1549">Key vault</span></span>

* <span data-ttu-id="05b9c-1550">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="05b9c-1550">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="05b9c-1551">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1551">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="05b9c-1552">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1552">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="05b9c-1553">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1553">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="05b9c-1554">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1554">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="05b9c-1555">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1555">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="05b9c-1556">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1556">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="05b9c-1557">(#3307)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1557">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="05b9c-1558">Laboratório</span><span class="sxs-lookup"><span data-stu-id="05b9c-1558">Lab</span></span>

* <span data-ttu-id="05b9c-1559">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1559">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="05b9c-1560">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1560">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="05b9c-1561">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="05b9c-1561">Monitor</span></span>

* <span data-ttu-id="05b9c-1562">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1562">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="05b9c-1563">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1563">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="05b9c-1564">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1564">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="05b9c-1565">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1565">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="05b9c-1566">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1566">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="05b9c-1567">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="05b9c-1567">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="05b9c-1568">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="05b9c-1568">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="05b9c-1569">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="05b9c-1569">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="05b9c-1570">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="05b9c-1570">`location` no longer required</span></span>
  * <span data-ttu-id="05b9c-1571">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="05b9c-1571">Add name and ID support for target</span></span>
  * <span data-ttu-id="05b9c-1572">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1572">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="05b9c-1573">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="05b9c-1573">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="05b9c-1574">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="05b9c-1574">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="05b9c-1575">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="05b9c-1575">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="05b9c-1576">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1576">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="05b9c-1577">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1577">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-1578">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-1578">Network</span></span>

* <span data-ttu-id="05b9c-1579">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1579">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="05b9c-1580">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1580">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="05b9c-1581">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="05b9c-1581">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="05b9c-1582">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="05b9c-1582">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="05b9c-1583">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1583">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="05b9c-1584">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1584">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="05b9c-1585">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1585">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="05b9c-1586">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1586">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="05b9c-1587">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1587">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="05b9c-1588">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1588">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="05b9c-1589">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1589">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="05b9c-1590">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1590">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="05b9c-1591">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1591">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="05b9c-1592">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1592">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="05b9c-1593">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1593">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="05b9c-1594">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1594">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="05b9c-1595">Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS</span><span class="sxs-lookup"><span data-stu-id="05b9c-1595">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="05b9c-1596">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1596">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="05b9c-1597">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1597">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="05b9c-1598">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1598">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="05b9c-1599">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1599">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="05b9c-1600">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1600">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="05b9c-1601">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1601">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="05b9c-1602">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="05b9c-1602">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="05b9c-1603">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="05b9c-1603">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="05b9c-1604">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="05b9c-1604">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="05b9c-1605">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="05b9c-1605">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="05b9c-1606">Perfil</span><span class="sxs-lookup"><span data-stu-id="05b9c-1606">Profile</span></span>

* <span data-ttu-id="05b9c-1607">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="05b9c-1607">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="05b9c-1608">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="05b9c-1608">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="05b9c-1609">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="05b9c-1609">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="05b9c-1610">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="05b9c-1610">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="05b9c-1611">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="05b9c-1611">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="05b9c-1612">RDBMS</span><span class="sxs-lookup"><span data-stu-id="05b9c-1612">RDBMS</span></span>

* <span data-ttu-id="05b9c-1613">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1613">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="05b9c-1614">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1614">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="05b9c-1615">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1615">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="05b9c-1616">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1616">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="05b9c-1617">Recurso</span><span class="sxs-lookup"><span data-stu-id="05b9c-1617">Resource</span></span>

* <span data-ttu-id="05b9c-1618">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1618">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="05b9c-1619">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1619">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="05b9c-1620">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1620">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="05b9c-1621">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1621">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="05b9c-1622">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1622">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="05b9c-1623">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1623">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="05b9c-1624">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1624">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="05b9c-1625">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1625">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="05b9c-1626">Função</span><span class="sxs-lookup"><span data-stu-id="05b9c-1626">Role</span></span>

* <span data-ttu-id="05b9c-1627">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1627">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="05b9c-1628">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1628">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="05b9c-1629">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1629">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="05b9c-1630">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1630">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="05b9c-1631">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1631">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="05b9c-1632">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="05b9c-1632">Service Fabric</span></span>
* <span data-ttu-id="05b9c-1633">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1633">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="05b9c-1634">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1634">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="05b9c-1635">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1635">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="05b9c-1636">SQL</span><span class="sxs-lookup"><span data-stu-id="05b9c-1636">SQL</span></span>

* <span data-ttu-id="05b9c-1637">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1637">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="05b9c-1638">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1638">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="05b9c-1639">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1639">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-1640">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-1640">Storage</span></span>

* <span data-ttu-id="05b9c-1641">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1641">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="05b9c-1642">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="05b9c-1642">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="05b9c-1643">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1643">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="05b9c-1644">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1644">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="05b9c-1645">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1645">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="05b9c-1646">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1646">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-1647">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-1647">VM</span></span>

* <span data-ttu-id="05b9c-1648">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="05b9c-1648">Support configuring nsg</span></span>
* <span data-ttu-id="05b9c-1649">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="05b9c-1649">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="05b9c-1650">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="05b9c-1650">Support managed service identities</span></span>
* <span data-ttu-id="05b9c-1651">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1651">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="05b9c-1652">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="05b9c-1652">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="05b9c-1653">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="05b9c-1653">May 10, 2017</span></span>

<span data-ttu-id="05b9c-1654">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="05b9c-1654">Version 2.0.6</span></span>

* <span data-ttu-id="05b9c-1655">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="05b9c-1655">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="05b9c-1656">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1656">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="05b9c-1657">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="05b9c-1657">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="05b9c-1658">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="05b9c-1658">Include Cognitive Services module</span></span>
* <span data-ttu-id="05b9c-1659">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="05b9c-1659">Include Service Fabric module</span></span>
* <span data-ttu-id="05b9c-1660">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1660">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="05b9c-1661">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="05b9c-1661">Add support for CDN commands</span></span>
* <span data-ttu-id="05b9c-1662">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="05b9c-1662">Remove Container module</span></span>
* <span data-ttu-id="05b9c-1663">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1663">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="05b9c-1664">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1664">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="05b9c-1665">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1665">Core</span></span>

* <span data-ttu-id="05b9c-1666">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="05b9c-1666">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="05b9c-1667">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1667">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="05b9c-1668">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1668">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="05b9c-1669">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1669">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="05b9c-1670">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1670">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="05b9c-1671">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1671">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="05b9c-1672">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1672">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="05b9c-1673">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1673">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="05b9c-1674">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1674">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="05b9c-1675">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="05b9c-1675">core: Improved performance</span></span>
* <span data-ttu-id="05b9c-1676">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="05b9c-1676">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="05b9c-1677">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="05b9c-1677">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-1678">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-1678">ACS</span></span>

* <span data-ttu-id="05b9c-1679">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05b9c-1679">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="05b9c-1680">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="05b9c-1680">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="05b9c-1681">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="05b9c-1681">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="05b9c-1682">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1682">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-1683">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-1683">AppService</span></span>

* <span data-ttu-id="05b9c-1684">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1684">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="05b9c-1685">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="05b9c-1685">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="05b9c-1686">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1686">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="05b9c-1687">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="05b9c-1687">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="05b9c-1688">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="05b9c-1688">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="05b9c-1689">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1689">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="05b9c-1690">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="05b9c-1690">support slot swap with preview</span></span>
* <span data-ttu-id="05b9c-1691">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1691">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="05b9c-1692">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1692">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="05b9c-1693">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="05b9c-1693">CosmosDB</span></span>

* <span data-ttu-id="05b9c-1694">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="05b9c-1694">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="05b9c-1695">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="05b9c-1695">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="05b9c-1696">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="05b9c-1696">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="05b9c-1697">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="05b9c-1697">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="05b9c-1698">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="05b9c-1698">Data Lake Analytics</span></span>

* <span data-ttu-id="05b9c-1699">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="05b9c-1699">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="05b9c-1700">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1700">Add support for new catalog item type: package.</span></span> <span data-ttu-id="05b9c-1701">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1701">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="05b9c-1702">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="05b9c-1702">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="05b9c-1703">Tabela</span><span class="sxs-lookup"><span data-stu-id="05b9c-1703">Table</span></span>
  * <span data-ttu-id="05b9c-1704">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="05b9c-1704">Table valued function</span></span>
  * <span data-ttu-id="05b9c-1705">Visualizar</span><span class="sxs-lookup"><span data-stu-id="05b9c-1705">View</span></span>
  * <span data-ttu-id="05b9c-1706">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1706">Table Statistics.</span></span> <span data-ttu-id="05b9c-1707">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="05b9c-1707">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="05b9c-1708">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="05b9c-1708">Data Lake Store</span></span>

* <span data-ttu-id="05b9c-1709">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="05b9c-1709">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="05b9c-1710">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1710">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="05b9c-1711">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1711">missed help for access show.</span></span> <span data-ttu-id="05b9c-1712">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1712">adding it.</span></span> <span data-ttu-id="05b9c-1713">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1713">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="05b9c-1714">Localizar</span><span class="sxs-lookup"><span data-stu-id="05b9c-1714">Find</span></span>

* <span data-ttu-id="05b9c-1715">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="05b9c-1715">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="05b9c-1716">KeyVault</span><span class="sxs-lookup"><span data-stu-id="05b9c-1716">KeyVault</span></span>

* <span data-ttu-id="05b9c-1717">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="05b9c-1717">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="05b9c-1718">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="05b9c-1718">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="05b9c-1719">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="05b9c-1719">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="05b9c-1720">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="05b9c-1720">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="05b9c-1721">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1721">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="05b9c-1722">Laboratório</span><span class="sxs-lookup"><span data-stu-id="05b9c-1722">Lab</span></span>

* <span data-ttu-id="05b9c-1723">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="05b9c-1723">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="05b9c-1724">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="05b9c-1724">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="05b9c-1725">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="05b9c-1725">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="05b9c-1726">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="05b9c-1726">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="05b9c-1727">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="05b9c-1727">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="05b9c-1728">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="05b9c-1728">Monitor</span></span>

* <span data-ttu-id="05b9c-1729">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1729">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="05b9c-1730">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1730">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="05b9c-1731">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-1731">Network</span></span>

* <span data-ttu-id="05b9c-1732">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1732">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="05b9c-1733">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1733">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="05b9c-1734">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1734">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="05b9c-1735">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1735">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="05b9c-1736">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="05b9c-1736">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="05b9c-1737">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="05b9c-1737">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="05b9c-1738">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="05b9c-1738">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="05b9c-1739">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="05b9c-1739">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="05b9c-1740">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1740">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="05b9c-1741">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="05b9c-1741">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="05b9c-1742">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1742">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="05b9c-1743">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1743">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="05b9c-1744">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="05b9c-1744">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="05b9c-1745">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="05b9c-1745">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="05b9c-1746">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="05b9c-1746">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="05b9c-1747">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="05b9c-1747">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="05b9c-1748">Perfil</span><span class="sxs-lookup"><span data-stu-id="05b9c-1748">Profile</span></span>

* <span data-ttu-id="05b9c-1749">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1749">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="05b9c-1750">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1750">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="05b9c-1751">Redis</span><span class="sxs-lookup"><span data-stu-id="05b9c-1751">Redis</span></span>

* <span data-ttu-id="05b9c-1752">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="05b9c-1752">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="05b9c-1753">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="05b9c-1753">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="05b9c-1754">Recurso</span><span class="sxs-lookup"><span data-stu-id="05b9c-1754">Resource</span></span>

* <span data-ttu-id="05b9c-1755">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1755">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="05b9c-1756">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1756">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="05b9c-1757">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1757">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="05b9c-1758">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1758">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="05b9c-1759">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1759">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="05b9c-1760">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1760">Add docs for az lock update.</span></span> <span data-ttu-id="05b9c-1761">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1761">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="05b9c-1762">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1762">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="05b9c-1763">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1763">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="05b9c-1764">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1764">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="05b9c-1765">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1765">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="05b9c-1766">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1766">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="05b9c-1767">Função</span><span class="sxs-lookup"><span data-stu-id="05b9c-1767">Role</span></span>

* <span data-ttu-id="05b9c-1768">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1768">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="05b9c-1769">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1769">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="05b9c-1770">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1770">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="05b9c-1771">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="05b9c-1771">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="05b9c-1772">SQL</span><span class="sxs-lookup"><span data-stu-id="05b9c-1772">SQL</span></span>

* <span data-ttu-id="05b9c-1773">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="05b9c-1773">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="05b9c-1774">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1774">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="05b9c-1775">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-1775">Storage</span></span>

* <span data-ttu-id="05b9c-1776">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1776">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="05b9c-1777">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="05b9c-1777">Add support for incremental blob copy</span></span>
* <span data-ttu-id="05b9c-1778">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="05b9c-1778">Add support for large block blob upload</span></span>
* <span data-ttu-id="05b9c-1779">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="05b9c-1779">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-1780">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-1780">VM</span></span>

* <span data-ttu-id="05b9c-1781">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="05b9c-1781">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="05b9c-1782">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="05b9c-1782">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="05b9c-1783">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="05b9c-1783">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="05b9c-1784">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="05b9c-1784">az vm/vmss disk</span></span>
  3. <span data-ttu-id="05b9c-1785">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="05b9c-1785">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="05b9c-1786">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="05b9c-1786">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="05b9c-1787">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1787">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="05b9c-1788">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="05b9c-1788">April 3, 2017</span></span>

<span data-ttu-id="05b9c-1789">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="05b9c-1789">Version 2.0.2</span></span>

<span data-ttu-id="05b9c-1790">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="05b9c-1790">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="05b9c-1791">Núcleo</span><span class="sxs-lookup"><span data-stu-id="05b9c-1791">Core</span></span>

* <span data-ttu-id="05b9c-1792">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="05b9c-1792">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="05b9c-1793">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1793">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="05b9c-1794">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1794">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="05b9c-1795">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1795">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="05b9c-1796">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1796">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="05b9c-1797">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1797">Add prompting for missing template parameters.</span></span> <span data-ttu-id="05b9c-1798">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1798">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="05b9c-1799">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="05b9c-1799">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="05b9c-1800">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="05b9c-1800">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="05b9c-1801">ACS</span><span class="sxs-lookup"><span data-stu-id="05b9c-1801">ACS</span></span>

* <span data-ttu-id="05b9c-1802">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1802">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="05b9c-1803">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1803">Add support for ssh key password prompting.</span></span> <span data-ttu-id="05b9c-1804">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1804">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="05b9c-1805">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1805">Add support for windows clusters.</span></span> <span data-ttu-id="05b9c-1806">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1806">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="05b9c-1807">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="05b9c-1807">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="05b9c-1808">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1808">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="05b9c-1809">AppService</span><span class="sxs-lookup"><span data-stu-id="05b9c-1809">AppService</span></span>

* <span data-ttu-id="05b9c-1810">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1810">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="05b9c-1811">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1811">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="05b9c-1812">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1812">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="05b9c-1813">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1813">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="05b9c-1814">DataLake</span><span class="sxs-lookup"><span data-stu-id="05b9c-1814">DataLake</span></span>

* <span data-ttu-id="05b9c-1815">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="05b9c-1815">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="05b9c-1816">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="05b9c-1816">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="05b9c-1817">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="05b9c-1817">DocuemntDB</span></span>

* <span data-ttu-id="05b9c-1818">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1818">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="05b9c-1819">VM</span><span class="sxs-lookup"><span data-stu-id="05b9c-1819">VM</span></span>

* <span data-ttu-id="05b9c-1820">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1820">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="05b9c-1821">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1821">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="05b9c-1822">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1822">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="05b9c-1823">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1823">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="05b9c-1824">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1824">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="05b9c-1825">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1825">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="05b9c-1826">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="05b9c-1826">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="05b9c-1827">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="05b9c-1827">February 27, 2017</span></span>

<span data-ttu-id="05b9c-1828">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="05b9c-1828">Version 2.0.0</span></span>

<span data-ttu-id="05b9c-1829">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="05b9c-1829">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="05b9c-1830">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1830">Container Service (acs)</span></span>
- <span data-ttu-id="05b9c-1831">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1831">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="05b9c-1832">Rede</span><span class="sxs-lookup"><span data-stu-id="05b9c-1832">Networking</span></span>
- <span data-ttu-id="05b9c-1833">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="05b9c-1833">Storage</span></span>

<span data-ttu-id="05b9c-1834">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1834">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="05b9c-1835">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="05b9c-1835">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="05b9c-1836">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="05b9c-1836">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="05b9c-1837">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="05b9c-1837">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="05b9c-1838">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1838">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="05b9c-1839">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="05b9c-1839">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="05b9c-1840">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1840">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="05b9c-1841">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="05b9c-1841">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="05b9c-1842">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="05b9c-1842">Provide feedback from the command line with the `az feedback` command</span></span>

