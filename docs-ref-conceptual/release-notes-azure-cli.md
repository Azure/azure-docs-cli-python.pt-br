---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/15/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 1c6b2cc57b80256faff0a174bec5f13bd84f5a1b
ms.sourcegitcommit: 7f79860c799e78fd8a591d7a5550464080e07aa9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "56157986"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="4b722-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="4b722-103">Azure CLI release notes</span></span>
## <a name="february-12-2019"></a><span data-ttu-id="4b722-104">12 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="4b722-104">February 12, 2019</span></span>

<span data-ttu-id="4b722-105">Versão 2.0.58</span><span class="sxs-lookup"><span data-stu-id="4b722-105">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="4b722-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-106">Core</span></span>

* <span data-ttu-id="4b722-107">`az --version` agora exibe uma notificação se você tiver pacotes para atualização</span><span class="sxs-lookup"><span data-stu-id="4b722-107">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="4b722-108">A regressão em que `--ids` não pode ser usado com a saída JSON foi corrigida</span><span class="sxs-lookup"><span data-stu-id="4b722-108">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-109">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-109">ACR</span></span>
* <span data-ttu-id="4b722-110">[ALTERAÇÃO SIGNIFICATIVA] O grupo de comandos `acr build-task` foi removido</span><span class="sxs-lookup"><span data-stu-id="4b722-110">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="4b722-111">[ALTERAÇÃO SIGNIFICATIVA] As opções `--tag` e `--manifest` de `acr repository delete` foram removidas</span><span class="sxs-lookup"><span data-stu-id="4b722-111">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-112">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-112">ACS</span></span>
* <span data-ttu-id="4b722-113">Suporte adicionado a `aks [enable-addons|disable-addons]` para nomes que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="4b722-113">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="4b722-114">Suporte adicionado para a operação de atualização do Azure Active Directory usando `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="4b722-114">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="4b722-115">Um esclarecimento informando que `--output` é ignorado para `aks get-credentials` foi adicionado</span><span class="sxs-lookup"><span data-stu-id="4b722-115">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="4b722-116">AMS</span><span class="sxs-lookup"><span data-stu-id="4b722-116">AMS</span></span>
* <span data-ttu-id="4b722-117">Adicionados os comandos `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="4b722-117">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="4b722-118">Adicionados os comandos `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="4b722-118">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-119">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-119">Appservice</span></span>
* <span data-ttu-id="4b722-120">Foi adicionada a capacidade de criar e configurar funções usando contêineres de ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-120">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="4b722-121">Suporte adicionado para a atualização das configurações de aplicativos Web por meio de JSON</span><span class="sxs-lookup"><span data-stu-id="4b722-121">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="4b722-122">A ajuda foi aprimorada para `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="4b722-122">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="4b722-123">Suporte adicionado para o App Insights para auxiliar na criação de aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="4b722-123">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="4b722-124">Os problemas com o SSH do aplicativo Web foram corrigidos</span><span class="sxs-lookup"><span data-stu-id="4b722-124">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="4b722-125">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="4b722-125">Botservice</span></span>
* <span data-ttu-id="4b722-126">A experiência do usuário para `bot publish` foi aprimorada</span><span class="sxs-lookup"><span data-stu-id="4b722-126">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="4b722-127">Foram adicionados avisos de tempos limite ao executar `npm install` durante `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="4b722-127">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="4b722-128">O caractere inválido `.` de `--name` em `az bot create` foi removido</span><span class="sxs-lookup"><span data-stu-id="4b722-128">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="4b722-129">Alteração para interromper a geração aleatória de nomes de recursos durante a criação do Armazenamento do Azure, Plano do Serviço de Aplicativo, Aplicativo Web/de funções e Application Insights</span><span class="sxs-lookup"><span data-stu-id="4b722-129">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="4b722-130">[PRETERIDO] O argumento `--proj-name` em favor de `--proj-file-path` foi preterido</span><span class="sxs-lookup"><span data-stu-id="4b722-130">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="4b722-131">`az bot publish` foi alterado para remover arquivos de implantação do Node.js do IIS buscados, caso eles já não existissem</span><span class="sxs-lookup"><span data-stu-id="4b722-131">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="4b722-132">Foi adicionado o argumento `--keep-node-modules` para `az bot publish` para não excluir a pasta `node_modules` no Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b722-132">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="4b722-133">O par chave-valor `"publishCommand"` foi adicionado à saída de `az bot create` durante a criação de uma função do Azure ou bot de aplicativo Web</span><span class="sxs-lookup"><span data-stu-id="4b722-133">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="4b722-134">O valor de `"publishCommand"` é um comando `az bot publish` que é automaticamente preenchido com os parâmetros necessários para publicar o bot recém-criado</span><span class="sxs-lookup"><span data-stu-id="4b722-134">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="4b722-135">O `"WEBSITE_NODE_DEFAULT_VERSION"` foi atualizado no modelo do ARM para que os bots de SDK v4 usem 10.14.1 em vez de 8.9.4</span><span class="sxs-lookup"><span data-stu-id="4b722-135">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="4b722-136">Key Vault</span><span class="sxs-lookup"><span data-stu-id="4b722-136">Key Vault</span></span>
* <span data-ttu-id="4b722-137">Foi corrigido o problema com `keyvault secret backup`, em que alguns usuários recebiam um erro `unexpected_keyword` ao usar `--id`</span><span class="sxs-lookup"><span data-stu-id="4b722-137">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="4b722-138">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="4b722-138">Monitor</span></span>
* <span data-ttu-id="4b722-139">`monitor metrics alert [create|update]` foi alterado para permitir o valor dimensional `*`</span><span class="sxs-lookup"><span data-stu-id="4b722-139">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="4b722-140">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-140">Network</span></span>
* <span data-ttu-id="4b722-141">`dns zone export` foi alterado para garantir que CNAMEs exportados fossem FQDNs</span><span class="sxs-lookup"><span data-stu-id="4b722-141">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="4b722-142">O parâmetro `--gateway-name` foi adicionado a `nic ip-config address-pool [add|remove]` para dar suporte a pools de endereços de back-end de gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b722-142">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="4b722-143">Os argumentos `--traffic-analytics` e `--workspace` foram adicionados a `network watcher flow-log configure` para dar suporte à análise de tráfego por meio de um workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="4b722-143">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="4b722-144">`--idle-timeout` e `--floating-ip` foram adicionados a `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-144">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="4b722-145">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="4b722-145">Policy Insights</span></span>
* <span data-ttu-id="4b722-146">Os comandos `policy remediation` foram adicionados para dar suporte a recursos de correção de política de recursos</span><span class="sxs-lookup"><span data-stu-id="4b722-146">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="4b722-147">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4b722-147">RDBMS</span></span>
* <span data-ttu-id="4b722-148">A mensagem e os parâmetros de comando de ajuda foram aprimorados</span><span class="sxs-lookup"><span data-stu-id="4b722-148">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="4b722-149">Redis</span><span class="sxs-lookup"><span data-stu-id="4b722-149">Redis</span></span>
* <span data-ttu-id="4b722-150">Foram adicionados comandos para gerenciar regras de firewall (criar, atualizar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="4b722-150">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="4b722-151">Foram adicionados comandos para gerenciar links do servidor (criar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="4b722-151">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="4b722-152">Foram adicionados comandos para gerenciar o agendamento de patches (criar, atualizar, excluir, mostrar)</span><span class="sxs-lookup"><span data-stu-id="4b722-152">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="4b722-153">Suporte adicionado para Zonas de Disponibilidade e versão mínima de TLS para criar Redis</span><span class="sxs-lookup"><span data-stu-id="4b722-153">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="4b722-154">[ALTERAÇÃO SIGNIFICATIVA] Os comandos `redis update-settings` e `redis list-all` foram removidos</span><span class="sxs-lookup"><span data-stu-id="4b722-154">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="4b722-155">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro para `redis create`: “configurações de locatário” não é aceito no formato chave[=valor]</span><span class="sxs-lookup"><span data-stu-id="4b722-155">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="4b722-156">[PRETERIDO] Uma mensagem de aviso foi adicionada para preterir o comando `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="4b722-156">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="4b722-157">Função</span><span class="sxs-lookup"><span data-stu-id="4b722-157">Role</span></span>
* <span data-ttu-id="4b722-158">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido dos comandos `vm` para esta localização</span><span class="sxs-lookup"><span data-stu-id="4b722-158">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="4b722-159">SQL VM</span><span class="sxs-lookup"><span data-stu-id="4b722-159">SQL VM</span></span>
* <span data-ttu-id="4b722-160">[PRETERIDO] O argumento `--boostrap-acc-pwd` foi preterido devido a um erro de digitação</span><span class="sxs-lookup"><span data-stu-id="4b722-160">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-161">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-161">VM</span></span>
* <span data-ttu-id="4b722-162">`vm list-skus` foi alterado para permitir o uso de `--all` no lugar de `--all true`</span><span class="sxs-lookup"><span data-stu-id="4b722-162">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="4b722-163">Adicionado `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="4b722-163">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="4b722-164">Foi corrigido o bug em que `vmss encryption enable` falhava se fosse executado anteriormente</span><span class="sxs-lookup"><span data-stu-id="4b722-164">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="4b722-165">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido para os comandos `role`</span><span class="sxs-lookup"><span data-stu-id="4b722-165">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="4b722-166">31 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="4b722-166">January 31, 2019</span></span>

<span data-ttu-id="4b722-167">Versão 2.0.57</span><span class="sxs-lookup"><span data-stu-id="4b722-167">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="4b722-168">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-168">Core</span></span>

* <span data-ttu-id="4b722-169">Hotfix para o [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="4b722-169">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="4b722-170">28 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="4b722-170">January 28, 2019</span></span>

<span data-ttu-id="4b722-171">Versão 2.0.56</span><span class="sxs-lookup"><span data-stu-id="4b722-171">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-172">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-172">ACR</span></span>
* <span data-ttu-id="4b722-173">Suporte adicionado para regras de rede virtual/IP</span><span class="sxs-lookup"><span data-stu-id="4b722-173">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-174">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-174">ACS</span></span>
* <span data-ttu-id="4b722-175">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="4b722-175">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="4b722-176">Comandos do OpenShift gerenciado foram adicionados</span><span class="sxs-lookup"><span data-stu-id="4b722-176">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="4b722-177">Suporte adicionado para operações de atualização da entidade de serviço com `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="4b722-177">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="4b722-178">AMS</span><span class="sxs-lookup"><span data-stu-id="4b722-178">AMS</span></span>
* <span data-ttu-id="4b722-179">[ALTERAÇÃO SIGNIFICATIVA] `ams asset get-streaming-locators` renomeado para `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="4b722-179">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="4b722-180">[ALTERAÇÃO SIGNIFICATIVA] `ams streaming-locator get-content-keys` renomeado para `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="4b722-180">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-181">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-181">Appservice</span></span>
* <span data-ttu-id="4b722-182">Suporte adicionado para o App Insights no `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="4b722-182">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="4b722-183">Suporte adicionado para a criação do plano de serviço de aplicativo (incluindo Elástico Premium) para Aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="4b722-183">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="4b722-184">Foram corrigidos os problemas com de configuração de aplicativo com os planos Elástico Premium</span><span class="sxs-lookup"><span data-stu-id="4b722-184">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="4b722-185">Contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-185">Container</span></span>
* <span data-ttu-id="4b722-186">Adicionado o comando `container start`</span><span class="sxs-lookup"><span data-stu-id="4b722-186">Added `container start` command</span></span>
* <span data-ttu-id="4b722-187">Alteração para permitir o uso de valores decimais para CPU durante a criação do contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-187">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="4b722-188">EventGrid</span><span class="sxs-lookup"><span data-stu-id="4b722-188">EventGrid</span></span>
* <span data-ttu-id="4b722-189">Parâmetro `--deadletter-endpoint` adicionado a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-189">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="4b722-190">Storagequeue e hybridconnection foram adicionados como novos valores para 'event-subscription [create|update] --endpoint-type\`</span><span class="sxs-lookup"><span data-stu-id="4b722-190">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="4b722-191">Os parâmetros `--max-delivery-attempts` e `--event-ttl` foram adicionados a `event-subscription create` para especificar a política de repetição para eventos</span><span class="sxs-lookup"><span data-stu-id="4b722-191">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="4b722-192">Uma mensagem de aviso foi adicionada a `event-subscription [create|update]` quando o webhook como destino for usado para uma assinatura de evento</span><span class="sxs-lookup"><span data-stu-id="4b722-192">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="4b722-193">O parâmetro source-resource-id foi adicionado para todos os comandos relacionados a eventos e marcar todos os outros parâmetros relacionados ao recurso de origem como preteridos</span><span class="sxs-lookup"><span data-stu-id="4b722-193">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4b722-194">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4b722-194">HDInsight</span></span>
* <span data-ttu-id="4b722-195">[ALTERAÇÃO SIGNIFICATIVA] Os parâmetros `--virtual-network` e `--subnet-name` de `hdinsight [application] create` foram removidos</span><span class="sxs-lookup"><span data-stu-id="4b722-195">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="4b722-196">[ALTERAÇÃO SIGNIFICATIVA] `hdinsight create --storage-account` foi alterado para aceitar o nome ou ID da conta de armazenamento, em vez de pontos de extremidade de blob</span><span class="sxs-lookup"><span data-stu-id="4b722-196">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="4b722-197">Parâmetros `--vnet-name` e `--subnet-name` adicionados a `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="4b722-197">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="4b722-198">Suporte adicionado para a criptografia de disco e Enterprise Security Package ao `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="4b722-198">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="4b722-199">Adicionado o comando `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="4b722-199">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="4b722-200">Adicionado o comando `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="4b722-200">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="4b722-201">IoT</span><span class="sxs-lookup"><span data-stu-id="4b722-201">IoT</span></span>
* <span data-ttu-id="4b722-202">O formato de codificação foi adicionado ao comando routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="4b722-202">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="4b722-203">Kusto</span><span class="sxs-lookup"><span data-stu-id="4b722-203">Kusto</span></span>
* <span data-ttu-id="4b722-204">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="4b722-204">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="4b722-205">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="4b722-205">Monitor</span></span>
* <span data-ttu-id="4b722-206">A comparação de ID foi alterada para diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="4b722-206">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="4b722-207">Perfil</span><span class="sxs-lookup"><span data-stu-id="4b722-207">Profile</span></span>
* <span data-ttu-id="4b722-208">A conta de nível de locatário foi habilitada para a identidade de serviço gerenciada de `login`</span><span class="sxs-lookup"><span data-stu-id="4b722-208">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="4b722-209">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-209">Network</span></span>
* <span data-ttu-id="4b722-210">Foi corrigido o problema com `express-route update`: em que o argumento `--bandwidth` era ignorado</span><span class="sxs-lookup"><span data-stu-id="4b722-210">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="4b722-211">Foi corrigido o problema com `ddos-protection update` em que definir a compreensão levava ao rastreamento de pilha</span><span class="sxs-lookup"><span data-stu-id="4b722-211">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="4b722-212">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-212">Resource</span></span>
* <span data-ttu-id="4b722-213">Suporte adicionado para o arquivo de parâmetros de URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="4b722-213">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="4b722-214">Suporte adicionado para a identidade gerenciada à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="4b722-214">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="4b722-215">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="4b722-215">SQL Virtual Machine</span></span>
* <span data-ttu-id="4b722-216">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="4b722-216">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-217">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-217">Storage</span></span>
* <span data-ttu-id="4b722-218">Alteração na correção para atualizar apenas as propriedades que são alteradas no mesmo objeto</span><span class="sxs-lookup"><span data-stu-id="4b722-218">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="4b722-219">#8021 foi corrigido, dados binários são codificados em base 64 quando retornados</span><span class="sxs-lookup"><span data-stu-id="4b722-219">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-220">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-220">VM</span></span>
* <span data-ttu-id="4b722-221">Alteração de `vm encryption enable` para validar o cofre de chaves de criptografia de disco e se esse cofre de chaves de criptografia de chave existe</span><span class="sxs-lookup"><span data-stu-id="4b722-221">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="4b722-222">O sinalizador `--force` foi adicionado a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="4b722-222">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="4b722-223">15 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="4b722-223">January 15, 2019</span></span>

<span data-ttu-id="4b722-224">Versão 2.0.55</span><span class="sxs-lookup"><span data-stu-id="4b722-224">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-225">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-225">ACR</span></span>
* <span data-ttu-id="4b722-226">Alteração para permitir forçar o envio por push de um gráfico Helm que não existe</span><span class="sxs-lookup"><span data-stu-id="4b722-226">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="4b722-227">Alteração para permitir operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="4b722-227">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="4b722-228">[PRETERIDO] O parâmetro `--resource-group` foi preterido nos comandos:</span><span class="sxs-lookup"><span data-stu-id="4b722-228">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="4b722-229">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-229">ACS</span></span>
* <span data-ttu-id="4b722-230">Suporte adicionado para novas regiões ACI</span><span class="sxs-lookup"><span data-stu-id="4b722-230">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-231">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-231">Appservice</span></span>
* <span data-ttu-id="4b722-232">Foi corrigido o problema com o carregamento de certificados para aplicativos que são hospedados em um ASE, em que o RG do ASE e o RG do aplicativo são diferentes</span><span class="sxs-lookup"><span data-stu-id="4b722-232">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="4b722-233">Alteração de `webapp up` para usar a SKU P1V1 como padrão para Linux</span><span class="sxs-lookup"><span data-stu-id="4b722-233">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="4b722-234">`[webapp|functionapp] deployment source config-zip` foi corrigido para mostrar a mensagem de erro adequada quando uma implantação falhar</span><span class="sxs-lookup"><span data-stu-id="4b722-234">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="4b722-235">Adicionado o comando `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="4b722-235">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="4b722-236">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="4b722-236">Botservice</span></span>
* <span data-ttu-id="4b722-237">Atualizações de status de implantação foram adicionadas a `bot create`</span><span class="sxs-lookup"><span data-stu-id="4b722-237">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="4b722-238">Configurar</span><span class="sxs-lookup"><span data-stu-id="4b722-238">Configure</span></span>
* <span data-ttu-id="4b722-239">`none` foi adicionado como um formato de saída configurável</span><span class="sxs-lookup"><span data-stu-id="4b722-239">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4b722-240">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4b722-240">CosmosDB</span></span>
* <span data-ttu-id="4b722-241">Suporte adicionado para criar o banco de dados com taxa de transferência compartilhada</span><span class="sxs-lookup"><span data-stu-id="4b722-241">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4b722-242">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4b722-242">HDInsight</span></span>
* <span data-ttu-id="4b722-243">Foram adicionados comandos para o gerenciamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="4b722-243">Added commands for managing applications</span></span>
* <span data-ttu-id="4b722-244">Foram adicionados comandos para o gerenciamento de ações de script</span><span class="sxs-lookup"><span data-stu-id="4b722-244">Added commands for managing script actions</span></span>
* <span data-ttu-id="4b722-245">Foram adicionados comandos para o gerenciamento do Operations Management Suite (OMS)</span><span class="sxs-lookup"><span data-stu-id="4b722-245">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="4b722-246">Suporte adicionado para listar a utilização regional ao `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="4b722-246">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="4b722-247">[ALTERAÇÃO SIGNIFICATIVA] O tipo de cluster padrão de `hdinsight create` foi removido</span><span class="sxs-lookup"><span data-stu-id="4b722-247">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="4b722-248">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-248">Network</span></span>
* <span data-ttu-id="4b722-249">Adicionados os argumentos `--custom-headers` e `--status-code-ranges` para `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-249">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="4b722-250">Novos tipos de roteamento foram adicionados: Subrede e múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="4b722-250">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="4b722-251">Adicionados os argumentos `--custom-headers` e `--subnets` para `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-251">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="4b722-252">Foi corrigido o problema no qual fornecer `--vnets ""` a `ddos-protection update` causava um erro</span><span class="sxs-lookup"><span data-stu-id="4b722-252">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="4b722-253">Função</span><span class="sxs-lookup"><span data-stu-id="4b722-253">Role</span></span>
* <span data-ttu-id="4b722-254">[PRETERIDO] O argumento `--password` para `create-for-rbac` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="4b722-254">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="4b722-255">Como alternativa, use senhas seguras geradas pela CLI</span><span class="sxs-lookup"><span data-stu-id="4b722-255">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="4b722-256">Segurança</span><span class="sxs-lookup"><span data-stu-id="4b722-256">Security</span></span>
* <span data-ttu-id="4b722-257">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="4b722-257">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-258">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-258">Storage</span></span>
* <span data-ttu-id="4b722-259">[ALTERAÇÃO SIGNIFICATIVA] O número padrão de resultados de `storage [blob|file|container|share] list` foi alterado para 5.000.</span><span class="sxs-lookup"><span data-stu-id="4b722-259">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="4b722-260">Use `--num-results *` para o comportamento original de retornar todos os resultados</span><span class="sxs-lookup"><span data-stu-id="4b722-260">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="4b722-261">Parâmetro `--marker` adicionado a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="4b722-261">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="4b722-262">Um marcador de log foi adicionado para a próxima página ao STDERR de `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="4b722-262">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="4b722-263">O comando `storage blob service-properties update` foi adicionado com suporte para sites estáticos</span><span class="sxs-lookup"><span data-stu-id="4b722-263">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-264">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-264">VM</span></span>
* <span data-ttu-id="4b722-265">`vm [disk|unmanaged-disk]` e `vmss disk` foram alterados para que tenham parâmetros mais consistentes</span><span class="sxs-lookup"><span data-stu-id="4b722-265">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="4b722-266">Suporte adicionado para referência cruzada de imagem de locatário a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="4b722-266">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="4b722-267">O bug de configuração padrão foi corrigido em `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="4b722-267">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="4b722-268">O argumento `--provision-after-extensions` foi adicionado a `vmss extension set` para definir quais extensões deverão ser provisionadas antes da extensão ser definida</span><span class="sxs-lookup"><span data-stu-id="4b722-268">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="4b722-269">O argumento `--replica-count` foi adicionado a `sig image-version update` para definir a contagem de replicação padrão</span><span class="sxs-lookup"><span data-stu-id="4b722-269">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="4b722-270">Foi corrigido o bug com `image create --source` em que o disco do sistema operacional de origem era confundido com uma VM do mesmo nome, mesmo se a ID de recurso completa fosse fornecida</span><span class="sxs-lookup"><span data-stu-id="4b722-270">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="4b722-271">20 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-271">December 20, 2018</span></span>

<span data-ttu-id="4b722-272">Versão 2.0.54</span><span class="sxs-lookup"><span data-stu-id="4b722-272">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="4b722-273">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-273">Appservice</span></span>
* <span data-ttu-id="4b722-274">Corrigido o problema que causava falha na reimplantação do `webapp up`</span><span class="sxs-lookup"><span data-stu-id="4b722-274">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="4b722-275">Adicionado suporte para listar e restaurar instantâneos de aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="4b722-275">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="4b722-276">Adicionado suporte para o sinalizador `--runtime` para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="4b722-276">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="4b722-277">IoT Central</span><span class="sxs-lookup"><span data-stu-id="4b722-277">IoTCentral</span></span>
* <span data-ttu-id="4b722-278">Corrigida a chamada à API do comando de atualização</span><span class="sxs-lookup"><span data-stu-id="4b722-278">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="4b722-279">Função</span><span class="sxs-lookup"><span data-stu-id="4b722-279">Role</span></span>
* <span data-ttu-id="4b722-280">[ALTERAÇÃO SIGNIFICATIVA] `ad [app|sp] list` alterado para listar somente os 100 primeiros objetos por padrão</span><span class="sxs-lookup"><span data-stu-id="4b722-280">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="4b722-281">SQL</span><span class="sxs-lookup"><span data-stu-id="4b722-281">SQL</span></span>
* <span data-ttu-id="4b722-282">Adicionado suporte para ordenação personalizada nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="4b722-282">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-283">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-283">VM</span></span>
* <span data-ttu-id="4b722-284">Parâmetro `---os-type` adicionado a `disk create`</span><span class="sxs-lookup"><span data-stu-id="4b722-284">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="4b722-285">18 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-285">December 18, 2018</span></span>

<span data-ttu-id="4b722-286">Versão 2.0.53</span><span class="sxs-lookup"><span data-stu-id="4b722-286">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="4b722-287">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-287">ACR</span></span>
* <span data-ttu-id="4b722-288">Adicionado suporte para importação de imagem de Registros de Contêiner externos</span><span class="sxs-lookup"><span data-stu-id="4b722-288">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="4b722-289">Simplificado o layout da tabela para a lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="4b722-289">Condensed the table layout for task list</span></span>
* <span data-ttu-id="4b722-290">Adicionado suporte para URLs do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="4b722-290">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-291">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-291">ACS</span></span>
* <span data-ttu-id="4b722-292">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="4b722-292">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="4b722-293">Removido “(VISUALIZAÇÃO)” de argumentos do AAD para `aks create`</span><span class="sxs-lookup"><span data-stu-id="4b722-293">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="4b722-294">[PRETERIDO] Comandos `az acs` preteridos.</span><span class="sxs-lookup"><span data-stu-id="4b722-294">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="4b722-295">O serviço ACS será desativado em 31 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="4b722-295">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="4b722-296">Adicionado suporte da Política de Rede durante a criação de novos clusters AKS</span><span class="sxs-lookup"><span data-stu-id="4b722-296">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="4b722-297">Removido o requisito do argumento `--nodepool-name` para `aks scale` se houver apenas um pool de nós</span><span class="sxs-lookup"><span data-stu-id="4b722-297">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-298">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-298">Appservice</span></span>
* <span data-ttu-id="4b722-299">Corrigido o problema em que `webapp config container` não honra o parâmetro `--slot`</span><span class="sxs-lookup"><span data-stu-id="4b722-299">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="4b722-300">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="4b722-300">Botservice</span></span>
* <span data-ttu-id="4b722-301">Suporte adicionado para análise do arquivo `.bot` ao chamar `bot show`</span><span class="sxs-lookup"><span data-stu-id="4b722-301">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="4b722-302">Corrigido o bug de provisionamento do AppInsights</span><span class="sxs-lookup"><span data-stu-id="4b722-302">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="4b722-303">Corrigido o bug de espaço em branco ao lidar com caminhos de arquivo</span><span class="sxs-lookup"><span data-stu-id="4b722-303">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="4b722-304">Reduzidas as chamadas de rede do Kudu</span><span class="sxs-lookup"><span data-stu-id="4b722-304">Reduced Kudu network calls</span></span>
* <span data-ttu-id="4b722-305">Melhorias de UX para comandos gerais</span><span class="sxs-lookup"><span data-stu-id="4b722-305">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="4b722-306">Consumo</span><span class="sxs-lookup"><span data-stu-id="4b722-306">Consumption</span></span>
* <span data-ttu-id="4b722-307">Corrigidos os bugs da API de orçamento ao mostrar notificações</span><span class="sxs-lookup"><span data-stu-id="4b722-307">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4b722-308">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4b722-308">CosmosDB</span></span>
* <span data-ttu-id="4b722-309">Suporte adicionado para atualizar a conta de vários mestres para mestre único</span><span class="sxs-lookup"><span data-stu-id="4b722-309">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="4b722-310">Mapas</span><span class="sxs-lookup"><span data-stu-id="4b722-310">Maps</span></span>
* <span data-ttu-id="4b722-311">Adicionado suporte ao SKU S1 para `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-311">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="4b722-312">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-312">Network</span></span>
* <span data-ttu-id="4b722-313">Adicionado suporte para `--format` e `--log-version` para `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="4b722-313">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="4b722-314">Corrigido o problema com `dns zone update` em que usar "" para limpar a resolução e o registro de redes virtuais não funcionava</span><span class="sxs-lookup"><span data-stu-id="4b722-314">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="4b722-315">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-315">Resource</span></span>
* <span data-ttu-id="4b722-316">Corrigido o tratamento do parâmetro de escopo para grupos de gerenciamento do `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-316">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="4b722-317">Adicionado o novo comando `resource wait`</span><span class="sxs-lookup"><span data-stu-id="4b722-317">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-318">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-318">Storage</span></span>
*  <span data-ttu-id="4b722-319">Adicionada a capacidade de atualizar a versão do esquema de log para serviços de armazenamento no `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="4b722-319">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-320">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-320">VM</span></span>
* <span data-ttu-id="4b722-321">Corrigida a falha em `vm identity remove` quando a VM especificada não tem nenhuma identidade de serviço gerenciado atribuída</span><span class="sxs-lookup"><span data-stu-id="4b722-321">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="4b722-322">4 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-322">December 4, 2018</span></span>

<span data-ttu-id="4b722-323">Versão 2.0.52</span><span class="sxs-lookup"><span data-stu-id="4b722-323">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="4b722-324">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-324">Core</span></span>
* <span data-ttu-id="4b722-325">Adicionado suporte para provisionamento de recursos de locatários cruzados para a entidade de serviço de multilocatários</span><span class="sxs-lookup"><span data-stu-id="4b722-325">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="4b722-326">Corrigido o bug onde as ids enviadas por pipe de um comando com a saída tsv eram analisados incorretamente</span><span class="sxs-lookup"><span data-stu-id="4b722-326">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-327">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-327">Appservice</span></span>
* <span data-ttu-id="4b722-328">[VERSÃO PRÉVIA] Adicionado o comando `webapp up` que ajuda a criar e implantar conteúdo em aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b722-328">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="4b722-329">Corrigido um bug no aplicativo com base em contêiner do Windows devido à alteração de back-end</span><span class="sxs-lookup"><span data-stu-id="4b722-329">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="4b722-330">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-330">Network</span></span>
* <span data-ttu-id="4b722-331">Adicionado o argumento `--exclusion` a `application-gateway waf-config set` para dar suporte a exclusões de WAF</span><span class="sxs-lookup"><span data-stu-id="4b722-331">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="4b722-332">Função</span><span class="sxs-lookup"><span data-stu-id="4b722-332">Role</span></span>
* <span data-ttu-id="4b722-333">Adicionado suporte para identificadores personalizados para a credencial de senha</span><span class="sxs-lookup"><span data-stu-id="4b722-333">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="4b722-334">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-334">VM</span></span>
* <span data-ttu-id="4b722-335">[PRETERIDO] Parâmetro preterido `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="4b722-335">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="4b722-336">Adicionado parâmetro `--force` a `vm restart` para reimplantar as VMs sem resposta</span><span class="sxs-lookup"><span data-stu-id="4b722-336">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="4b722-337">Alterado `[vm|vmss] create --authentication-type` para aceitar "todos" para criar uma VM com senha e autenticação SSH</span><span class="sxs-lookup"><span data-stu-id="4b722-337">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="4b722-338">Adicionado parâmetro `image create --os-disk-caching` para definir o cache de disco do sistema operacional para uma imagem</span><span class="sxs-lookup"><span data-stu-id="4b722-338">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="4b722-339">20 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-339">November 20, 2018</span></span>

<span data-ttu-id="4b722-340">Versão 2.0.51</span><span class="sxs-lookup"><span data-stu-id="4b722-340">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="4b722-341">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-341">Core</span></span>
* <span data-ttu-id="4b722-342">Logon do MSI alterado para não reutilizar o nome da assinatura na identidade</span><span class="sxs-lookup"><span data-stu-id="4b722-342">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-343">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-343">ACR</span></span>
* <span data-ttu-id="4b722-344">Token de contexto adicionado à etapa da tarefa</span><span class="sxs-lookup"><span data-stu-id="4b722-344">Added context token to task step</span></span>
* <span data-ttu-id="4b722-345">Suporte adicionado para definir segredos na execução do acr para espelhar a tarefa do acr</span><span class="sxs-lookup"><span data-stu-id="4b722-345">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="4b722-346">Suporte aprimorado para `--top` e `--orderby` para os comandos `show-tags` e `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="4b722-346">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-347">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-347">Appservice</span></span>
* <span data-ttu-id="4b722-348">Tempo limite padrão para a implantação do zip alterado para sondar o status aumentado para 5 minutos, também adicionando uma propriedade de tempo limite para personalizar esse valor</span><span class="sxs-lookup"><span data-stu-id="4b722-348">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="4b722-349">Padrão `node_version` atualizado.</span><span class="sxs-lookup"><span data-stu-id="4b722-349">Updated the default `node_version`.</span></span> <span data-ttu-id="4b722-350">Redefinir a ação de troca de slots durante uma troca de duas fases preserva todas as configurações do aplicativo e cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="4b722-350">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="4b722-351">Verificação da SKU no lado do cliente removida para o Linux criar o plano do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b722-351">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="4b722-352">Erro corrigido ao tentar obter o status de implantação do zip</span><span class="sxs-lookup"><span data-stu-id="4b722-352">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="4b722-353">Iot Central</span><span class="sxs-lookup"><span data-stu-id="4b722-353">IotCentral</span></span>
* <span data-ttu-id="4b722-354">Verificação de disponibilidade do subdomínio adicionada ao criar um aplicativo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="4b722-354">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b722-355">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4b722-355">KeyVault</span></span>
* <span data-ttu-id="4b722-356">Bug corrigido em que os erros podem ter sido ignorados</span><span class="sxs-lookup"><span data-stu-id="4b722-356">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="4b722-357">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-357">Network</span></span>
* <span data-ttu-id="4b722-358">Subcomandos `root-cert` adicionados a `application-gateway` para lidar com os certificados de raiz confiável</span><span class="sxs-lookup"><span data-stu-id="4b722-358">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="4b722-359">Opções `--min-capacity` e `--custom-error-pages` adicionadas a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="4b722-359">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="4b722-360">`--zones` adicionado para suporte da zona de disponibilidade a `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="4b722-360">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="4b722-361">Argumentos `--file-upload-limit`, `--max-request-body-size` e `--request-body-check` a `application-gateway waf-config set` adicionados</span><span class="sxs-lookup"><span data-stu-id="4b722-361">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="4b722-362">Rdbms</span><span class="sxs-lookup"><span data-stu-id="4b722-362">Rdbms</span></span>
* <span data-ttu-id="4b722-363">Comandos vnet do mariadb adicionados</span><span class="sxs-lookup"><span data-stu-id="4b722-363">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="4b722-364">Rbac</span><span class="sxs-lookup"><span data-stu-id="4b722-364">Rbac</span></span>
* <span data-ttu-id="4b722-365">Um problema corrigido ao tentar atualizar credenciais inalteradas em `ad app update`</span><span class="sxs-lookup"><span data-stu-id="4b722-365">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="4b722-366">Avisos de saída adicionados para comunicar alterações de falha em um futuro próximo para `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="4b722-366">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="4b722-367">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-367">Storage</span></span>
* <span data-ttu-id="4b722-368">Melhor manipulação de casos incomuns para os comandos da cópia de armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-368">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="4b722-369">Corrigido o problema em que `storage blob copy start-batch` não usava credenciais de logon quando as contas de origem e destino eram iguais</span><span class="sxs-lookup"><span data-stu-id="4b722-369">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="4b722-370">Bug corrigido com `storage [blob|file] url` em que `sas_token` não foi incorporado na URL</span><span class="sxs-lookup"><span data-stu-id="4b722-370">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="4b722-371">Aviso de alteração da falha adicionado a `[blob|container] list`: produzirá apenas os primeiros 5.000 resultados por padrão</span><span class="sxs-lookup"><span data-stu-id="4b722-371">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-372">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-372">VM</span></span>
* <span data-ttu-id="4b722-373">Suporte adicionado a `[vm|vmss] create --storage-sku` para especificar a SKU da conta de armazenamento para o SO gerenciado e os discos de dados separadamente</span><span class="sxs-lookup"><span data-stu-id="4b722-373">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="4b722-374">Parâmetros do nome da versão alterados de `sig image-version` para `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="4b722-374">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="4b722-375">Argumento `sig image-version` preterido `--image-version-name`, substituído por `--image-version`</span><span class="sxs-lookup"><span data-stu-id="4b722-375">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="4b722-376">Suporte adicionado para usar o disco local do SO a `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="4b722-376">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="4b722-377">Adicionado o suporte ao `--no-wait` para `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="4b722-377">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="4b722-378">Adicionado o comando `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="4b722-378">Added `snapshot wait` command</span></span>
* <span data-ttu-id="4b722-379">Suporte adicionado para usar o nome da instância com `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="4b722-379">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="4b722-380">6 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-380">November 6, 2018</span></span>

<span data-ttu-id="4b722-381">Versão 2.0.50</span><span class="sxs-lookup"><span data-stu-id="4b722-381">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="4b722-382">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-382">Core</span></span>
* <span data-ttu-id="4b722-383">Foi adicionado suporte para o serviço principal sn + autenticação do emissor</span><span class="sxs-lookup"><span data-stu-id="4b722-383">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-384">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-384">ACR</span></span>
* <span data-ttu-id="4b722-385">Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa</span><span class="sxs-lookup"><span data-stu-id="4b722-385">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="4b722-386">Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação</span><span class="sxs-lookup"><span data-stu-id="4b722-386">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-387">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-387">ACS</span></span>
* <span data-ttu-id="4b722-388">[ALTERAÇÃO SIGNIFICATIVA] `enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão</span><span class="sxs-lookup"><span data-stu-id="4b722-388">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="4b722-389">Supervisor</span><span class="sxs-lookup"><span data-stu-id="4b722-389">Advisor</span></span>
* <span data-ttu-id="4b722-390">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="4b722-390">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="4b722-391">AMS</span><span class="sxs-lookup"><span data-stu-id="4b722-391">AMS</span></span>
* <span data-ttu-id="4b722-392">Novos grupos de comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="4b722-392">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="4b722-393">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="4b722-393">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="4b722-394">Adicionados parâmetros de criptografia com suporte para `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="4b722-394">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="4b722-395">O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido</span><span class="sxs-lookup"><span data-stu-id="4b722-395">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="4b722-396">Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="4b722-396">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="4b722-397">Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="4b722-397">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="4b722-398">Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="4b722-398">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="4b722-399">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming locator` foi substituído por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="4b722-399">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="4b722-400">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--content-keys` de `ams streaming locator` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="4b722-400">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="4b722-401">[ALTERAÇÃO SIGNIFICATIVA] `--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="4b722-401">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="4b722-402">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming policy` foi substituído por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="4b722-402">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="4b722-403">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="4b722-403">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="4b722-404">Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="4b722-404">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="4b722-405">Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado</span><span class="sxs-lookup"><span data-stu-id="4b722-405">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="4b722-406">[ALTERAÇÃO SIGNIFICATIVA] `--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="4b722-406">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="4b722-407">Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'.</span><span class="sxs-lookup"><span data-stu-id="4b722-407">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="4b722-408">Um ativo sem rótulo pode ser enviado assim: 'assetName='</span><span class="sxs-lookup"><span data-stu-id="4b722-408">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-409">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-409">AppService</span></span>
* <span data-ttu-id="4b722-410">Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido</span><span class="sxs-lookup"><span data-stu-id="4b722-410">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="4b722-411">Configurar</span><span class="sxs-lookup"><span data-stu-id="4b722-411">Configure</span></span>
* <span data-ttu-id="4b722-412">O YAML foi adicionado às opções de formato de saída</span><span class="sxs-lookup"><span data-stu-id="4b722-412">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="4b722-413">Contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-413">Container</span></span>
* <span data-ttu-id="4b722-414">Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml</span><span class="sxs-lookup"><span data-stu-id="4b722-414">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="4b722-415">EventHub</span><span class="sxs-lookup"><span data-stu-id="4b722-415">EventHub</span></span>
* <span data-ttu-id="4b722-416">O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-416">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="4b722-417">Interativo</span><span class="sxs-lookup"><span data-stu-id="4b722-417">Interactive</span></span>
* <span data-ttu-id="4b722-418">O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos</span><span class="sxs-lookup"><span data-stu-id="4b722-418">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="4b722-419">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="4b722-419">Monitor</span></span>
* <span data-ttu-id="4b722-420">Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) para `--condition` em `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-420">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="4b722-421">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-421">Network</span></span>
* <span data-ttu-id="4b722-422">Os nomes de comandos `network interface-endpoint` foram preteridos em benefício de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="4b722-422">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="4b722-423">Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID</span><span class="sxs-lookup"><span data-stu-id="4b722-423">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="4b722-424">Foi corrigido um problema onde `--ip-tags` não funcionava corretamente com `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="4b722-424">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="4b722-425">Perfil</span><span class="sxs-lookup"><span data-stu-id="4b722-425">Profile</span></span>
* <span data-ttu-id="4b722-426">`--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado</span><span class="sxs-lookup"><span data-stu-id="4b722-426">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="4b722-427">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4b722-427">RDBMS</span></span>
* <span data-ttu-id="4b722-428">Adicionados comandos da réplica mysql</span><span class="sxs-lookup"><span data-stu-id="4b722-428">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="4b722-429">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-429">Resource</span></span>
* <span data-ttu-id="4b722-430">Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="4b722-430">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="4b722-431">Função</span><span class="sxs-lookup"><span data-stu-id="4b722-431">Role</span></span>
* <span data-ttu-id="4b722-432">Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais</span><span class="sxs-lookup"><span data-stu-id="4b722-432">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="4b722-433">`ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="4b722-433">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="4b722-434">Suporte adicionado para conceder permissões a aplicativos do AAD</span><span class="sxs-lookup"><span data-stu-id="4b722-434">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-435">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-435">Storage</span></span>
* <span data-ttu-id="4b722-436">Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="4b722-436">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-437">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-437">VM</span></span>
* <span data-ttu-id="4b722-438">O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem</span><span class="sxs-lookup"><span data-stu-id="4b722-438">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="4b722-439">O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido</span><span class="sxs-lookup"><span data-stu-id="4b722-439">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="4b722-440">O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado</span><span class="sxs-lookup"><span data-stu-id="4b722-440">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="4b722-441">`vm secret format` foi alterado para exigir a saída json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="4b722-441">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="4b722-442">Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido</span><span class="sxs-lookup"><span data-stu-id="4b722-442">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="4b722-443">Validação de argumento aprimorado para `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="4b722-443">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="4b722-444">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-444">October 23, 2018</span></span>

<span data-ttu-id="4b722-445">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="4b722-445">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="4b722-446">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-446">Core</span></span>
* <span data-ttu-id="4b722-447">Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`</span><span class="sxs-lookup"><span data-stu-id="4b722-447">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="4b722-448">Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="4b722-448">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-449">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-449">ACR</span></span>
* <span data-ttu-id="4b722-450">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="4b722-450">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="4b722-451">CDN</span><span class="sxs-lookup"><span data-stu-id="4b722-451">CDN</span></span>
* <span data-ttu-id="4b722-452">[ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="4b722-452">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="4b722-453">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="4b722-453">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="4b722-454">Contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-454">Container</span></span>
* <span data-ttu-id="4b722-455">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="4b722-455">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="4b722-456">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="4b722-456">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="4b722-457">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="4b722-457">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="4b722-458">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="4b722-458">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="4b722-459">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="4b722-459">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="4b722-460">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="4b722-460">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="4b722-461">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="4b722-461">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4b722-462">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4b722-462">CosmosDB</span></span>
* <span data-ttu-id="4b722-463">Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="4b722-463">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="4b722-464">Interativo</span><span class="sxs-lookup"><span data-stu-id="4b722-464">Interactive</span></span>
* <span data-ttu-id="4b722-465">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="4b722-465">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="4b722-466">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="4b722-466">IoT Central</span></span>
* <span data-ttu-id="4b722-467">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="4b722-467">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="4b722-468">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="4b722-468">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="4b722-469">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="4b722-469">Monitor</span></span>
* <span data-ttu-id="4b722-470">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="4b722-470">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="4b722-471">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="4b722-471">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="4b722-472">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="4b722-472">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="4b722-473">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="4b722-473">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="4b722-474">Adicionado `--namespace` como alias para a opção preterida `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="4b722-474">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="4b722-475">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="4b722-475">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="4b722-476">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="4b722-476">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="4b722-477">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="4b722-477">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="4b722-478">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="4b722-478">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="4b722-479">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="4b722-479">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="4b722-480">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-480">Network</span></span>
* <span data-ttu-id="4b722-481">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="4b722-481">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="4b722-482">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="4b722-482">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="4b722-483">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="4b722-483">ServiceBus</span></span>
* <span data-ttu-id="4b722-484">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="4b722-484">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="4b722-485">SQL</span><span class="sxs-lookup"><span data-stu-id="4b722-485">SQL</span></span>
* <span data-ttu-id="4b722-486">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="4b722-486">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-487">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-487">Storage</span></span>
* <span data-ttu-id="4b722-488">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="4b722-488">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="4b722-489">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="4b722-489">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-490">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-490">VM</span></span>
* <span data-ttu-id="4b722-491">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="4b722-491">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="4b722-492">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`</span><span class="sxs-lookup"><span data-stu-id="4b722-492">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="4b722-493">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`</span><span class="sxs-lookup"><span data-stu-id="4b722-493">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="4b722-494">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-494">October 16, 2018</span></span>

<span data-ttu-id="4b722-495">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="4b722-495">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-496">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-496">VM</span></span>
* <span data-ttu-id="4b722-497">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="4b722-497">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="4b722-498">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-498">October 9, 2018</span></span>

<span data-ttu-id="4b722-499">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="4b722-499">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="4b722-500">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-500">Core</span></span>
* <span data-ttu-id="4b722-501">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="4b722-501">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-502">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-502">ACR</span></span>
* <span data-ttu-id="4b722-503">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="4b722-503">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-504">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-504">ACS</span></span>
* <span data-ttu-id="4b722-505">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="4b722-505">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="4b722-506">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="4b722-506">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="4b722-507">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="4b722-507">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="4b722-508">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="4b722-508">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="4b722-509">Contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-509">Container</span></span>
* <span data-ttu-id="4b722-510">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um tempo de execução específico</span><span class="sxs-lookup"><span data-stu-id="4b722-510">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="4b722-511">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="4b722-511">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="4b722-512">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="4b722-512">Event Hub</span></span>
* <span data-ttu-id="4b722-513">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="4b722-513">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="4b722-514">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="4b722-514">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="4b722-515">Extensões</span><span class="sxs-lookup"><span data-stu-id="4b722-515">Extensions</span></span>
* <span data-ttu-id="4b722-516">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="4b722-516">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4b722-517">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4b722-517">HDInsight</span></span>
* <span data-ttu-id="4b722-518">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="4b722-518">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="4b722-519">IoT</span><span class="sxs-lookup"><span data-stu-id="4b722-519">IoT</span></span>
* <span data-ttu-id="4b722-520">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="4b722-520">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b722-521">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4b722-521">KeyVault</span></span>
* <span data-ttu-id="4b722-522">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="4b722-522">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="4b722-523">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-523">Network</span></span>
* <span data-ttu-id="4b722-524">Corrigido `network dns zone create`: O comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="4b722-524">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="4b722-525">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="4b722-525">See #6052</span></span>
* <span data-ttu-id="4b722-526">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="4b722-526">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="4b722-527">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="4b722-527">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="4b722-528">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="4b722-528">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="4b722-529">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="4b722-529">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="4b722-530">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="4b722-530">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="4b722-531">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="4b722-531">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="4b722-532">Função</span><span class="sxs-lookup"><span data-stu-id="4b722-532">Role</span></span>
* <span data-ttu-id="4b722-533">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="4b722-533">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="4b722-534">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="4b722-534">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="4b722-535">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="4b722-535">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="4b722-536">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="4b722-536">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="4b722-537">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="4b722-537">Service Bus</span></span>
* <span data-ttu-id="4b722-538">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="4b722-538">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-539">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-539">VM</span></span>
* <span data-ttu-id="4b722-540">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="4b722-540">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="4b722-541">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="4b722-541">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="4b722-542">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="4b722-542">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="4b722-543">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="4b722-543">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="4b722-544">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="4b722-544">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="4b722-545">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="4b722-545">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="4b722-546">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-546">September 21, 2018</span></span>

<span data-ttu-id="4b722-547">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="4b722-547">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-548">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-548">ACR</span></span>
* <span data-ttu-id="4b722-549">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-549">Added ACR Task commands</span></span>
* <span data-ttu-id="4b722-550">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="4b722-550">Added quick run command</span></span>
* <span data-ttu-id="4b722-551">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="4b722-551">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="4b722-552">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-552">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="4b722-553">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="4b722-553">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="4b722-554">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="4b722-554">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-555">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-555">ACS</span></span>
* <span data-ttu-id="4b722-556">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="4b722-556">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="4b722-557">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="4b722-557">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-558">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-558">AppService</span></span>

* <span data-ttu-id="4b722-559">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="4b722-559">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="4b722-560">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="4b722-560">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="4b722-561">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="4b722-561">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="4b722-562">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="4b722-562">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="4b722-563">Lote</span><span class="sxs-lookup"><span data-stu-id="4b722-563">Batch</span></span>
* <span data-ttu-id="4b722-564">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="4b722-564">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="4b722-565">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="4b722-565">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="4b722-566">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="4b722-566">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="4b722-567">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="4b722-567">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4b722-568">Lote AI</span><span class="sxs-lookup"><span data-stu-id="4b722-568">Batch AI</span></span> 
* <span data-ttu-id="4b722-569">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="4b722-569">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4b722-570">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="4b722-570">Cognitive Services</span></span>
* <span data-ttu-id="4b722-571">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="4b722-571">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="4b722-572">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="4b722-572">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="4b722-573">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="4b722-573">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="4b722-574">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="4b722-574">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="4b722-575">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="4b722-575">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="4b722-576">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="4b722-576">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="4b722-577">Contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-577">Container</span></span>
* <span data-ttu-id="4b722-578">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="4b722-578">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="4b722-579">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="4b722-579">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="4b722-580">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="4b722-580">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="4b722-581">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="4b722-581">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="4b722-582">DataLake</span><span class="sxs-lookup"><span data-stu-id="4b722-582">Datalake</span></span>
* <span data-ttu-id="4b722-583">Comandos adicionados para regras de rede virtual</span><span class="sxs-lookup"><span data-stu-id="4b722-583">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="4b722-584">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="4b722-584">Interactive Shell</span></span>
* <span data-ttu-id="4b722-585">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="4b722-585">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="4b722-586">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="4b722-586">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="4b722-587">IoT</span><span class="sxs-lookup"><span data-stu-id="4b722-587">IoT</span></span>
* <span data-ttu-id="4b722-588">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="4b722-588">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="4b722-589">Key Vault</span><span class="sxs-lookup"><span data-stu-id="4b722-589">Key Vault</span></span>
* <span data-ttu-id="4b722-590">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="4b722-590">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="4b722-591">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-591">Network</span></span>
* <span data-ttu-id="4b722-592">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="4b722-592">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="4b722-593">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="4b722-593">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="4b722-594">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="4b722-594">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="4b722-595">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="4b722-595">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="4b722-596">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="4b722-596">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="4b722-597">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="4b722-597">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="4b722-598">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="4b722-598">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="4b722-599">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="4b722-599">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="4b722-600">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="4b722-600">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="4b722-601">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="4b722-601">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="4b722-602">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="4b722-602">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="4b722-603">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="4b722-603">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="4b722-604">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="4b722-604">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="4b722-605">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="4b722-605">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="4b722-606">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="4b722-606">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="4b722-607">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="4b722-607">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="4b722-608">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="4b722-608">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="4b722-609">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="4b722-609">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="4b722-610">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4b722-610">RDBMS</span></span>
* <span data-ttu-id="4b722-611">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="4b722-611">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="4b722-612">Reserva</span><span class="sxs-lookup"><span data-stu-id="4b722-612">Reservation</span></span>
* <span data-ttu-id="4b722-613">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="4b722-613">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="4b722-614">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="4b722-614">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="4b722-615">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b722-615">Manage App</span></span>
* <span data-ttu-id="4b722-616">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="4b722-616">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="4b722-617">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="4b722-617">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="4b722-618">Função</span><span class="sxs-lookup"><span data-stu-id="4b722-618">Role</span></span>
* <span data-ttu-id="4b722-619">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="4b722-619">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="4b722-620">SignalR</span><span class="sxs-lookup"><span data-stu-id="4b722-620">SignalR</span></span>
* <span data-ttu-id="4b722-621">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="4b722-621">First release</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-622">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-622">Storage</span></span>
* <span data-ttu-id="4b722-623">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="4b722-623">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="4b722-624">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="4b722-624">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-625">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-625">VM</span></span>
* <span data-ttu-id="4b722-626">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="4b722-626">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="4b722-627">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="4b722-627">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="4b722-628">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-628">August 28, 2018</span></span>

<span data-ttu-id="4b722-629">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="4b722-629">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="4b722-630">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-630">Core</span></span>

* <span data-ttu-id="4b722-631">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="4b722-631">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="4b722-632">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="4b722-632">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-633">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-633">ACR</span></span>

* <span data-ttu-id="4b722-634">Adicionada uma solução alternativa para operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="4b722-634">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="4b722-635">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="4b722-635">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-636">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-636">ACS</span></span>

* <span data-ttu-id="4b722-637">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="4b722-637">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="4b722-638">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="4b722-638">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-639">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-639">AppService</span></span>

* <span data-ttu-id="4b722-640">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="4b722-640">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="4b722-641">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="4b722-641">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="4b722-642">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="4b722-642">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="4b722-643">Backup</span><span class="sxs-lookup"><span data-stu-id="4b722-643">Backup</span></span>

* <span data-ttu-id="4b722-644">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="4b722-644">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="4b722-645">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="4b722-645">Bot Service</span></span>

* <span data-ttu-id="4b722-646">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="4b722-646">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4b722-647">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="4b722-647">Cognitive Services</span></span>

* <span data-ttu-id="4b722-648">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="4b722-648">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="4b722-649">IoT</span><span class="sxs-lookup"><span data-stu-id="4b722-649">IoT</span></span>

* <span data-ttu-id="4b722-650">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="4b722-650">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="4b722-651">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="4b722-651">Monitor</span></span>

* <span data-ttu-id="4b722-652">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="4b722-652">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="4b722-653">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="4b722-653">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="4b722-654">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-654">Network</span></span>

* <span data-ttu-id="4b722-655">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="4b722-655">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="4b722-656">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-656">Resource</span></span>

* <span data-ttu-id="4b722-657">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="4b722-657">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-658">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-658">Storage</span></span>

* <span data-ttu-id="4b722-659">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="4b722-659">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-660">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-660">VM</span></span>

* <span data-ttu-id="4b722-661">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="4b722-661">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="4b722-662">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="4b722-662">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="4b722-663">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-663">Auguest 14, 2018</span></span>

<span data-ttu-id="4b722-664">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="4b722-664">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="4b722-665">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-665">Core</span></span>

* <span data-ttu-id="4b722-666">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="4b722-666">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="4b722-667">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="4b722-667">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="4b722-668">Telemetria</span><span class="sxs-lookup"><span data-stu-id="4b722-668">Telemetry</span></span>

* <span data-ttu-id="4b722-669">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="4b722-669">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-670">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-670">ACR</span></span>

* <span data-ttu-id="4b722-671">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="4b722-671">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="4b722-672">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="4b722-672">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-673">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-673">ACS</span></span>

* <span data-ttu-id="4b722-674">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="4b722-674">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="4b722-675">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="4b722-675">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="4b722-676">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="4b722-676">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="4b722-677">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="4b722-677">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="4b722-678">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="4b722-678">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="4b722-679">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-679">AppService</span></span>

* <span data-ttu-id="4b722-680">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="4b722-680">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="4b722-681">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="4b722-681">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="4b722-682">BatchAI</span><span class="sxs-lookup"><span data-stu-id="4b722-682">BatchAI</span></span>

* <span data-ttu-id="4b722-683">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="4b722-683">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="4b722-684">Contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-684">Container</span></span>

* <span data-ttu-id="4b722-685">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-685">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="4b722-686">IoT</span><span class="sxs-lookup"><span data-stu-id="4b722-686">IoT</span></span>

* <span data-ttu-id="4b722-687">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="4b722-687">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="4b722-688">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="4b722-688">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="4b722-689">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="4b722-689">Iot Central</span></span>

* <span data-ttu-id="4b722-690">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="4b722-690">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b722-691">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4b722-691">KeyVault</span></span>


* <span data-ttu-id="4b722-692">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="4b722-692">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="4b722-693">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="4b722-693">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="4b722-694">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="4b722-694">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="4b722-695">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="4b722-695">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="4b722-696">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="4b722-696">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="4b722-697">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="4b722-697">Relay</span></span>

* <span data-ttu-id="4b722-698">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="4b722-698">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="4b722-699">Sql</span><span class="sxs-lookup"><span data-stu-id="4b722-699">Sql</span></span>

* <span data-ttu-id="4b722-700">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="4b722-700">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-701">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-701">Storage</span></span>

* <span data-ttu-id="4b722-702">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="4b722-702">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="4b722-703">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="4b722-703">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="4b722-704">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="4b722-704">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="4b722-705">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="4b722-705">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="4b722-706">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-706">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-707">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-707">VM</span></span>

* <span data-ttu-id="4b722-708">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="4b722-708">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="4b722-709">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-709">July 31, 2018</span></span>

<span data-ttu-id="4b722-710">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="4b722-710">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-711">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-711">ACR</span></span>

* <span data-ttu-id="4b722-712">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="4b722-712">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="4b722-713">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="4b722-713">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-714">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-714">ACS</span></span>

* <span data-ttu-id="4b722-715">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="4b722-715">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="4b722-716">Lote</span><span class="sxs-lookup"><span data-stu-id="4b722-716">Batch</span></span>

* <span data-ttu-id="4b722-717">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="4b722-717">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="4b722-718">Contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-718">Container</span></span>

* <span data-ttu-id="4b722-719">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="4b722-719">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="4b722-720">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-720">Network</span></span>

* <span data-ttu-id="4b722-721">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="4b722-721">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="4b722-722">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-722">Resource</span></span>

* <span data-ttu-id="4b722-723">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="4b722-723">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="4b722-724">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="4b722-724">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="4b722-725">Função</span><span class="sxs-lookup"><span data-stu-id="4b722-725">Role</span></span>

* <span data-ttu-id="4b722-726">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="4b722-726">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="4b722-727">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="4b722-727">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="4b722-728">Search</span><span class="sxs-lookup"><span data-stu-id="4b722-728">Search</span></span>

* <span data-ttu-id="4b722-729">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="4b722-729">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="4b722-730">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="4b722-730">Service Bus</span></span>

* <span data-ttu-id="4b722-731">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="4b722-731">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="4b722-732">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="4b722-732">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="4b722-733">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="4b722-733">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="4b722-734">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="4b722-734">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-735">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-735">Storage</span></span>

* <span data-ttu-id="4b722-736">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="4b722-736">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="4b722-737">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="4b722-737">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-738">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-738">VM</span></span>

* <span data-ttu-id="4b722-739">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="4b722-739">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="4b722-740">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="4b722-740">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="4b722-741">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="4b722-741">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="4b722-742">[ALTERAÇÃO SIGNIFICATIVA] `[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="4b722-742">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="4b722-743">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-743">July 18, 2018</span></span>

<span data-ttu-id="4b722-744">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="4b722-744">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="4b722-745">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-745">Core</span></span>

* <span data-ttu-id="4b722-746">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="4b722-746">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="4b722-747">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="4b722-747">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="4b722-748">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="4b722-748">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-749">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-749">ACR</span></span>

* <span data-ttu-id="4b722-750">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="4b722-750">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="4b722-751">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="4b722-751">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="4b722-752">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="4b722-752">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="4b722-753">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="4b722-753">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-754">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-754">ACS</span></span>

* <span data-ttu-id="4b722-755">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="4b722-755">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-756">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-756">AppService</span></span>

* <span data-ttu-id="4b722-757">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="4b722-757">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="4b722-758">Lote</span><span class="sxs-lookup"><span data-stu-id="4b722-758">Batch</span></span>

* <span data-ttu-id="4b722-759">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="4b722-759">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="4b722-760">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="4b722-760">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4b722-761">Lote AI</span><span class="sxs-lookup"><span data-stu-id="4b722-761">Batch AI</span></span>

* <span data-ttu-id="4b722-762">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="4b722-762">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="4b722-763">Contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-763">Container</span></span>

* <span data-ttu-id="4b722-764">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="4b722-764">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="4b722-765">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="4b722-765">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="4b722-766">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-766">Network</span></span>

* <span data-ttu-id="4b722-767">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="4b722-767">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="4b722-768">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="4b722-768">Added `network nic wait`</span></span>
* <span data-ttu-id="4b722-769">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="4b722-769">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="4b722-770">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="4b722-770">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="4b722-771">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-771">Resource</span></span>

* <span data-ttu-id="4b722-772">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="4b722-772">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="4b722-773">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="4b722-773">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="4b722-774">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="4b722-774">Added `deployment wait` command</span></span>
* <span data-ttu-id="4b722-775">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="4b722-775">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="4b722-776">SQL</span><span class="sxs-lookup"><span data-stu-id="4b722-776">SQL</span></span>

* <span data-ttu-id="4b722-777">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="4b722-777">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="4b722-778">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="4b722-778">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="4b722-779">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="4b722-779">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-780">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-780">Storage</span></span>

* <span data-ttu-id="4b722-781">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="4b722-781">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-782">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-782">VM</span></span>

* <span data-ttu-id="4b722-783">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="4b722-783">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="4b722-784">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="4b722-784">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="4b722-785">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="4b722-785">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="4b722-786">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-786">July 3, 2018</span></span>

<span data-ttu-id="4b722-787">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="4b722-787">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="4b722-788">AKS</span><span class="sxs-lookup"><span data-stu-id="4b722-788">AKS</span></span>

* <span data-ttu-id="4b722-789">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="4b722-789">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="4b722-790">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-790">July 3, 2018</span></span>

<span data-ttu-id="4b722-791">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="4b722-791">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="4b722-792">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-792">Core</span></span>

* <span data-ttu-id="4b722-793">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="4b722-793">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-794">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-794">ACR</span></span>

* <span data-ttu-id="4b722-795">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="4b722-795">Added polling build status</span></span>
* <span data-ttu-id="4b722-796">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="4b722-796">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="4b722-797">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="4b722-797">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-798">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-798">ACS</span></span>

* <span data-ttu-id="4b722-799">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="4b722-799">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="4b722-800">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="4b722-800">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="4b722-801">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="4b722-801">Updated options for `aks browse` command.</span></span> <span data-ttu-id="4b722-802">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="4b722-802">Added `--listen-port` support</span></span>
* <span data-ttu-id="4b722-803">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="4b722-803">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="4b722-804">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="4b722-804">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="4b722-805">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="4b722-805">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-806">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-806">AppService</span></span>

* <span data-ttu-id="4b722-807">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="4b722-807">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="4b722-808">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="4b722-808">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="4b722-809">Backup</span><span class="sxs-lookup"><span data-stu-id="4b722-809">Backup</span></span>

* <span data-ttu-id="4b722-810">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="4b722-810">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="4b722-811">BatchAI</span><span class="sxs-lookup"><span data-stu-id="4b722-811">BatchAI</span></span>

* <span data-ttu-id="4b722-812">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="4b722-812">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="4b722-813">Nuvem</span><span class="sxs-lookup"><span data-stu-id="4b722-813">Cloud</span></span>

* <span data-ttu-id="4b722-814">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="4b722-814">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="4b722-815">Contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-815">Container</span></span>

* <span data-ttu-id="4b722-816">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="4b722-816">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="4b722-817">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="4b722-817">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="4b722-818">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="4b722-818">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="4b722-819">Extensão</span><span class="sxs-lookup"><span data-stu-id="4b722-819">Extension</span></span>

* <span data-ttu-id="4b722-820">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="4b722-820">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="4b722-821">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-821">Network</span></span>

* <span data-ttu-id="4b722-822">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="4b722-822">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="4b722-823">Rdbms</span><span class="sxs-lookup"><span data-stu-id="4b722-823">Rdbms</span></span>

* <span data-ttu-id="4b722-824">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="4b722-824">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="4b722-825">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-825">Resource</span></span>

* <span data-ttu-id="4b722-826">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="4b722-826">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-827">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-827">VM</span></span>

* <span data-ttu-id="4b722-828">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="4b722-828">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="4b722-829">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-829">June 25, 2018</span></span>

<span data-ttu-id="4b722-830">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="4b722-830">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="4b722-831">CLI</span><span class="sxs-lookup"><span data-stu-id="4b722-831">CLI</span></span>

* <span data-ttu-id="4b722-832">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="4b722-832">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="4b722-833">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-833">June 19, 2018</span></span>

<span data-ttu-id="4b722-834">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="4b722-834">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="4b722-835">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-835">Core</span></span>

* <span data-ttu-id="4b722-836">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="4b722-836">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-837">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-837">ACR</span></span>

* <span data-ttu-id="4b722-838">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="4b722-838">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="4b722-839">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="4b722-839">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-840">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-840">ACS</span></span>

* <span data-ttu-id="4b722-841">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="4b722-841">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="4b722-842">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="4b722-842">Added `--update` support</span></span>
* <span data-ttu-id="4b722-843">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="4b722-843">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="4b722-844">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="4b722-844">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="4b722-845">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="4b722-845">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="4b722-846">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="4b722-846">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="4b722-847">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="4b722-847">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="4b722-848">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="4b722-848">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-849">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-849">AppService</span></span>

* <span data-ttu-id="4b722-850">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="4b722-850">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="4b722-851">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="4b722-851">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="4b722-852">Lote</span><span class="sxs-lookup"><span data-stu-id="4b722-852">Batch</span></span>

* <span data-ttu-id="4b722-853">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="4b722-853">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4b722-854">Lote AI</span><span class="sxs-lookup"><span data-stu-id="4b722-854">Batch AI</span></span>

* <span data-ttu-id="4b722-855">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="4b722-855">Added support for workspaces.</span></span> <span data-ttu-id="4b722-856">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="4b722-856">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="4b722-857">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="4b722-857">Added support for experiments.</span></span> <span data-ttu-id="4b722-858">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="4b722-858">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="4b722-859">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="4b722-859">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="4b722-860">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="4b722-860">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="4b722-861">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="4b722-861">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="4b722-862">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="4b722-862">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="4b722-863">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="4b722-863">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="4b722-864">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="4b722-864">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="4b722-865">[ALTERAÇÃO SIGNIFICATIVA] `--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="4b722-865">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="4b722-866">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="4b722-866">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="4b722-867">[ALTERAÇÃO SIGNIFICATIVA] `--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="4b722-867">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="4b722-868">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="4b722-868">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="4b722-869">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="4b722-869">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="4b722-870">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="4b722-870">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="4b722-871">[ALTERAÇÃO SIGNIFICATIVA] `--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="4b722-871">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="4b722-872">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="4b722-872">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="4b722-873">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="4b722-873">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="4b722-874">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="4b722-874">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="4b722-875">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="4b722-875">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="4b722-876">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="4b722-876">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="4b722-877">Mapas</span><span class="sxs-lookup"><span data-stu-id="4b722-877">Maps</span></span>

* <span data-ttu-id="4b722-878">[ALTERAÇÃO SIGNIFICATIVA] `maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="4b722-878">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="4b722-879">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-879">Network</span></span>

* <span data-ttu-id="4b722-880">Foi adicionado suporte a `https` para `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="4b722-880">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="4b722-881">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="4b722-881">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="4b722-882">#6502</span><span class="sxs-lookup"><span data-stu-id="4b722-882">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="4b722-883">Reservas</span><span class="sxs-lookup"><span data-stu-id="4b722-883">Reservations</span></span>

* <span data-ttu-id="4b722-884">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="4b722-884">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="4b722-885">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="4b722-885">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="4b722-886">[ALTERAÇÃO SIGNIFICATIVA] `kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="4b722-886">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="4b722-887">[ALTERAÇÃO SIGNIFICATIVA] `capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="4b722-887">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="4b722-888">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="4b722-888">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="4b722-889">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="4b722-889">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="4b722-890">Função</span><span class="sxs-lookup"><span data-stu-id="4b722-890">Role</span></span>

* <span data-ttu-id="4b722-891">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="4b722-891">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="4b722-892">SQL</span><span class="sxs-lookup"><span data-stu-id="4b722-892">SQL</span></span>

* <span data-ttu-id="4b722-893">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="4b722-893">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-894">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-894">Storage</span></span>

* <span data-ttu-id="4b722-895">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="4b722-895">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-896">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-896">VM</span></span>

* <span data-ttu-id="4b722-897">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="4b722-897">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="4b722-898">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="4b722-898">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="4b722-899">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="4b722-899">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="4b722-900">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-900">June 13, 2018</span></span>

<span data-ttu-id="4b722-901">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="4b722-901">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="4b722-902">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-902">Core</span></span>

* <span data-ttu-id="4b722-903">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="4b722-903">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="4b722-904">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-904">June 13, 2018</span></span>

<span data-ttu-id="4b722-905">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="4b722-905">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="4b722-906">AKS</span><span class="sxs-lookup"><span data-stu-id="4b722-906">AKS</span></span>

* <span data-ttu-id="4b722-907">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="4b722-907">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="4b722-908">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="4b722-908">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="4b722-909">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="4b722-909">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="4b722-910">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="4b722-910">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="4b722-911">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="4b722-911">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-912">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-912">AppService</span></span>

* <span data-ttu-id="4b722-913">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="4b722-913">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="4b722-914">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-914">June 5, 2018</span></span>

<span data-ttu-id="4b722-915">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="4b722-915">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="4b722-916">Interativo</span><span class="sxs-lookup"><span data-stu-id="4b722-916">Interactive</span></span>

* <span data-ttu-id="4b722-917">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="4b722-917">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="4b722-918">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-918">June 5, 2018</span></span>

<span data-ttu-id="4b722-919">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="4b722-919">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="4b722-920">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-920">Core</span></span>

* <span data-ttu-id="4b722-921">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="4b722-921">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="4b722-922">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="4b722-922">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-923">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-923">ACR</span></span>

* <span data-ttu-id="4b722-924">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="4b722-924">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="4b722-925">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="4b722-925">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="4b722-926">AKS</span><span class="sxs-lookup"><span data-stu-id="4b722-926">AKS</span></span>

* <span data-ttu-id="4b722-927">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="4b722-927">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="4b722-928">Lote</span><span class="sxs-lookup"><span data-stu-id="4b722-928">Batch</span></span>

* <span data-ttu-id="4b722-929">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="4b722-929">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="4b722-930">IOT</span><span class="sxs-lookup"><span data-stu-id="4b722-930">IOT</span></span>

* <span data-ttu-id="4b722-931">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="4b722-931">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="4b722-932">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-932">Network</span></span>

* <span data-ttu-id="4b722-933">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="4b722-933">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="4b722-934">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="4b722-934">Policy Insights</span></span>

* <span data-ttu-id="4b722-935">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="4b722-935">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="4b722-936">ARM</span><span class="sxs-lookup"><span data-stu-id="4b722-936">ARM</span></span>

* <span data-ttu-id="4b722-937">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="4b722-937">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="4b722-938">SQL</span><span class="sxs-lookup"><span data-stu-id="4b722-938">SQL</span></span>

* <span data-ttu-id="4b722-939">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="4b722-939">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="4b722-940">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="4b722-940">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="4b722-941">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-941">Storage</span></span>

* <span data-ttu-id="4b722-942">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="4b722-942">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-943">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-943">VM</span></span>

* <span data-ttu-id="4b722-944">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="4b722-944">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="4b722-945">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="4b722-945">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="4b722-946">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="4b722-946">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="4b722-947">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-947">May 22, 2018</span></span>

<span data-ttu-id="4b722-948">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="4b722-948">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="4b722-949">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-949">Core</span></span>

* <span data-ttu-id="4b722-950">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="4b722-950">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-951">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-951">ACS</span></span>

* <span data-ttu-id="4b722-952">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="4b722-952">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="4b722-953">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="4b722-953">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-954">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-954">AppService</span></span>

* <span data-ttu-id="4b722-955">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="4b722-955">Improved generic update commands</span></span>
* <span data-ttu-id="4b722-956">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="4b722-956">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="4b722-957">Contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-957">Container</span></span>

* <span data-ttu-id="4b722-958">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="4b722-958">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="4b722-959">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-959">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="4b722-960">Extensão</span><span class="sxs-lookup"><span data-stu-id="4b722-960">Extension</span></span>

* <span data-ttu-id="4b722-961">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="4b722-961">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="4b722-962">Interativo</span><span class="sxs-lookup"><span data-stu-id="4b722-962">Interactive</span></span>

* <span data-ttu-id="4b722-963">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="4b722-963">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="4b722-964">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="4b722-964">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b722-965">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4b722-965">KeyVault</span></span>

* <span data-ttu-id="4b722-966">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="4b722-966">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="4b722-967">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-967">Network</span></span>

* <span data-ttu-id="4b722-968">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="4b722-968">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="4b722-969">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="4b722-969">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="4b722-970">SQL</span><span class="sxs-lookup"><span data-stu-id="4b722-970">SQL</span></span>

* <span data-ttu-id="4b722-971">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="4b722-971">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="4b722-972">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="4b722-972">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="4b722-973">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="4b722-973">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="4b722-974">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b722-974">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="4b722-975">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="4b722-975">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="4b722-976">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="4b722-976">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="4b722-977">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="4b722-977">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="4b722-978">`edition`.</span><span class="sxs-lookup"><span data-stu-id="4b722-978">`edition`.</span></span> <span data-ttu-id="4b722-979">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="4b722-979">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="4b722-980">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="4b722-980">`elasticPoolName`.</span></span> <span data-ttu-id="4b722-981">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="4b722-981">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="4b722-982">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="4b722-982">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="4b722-983">`edition`.</span><span class="sxs-lookup"><span data-stu-id="4b722-983">`edition`.</span></span> <span data-ttu-id="4b722-984">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="4b722-984">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="4b722-985">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="4b722-985">`dtu`.</span></span> <span data-ttu-id="4b722-986">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="4b722-986">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="4b722-987">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="4b722-987">`databaseDtuMin`.</span></span> <span data-ttu-id="4b722-988">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="4b722-988">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="4b722-989">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="4b722-989">`databaseDtuMax`.</span></span> <span data-ttu-id="4b722-990">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="4b722-990">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="4b722-991">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="4b722-991">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="4b722-992">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="4b722-992">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-993">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-993">Storage</span></span>

* <span data-ttu-id="4b722-994">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="4b722-994">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="4b722-995">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="4b722-995">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-996">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-996">VM</span></span>

* <span data-ttu-id="4b722-997">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="4b722-997">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="4b722-998">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="4b722-998">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="4b722-999">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="4b722-999">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="4b722-1000">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="4b722-1000">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="4b722-1001">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1001">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="4b722-1002">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-1002">May 7, 2018</span></span>

<span data-ttu-id="4b722-1003">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="4b722-1003">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="4b722-1004">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-1004">Core</span></span>

* <span data-ttu-id="4b722-1005">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="4b722-1005">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="4b722-1006">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="4b722-1006">Added limited support for positional arguments</span></span>
* <span data-ttu-id="4b722-1007">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="4b722-1007">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="4b722-1008">#5591</span><span class="sxs-lookup"><span data-stu-id="4b722-1008">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="4b722-1009">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="4b722-1009">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="4b722-1010">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="4b722-1010">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="4b722-1011">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="4b722-1011">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="4b722-1012">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="4b722-1012">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="4b722-1013">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="4b722-1013">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-1014">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-1014">ACR</span></span>

* <span data-ttu-id="4b722-1015">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-1015">Added ACR Build commands</span></span>
* <span data-ttu-id="4b722-1016">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="4b722-1016">Improved resource not found error messages</span></span>
* <span data-ttu-id="4b722-1017">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="4b722-1017">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="4b722-1018">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="4b722-1018">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="4b722-1019">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="4b722-1019">Improved repository commands error messages</span></span>
* <span data-ttu-id="4b722-1020">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="4b722-1020">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-1021">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-1021">ACS</span></span>

* <span data-ttu-id="4b722-1022">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="4b722-1022">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="4b722-1023">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="4b722-1023">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="4b722-1024">AMS</span><span class="sxs-lookup"><span data-stu-id="4b722-1024">AMS</span></span>

* <span data-ttu-id="4b722-1025">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="4b722-1025">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-1026">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-1026">Appservice</span></span>

* <span data-ttu-id="4b722-1027">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="4b722-1027">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="4b722-1028">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1028">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="4b722-1029">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="4b722-1029">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="4b722-1030">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="4b722-1030">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4b722-1031">Lote AI</span><span class="sxs-lookup"><span data-stu-id="4b722-1031">Batch AI</span></span>

* <span data-ttu-id="4b722-1032">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="4b722-1032">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4b722-1033">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="4b722-1033">Cognitive Services</span></span>

* <span data-ttu-id="4b722-1034">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="4b722-1034">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="4b722-1035">Consumo</span><span class="sxs-lookup"><span data-stu-id="4b722-1035">Consumption</span></span>

* <span data-ttu-id="4b722-1036">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="4b722-1036">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="4b722-1037">Contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-1037">Container</span></span>

* <span data-ttu-id="4b722-1038">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="4b722-1038">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="4b722-1039">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4b722-1039">Cosmos DB</span></span>

* <span data-ttu-id="4b722-1040">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4b722-1040">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="4b722-1041">DMS</span><span class="sxs-lookup"><span data-stu-id="4b722-1041">DMS</span></span>

* <span data-ttu-id="4b722-1042">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="4b722-1042">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="4b722-1043">Extensão</span><span class="sxs-lookup"><span data-stu-id="4b722-1043">Extension</span></span>

* <span data-ttu-id="4b722-1044">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="4b722-1044">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="4b722-1045">Interativo</span><span class="sxs-lookup"><span data-stu-id="4b722-1045">Interactive</span></span>

* <span data-ttu-id="4b722-1046">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="4b722-1046">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="4b722-1047">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="4b722-1047">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="4b722-1048">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="4b722-1048">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="4b722-1049">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="4b722-1049">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="4b722-1050">Laboratório</span><span class="sxs-lookup"><span data-stu-id="4b722-1050">Lab</span></span>

* <span data-ttu-id="4b722-1051">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="4b722-1051">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="4b722-1052">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-1052">Network</span></span>

* <span data-ttu-id="4b722-1053">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="4b722-1053">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="4b722-1054">Perfil</span><span class="sxs-lookup"><span data-stu-id="4b722-1054">Profile</span></span>

* <span data-ttu-id="4b722-1055">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="4b722-1055">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="4b722-1056">[ALTERAÇÃO SIGNIFICATIVA] `--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="4b722-1056">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="4b722-1057">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="4b722-1057">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="4b722-1058">Redis</span><span class="sxs-lookup"><span data-stu-id="4b722-1058">Redis</span></span>

* <span data-ttu-id="4b722-1059">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="4b722-1059">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="4b722-1060">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="4b722-1060">Deprecated `redis list-all`.</span></span> <span data-ttu-id="4b722-1061">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="4b722-1061">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="4b722-1062">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="4b722-1062">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="4b722-1063">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="4b722-1063">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="4b722-1064">Função</span><span class="sxs-lookup"><span data-stu-id="4b722-1064">Role</span></span>

* <span data-ttu-id="4b722-1065">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="4b722-1065">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-1066">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-1066">Storage</span></span>

* <span data-ttu-id="4b722-1067">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="4b722-1067">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="4b722-1068">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="4b722-1068">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="4b722-1069">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="4b722-1069">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="4b722-1070">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="4b722-1070">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="4b722-1071">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="4b722-1071">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-1072">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-1072">VM</span></span>

* <span data-ttu-id="4b722-1073">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="4b722-1073">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="4b722-1074">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="4b722-1074">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="4b722-1075">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="4b722-1075">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="4b722-1076">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="4b722-1076">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="4b722-1077">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="4b722-1077">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="4b722-1078">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="4b722-1078">Added write accelerator support</span></span>
* <span data-ttu-id="4b722-1079">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="4b722-1079">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="4b722-1080">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="4b722-1080">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="4b722-1081">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="4b722-1081">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="4b722-1082">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-1082">April 10, 2018</span></span>

<span data-ttu-id="4b722-1083">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="4b722-1083">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-1084">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-1084">ACR</span></span>

* <span data-ttu-id="4b722-1085">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="4b722-1085">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-1086">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-1086">ACS</span></span>

* <span data-ttu-id="4b722-1087">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="4b722-1087">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-1088">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-1088">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="4b722-1090">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="4b722-1090">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="4b722-1091">BatchAI</span><span class="sxs-lookup"><span data-stu-id="4b722-1091">BatchAI</span></span>

* <span data-ttu-id="4b722-1092">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="4b722-1092">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="4b722-1093">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="4b722-1093">Job level mounting</span></span>
  - <span data-ttu-id="4b722-1094">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="4b722-1094">Environment variables with secret values</span></span>
  - <span data-ttu-id="4b722-1095">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="4b722-1095">Performance counters settings</span></span>
  - <span data-ttu-id="4b722-1096">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="4b722-1096">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="4b722-1097">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="4b722-1097">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="4b722-1098">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="4b722-1098">Usage and limits reporting</span></span>
  - <span data-ttu-id="4b722-1099">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="4b722-1099">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="4b722-1100">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="4b722-1100">Support for custom images</span></span>
  - <span data-ttu-id="4b722-1101">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="4b722-1101">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="4b722-1102">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="4b722-1102">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="4b722-1103">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="4b722-1103">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="4b722-1104">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="4b722-1104">National clouds are supported</span></span>
* <span data-ttu-id="4b722-1105">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="4b722-1105">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="4b722-1106">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="4b722-1106">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="4b722-1107">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="4b722-1107">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="4b722-1108">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="4b722-1108">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="4b722-1109">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="4b722-1109">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="4b722-1110">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="4b722-1110">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="4b722-1111">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="4b722-1111">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="4b722-1112">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="4b722-1112">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="4b722-1113">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="4b722-1113">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="4b722-1114">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1114">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="4b722-1115">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="4b722-1115">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="4b722-1116">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="4b722-1116">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="4b722-1117">[ALTERAÇÃO SIGNIFICATIVA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1117">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="4b722-1118">Cobrança</span><span class="sxs-lookup"><span data-stu-id="4b722-1118">Billing</span></span>

* <span data-ttu-id="4b722-1119">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="4b722-1119">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="4b722-1120">Consumo</span><span class="sxs-lookup"><span data-stu-id="4b722-1120">Consumption</span></span>

* <span data-ttu-id="4b722-1121">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="4b722-1121">Added `marketplace` commands</span></span>
* <span data-ttu-id="4b722-1122">[ALTERAÇÃO SIGNIFICATIVA] `reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="4b722-1122">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="4b722-1123">[ALTERAÇÃO SIGNIFICATIVA] `reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="4b722-1123">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="4b722-1124">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="4b722-1124">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="4b722-1125">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="4b722-1125">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="4b722-1126">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="4b722-1126">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="4b722-1127">Contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-1127">Container</span></span>

* <span data-ttu-id="4b722-1128">Adição dos parâmetros de montagem de volume de repositório git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="4b722-1128">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="4b722-1129">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="4b722-1129">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="4b722-1130">Extensão</span><span class="sxs-lookup"><span data-stu-id="4b722-1130">Extension</span></span>

* <span data-ttu-id="4b722-1131">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="4b722-1131">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="4b722-1132">Interativo</span><span class="sxs-lookup"><span data-stu-id="4b722-1132">Interactive</span></span>

* <span data-ttu-id="4b722-1133">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="4b722-1133">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="4b722-1134">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="4b722-1134">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="4b722-1135">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="4b722-1135">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="4b722-1136">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-1136">Network</span></span>

* <span data-ttu-id="4b722-1137">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="4b722-1137">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="4b722-1138">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4b722-1138">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="4b722-1139">#4910</span><span class="sxs-lookup"><span data-stu-id="4b722-1139">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="4b722-1140">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="4b722-1140">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="4b722-1141">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="4b722-1141">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="4b722-1142">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1142">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="4b722-1143">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1143">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="4b722-1144">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="4b722-1144">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="4b722-1145">Perfil</span><span class="sxs-lookup"><span data-stu-id="4b722-1145">Profile</span></span>

* <span data-ttu-id="4b722-1146">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="4b722-1146">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="4b722-1147">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="4b722-1147">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="4b722-1148">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4b722-1148">RDBMS</span></span>

* <span data-ttu-id="4b722-1149">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="4b722-1149">Added `georestore` command</span></span>
* <span data-ttu-id="4b722-1150">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1150">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="4b722-1151">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-1151">Resource</span></span>

* <span data-ttu-id="4b722-1152">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1152">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="4b722-1153">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1153">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="4b722-1154">SQL</span><span class="sxs-lookup"><span data-stu-id="4b722-1154">SQL</span></span>

* <span data-ttu-id="4b722-1155">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="4b722-1155">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-1156">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-1156">Storage</span></span>

* <span data-ttu-id="4b722-1157">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="4b722-1157">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-1158">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-1158">VM</span></span>

* <span data-ttu-id="4b722-1159">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1159">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="4b722-1160">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="4b722-1160">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="4b722-1162">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1162">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="4b722-1163">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="4b722-1163">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="4b722-1164">#5718</span><span class="sxs-lookup"><span data-stu-id="4b722-1164">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="4b722-1165">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="4b722-1165">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="4b722-1166">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-1166">March 27, 2018</span></span>

<span data-ttu-id="4b722-1167">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="4b722-1167">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="4b722-1168">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-1168">Core</span></span>

* <span data-ttu-id="4b722-1169">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="4b722-1169">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-1170">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-1170">ACS</span></span>

* <span data-ttu-id="4b722-1171">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="4b722-1171">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-1172">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-1172">Appservice</span></span>

* <span data-ttu-id="4b722-1173">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1173">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="4b722-1174">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1174">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="4b722-1175">Backup</span><span class="sxs-lookup"><span data-stu-id="4b722-1175">Backup</span></span>

* <span data-ttu-id="4b722-1176">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="4b722-1176">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="4b722-1177">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="4b722-1177">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="4b722-1178">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="4b722-1178">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="4b722-1179">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="4b722-1179">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="4b722-1180">Contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-1180">Container</span></span>

* <span data-ttu-id="4b722-1181">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="4b722-1181">Added `container exec` command.</span></span> <span data-ttu-id="4b722-1182">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="4b722-1182">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="4b722-1183">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-1183">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="4b722-1184">Extensão</span><span class="sxs-lookup"><span data-stu-id="4b722-1184">Extension</span></span>

* <span data-ttu-id="4b722-1185">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="4b722-1185">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="4b722-1186">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="4b722-1186">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="4b722-1187">[ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="4b722-1187">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="4b722-1188">Interativo</span><span class="sxs-lookup"><span data-stu-id="4b722-1188">Interactive</span></span>

* <span data-ttu-id="4b722-1189">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="4b722-1189">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="4b722-1190">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="4b722-1190">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="4b722-1191">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="4b722-1191">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="4b722-1192">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="4b722-1192">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="4b722-1193">Laboratório</span><span class="sxs-lookup"><span data-stu-id="4b722-1193">Lab</span></span>

* <span data-ttu-id="4b722-1194">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="4b722-1194">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="4b722-1195">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="4b722-1195">Monitor</span></span>

* <span data-ttu-id="4b722-1196">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="4b722-1196">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="4b722-1197">Corrigido [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="4b722-1197">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="4b722-1198">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="4b722-1198">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="4b722-1199">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-1199">Network</span></span>

* <span data-ttu-id="4b722-1200">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="4b722-1200">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="4b722-1201">Perfil</span><span class="sxs-lookup"><span data-stu-id="4b722-1201">Profile</span></span>

* <span data-ttu-id="4b722-1202">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="4b722-1202">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="4b722-1203">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4b722-1203">RDBMS</span></span>

* <span data-ttu-id="4b722-1204">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="4b722-1204">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="4b722-1205">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-1205">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="4b722-1207">Função</span><span class="sxs-lookup"><span data-stu-id="4b722-1207">Role</span></span>

* <span data-ttu-id="4b722-1208">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1208">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="4b722-1209">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="4b722-1209">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="4b722-1210">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1210">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="4b722-1211">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1211">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="4b722-1212">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="4b722-1212">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-1213">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-1213">Storage</span></span>

* <span data-ttu-id="4b722-1214">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="4b722-1214">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="4b722-1215">Corrigido [#4049](https://github.com/Azure/azure-cli/issues/4049): problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="4b722-1215">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-1216">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-1216">VM</span></span>

* <span data-ttu-id="4b722-1217">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="4b722-1217">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="4b722-1218">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1218">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="4b722-1219">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="4b722-1219">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="4b722-1220">[ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="4b722-1220">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="4b722-1221">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-1221">March 13, 2018</span></span>

<span data-ttu-id="4b722-1222">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="4b722-1222">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-1223">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-1223">ACR</span></span>

* <span data-ttu-id="4b722-1224">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="4b722-1224">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="4b722-1225">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="4b722-1225">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="4b722-1226">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="4b722-1226">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-1227">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-1227">ACS</span></span>

* <span data-ttu-id="4b722-1228">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="4b722-1228">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="4b722-1229">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="4b722-1229">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="4b722-1230">Supervisor</span><span class="sxs-lookup"><span data-stu-id="4b722-1230">Advisor</span></span>

* <span data-ttu-id="4b722-1231">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="4b722-1231">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="4b722-1232">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1232">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="4b722-1233">[ALTERAÇÃO SIGNIFICATIVA] `advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="4b722-1233">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="4b722-1234">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="4b722-1234">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="4b722-1235">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="4b722-1235">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-1236">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-1236">Appservice</span></span>

* <span data-ttu-id="4b722-1237">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="4b722-1237">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="4b722-1238">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="4b722-1238">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="4b722-1239">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="4b722-1239">Eventhubs</span></span>

* <span data-ttu-id="4b722-1240">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="4b722-1240">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="4b722-1241">Extensão</span><span class="sxs-lookup"><span data-stu-id="4b722-1241">Extension</span></span>

* <span data-ttu-id="4b722-1242">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="4b722-1242">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="4b722-1243">Interativo</span><span class="sxs-lookup"><span data-stu-id="4b722-1243">Interactive</span></span>

* <span data-ttu-id="4b722-1244">Corrigido [#5625](https://github.com/Azure/azure-cli/issues/5625): manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="4b722-1244">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="4b722-1245">Corrigido [#3016](https://github.com/Azure/azure-cli/issues/3016): histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="4b722-1245">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="4b722-1246">Corrigido [#5688](https://github.com/Azure/azure-cli/issues/5688): as conclusões não aparecerão se o carregamento da tabela de comando encontrar uma exceção</span><span class="sxs-lookup"><span data-stu-id="4b722-1246">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="4b722-1247">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="4b722-1247">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="4b722-1248">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="4b722-1248">Monitor</span></span>

* <span data-ttu-id="4b722-1249">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="4b722-1249">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="4b722-1250">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="4b722-1250">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="4b722-1251">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="4b722-1251">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="4b722-1252">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="4b722-1252">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="4b722-1253">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-1253">Network</span></span>

* <span data-ttu-id="4b722-1254">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1254">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="4b722-1255">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="4b722-1255">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="4b722-1256">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="4b722-1256">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="4b722-1257">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="4b722-1257">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="4b722-1258">Perfil</span><span class="sxs-lookup"><span data-stu-id="4b722-1258">Profile</span></span>

* <span data-ttu-id="4b722-1259">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="4b722-1259">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="4b722-1260">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="4b722-1260">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="4b722-1261">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4b722-1261">RDBMS</span></span>

* <span data-ttu-id="4b722-1262">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="4b722-1262">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="4b722-1263">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="4b722-1263">Service Bus</span></span>

* <span data-ttu-id="4b722-1264">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="4b722-1264">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-1265">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-1265">Storage</span></span>

* <span data-ttu-id="4b722-1266">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="4b722-1266">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="4b722-1267">Corrigido [#5286](https://github.com/Azure/azure-cli/issues/5286): os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="4b722-1267">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-1268">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-1268">VM</span></span>

* <span data-ttu-id="4b722-1269">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="4b722-1269">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="4b722-1270">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="4b722-1270">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="4b722-1271">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="4b722-1271">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="4b722-1272">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="4b722-1272">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="4b722-1273">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-1273">February 27, 2018</span></span>

<span data-ttu-id="4b722-1274">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="4b722-1274">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="4b722-1275">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-1275">Core</span></span>

* <span data-ttu-id="4b722-1276">Corrigido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="4b722-1276">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="4b722-1277">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="4b722-1277">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="4b722-1278">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="4b722-1278">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-1279">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-1279">ACS</span></span>

* <span data-ttu-id="4b722-1280">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="4b722-1280">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="4b722-1281">Problema corrigido: permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="4b722-1281">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="4b722-1282">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="4b722-1282">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="4b722-1283">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="4b722-1283">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-1284">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-1284">Appservice</span></span>

* <span data-ttu-id="4b722-1285">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="4b722-1285">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="4b722-1286">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="4b722-1286">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4b722-1287">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="4b722-1287">Cognitive Services</span></span>

* <span data-ttu-id="4b722-1288">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="4b722-1288">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="4b722-1289">Consumo</span><span class="sxs-lookup"><span data-stu-id="4b722-1289">Consumption</span></span>

* <span data-ttu-id="4b722-1290">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="4b722-1290">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="4b722-1291">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="4b722-1291">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="4b722-1292">Contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-1292">Container</span></span>

* <span data-ttu-id="4b722-1293">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="4b722-1293">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="4b722-1294">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-1294">Network</span></span>

* <span data-ttu-id="4b722-1295">Corrigido [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="4b722-1295">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="4b722-1296">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-1296">Resource</span></span>

* <span data-ttu-id="4b722-1297">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="4b722-1297">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="4b722-1298">Função</span><span class="sxs-lookup"><span data-stu-id="4b722-1298">Role</span></span>

* <span data-ttu-id="4b722-1299">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="4b722-1299">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="4b722-1300">SQL</span><span class="sxs-lookup"><span data-stu-id="4b722-1300">SQL</span></span>

* <span data-ttu-id="4b722-1301">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="4b722-1301">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-1302">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-1302">Storage</span></span>

* <span data-ttu-id="4b722-1303">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1303">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-1304">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-1304">VM</span></span>

* <span data-ttu-id="4b722-1305">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="4b722-1305">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="4b722-1306">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-1306">February 13, 2018</span></span>

<span data-ttu-id="4b722-1307">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="4b722-1307">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="4b722-1308">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-1308">Core</span></span>

* <span data-ttu-id="4b722-1309">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="4b722-1309">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-1310">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-1310">ACS</span></span>

* <span data-ttu-id="4b722-1311">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="4b722-1311">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="4b722-1312">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1312">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="4b722-1313">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="4b722-1313">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="4b722-1314">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="4b722-1314">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="4b722-1315">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="4b722-1315">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="4b722-1316">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="4b722-1316">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="4b722-1317">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="4b722-1317">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="4b722-1318">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="4b722-1318">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-1319">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-1319">Appservice</span></span>

* <span data-ttu-id="4b722-1320">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="4b722-1320">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="4b722-1321">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="4b722-1321">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="4b722-1322">CDN</span><span class="sxs-lookup"><span data-stu-id="4b722-1322">CDN</span></span>

* <span data-ttu-id="4b722-1323">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1323">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="4b722-1324">Contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-1324">Container</span></span>

* <span data-ttu-id="4b722-1325">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="4b722-1325">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="4b722-1326">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-1326">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4b722-1327">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4b722-1327">CosmosDB</span></span>

* <span data-ttu-id="4b722-1328">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="4b722-1328">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="4b722-1329">Extensão</span><span class="sxs-lookup"><span data-stu-id="4b722-1329">Extension</span></span>

* <span data-ttu-id="4b722-1330">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1330">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="4b722-1331">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1331">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="4b722-1332">Comentários</span><span class="sxs-lookup"><span data-stu-id="4b722-1332">Feedback</span></span>

* <span data-ttu-id="4b722-1333">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="4b722-1333">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="4b722-1334">Interativo</span><span class="sxs-lookup"><span data-stu-id="4b722-1334">Interactive</span></span>

* <span data-ttu-id="4b722-1335">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="4b722-1335">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="4b722-1336">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="4b722-1336">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="4b722-1337">IoT</span><span class="sxs-lookup"><span data-stu-id="4b722-1337">IoT</span></span>

* <span data-ttu-id="4b722-1338">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="4b722-1338">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="4b722-1339">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="4b722-1339">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="4b722-1340">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1340">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="4b722-1341">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="4b722-1341">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="4b722-1342">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="4b722-1342">Monitor</span></span>

* <span data-ttu-id="4b722-1343">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1343">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="4b722-1344">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-1344">Network</span></span>

* <span data-ttu-id="4b722-1345">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="4b722-1345">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="4b722-1346">Perfil</span><span class="sxs-lookup"><span data-stu-id="4b722-1346">Profile</span></span>

* <span data-ttu-id="4b722-1347">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="4b722-1347">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="4b722-1348">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-1348">Resource</span></span>

* <span data-ttu-id="4b722-1349">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="4b722-1349">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="4b722-1350">Função</span><span class="sxs-lookup"><span data-stu-id="4b722-1350">Role</span></span>

* <span data-ttu-id="4b722-1351">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1351">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="4b722-1352">SQL</span><span class="sxs-lookup"><span data-stu-id="4b722-1352">SQL</span></span>

* <span data-ttu-id="4b722-1353">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="4b722-1353">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="4b722-1354">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="4b722-1354">Added `sql db rename`</span></span>
* <span data-ttu-id="4b722-1355">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="4b722-1355">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-1356">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-1356">Storage</span></span>

* <span data-ttu-id="4b722-1357">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="4b722-1357">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-1358">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-1358">VM</span></span>

* <span data-ttu-id="4b722-1359">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="4b722-1359">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="4b722-1360">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="4b722-1360">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="4b722-1361">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="4b722-1361">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="4b722-1362">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-1362">January 31, 2018</span></span>

<span data-ttu-id="4b722-1363">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="4b722-1363">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="4b722-1364">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-1364">Core</span></span>

* <span data-ttu-id="4b722-1365">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="4b722-1365">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="4b722-1366">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="4b722-1366">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="4b722-1367">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="4b722-1367">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="4b722-1368">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="4b722-1368">Use `--verbose` to see</span></span>
* <span data-ttu-id="4b722-1369">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="4b722-1369">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-1370">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-1370">ACS</span></span>

* <span data-ttu-id="4b722-1371">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="4b722-1371">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="4b722-1372">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="4b722-1372">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-1373">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-1373">Appservice</span></span>

* <span data-ttu-id="4b722-1374">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="4b722-1374">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="4b722-1375">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="4b722-1375">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="4b722-1376">CDN</span><span class="sxs-lookup"><span data-stu-id="4b722-1376">CDN</span></span>

* <span data-ttu-id="4b722-1377">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1377">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4b722-1378">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4b722-1378">CosmosDB</span></span>

* <span data-ttu-id="4b722-1379">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="4b722-1379">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="4b722-1380">Interativo</span><span class="sxs-lookup"><span data-stu-id="4b722-1380">Interactive</span></span>

* <span data-ttu-id="4b722-1381">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="4b722-1381">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="4b722-1382">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-1382">Network</span></span>

* <span data-ttu-id="4b722-1383">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1383">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="4b722-1384">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="4b722-1384">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="4b722-1385">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1385">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="4b722-1386">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1386">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="4b722-1387">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="4b722-1387">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="4b722-1388">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="4b722-1388">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="4b722-1389">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="4b722-1389">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="4b722-1390">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="4b722-1390">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="4b722-1391">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="4b722-1391">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="4b722-1392">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="4b722-1392">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="4b722-1393">Perfil</span><span class="sxs-lookup"><span data-stu-id="4b722-1393">Profile</span></span>

* <span data-ttu-id="4b722-1394">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="4b722-1394">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="4b722-1395">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-1395">Resource</span></span>

* <span data-ttu-id="4b722-1396">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="4b722-1396">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-1397">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-1397">Storage</span></span>

* <span data-ttu-id="4b722-1398">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="4b722-1398">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="4b722-1399">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="4b722-1399">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="4b722-1400">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="4b722-1400">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="4b722-1401">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1401">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="4b722-1402">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="4b722-1402">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-1403">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-1403">VM</span></span>

* <span data-ttu-id="4b722-1404">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="4b722-1404">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="4b722-1405">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="4b722-1405">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="4b722-1406">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="4b722-1406">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="4b722-1407">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1407">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="4b722-1408">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="4b722-1408">January 17, 2018</span></span>

<span data-ttu-id="4b722-1409">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="4b722-1409">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-1410">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-1410">ACR</span></span>

* <span data-ttu-id="4b722-1411">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="4b722-1411">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="4b722-1412">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="4b722-1412">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-1413">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-1413">ACS</span></span>

* <span data-ttu-id="4b722-1414">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="4b722-1414">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="4b722-1415">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="4b722-1415">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-1416">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-1416">Appservice</span></span>

* <span data-ttu-id="4b722-1417">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="4b722-1417">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="4b722-1418">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="4b722-1418">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="4b722-1419">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="4b722-1419">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="4b722-1420">Backup</span><span class="sxs-lookup"><span data-stu-id="4b722-1420">Backup</span></span>

* <span data-ttu-id="4b722-1421">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="4b722-1421">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="4b722-1422">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="4b722-1422">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="4b722-1423">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="4b722-1423">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="4b722-1424">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="4b722-1424">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="4b722-1425">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="4b722-1425">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="4b722-1426">Lote</span><span class="sxs-lookup"><span data-stu-id="4b722-1426">Batch</span></span>

* <span data-ttu-id="4b722-1427">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="4b722-1427">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="4b722-1428">Nuvem</span><span class="sxs-lookup"><span data-stu-id="4b722-1428">Cloud</span></span>

* <span data-ttu-id="4b722-1429">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="4b722-1429">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="4b722-1430">Consumo</span><span class="sxs-lookup"><span data-stu-id="4b722-1430">Consumption</span></span>

* <span data-ttu-id="4b722-1431">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="4b722-1431">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="4b722-1432">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="4b722-1432">Event Grid</span></span>

* <span data-ttu-id="4b722-1433">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="4b722-1433">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="4b722-1434">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="4b722-1434">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="4b722-1435">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="4b722-1435">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="4b722-1436">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="4b722-1436">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="4b722-1437">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1437">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="4b722-1438">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1438">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="4b722-1439">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="4b722-1439">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="4b722-1440">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="4b722-1440">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="4b722-1441">Interativo</span><span class="sxs-lookup"><span data-stu-id="4b722-1441">Interactive</span></span>

* <span data-ttu-id="4b722-1442">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="4b722-1442">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="4b722-1443">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="4b722-1443">Fixed errors on startup</span></span>
* <span data-ttu-id="4b722-1444">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="4b722-1444">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="4b722-1445">IoT</span><span class="sxs-lookup"><span data-stu-id="4b722-1445">IoT</span></span>

* <span data-ttu-id="4b722-1446">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="4b722-1446">Added support for device provisioning service</span></span>
* <span data-ttu-id="4b722-1447">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="4b722-1447">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="4b722-1448">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="4b722-1448">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="4b722-1449">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="4b722-1449">Monitor</span></span>

* <span data-ttu-id="4b722-1450">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="4b722-1450">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="4b722-1451">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1451">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="4b722-1452">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="4b722-1452">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="4b722-1453">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-1453">Network</span></span>

* <span data-ttu-id="4b722-1454">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1454">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="4b722-1455">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1455">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="4b722-1456">Perfil</span><span class="sxs-lookup"><span data-stu-id="4b722-1456">Profile</span></span>

* <span data-ttu-id="4b722-1457">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="4b722-1457">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="4b722-1458">Função</span><span class="sxs-lookup"><span data-stu-id="4b722-1458">Role</span></span>

* <span data-ttu-id="4b722-1459">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="4b722-1459">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4b722-1460">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4b722-1460">Service Fabric</span></span>

* <span data-ttu-id="4b722-1461">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="4b722-1461">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="4b722-1462">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="4b722-1462">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-1463">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-1463">VM</span></span>

* <span data-ttu-id="4b722-1464">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="4b722-1464">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="4b722-1465">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="4b722-1465">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="4b722-1466">[ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="4b722-1466">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="4b722-1467">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="4b722-1467">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="4b722-1468">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="4b722-1468">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="4b722-1469">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1469">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="4b722-1470">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1470">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="4b722-1471">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="4b722-1471">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="4b722-1472">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="4b722-1472">December 19, 2017</span></span>

<span data-ttu-id="4b722-1473">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="4b722-1473">Version 2.0.23</span></span>

* <span data-ttu-id="4b722-1474">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="4b722-1474">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="4b722-1475">Contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-1475">Container</span></span>

* <span data-ttu-id="4b722-1476">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-1476">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="4b722-1477">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-1477">Network</span></span>

* <span data-ttu-id="4b722-1478">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1478">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="4b722-1479">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1479">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-1480">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-1480">Storage</span></span>

* <span data-ttu-id="4b722-1481">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="4b722-1481">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-1482">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-1482">VM</span></span>

* <span data-ttu-id="4b722-1483">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="4b722-1483">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="4b722-1484">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="4b722-1484">December 5, 2017</span></span>

<span data-ttu-id="4b722-1485">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="4b722-1485">Version 2.0.22</span></span>

* <span data-ttu-id="4b722-1486">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="4b722-1486">Removed `az component` commands.</span></span> <span data-ttu-id="4b722-1487">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="4b722-1487">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="4b722-1488">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-1488">Core</span></span>
* <span data-ttu-id="4b722-1489">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="4b722-1489">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="4b722-1490">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="4b722-1490">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-1491">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-1491">ACS</span></span>

* <span data-ttu-id="4b722-1492">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="4b722-1492">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="4b722-1493">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1493">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="4b722-1494">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="4b722-1494">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="4b722-1495">Supervisor</span><span class="sxs-lookup"><span data-stu-id="4b722-1495">Advisor</span></span>

* <span data-ttu-id="4b722-1496">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="4b722-1496">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-1497">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-1497">Appservice</span></span>

* <span data-ttu-id="4b722-1498">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="4b722-1498">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="4b722-1499">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="4b722-1499">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="4b722-1500">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="4b722-1500">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="4b722-1501">Consumo</span><span class="sxs-lookup"><span data-stu-id="4b722-1501">Consumption</span></span>

* <span data-ttu-id="4b722-1502">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="4b722-1502">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="4b722-1503">Contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-1503">Container</span></span>

* <span data-ttu-id="4b722-1504">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="4b722-1504">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="4b722-1505">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="4b722-1505">Monitor</span></span>

* <span data-ttu-id="4b722-1506">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="4b722-1506">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="4b722-1507">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-1507">Resource</span></span>

* <span data-ttu-id="4b722-1508">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="4b722-1508">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="4b722-1509">Função</span><span class="sxs-lookup"><span data-stu-id="4b722-1509">Role</span></span>

* <span data-ttu-id="4b722-1510">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="4b722-1510">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="4b722-1511">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="4b722-1511">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="4b722-1512">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="4b722-1512">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="4b722-1513">SQL</span><span class="sxs-lookup"><span data-stu-id="4b722-1513">SQL</span></span>

* <span data-ttu-id="4b722-1514">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="4b722-1514">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="4b722-1515">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="4b722-1515">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-1516">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-1516">VM</span></span>

* <span data-ttu-id="4b722-1517">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="4b722-1517">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="4b722-1518">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="4b722-1518">November 14, 2017</span></span>

<span data-ttu-id="4b722-1519">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="4b722-1519">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-1520">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-1520">ACR</span></span>

* <span data-ttu-id="4b722-1521">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="4b722-1521">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="4b722-1522">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-1522">ACS</span></span>

* <span data-ttu-id="4b722-1523">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="4b722-1523">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="4b722-1524">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1524">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="4b722-1525">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="4b722-1525">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="4b722-1526">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="4b722-1526">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="4b722-1527">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="4b722-1527">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-1528">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-1528">Appservice</span></span>

* <span data-ttu-id="4b722-1529">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="4b722-1529">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="4b722-1530">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="4b722-1530">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="4b722-1531">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="4b722-1531">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="4b722-1532">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="4b722-1532">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="4b722-1533">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="4b722-1533">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="4b722-1534">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="4b722-1534">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="4b722-1535">Lote</span><span class="sxs-lookup"><span data-stu-id="4b722-1535">Batch</span></span>

* <span data-ttu-id="4b722-1536">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="4b722-1536">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="4b722-1537">Batchai</span><span class="sxs-lookup"><span data-stu-id="4b722-1537">Batchai</span></span>

* <span data-ttu-id="4b722-1538">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1538">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="4b722-1539">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1539">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="4b722-1540">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="4b722-1540">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="4b722-1541">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1541">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="4b722-1542">Nuvem</span><span class="sxs-lookup"><span data-stu-id="4b722-1542">Cloud</span></span>

* <span data-ttu-id="4b722-1543">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="4b722-1543">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="4b722-1544">Contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-1544">Container</span></span>

* <span data-ttu-id="4b722-1545">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="4b722-1545">Added support to open multiple ports</span></span>
* <span data-ttu-id="4b722-1546">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="4b722-1546">Added container group restart policy</span></span>
* <span data-ttu-id="4b722-1547">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="4b722-1547">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="4b722-1548">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="4b722-1548">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4b722-1549">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4b722-1549">Data Lake Analytics</span></span>

* <span data-ttu-id="4b722-1550">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="4b722-1550">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4b722-1551">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4b722-1551">Data Lake Store</span></span>

* <span data-ttu-id="4b722-1552">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="4b722-1552">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="4b722-1553">Extensão</span><span class="sxs-lookup"><span data-stu-id="4b722-1553">Extension</span></span>

* <span data-ttu-id="4b722-1554">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="4b722-1554">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="4b722-1555">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="4b722-1555">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="4b722-1556">IoT</span><span class="sxs-lookup"><span data-stu-id="4b722-1556">IoT</span></span>

* <span data-ttu-id="4b722-1557">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="4b722-1557">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="4b722-1558">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="4b722-1558">Monitor</span></span>

* <span data-ttu-id="4b722-1559">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="4b722-1559">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="4b722-1560">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-1560">Network</span></span>

* <span data-ttu-id="4b722-1561">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="4b722-1561">Added support for CAA DNS records</span></span>
* <span data-ttu-id="4b722-1562">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1562">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="4b722-1563">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="4b722-1563">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="4b722-1564">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="4b722-1564">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="4b722-1565">Reservas</span><span class="sxs-lookup"><span data-stu-id="4b722-1565">Reservations</span></span>

* <span data-ttu-id="4b722-1566">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="4b722-1566">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="4b722-1567">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-1567">Resource</span></span>

* <span data-ttu-id="4b722-1568">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-1568">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="4b722-1569">SQL</span><span class="sxs-lookup"><span data-stu-id="4b722-1569">SQL</span></span>

* <span data-ttu-id="4b722-1570">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1570">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-1571">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-1571">Storage</span></span>

* <span data-ttu-id="4b722-1572">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="4b722-1572">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="4b722-1573">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="4b722-1573">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="4b722-1574">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="4b722-1574">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="4b722-1575">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="4b722-1575">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="4b722-1576">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1576">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="4b722-1577">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="4b722-1577">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="4b722-1578">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1578">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-1579">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-1579">VM</span></span>

* <span data-ttu-id="4b722-1580">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="4b722-1580">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="4b722-1581">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="4b722-1581">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="4b722-1582">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="4b722-1582">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="4b722-1583">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="4b722-1583">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="4b722-1584">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="4b722-1584">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="4b722-1585">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="4b722-1585">October 24, 2017</span></span>

<span data-ttu-id="4b722-1586">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="4b722-1586">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="4b722-1587">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-1587">Core</span></span>

* <span data-ttu-id="4b722-1588">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="4b722-1588">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-1589">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-1589">ACR</span></span>

* <span data-ttu-id="4b722-1590">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="4b722-1590">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="4b722-1591">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="4b722-1591">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="4b722-1592">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="4b722-1592">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-1593">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-1593">ACS</span></span>

* <span data-ttu-id="4b722-1594">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="4b722-1594">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="4b722-1595">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="4b722-1595">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-1596">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-1596">Appservice</span></span>

* <span data-ttu-id="4b722-1597">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="4b722-1597">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="4b722-1598">Componente</span><span class="sxs-lookup"><span data-stu-id="4b722-1598">Component</span></span>

* <span data-ttu-id="4b722-1599">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="4b722-1599">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="4b722-1600">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="4b722-1600">Monitor</span></span>

* <span data-ttu-id="4b722-1601">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="4b722-1601">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="4b722-1602">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-1602">Resource</span></span>

* <span data-ttu-id="4b722-1603">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="4b722-1603">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="4b722-1604">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="4b722-1604">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-1605">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-1605">VM</span></span>

* <span data-ttu-id="4b722-1606">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1606">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="4b722-1607">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="4b722-1607">October 9, 2017</span></span>

<span data-ttu-id="4b722-1608">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="4b722-1608">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="4b722-1609">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-1609">Core</span></span>

* <span data-ttu-id="4b722-1610">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="4b722-1610">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-1611">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-1611">Appservice</span></span>

* <span data-ttu-id="4b722-1612">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1612">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="4b722-1613">Lote</span><span class="sxs-lookup"><span data-stu-id="4b722-1613">Batch</span></span>

* <span data-ttu-id="4b722-1614">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="4b722-1614">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="4b722-1615">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="4b722-1615">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="4b722-1616">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="4b722-1616">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="4b722-1617">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="4b722-1617">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="4b722-1618">Batchai</span><span class="sxs-lookup"><span data-stu-id="4b722-1618">Batchai</span></span>

* <span data-ttu-id="4b722-1619">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="4b722-1619">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b722-1620">Keyvault</span><span class="sxs-lookup"><span data-stu-id="4b722-1620">Keyvault</span></span>

* <span data-ttu-id="4b722-1621">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="4b722-1621">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="4b722-1622">(#4448)</span><span class="sxs-lookup"><span data-stu-id="4b722-1622">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="4b722-1623">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-1623">Network</span></span>

* <span data-ttu-id="4b722-1624">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="4b722-1624">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="4b722-1625">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="4b722-1625">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="4b722-1626">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-1626">Resource</span></span>

* <span data-ttu-id="4b722-1627">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="4b722-1627">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="4b722-1628">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="4b722-1628">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="4b722-1629">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="4b722-1629">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="4b722-1630">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-1630">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="4b722-1631">Sql</span><span class="sxs-lookup"><span data-stu-id="4b722-1631">Sql</span></span>

* <span data-ttu-id="4b722-1632">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="4b722-1632">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="4b722-1633">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="4b722-1633">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="4b722-1634">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="4b722-1634">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-1635">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-1635">Storage</span></span>

* <span data-ttu-id="4b722-1636">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="4b722-1636">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-1637">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-1637">Vm</span></span>

* <span data-ttu-id="4b722-1638">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="4b722-1638">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="4b722-1639">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1639">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="4b722-1640">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="4b722-1640">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="4b722-1641">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1641">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="4b722-1642">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1642">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="4b722-1643">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="4b722-1643">September 22, 2017</span></span>

<span data-ttu-id="4b722-1644">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="4b722-1644">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="4b722-1645">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-1645">Resource</span></span>

* <span data-ttu-id="4b722-1646">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="4b722-1646">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="4b722-1647">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="4b722-1647">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="4b722-1648">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1648">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="4b722-1649">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="4b722-1649">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="4b722-1650">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-1650">Network</span></span>

* <span data-ttu-id="4b722-1651">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="4b722-1651">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="4b722-1652">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="4b722-1652">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="4b722-1653">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b722-1653">Added `asg` application security group commands</span></span>
* <span data-ttu-id="4b722-1654">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1654">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="4b722-1655">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1655">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="4b722-1656">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1656">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="4b722-1657">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1657">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-1658">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-1658">Storage</span></span>

* <span data-ttu-id="4b722-1659">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="4b722-1659">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="4b722-1660">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="4b722-1660">Eventgrid</span></span>

* <span data-ttu-id="4b722-1661">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="4b722-1661">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="4b722-1662">SQL</span><span class="sxs-lookup"><span data-stu-id="4b722-1662">SQL</span></span>

* <span data-ttu-id="4b722-1663">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="4b722-1663">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="4b722-1664">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="4b722-1664">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="4b722-1665">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1665">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b722-1666">Keyvault</span><span class="sxs-lookup"><span data-stu-id="4b722-1666">Keyvault</span></span>

* <span data-ttu-id="4b722-1667">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="4b722-1667">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-1668">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-1668">VM</span></span>

* <span data-ttu-id="4b722-1669">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1669">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="4b722-1670">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="4b722-1670">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="4b722-1671">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1671">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="4b722-1672">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="4b722-1672">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="4b722-1673">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="4b722-1673">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="4b722-1674">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="4b722-1674">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-1675">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-1675">ACS</span></span>

* <span data-ttu-id="4b722-1676">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-1676">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-1677">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-1677">Appservice</span></span>

* <span data-ttu-id="4b722-1678">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1678">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="4b722-1679">Backup</span><span class="sxs-lookup"><span data-stu-id="4b722-1679">Backup</span></span>

* <span data-ttu-id="4b722-1680">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="4b722-1680">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="4b722-1681">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="4b722-1681">September 11, 2017</span></span>

<span data-ttu-id="4b722-1682">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="4b722-1682">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="4b722-1683">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-1683">Core</span></span>

* <span data-ttu-id="4b722-1684">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="4b722-1684">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="4b722-1685">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="4b722-1685">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-1686">Acs</span><span class="sxs-lookup"><span data-stu-id="4b722-1686">Acs</span></span>

* <span data-ttu-id="4b722-1687">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="4b722-1687">Added `acs list-locations` command</span></span>
* <span data-ttu-id="4b722-1688">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="4b722-1688">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-1689">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-1689">Appservice</span></span>

* <span data-ttu-id="4b722-1690">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="4b722-1690">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="4b722-1691">CDN</span><span class="sxs-lookup"><span data-stu-id="4b722-1691">CDN</span></span>

* <span data-ttu-id="4b722-1692">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1692">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="4b722-1693">Extensão</span><span class="sxs-lookup"><span data-stu-id="4b722-1693">Extension</span></span>

* <span data-ttu-id="4b722-1694">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="4b722-1694">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b722-1695">Keyvault</span><span class="sxs-lookup"><span data-stu-id="4b722-1695">Keyvault</span></span>

* <span data-ttu-id="4b722-1696">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="4b722-1696">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="4b722-1697">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-1697">Network</span></span>

* <span data-ttu-id="4b722-1698">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="4b722-1698">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="4b722-1699">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1699">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="4b722-1700">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1700">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="4b722-1701">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1701">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="4b722-1702">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1702">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="4b722-1703">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-1703">Resource</span></span>

* <span data-ttu-id="4b722-1704">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1704">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="4b722-1705">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1705">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="4b722-1706">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="4b722-1706">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="4b722-1707">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="4b722-1707">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="4b722-1708">SQL</span><span class="sxs-lookup"><span data-stu-id="4b722-1708">SQL</span></span>

* <span data-ttu-id="4b722-1709">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="4b722-1709">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-1710">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-1710">VM</span></span>

* <span data-ttu-id="4b722-1711">Corrigido: não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="4b722-1711">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="4b722-1712">Corrigido: usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="4b722-1712">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="4b722-1713">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1713">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="4b722-1714">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="4b722-1714">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="4b722-1715">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="4b722-1715">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="4b722-1716">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="4b722-1716">August 31, 2017</span></span>

<span data-ttu-id="4b722-1717">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="4b722-1717">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b722-1718">Keyvault</span><span class="sxs-lookup"><span data-stu-id="4b722-1718">Keyvault</span></span>

* <span data-ttu-id="4b722-1719">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="4b722-1719">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="4b722-1720">Sf</span><span class="sxs-lookup"><span data-stu-id="4b722-1720">Sf</span></span>

* <span data-ttu-id="4b722-1721">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="4b722-1721">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-1722">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-1722">Storage</span></span>

* <span data-ttu-id="4b722-1723">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="4b722-1723">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="4b722-1724">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="4b722-1724">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="4b722-1725">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="4b722-1725">August 28, 2017</span></span>

<span data-ttu-id="4b722-1726">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="4b722-1726">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="4b722-1727">CLI</span><span class="sxs-lookup"><span data-stu-id="4b722-1727">CLI</span></span>

* <span data-ttu-id="4b722-1728">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="4b722-1728">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-1729">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-1729">ACS</span></span>

* <span data-ttu-id="4b722-1730">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="4b722-1730">Corrected preview regions</span></span>
* <span data-ttu-id="4b722-1731">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="4b722-1731">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="4b722-1732">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="4b722-1732">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-1733">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-1733">Appservice</span></span>

* <span data-ttu-id="4b722-1734">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1734">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="4b722-1735">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="4b722-1735">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="4b722-1736">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="4b722-1736">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="4b722-1737">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b722-1737">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="4b722-1738">Corrigido: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="4b722-1738">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="4b722-1739">IoT</span><span class="sxs-lookup"><span data-stu-id="4b722-1739">IoT</span></span>

* <span data-ttu-id="4b722-1740">Corrigido #3934: a criação de uma política não limpa mais as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="4b722-1740">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="4b722-1741">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-1741">Network</span></span>

* <span data-ttu-id="4b722-1742">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="4b722-1742">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="4b722-1743">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1743">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="4b722-1744">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4b722-1744">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="4b722-1745">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1745">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="4b722-1746">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1746">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="4b722-1747">Perfil</span><span class="sxs-lookup"><span data-stu-id="4b722-1747">Profile</span></span>

* <span data-ttu-id="4b722-1748">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="4b722-1748">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4b722-1749">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4b722-1749">Service Fabric</span></span>

* <span data-ttu-id="4b722-1750">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="4b722-1750">Preview release</span></span>
* <span data-ttu-id="4b722-1751">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="4b722-1751">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="4b722-1752">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="4b722-1752">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="4b722-1753">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="4b722-1753">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-1754">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-1754">Storage</span></span>

* <span data-ttu-id="4b722-1755">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="4b722-1755">Enabled setting blob tier</span></span>
* <span data-ttu-id="4b722-1756">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="4b722-1756">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="4b722-1757">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="4b722-1757">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="4b722-1758">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="4b722-1758">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="4b722-1759">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1759">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="4b722-1760">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="4b722-1760">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-1761">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-1761">VM</span></span>

* <span data-ttu-id="4b722-1762">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="4b722-1762">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="4b722-1763">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="4b722-1763">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="4b722-1764">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1764">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="4b722-1765">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="4b722-1765">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="4b722-1766">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="4b722-1766">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="4b722-1767">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1767">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="4b722-1768">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="4b722-1768">August 15, 2017</span></span>

<span data-ttu-id="4b722-1769">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="4b722-1769">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-1770">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-1770">ACS</span></span>

* <span data-ttu-id="4b722-1771">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="4b722-1771">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-1772">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-1772">Appservice</span></span>

* <span data-ttu-id="4b722-1773">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="4b722-1773">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="4b722-1774">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="4b722-1774">Event Grid</span></span>

* <span data-ttu-id="4b722-1775">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="4b722-1775">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="4b722-1776">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="4b722-1776">August 11, 2017</span></span>

<span data-ttu-id="4b722-1777">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="4b722-1777">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-1778">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-1778">ACS</span></span>

* <span data-ttu-id="4b722-1779">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="4b722-1779">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="4b722-1780">Lote</span><span class="sxs-lookup"><span data-stu-id="4b722-1780">Batch</span></span>

* <span data-ttu-id="4b722-1781">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="4b722-1781">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="4b722-1782">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="4b722-1782">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="4b722-1783">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-1783">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="4b722-1784">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="4b722-1784">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="4b722-1785">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="4b722-1785">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="4b722-1786">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="4b722-1786">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="4b722-1787">Componente</span><span class="sxs-lookup"><span data-stu-id="4b722-1787">Component</span></span>

* <span data-ttu-id="4b722-1788">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="4b722-1788">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="4b722-1789">Contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-1789">Container</span></span>

* <span data-ttu-id="4b722-1790">`create`: corrigido o problema em que o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="4b722-1790">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="4b722-1791">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4b722-1791">Data Lake Store</span></span>

* <span data-ttu-id="4b722-1792">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="4b722-1792">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="4b722-1793">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="4b722-1793">Event Grid</span></span>

* <span data-ttu-id="4b722-1794">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="4b722-1794">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="4b722-1795">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-1795">Network</span></span>

* <span data-ttu-id="4b722-1796">`lb`: corrigido o problema em que os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="4b722-1796">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="4b722-1797">`application-gateway {subresource} delete`: corrigido o problema em que `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="4b722-1797">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="4b722-1798">`application-gateway http-settings update`: corrigido o problema em que `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="4b722-1798">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="4b722-1799">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="4b722-1799">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="4b722-1800">Perfil</span><span class="sxs-lookup"><span data-stu-id="4b722-1800">Profile</span></span>

* <span data-ttu-id="4b722-1801">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="4b722-1801">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-1802">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-1802">Storage</span></span>

* <span data-ttu-id="4b722-1803">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="4b722-1803">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-1804">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-1804">VM</span></span>

* <span data-ttu-id="4b722-1805">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="4b722-1805">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="4b722-1806">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="4b722-1806">Exposed `list-skus` command</span></span>
* <span data-ttu-id="4b722-1807">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="4b722-1807">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="4b722-1808">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="4b722-1808">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="4b722-1809">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="4b722-1809">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="4b722-1810">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="4b722-1810">July 28, 2017</span></span>

<span data-ttu-id="4b722-1811">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="4b722-1811">Version 2.0.12</span></span>

* <span data-ttu-id="4b722-1812">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-1812">Added container commands</span></span>
* <span data-ttu-id="4b722-1813">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="4b722-1813">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="4b722-1814">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-1814">Core</span></span>

* <span data-ttu-id="4b722-1815">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="4b722-1815">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="4b722-1816">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="4b722-1816">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="4b722-1817">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="4b722-1817">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="4b722-1818">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="4b722-1818">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="4b722-1819">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="4b722-1819">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="4b722-1820">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="4b722-1820">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="4b722-1821">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="4b722-1821">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="4b722-1822">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="4b722-1822">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="4b722-1823">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="4b722-1823">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="4b722-1824">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="4b722-1824">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="4b722-1825">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="4b722-1825">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="4b722-1826">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="4b722-1826">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="4b722-1827">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="4b722-1827">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="4b722-1828">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="4b722-1828">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="4b722-1829">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="4b722-1829">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="4b722-1830">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="4b722-1830">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="4b722-1831">ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-1831">ACR</span></span>

* <span data-ttu-id="4b722-1832">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="4b722-1832">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="4b722-1833">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="4b722-1833">Support SKU update for managed registries</span></span>
* <span data-ttu-id="4b722-1834">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="4b722-1834">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="4b722-1835">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-1835">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="4b722-1836">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-1836">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="4b722-1837">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="4b722-1837">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-1838">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-1838">ACS</span></span>

* <span data-ttu-id="4b722-1839">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="4b722-1839">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-1840">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-1840">Appservice</span></span>

* <span data-ttu-id="4b722-1841">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="4b722-1841">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="4b722-1842">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="4b722-1842">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="4b722-1843">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="4b722-1843">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="4b722-1844">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="4b722-1844">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="4b722-1845">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="4b722-1845">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="4b722-1846">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="4b722-1846">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="4b722-1847">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="4b722-1847">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="4b722-1848">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="4b722-1848">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="4b722-1849">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="4b722-1849">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="4b722-1850">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="4b722-1850">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="4b722-1851">Lote</span><span class="sxs-lookup"><span data-stu-id="4b722-1851">Batch</span></span>

* <span data-ttu-id="4b722-1852">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="4b722-1852">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="4b722-1853">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="4b722-1853">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="4b722-1854">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="4b722-1854">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="4b722-1855">CDN</span><span class="sxs-lookup"><span data-stu-id="4b722-1855">CDN</span></span>

* <span data-ttu-id="4b722-1856">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="4b722-1856">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="4b722-1857">Nuvem</span><span class="sxs-lookup"><span data-stu-id="4b722-1857">Cloud</span></span>

* <span data-ttu-id="4b722-1858">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="4b722-1858">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="4b722-1859">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="4b722-1859">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="4b722-1860">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="4b722-1860">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="4b722-1861">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="4b722-1861">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="4b722-1862">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="4b722-1862">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4b722-1863">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4b722-1863">CosmosDB</span></span>

* <span data-ttu-id="4b722-1864">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="4b722-1864">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="4b722-1865">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="4b722-1865">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4b722-1866">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4b722-1866">Data Lake Analytics</span></span>

* <span data-ttu-id="4b722-1867">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="4b722-1867">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="4b722-1868">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="4b722-1868">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="4b722-1869">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="4b722-1869">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4b722-1870">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4b722-1870">Data Lake Store</span></span>

* <span data-ttu-id="4b722-1871">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1871">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="4b722-1872">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="4b722-1872">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="4b722-1873">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="4b722-1873">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="4b722-1874">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4b722-1874">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="4b722-1875">Interativo</span><span class="sxs-lookup"><span data-stu-id="4b722-1875">Interactive</span></span>

* <span data-ttu-id="4b722-1876">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="4b722-1876">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="4b722-1877">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="4b722-1877">Increased test coverage</span></span>
* <span data-ttu-id="4b722-1878">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="4b722-1878">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="4b722-1879">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="4b722-1879">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="4b722-1880">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="4b722-1880">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="4b722-1881">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="4b722-1881">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="4b722-1882">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="4b722-1882">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="4b722-1883">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="4b722-1883">Added `--progress` flag</span></span>
* <span data-ttu-id="4b722-1884">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="4b722-1884">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="4b722-1885">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="4b722-1885">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="4b722-1886">IoT</span><span class="sxs-lookup"><span data-stu-id="4b722-1886">IoT</span></span>

* <span data-ttu-id="4b722-1887">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="4b722-1887">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="4b722-1888">(#3934)</span><span class="sxs-lookup"><span data-stu-id="4b722-1888">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="4b722-1889">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="4b722-1889">Key vault</span></span>

* <span data-ttu-id="4b722-1890">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="4b722-1890">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="4b722-1891">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="4b722-1891">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="4b722-1892">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="4b722-1892">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="4b722-1893">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="4b722-1893">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="4b722-1894">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="4b722-1894">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="4b722-1895">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="4b722-1895">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="4b722-1896">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="4b722-1896">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="4b722-1897">(#3307)</span><span class="sxs-lookup"><span data-stu-id="4b722-1897">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="4b722-1898">Laboratório</span><span class="sxs-lookup"><span data-stu-id="4b722-1898">Lab</span></span>

* <span data-ttu-id="4b722-1899">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="4b722-1899">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="4b722-1900">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="4b722-1900">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="4b722-1901">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="4b722-1901">Monitor</span></span>

* <span data-ttu-id="4b722-1902">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="4b722-1902">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="4b722-1903">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="4b722-1903">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="4b722-1904">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="4b722-1904">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="4b722-1905">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="4b722-1905">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="4b722-1906">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="4b722-1906">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="4b722-1907">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="4b722-1907">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="4b722-1908">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="4b722-1908">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="4b722-1909">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="4b722-1909">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="4b722-1910">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="4b722-1910">`location` no longer required</span></span>
  * <span data-ttu-id="4b722-1911">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="4b722-1911">Add name and ID support for target</span></span>
  * <span data-ttu-id="4b722-1912">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="4b722-1912">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="4b722-1913">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="4b722-1913">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="4b722-1914">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="4b722-1914">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="4b722-1915">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="4b722-1915">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="4b722-1916">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="4b722-1916">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="4b722-1917">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1917">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="4b722-1918">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-1918">Network</span></span>

* <span data-ttu-id="4b722-1919">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="4b722-1919">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="4b722-1920">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1920">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="4b722-1921">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="4b722-1921">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="4b722-1922">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="4b722-1922">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="4b722-1923">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1923">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="4b722-1924">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="4b722-1924">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="4b722-1925">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="4b722-1925">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="4b722-1926">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="4b722-1926">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="4b722-1927">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="4b722-1927">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="4b722-1928">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="4b722-1928">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="4b722-1929">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1929">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="4b722-1930">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="4b722-1930">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="4b722-1931">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="4b722-1931">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="4b722-1932">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1932">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="4b722-1933">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1933">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="4b722-1934">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1934">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="4b722-1935">Adicionado o suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para --dns-servers</span><span class="sxs-lookup"><span data-stu-id="4b722-1935">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="4b722-1936">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="4b722-1936">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="4b722-1937">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1937">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="4b722-1938">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1938">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="4b722-1939">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1939">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="4b722-1940">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="4b722-1940">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="4b722-1941">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="4b722-1941">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="4b722-1942">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="4b722-1942">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="4b722-1943">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="4b722-1943">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="4b722-1944">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="4b722-1944">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="4b722-1945">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="4b722-1945">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="4b722-1946">Perfil</span><span class="sxs-lookup"><span data-stu-id="4b722-1946">Profile</span></span>

* <span data-ttu-id="4b722-1947">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="4b722-1947">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="4b722-1948">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="4b722-1948">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="4b722-1949">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="4b722-1949">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="4b722-1950">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="4b722-1950">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="4b722-1951">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="4b722-1951">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="4b722-1952">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4b722-1952">RDBMS</span></span>

* <span data-ttu-id="4b722-1953">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="4b722-1953">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="4b722-1954">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="4b722-1954">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="4b722-1955">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="4b722-1955">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="4b722-1956">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="4b722-1956">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="4b722-1957">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-1957">Resource</span></span>

* <span data-ttu-id="4b722-1958">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="4b722-1958">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="4b722-1959">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="4b722-1959">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="4b722-1960">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="4b722-1960">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="4b722-1961">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="4b722-1961">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="4b722-1962">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="4b722-1962">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="4b722-1963">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="4b722-1963">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="4b722-1964">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="4b722-1964">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="4b722-1965">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="4b722-1965">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="4b722-1966">Função</span><span class="sxs-lookup"><span data-stu-id="4b722-1966">Role</span></span>

* <span data-ttu-id="4b722-1967">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="4b722-1967">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="4b722-1968">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="4b722-1968">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="4b722-1969">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="4b722-1969">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="4b722-1970">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="4b722-1970">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="4b722-1971">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="4b722-1971">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4b722-1972">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4b722-1972">Service Fabric</span></span>
* <span data-ttu-id="4b722-1973">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="4b722-1973">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="4b722-1974">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="4b722-1974">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="4b722-1975">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="4b722-1975">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="4b722-1976">SQL</span><span class="sxs-lookup"><span data-stu-id="4b722-1976">SQL</span></span>

* <span data-ttu-id="4b722-1977">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="4b722-1977">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="4b722-1978">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="4b722-1978">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="4b722-1979">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="4b722-1979">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-1980">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-1980">Storage</span></span>

* <span data-ttu-id="4b722-1981">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="4b722-1981">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="4b722-1982">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="4b722-1982">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="4b722-1983">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="4b722-1983">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="4b722-1984">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="4b722-1984">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="4b722-1985">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="4b722-1985">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="4b722-1986">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="4b722-1986">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-1987">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-1987">VM</span></span>

* <span data-ttu-id="4b722-1988">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="4b722-1988">Support configuring nsg</span></span>
* <span data-ttu-id="4b722-1989">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="4b722-1989">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="4b722-1990">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="4b722-1990">Support managed service identities</span></span>
* <span data-ttu-id="4b722-1991">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="4b722-1991">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="4b722-1992">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="4b722-1992">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="4b722-1993">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="4b722-1993">May 10, 2017</span></span>

<span data-ttu-id="4b722-1994">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="4b722-1994">Version 2.0.6</span></span>

* <span data-ttu-id="4b722-1995">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4b722-1995">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="4b722-1996">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="4b722-1996">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="4b722-1997">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4b722-1997">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="4b722-1998">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="4b722-1998">Include Cognitive Services module</span></span>
* <span data-ttu-id="4b722-1999">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4b722-1999">Include Service Fabric module</span></span>
* <span data-ttu-id="4b722-2000">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="4b722-2000">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="4b722-2001">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="4b722-2001">Add support for CDN commands</span></span>
* <span data-ttu-id="4b722-2002">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="4b722-2002">Remove Container module</span></span>
* <span data-ttu-id="4b722-2003">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="4b722-2003">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="4b722-2004">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="4b722-2004">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="4b722-2005">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-2005">Core</span></span>

* <span data-ttu-id="4b722-2006">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="4b722-2006">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="4b722-2007">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="4b722-2007">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="4b722-2008">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="4b722-2008">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="4b722-2009">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="4b722-2009">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="4b722-2010">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="4b722-2010">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="4b722-2011">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="4b722-2011">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="4b722-2012">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="4b722-2012">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="4b722-2013">núcleo: permitir que o caminho do arquivo accessTokens.json seja configurável por meio de uma variável de ambiente ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="4b722-2013">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="4b722-2014">núcleo: permitir que padrões configurados sejam aplicados em argumentos opcionais ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="4b722-2014">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="4b722-2015">núcleo: desempenho aprimorado</span><span class="sxs-lookup"><span data-stu-id="4b722-2015">core: Improved performance</span></span>
* <span data-ttu-id="4b722-2016">núcleo: certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="4b722-2016">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="4b722-2017">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="4b722-2017">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-2018">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-2018">ACS</span></span>

* <span data-ttu-id="4b722-2019">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b722-2019">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="4b722-2020">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="4b722-2020">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="4b722-2021">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="4b722-2021">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="4b722-2022">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="4b722-2022">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-2023">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-2023">AppService</span></span>

* <span data-ttu-id="4b722-2024">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="4b722-2024">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="4b722-2025">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="4b722-2025">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="4b722-2026">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="4b722-2026">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="4b722-2027">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="4b722-2027">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="4b722-2028">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="4b722-2028">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="4b722-2029">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="4b722-2029">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="4b722-2030">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="4b722-2030">support slot swap with preview</span></span>
* <span data-ttu-id="4b722-2031">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="4b722-2031">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="4b722-2032">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="4b722-2032">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4b722-2033">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4b722-2033">CosmosDB</span></span>

* <span data-ttu-id="4b722-2034">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4b722-2034">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="4b722-2035">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="4b722-2035">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="4b722-2036">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="4b722-2036">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="4b722-2037">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="4b722-2037">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4b722-2038">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4b722-2038">Data Lake Analytics</span></span>

* <span data-ttu-id="4b722-2039">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="4b722-2039">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="4b722-2040">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="4b722-2040">Add support for new catalog item type: package.</span></span> <span data-ttu-id="4b722-2041">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="4b722-2041">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="4b722-2042">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="4b722-2042">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="4b722-2043">Tabela</span><span class="sxs-lookup"><span data-stu-id="4b722-2043">Table</span></span>
  * <span data-ttu-id="4b722-2044">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="4b722-2044">Table valued function</span></span>
  * <span data-ttu-id="4b722-2045">Visualizar</span><span class="sxs-lookup"><span data-stu-id="4b722-2045">View</span></span>
  * <span data-ttu-id="4b722-2046">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="4b722-2046">Table Statistics.</span></span> <span data-ttu-id="4b722-2047">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="4b722-2047">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4b722-2048">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4b722-2048">Data Lake Store</span></span>

* <span data-ttu-id="4b722-2049">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="4b722-2049">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="4b722-2050">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="4b722-2050">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="4b722-2051">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="4b722-2051">missed help for access show.</span></span> <span data-ttu-id="4b722-2052">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="4b722-2052">adding it.</span></span> <span data-ttu-id="4b722-2053">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="4b722-2053">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="4b722-2054">Localizar</span><span class="sxs-lookup"><span data-stu-id="4b722-2054">Find</span></span>

* <span data-ttu-id="4b722-2055">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="4b722-2055">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b722-2056">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4b722-2056">KeyVault</span></span>

* <span data-ttu-id="4b722-2057">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="4b722-2057">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="4b722-2058">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois estes parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="4b722-2058">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="4b722-2059">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="4b722-2059">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="4b722-2060">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="4b722-2060">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="4b722-2061">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="4b722-2061">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="4b722-2062">Laboratório</span><span class="sxs-lookup"><span data-stu-id="4b722-2062">Lab</span></span>

* <span data-ttu-id="4b722-2063">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="4b722-2063">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="4b722-2064">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="4b722-2064">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="4b722-2065">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="4b722-2065">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="4b722-2066">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="4b722-2066">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="4b722-2067">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="4b722-2067">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="4b722-2068">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="4b722-2068">Monitor</span></span>

* <span data-ttu-id="4b722-2069">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="4b722-2069">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="4b722-2070">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="4b722-2070">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="4b722-2071">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-2071">Network</span></span>

* <span data-ttu-id="4b722-2072">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="4b722-2072">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="4b722-2073">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="4b722-2073">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="4b722-2074">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b722-2074">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="4b722-2075">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b722-2075">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="4b722-2076">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="4b722-2076">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="4b722-2077">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="4b722-2077">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="4b722-2078">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="4b722-2078">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="4b722-2079">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="4b722-2079">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="4b722-2080">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="4b722-2080">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="4b722-2081">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="4b722-2081">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="4b722-2082">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="4b722-2082">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="4b722-2083">BC: corrigido um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="4b722-2083">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="4b722-2084">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="4b722-2084">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="4b722-2085">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="4b722-2085">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="4b722-2086">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="4b722-2086">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="4b722-2087">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="4b722-2087">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="4b722-2088">Perfil</span><span class="sxs-lookup"><span data-stu-id="4b722-2088">Profile</span></span>

* <span data-ttu-id="4b722-2089">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="4b722-2089">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="4b722-2090">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="4b722-2090">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="4b722-2091">Redis</span><span class="sxs-lookup"><span data-stu-id="4b722-2091">Redis</span></span>

* <span data-ttu-id="4b722-2092">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="4b722-2092">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="4b722-2093">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="4b722-2093">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="4b722-2094">Recurso</span><span class="sxs-lookup"><span data-stu-id="4b722-2094">Resource</span></span>

* <span data-ttu-id="4b722-2095">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="4b722-2095">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="4b722-2096">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="4b722-2096">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="4b722-2097">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="4b722-2097">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="4b722-2098">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="4b722-2098">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="4b722-2099">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="4b722-2099">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="4b722-2100">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="4b722-2100">Add docs for az lock update.</span></span> <span data-ttu-id="4b722-2101">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="4b722-2101">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="4b722-2102">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="4b722-2102">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="4b722-2103">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="4b722-2103">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="4b722-2104">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="4b722-2104">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="4b722-2105">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="4b722-2105">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="4b722-2106">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="4b722-2106">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="4b722-2107">Função</span><span class="sxs-lookup"><span data-stu-id="4b722-2107">Role</span></span>

* <span data-ttu-id="4b722-2108">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="4b722-2108">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="4b722-2109">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="4b722-2109">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="4b722-2110">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="4b722-2110">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="4b722-2111">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="4b722-2111">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="4b722-2112">SQL</span><span class="sxs-lookup"><span data-stu-id="4b722-2112">SQL</span></span>

* <span data-ttu-id="4b722-2113">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="4b722-2113">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="4b722-2114">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="4b722-2114">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="4b722-2115">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-2115">Storage</span></span>

* <span data-ttu-id="4b722-2116">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="4b722-2116">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="4b722-2117">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="4b722-2117">Add support for incremental blob copy</span></span>
* <span data-ttu-id="4b722-2118">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="4b722-2118">Add support for large block blob upload</span></span>
* <span data-ttu-id="4b722-2119">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="4b722-2119">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-2120">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-2120">VM</span></span>

* <span data-ttu-id="4b722-2121">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="4b722-2121">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="4b722-2122">observação: em comandos da VM em nuvens soberanas, evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="4b722-2122">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="4b722-2123">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="4b722-2123">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="4b722-2124">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="4b722-2124">az vm/vmss disk</span></span>
  3. <span data-ttu-id="4b722-2125">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="4b722-2125">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="4b722-2126">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="4b722-2126">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="4b722-2127">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="4b722-2127">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="4b722-2128">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="4b722-2128">April 3, 2017</span></span>

<span data-ttu-id="4b722-2129">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="4b722-2129">Version 2.0.2</span></span>

<span data-ttu-id="4b722-2130">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="4b722-2130">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="4b722-2131">Núcleo</span><span class="sxs-lookup"><span data-stu-id="4b722-2131">Core</span></span>

* <span data-ttu-id="4b722-2132">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="4b722-2132">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="4b722-2133">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="4b722-2133">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="4b722-2134">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="4b722-2134">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="4b722-2135">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="4b722-2135">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="4b722-2136">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="4b722-2136">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="4b722-2137">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="4b722-2137">Add prompting for missing template parameters.</span></span> <span data-ttu-id="4b722-2138">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="4b722-2138">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="4b722-2139">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="4b722-2139">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="4b722-2140">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="4b722-2140">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="4b722-2141">ACS</span><span class="sxs-lookup"><span data-stu-id="4b722-2141">ACS</span></span>

* <span data-ttu-id="4b722-2142">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="4b722-2142">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="4b722-2143">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="4b722-2143">Add support for ssh key password prompting.</span></span> <span data-ttu-id="4b722-2144">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="4b722-2144">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="4b722-2145">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="4b722-2145">Add support for windows clusters.</span></span> <span data-ttu-id="4b722-2146">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="4b722-2146">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="4b722-2147">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="4b722-2147">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="4b722-2148">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="4b722-2148">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="4b722-2149">AppService</span><span class="sxs-lookup"><span data-stu-id="4b722-2149">AppService</span></span>

* <span data-ttu-id="4b722-2150">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="4b722-2150">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="4b722-2151">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="4b722-2151">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="4b722-2152">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="4b722-2152">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="4b722-2153">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="4b722-2153">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="4b722-2154">DataLake</span><span class="sxs-lookup"><span data-stu-id="4b722-2154">DataLake</span></span>

* <span data-ttu-id="4b722-2155">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4b722-2155">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="4b722-2156">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4b722-2156">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="4b722-2157">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="4b722-2157">DocuemntDB</span></span>

* <span data-ttu-id="4b722-2158">DocumentDB: adicionado suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="4b722-2158">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="4b722-2159">VM</span><span class="sxs-lookup"><span data-stu-id="4b722-2159">VM</span></span>

* <span data-ttu-id="4b722-2160">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="4b722-2160">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="4b722-2161">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="4b722-2161">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="4b722-2162">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="4b722-2162">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="4b722-2163">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="4b722-2163">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="4b722-2164">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="4b722-2164">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="4b722-2165">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="4b722-2165">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="4b722-2166">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="4b722-2166">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="4b722-2167">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="4b722-2167">February 27, 2017</span></span>

<span data-ttu-id="4b722-2168">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="4b722-2168">Version 2.0.0</span></span>

<span data-ttu-id="4b722-2169">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="4b722-2169">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="4b722-2170">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="4b722-2170">Container Service (acs)</span></span>
- <span data-ttu-id="4b722-2171">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="4b722-2171">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="4b722-2172">Rede</span><span class="sxs-lookup"><span data-stu-id="4b722-2172">Networking</span></span>
- <span data-ttu-id="4b722-2173">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="4b722-2173">Storage</span></span>

<span data-ttu-id="4b722-2174">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="4b722-2174">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="4b722-2175">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="4b722-2175">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="4b722-2176">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="4b722-2176">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="4b722-2177">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="4b722-2177">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="4b722-2178">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="4b722-2178">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="4b722-2179">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="4b722-2179">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="4b722-2180">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="4b722-2180">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="4b722-2181">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="4b722-2181">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="4b722-2182">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="4b722-2182">Provide feedback from the command line with the `az feedback` command</span></span>

