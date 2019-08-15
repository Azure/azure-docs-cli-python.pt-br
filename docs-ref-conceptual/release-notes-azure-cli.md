---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 08/13/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: d315046287a552e89112fa415e1219f9a97d4944
ms.sourcegitcommit: b00555c528697c0a6419cf23380e48c8705026db
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "68974271"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="7938c-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="7938c-103">Azure CLI release notes</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="7938c-104">13 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="7938c-104">August 13, 2019</span></span>

<span data-ttu-id="7938c-105">Versão 2.0.71</span><span class="sxs-lookup"><span data-stu-id="7938c-105">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-106">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-106">AppService</span></span>

* <span data-ttu-id="7938c-107">Um problema de falha de slots com os comandos `webapp webjob continuous` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="7938c-107">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="7938c-108">BotService</span><span class="sxs-lookup"><span data-stu-id="7938c-108">BotService</span></span>

* <span data-ttu-id="7938c-109">[ALTERAÇÃO SIGNIFICATIVA] O suporte para a criação de bots SDK v3 foi removido</span><span class="sxs-lookup"><span data-stu-id="7938c-109">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="7938c-110">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="7938c-110">CognitiveServices</span></span>

* <span data-ttu-id="7938c-111">Adicionados os comandos `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="7938c-111">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="7938c-112">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7938c-112">Cosmos DB</span></span>

* <span data-ttu-id="7938c-113">Removido o aviso ao atualizar vários locais de gravação</span><span class="sxs-lookup"><span data-stu-id="7938c-113">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="7938c-114">Foram adicionados os comandos CRUD para o CosmosDB SQL, MongoDB, Cassandra, Gremlin e Recursos de tabela e taxa de transferência do recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-114">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7938c-115">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7938c-115">HDInsight</span></span>

<span data-ttu-id="7938c-116">Esta versão contém um grande número de alterações da falha.</span><span class="sxs-lookup"><span data-stu-id="7938c-116">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="7938c-117">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="7938c-117">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="7938c-118">`--storage-default-container` renomeado para `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="7938c-118">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="7938c-119">`--storage-default-filesystem` renomeado para `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="7938c-119">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="7938c-120">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--name` de `application create` foi alterado para representar o nome do aplicativo em vez do nome do cluster</span><span class="sxs-lookup"><span data-stu-id="7938c-120">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="7938c-121">O argumento `--cluster-name` foi adicionado a `application create` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="7938c-121">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="7938c-122">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `application create`:</span><span class="sxs-lookup"><span data-stu-id="7938c-122">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="7938c-123">`--application-type` renomeado para `--type`</span><span class="sxs-lookup"><span data-stu-id="7938c-123">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="7938c-124">`--marketplace-identifier` renomeado para `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="7938c-124">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="7938c-125">`--https-endpoint-access-mode` renomeado para `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="7938c-125">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="7938c-126">Renomeado de `--https-endpoint-destination-port` para `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="7938c-126">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="7938c-127">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros removidos para `application create`:</span><span class="sxs-lookup"><span data-stu-id="7938c-127">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="7938c-128">[ALTERAÇÃO DA FALHA] Renomeado de `--target-instance-count` para `--workernode-count` para `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="7938c-128">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="7938c-129">[ALTERAÇÃO SIGNIFICATIVA] Todos os comandos no grupo `hdinsight script-action` foram alterados para usar o parâmetro `--name` como o nome da ação de script.</span><span class="sxs-lookup"><span data-stu-id="7938c-129">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="7938c-130">O argumento `--cluster-name` foi adicionado a todos os comandos `hdinsight script-action` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="7938c-130">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="7938c-131">[ALTERAÇÃO SIGNIFICATIVA] Renomeado de `--script-execution-id` para `--execution-id` para todos os comandos `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="7938c-131">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="7938c-132">[ALTERAÇÃO SIGNIFICATIVA] `hdinsight script-action show` renomeado para `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="7938c-132">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="7938c-133">[ALTERAÇÃO DA FALHA] Os parâmetros foram alterados para `hdinsight script-action execute --roles` para serem separados por espaços em vez de separados por vírgula</span><span class="sxs-lookup"><span data-stu-id="7938c-133">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="7938c-134">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro `--persisted` de `hdinsight script-action list` foi removido</span><span class="sxs-lookup"><span data-stu-id="7938c-134">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="7938c-135">O parâmetro `hdinsight create --cluster-configurations` foi alterado para aceitar um caminho para um arquivo JSON local ou uma cadeia de caracteres JSON</span><span class="sxs-lookup"><span data-stu-id="7938c-135">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="7938c-136">Adicionado o comando `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="7938c-136">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="7938c-137">Alterado `hdinsight monitor enable --workspace` para aceitar uma ID do workspace ou nome do workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="7938c-137">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="7938c-138">O argumento `hdinsight monitor enable --primary-key`, que será necessário caso uma ID do workspace seja fornecida como o parâmetro, foi adicionado</span><span class="sxs-lookup"><span data-stu-id="7938c-138">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="7938c-139">Foram adicionados mais exemplos e atualização das descrições das mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="7938c-139">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="7938c-140">Interativo</span><span class="sxs-lookup"><span data-stu-id="7938c-140">Interactive</span></span>

* <span data-ttu-id="7938c-141">Um erro no carregamento foi corrigido</span><span class="sxs-lookup"><span data-stu-id="7938c-141">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="7938c-142">kubernetes</span><span class="sxs-lookup"><span data-stu-id="7938c-142">Kubernetes</span></span>

* <span data-ttu-id="7938c-143">Alterado para usar `https` se a porta do contêiner do painel estiver usando `https`</span><span class="sxs-lookup"><span data-stu-id="7938c-143">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="7938c-144">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-144">Network</span></span>

* <span data-ttu-id="7938c-145">O argumento `--yes` foi adicionado a `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="7938c-145">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="7938c-146">Perfil</span><span class="sxs-lookup"><span data-stu-id="7938c-146">Profile</span></span>

* <span data-ttu-id="7938c-147">O argumento `--resource-type` foi adicionado a `account get-access-token` para obter tokens de acesso de recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-147">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="7938c-148">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7938c-148">ServiceFabric</span></span>

* <span data-ttu-id="7938c-149">Todas as versões de sistema operacional com suporte para criação do cluster sf foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="7938c-149">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="7938c-150">Foi corrigido o bug de validação do certificado primário</span><span class="sxs-lookup"><span data-stu-id="7938c-150">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-151">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-151">Storage</span></span>

* <span data-ttu-id="7938c-152">Adicionado o comando `storage copy`</span><span class="sxs-lookup"><span data-stu-id="7938c-152">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="7938c-153">30 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="7938c-153">July 30, 2019</span></span>

<span data-ttu-id="7938c-154">Versão 2.0.70</span><span class="sxs-lookup"><span data-stu-id="7938c-154">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-155">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-155">ACR</span></span>

* <span data-ttu-id="7938c-156">Corrigido o problema #9952 (uma regressão no comando `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="7938c-156">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="7938c-157">Removido o nome da imagem do construtor padrão em `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="7938c-157">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-158">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-158">Appservice</span></span>

* <span data-ttu-id="7938c-159">Alterado `webapp config ssl` para mostrar uma mensagem se um recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="7938c-159">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="7938c-160">Corrigido o problema em que `functionapp create` não aceita o tipo de conta de armazenamento `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="7938c-160">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="7938c-161">Corrigido um problema em que `webapp up` falharia se fosse executado usando versões mais antigas do Python</span><span class="sxs-lookup"><span data-stu-id="7938c-161">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="7938c-162">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-162">Network</span></span>

* <span data-ttu-id="7938c-163">Removido parâmetro inválido `--ids` de `network nic ip-config add` (corrige o #9861)</span><span class="sxs-lookup"><span data-stu-id="7938c-163">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="7938c-164">Corrige o #9604.</span><span class="sxs-lookup"><span data-stu-id="7938c-164">Fixes #9604.</span></span> <span data-ttu-id="7938c-165">Adicionado o parâmetro `--root-certs` ao `network application-gateway http-settings [create|update]` para dar suporte a certificados raiz confiáveis associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="7938c-165">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="7938c-166">Fixado argumento `--subscription` para `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="7938c-166">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="7938c-167">RBAC</span><span class="sxs-lookup"><span data-stu-id="7938c-167">RBAC</span></span>

* <span data-ttu-id="7938c-168">Adicionado o comando `user update`</span><span class="sxs-lookup"><span data-stu-id="7938c-168">Added `user update` command</span></span>
* <span data-ttu-id="7938c-169">[PRETERIDO] Preterido `--upn-or-object-id` de comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="7938c-169">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="7938c-170">Usar argumento de substituição `--id`</span><span class="sxs-lookup"><span data-stu-id="7938c-170">Use replacement argument `--id`</span></span>
* <span data-ttu-id="7938c-171">Adicionado argumento `--id` para comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="7938c-171">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-172">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-172">SQL</span></span>

* <span data-ttu-id="7938c-173">Adicionados comandos de gerenciamento para chaves de instância gerenciada e protetor de TDE</span><span class="sxs-lookup"><span data-stu-id="7938c-173">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-174">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-174">Storage</span></span>

* <span data-ttu-id="7938c-175">Adicionado o comando `storage remove`</span><span class="sxs-lookup"><span data-stu-id="7938c-175">Added `storage remove` command</span></span>
* <span data-ttu-id="7938c-176">Corrigido um problema com `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="7938c-176">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-177">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-177">VM</span></span>

* <span data-ttu-id="7938c-178">Alterado `list-skus` para usar versão de API mais recente a fim de externar detalhes de zona</span><span class="sxs-lookup"><span data-stu-id="7938c-178">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="7938c-179">Alterado o padrão de `--single-placement-group` para `false` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="7938c-179">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="7938c-180">Adicionada a capacidade de selecionar SKUs de armazenamento ZRS para `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="7938c-180">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="7938c-181">Adicionado novo grupo de comandos `vm host` para dar suporte a hosts dedicados</span><span class="sxs-lookup"><span data-stu-id="7938c-181">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="7938c-182">Adicionados parâmetros `--host` e `--host-group` em `vm create` para definir o host dedicado da VM</span><span class="sxs-lookup"><span data-stu-id="7938c-182">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="7938c-183">16 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="7938c-183">July 16, 2019</span></span>

<span data-ttu-id="7938c-184">Versão 2.0.69</span><span class="sxs-lookup"><span data-stu-id="7938c-184">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-185">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-185">Appservice</span></span>

* <span data-ttu-id="7938c-186">Os comandos `webapp identity` foram alterados para retornar uma mensagem de erro apropriada se o nome do aplicativo ou ResourceGroupName for inválido</span><span class="sxs-lookup"><span data-stu-id="7938c-186">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="7938c-187">`webapp list` corrigido para retornar o valor correto para numberOfSites se nenhum ResourceGroup foi fornecido</span><span class="sxs-lookup"><span data-stu-id="7938c-187">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="7938c-188">Corrigidos os efeitos colaterais de `appservice plan create` e `webapp create`</span><span class="sxs-lookup"><span data-stu-id="7938c-188">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="7938c-189">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-189">Core</span></span>

* <span data-ttu-id="7938c-190">Corrigido um problema em que `--subscription` aparecia apesar de não ser aplicável</span><span class="sxs-lookup"><span data-stu-id="7938c-190">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="7938c-191">Lote</span><span class="sxs-lookup"><span data-stu-id="7938c-191">Batch</span></span>

* <span data-ttu-id="7938c-192">[ALTERAÇÃO SIGNIFICATIVA] `batch pool node-agent-skus list` foi substituído por `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="7938c-192">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="7938c-193">Adicionado suporte para regras de segurança bloqueando o acesso de rede a um pool com base na porta de origem do tráfego ao usar a opção `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="7938c-193">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="7938c-194">Suporte adicionado para executar a tarefa no diretório de trabalho de contêiner ou no diretório de trabalho de tarefa em lotes ao usar a opção `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="7938c-194">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="7938c-195">Corrigido o erro na opção `--application-package-references` de `batch pool create` em que ela funcionaria apenas com padrões</span><span class="sxs-lookup"><span data-stu-id="7938c-195">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="7938c-196">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="7938c-196">Eventhubs</span></span>

* <span data-ttu-id="7938c-197">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="7938c-197">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="7938c-198">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7938c-198">RDBMS</span></span>

* <span data-ttu-id="7938c-199">Adicionado um parâmetro opcional para especificar a réplica de SKU para criar o comando de réplica</span><span class="sxs-lookup"><span data-stu-id="7938c-199">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="7938c-200">Corrigido o problema com a falha no teste de CI com a criação de réplica de MySQL</span><span class="sxs-lookup"><span data-stu-id="7938c-200">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="7938c-201">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="7938c-201">Relay</span></span>

* <span data-ttu-id="7938c-202">Corrigido o problema com a conexão híbrida quando a autorização do cliente desabilitava [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="7938c-202">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="7938c-203">Parâmetro `--requires-transport-security` adicionado a `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="7938c-203">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="7938c-204">Barramento de serviço</span><span class="sxs-lookup"><span data-stu-id="7938c-204">Servicebus</span></span>

* <span data-ttu-id="7938c-205">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="7938c-205">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-206">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-206">Storage</span></span>

* <span data-ttu-id="7938c-207">Habilitar AADDS de arquivos para atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-207">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="7938c-208">Problema corrigido `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="7938c-208">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="7938c-209">2 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="7938c-209">July 2, 2019</span></span>

<span data-ttu-id="7938c-210">Versão 2.0.68</span><span class="sxs-lookup"><span data-stu-id="7938c-210">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="7938c-211">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-211">Core</span></span>

* <span data-ttu-id="7938c-212">Agora, os módulos de comando são consolidados em um único Python distribuível.</span><span class="sxs-lookup"><span data-stu-id="7938c-212">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="7938c-213">Isso substitui o uso direto de muitos pacotes `azure-cli-` no PyPI.</span><span class="sxs-lookup"><span data-stu-id="7938c-213">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="7938c-214">Assim, o tamanho da instalação será reduzido e apenas os usuários que tiverem instalado diretamente por meio do `pip` serão afetados.</span><span class="sxs-lookup"><span data-stu-id="7938c-214">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-215">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-215">ACR</span></span>

* <span data-ttu-id="7938c-216">Foi adicionado o suporte para gatilhos de temporizador para tarefa</span><span class="sxs-lookup"><span data-stu-id="7938c-216">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-217">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-217">Appservice</span></span>

* <span data-ttu-id="7938c-218">O `functionapp create` foi alterado para habilitar o Application Insights por padrão</span><span class="sxs-lookup"><span data-stu-id="7938c-218">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="7938c-219">[ALTERAÇÃO SIGNIFICATIVA] Foi removido o comando `functionapp devops-build` preterido.</span><span class="sxs-lookup"><span data-stu-id="7938c-219">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="7938c-220">Agora, use o novo comando `az functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="7938c-220">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="7938c-221">Foi adicionado o suporte ao plano de aplicativo de funções Consumo em Linux ao `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="7938c-221">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="7938c-222">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7938c-222">Cosmos DB</span></span>

* <span data-ttu-id="7938c-223">Foi adicionado o suporte para desabilitar a TTL</span><span class="sxs-lookup"><span data-stu-id="7938c-223">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="7938c-224">DLS</span><span class="sxs-lookup"><span data-stu-id="7938c-224">DLS</span></span>

* <span data-ttu-id="7938c-225">Versão atualizada do ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="7938c-225">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="7938c-226">Comentários</span><span class="sxs-lookup"><span data-stu-id="7938c-226">Feedback</span></span>

* <span data-ttu-id="7938c-227">Ao relatar um comando de extensão com falha, agora, o `az feedback` tenta abrir o navegador na URL do projeto/repositório da extensão por meio do índice</span><span class="sxs-lookup"><span data-stu-id="7938c-227">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7938c-228">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7938c-228">HDInsight</span></span>

* <span data-ttu-id="7938c-229">[ALTERAÇÃO SIGNIFICATIVA] O nome do grupo de comandos `oms` foi alterado para `monitor`</span><span class="sxs-lookup"><span data-stu-id="7938c-229">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="7938c-230">[ALTERAÇÃO SIGNIFICATIVA] `--http-password/-p` tornou-se um parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="7938c-230">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="7938c-231">Foram adicionados preenchedores para o preenchedor dos parâmetros `--cluster-admin-account` e `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="7938c-231">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="7938c-232">O parâmetro `cluster-users-group-dns` foi alterado para ser obrigatório quando `—esp` estiver presente</span><span class="sxs-lookup"><span data-stu-id="7938c-232">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="7938c-233">Foi adicionado um tempo limite para todos os preenchedores automáticos de argumento existentes</span><span class="sxs-lookup"><span data-stu-id="7938c-233">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="7938c-234">Foi adicionado um tempo limite para transformar o nome do recurso na ID de recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-234">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="7938c-235">Os preenchedores automáticos foram alterados para selecionar recursos de qualquer grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="7938c-235">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="7938c-236">Pode ser um grupo de recursos diferente daquele especificado com `-g`</span><span class="sxs-lookup"><span data-stu-id="7938c-236">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="7938c-237">Foi adicionado o suporte para os parâmetros `--sub-domain-suffix` e `--disable_gateway_auth` no comando `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="7938c-237">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="7938c-238">Serviços gerenciados</span><span class="sxs-lookup"><span data-stu-id="7938c-238">Managed Services</span></span>

* <span data-ttu-id="7938c-239">Introdução ao módulo de comando de serviço gerenciado em versão prévia</span><span class="sxs-lookup"><span data-stu-id="7938c-239">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="7938c-240">Perfil</span><span class="sxs-lookup"><span data-stu-id="7938c-240">Profile</span></span>
* <span data-ttu-id="7938c-241">Suprimir o argumento `--subscription` para o comando de logoff</span><span class="sxs-lookup"><span data-stu-id="7938c-241">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="7938c-242">RBAC</span><span class="sxs-lookup"><span data-stu-id="7938c-242">RBAC</span></span>

* <span data-ttu-id="7938c-243">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--password` foi removido de `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="7938c-243">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="7938c-244">Foi adicionado o parâmetro `--assignee-principal-type` ao comando `create` para evitar falhas intermitentes causadas pela latência de replicação do servidor do AAD Graph</span><span class="sxs-lookup"><span data-stu-id="7938c-244">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="7938c-245">Foi corrigida uma falha em `ad signed-in-user` ao listar objetos de propriedade</span><span class="sxs-lookup"><span data-stu-id="7938c-245">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="7938c-246">Foi corrigido um problema em que o `ad sp` não localizava o aplicativo certo de uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="7938c-246">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="7938c-247">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7938c-247">RDBMS</span></span>

* <span data-ttu-id="7938c-248">Foi adicionado o suporte à replicação para o MariaDB</span><span class="sxs-lookup"><span data-stu-id="7938c-248">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-249">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-249">SQL</span></span>

* <span data-ttu-id="7938c-250">Valores permitidos documentados para `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="7938c-250">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-251">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-251">Storage</span></span>

* <span data-ttu-id="7938c-252">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="7938c-252">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="7938c-253">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="7938c-253">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="7938c-254">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-254">VM</span></span>

* <span data-ttu-id="7938c-255">Foi corrigido o bug em que o `vmss create` retornava uma mensagem de erro quando era executado com `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="7938c-255">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="7938c-256">Foi removida a validação do lado do cliente de `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="7938c-256">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="7938c-257">Não falha quando `--single-placement-group` é definido como `true` e `--instance-count` é maior que 100 ou quando são especificadas zonas de disponibilidade, mas deixa essa validação para o serviço de computação</span><span class="sxs-lookup"><span data-stu-id="7938c-257">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="7938c-258">Foi corrigido o bug em que o `[vm|vmss] extension image list` falhava quando era usado com `--latest`</span><span class="sxs-lookup"><span data-stu-id="7938c-258">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="7938c-259">18 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="7938c-259">June 18, 2019</span></span>

<span data-ttu-id="7938c-260">Versão 2.0.67</span><span class="sxs-lookup"><span data-stu-id="7938c-260">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="7938c-261">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-261">Core</span></span>

<span data-ttu-id="7938c-262">Esta versão apresenta uma nova marca [Versão prévia] para comunicar com mais clareza aos clientes quando um comando, um grupo de comandos ou um argumento está no status de versão prévia.</span><span class="sxs-lookup"><span data-stu-id="7938c-262">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="7938c-263">Anteriormente, essa informação era transmitida no texto de ajuda ou, implicitamente, pelo número da versão do módulo de comando.</span><span class="sxs-lookup"><span data-stu-id="7938c-263">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="7938c-264">A CLI removerá os números de versão dos pacotes individuais no futuro.</span><span class="sxs-lookup"><span data-stu-id="7938c-264">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="7938c-265">Se um comando estiver em versão prévia, todos os seus argumentos também estarão.</span><span class="sxs-lookup"><span data-stu-id="7938c-265">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="7938c-266">Se um grupo de comandos for rotulado com o status de versão prévia, então todos os seus comandos e argumentos também serão considerados em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="7938c-266">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="7938c-267">Como resultado dessa alteração, diversos grupos de comandos podem parecer surgir "de repente" com o status de versão prévia com esta liberação.</span><span class="sxs-lookup"><span data-stu-id="7938c-267">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="7938c-268">O que realmente aconteceu é que a maioria dos pacotes já estava com status de versão prévia, mas estão sendo consideradas GA com esta liberação</span><span class="sxs-lookup"><span data-stu-id="7938c-268">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-269">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-269">ACR</span></span>
* <span data-ttu-id="7938c-270">Adicionado o comando 'acr check-health'</span><span class="sxs-lookup"><span data-stu-id="7938c-270">Added 'acr check-health' command</span></span>
* <span data-ttu-id="7938c-271">Melhorado o tratamento de erro para tokens do AAD e para recuperar comandos externos</span><span class="sxs-lookup"><span data-stu-id="7938c-271">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-272">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-272">ACS</span></span>
* <span data-ttu-id="7938c-273">Comandos preteridos do ACS agora ficam ocultos da exibição da ajuda</span><span class="sxs-lookup"><span data-stu-id="7938c-273">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="7938c-274">AMS</span><span class="sxs-lookup"><span data-stu-id="7938c-274">AMS</span></span>
* <span data-ttu-id="7938c-275">[ALTERAÇÃO SIGNIFICATIVA] Alterada para retornar cadeias de caracteres de tempo da ISO 8601 para archive-window-length e key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="7938c-275">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-276">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-276">AppService</span></span>
* <span data-ttu-id="7938c-277">Adicionado roteamento com base no local para `webapp deleted list` e `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="7938c-277">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="7938c-278">Corrigido problema em que a URL de destino registrada do webapp ("Não é possível iniciar o aplicativo em...") não era clicável no Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="7938c-278">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="7938c-279">Corrigido um problema em que a criação de aplicativos com algumas SKUs falhava com um erro de AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="7938c-279">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="7938c-280">Adicionada a pré-validação para o `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="7938c-280">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="7938c-281">Corrigido o `[webapp|functionapp] traffic-routing` para usar o actionHostName correto</span><span class="sxs-lookup"><span data-stu-id="7938c-281">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="7938c-282">Adicionado o suporte de slot para comandos `functionapp`</span><span class="sxs-lookup"><span data-stu-id="7938c-282">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="7938c-283">Lote</span><span class="sxs-lookup"><span data-stu-id="7938c-283">Batch</span></span>
* <span data-ttu-id="7938c-284">Corrigida a regressão de autenticação do AAD causada pela geração de relatórios de erros superagressiva para autenticação de chave compartilhada</span><span class="sxs-lookup"><span data-stu-id="7938c-284">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="7938c-285">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7938c-285">BatchAI</span></span>
* <span data-ttu-id="7938c-286">Agora os comandos do BatchAI estão preteridos e ocultos</span><span class="sxs-lookup"><span data-stu-id="7938c-286">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="7938c-287">BotService</span><span class="sxs-lookup"><span data-stu-id="7938c-287">BotService</span></span>
* <span data-ttu-id="7938c-288">Adição das mensagens de aviso "suporte descontinuado"/"modo de manutenção" para os comandos compatíveis com a v3 do SDK</span><span class="sxs-lookup"><span data-stu-id="7938c-288">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7938c-289">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7938c-289">CosmosDB</span></span>
* <span data-ttu-id="7938c-290">[PRETERIDO] Preterido o comando `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="7938c-290">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="7938c-291">Adicionado o comando `cosmosdb keys list` – substitui o `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="7938c-291">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="7938c-292">`cosmsodb create/update`: Adicionado novo formato para --location a fim de permitir a configuração da propriedade "isZoneRedundant".</span><span class="sxs-lookup"><span data-stu-id="7938c-292">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="7938c-293">Formato antigo preterido</span><span class="sxs-lookup"><span data-stu-id="7938c-293">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="7938c-294">EventGrid</span><span class="sxs-lookup"><span data-stu-id="7938c-294">EventGrid</span></span>
* <span data-ttu-id="7938c-295">Adicionados comandos do `eventgrid domain` para operações de CRUD no domínio</span><span class="sxs-lookup"><span data-stu-id="7938c-295">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="7938c-296">Adicionados comandos do `eventgrid domain topic` para operações de CRUD nos tópicos do domínio</span><span class="sxs-lookup"><span data-stu-id="7938c-296">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="7938c-297">Adicionado argumento do `--odata-query` ao `eventgrid [topic|event-subscription] list` para filtrar os resultados usando a sintaxe do OData</span><span class="sxs-lookup"><span data-stu-id="7938c-297">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="7938c-298">`event-subscription create/update`: Adicionado o servicebusqueue como novos valores para o parâmetro `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="7938c-298">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="7938c-299">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para `--included-event-types All` com `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-299">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7938c-300">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7938c-300">HDInsight</span></span>
* <span data-ttu-id="7938c-301">Adicionado suporte para o parâmetro `--ssh-public-key` no comando `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="7938c-301">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="7938c-302">IoT</span><span class="sxs-lookup"><span data-stu-id="7938c-302">IoT</span></span>
* <span data-ttu-id="7938c-303">Adicionado suporte para regenerar as chaves da política de autorização</span><span class="sxs-lookup"><span data-stu-id="7938c-303">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="7938c-304">Adicionados SDK e suporte para o serviço de provisionamento de repositórios do DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="7938c-304">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="7938c-305">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-305">Network</span></span>
* <span data-ttu-id="7938c-306">Adicionado suporte de zona para o Gateway da NAT</span><span class="sxs-lookup"><span data-stu-id="7938c-306">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="7938c-307">Adicionado o comando `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="7938c-307">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="7938c-308">Corrigido o problema com o `dns zone import` em que os usuários não conseguiam importar registros do curinga A</span><span class="sxs-lookup"><span data-stu-id="7938c-308">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="7938c-309">Corrigido o problema com o `watcher flow-log configure` em que o registro de fluxo não podia ser habilitado em determinadas regiões</span><span class="sxs-lookup"><span data-stu-id="7938c-309">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-310">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-310">Resource</span></span>
* <span data-ttu-id="7938c-311">Adicionado o comando do `az rest` para fazer chamadas REST</span><span class="sxs-lookup"><span data-stu-id="7938c-311">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="7938c-312">Corrigido o erro ao usar o `policy assignment list` com um grupo de recursos ou o nível de assinatura `--scope`</span><span class="sxs-lookup"><span data-stu-id="7938c-312">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="7938c-313">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7938c-313">ServiceBus</span></span>
* <span data-ttu-id="7938c-314">Corrigido o problema com o `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="7938c-314">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-315">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-315">SQL</span></span>
* <span data-ttu-id="7938c-316">Alterado o `--location` para ser opcional para `sql [server|mi] create` – usa o local do grupo de recursos se não especificado</span><span class="sxs-lookup"><span data-stu-id="7938c-316">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="7938c-317">Corrigido o erro "objeto 'NoneType' não é iterável" para `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="7938c-317">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="7938c-318">SQLVm</span><span class="sxs-lookup"><span data-stu-id="7938c-318">SQLVm</span></span>
* <span data-ttu-id="7938c-319">[ALTERAÇÃO DA FALHA] Alterado `sql vm create` para exigir o parâmetro `--license-type`</span><span class="sxs-lookup"><span data-stu-id="7938c-319">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="7938c-320">Alterado para permitir a configuração da SKU da imagem do SQL ao criar ou atualizar uma VM do SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-320">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-321">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-321">Storage</span></span>
* <span data-ttu-id="7938c-322">Corrigido o problema com a chave de conta ignorada para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="7938c-322">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="7938c-323">Corrigido o problema com o `storage blob sync` no Linux</span><span class="sxs-lookup"><span data-stu-id="7938c-323">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-324">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-324">VM</span></span>
* <span data-ttu-id="7938c-325">[VERSÃO PRÉVIA] Adicionados os comandos `vm image template` para criar imagens de VM</span><span class="sxs-lookup"><span data-stu-id="7938c-325">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="7938c-326">4 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="7938c-326">June 4, 2019</span></span>

<span data-ttu-id="7938c-327">Versão 2.0.66</span><span class="sxs-lookup"><span data-stu-id="7938c-327">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="7938c-328">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-328">Core</span></span>
* <span data-ttu-id="7938c-329">Foi corrigido o bug em que os comandos falhavam quando `--output yaml` era usado com `--query`</span><span class="sxs-lookup"><span data-stu-id="7938c-329">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-330">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-330">ACR</span></span>
* <span data-ttu-id="7938c-331">Foi adicionado o grupo de comando 'pack acr' para a criação de Tarefas de build rápida usando Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="7938c-331">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-332">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-332">ACS</span></span>
* <span data-ttu-id="7938c-333">Permitir a opção de habilitar/desabilitar o complemento kube-dashboard do AKS</span><span class="sxs-lookup"><span data-stu-id="7938c-333">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="7938c-334">Imprimir uma mensagem amigável quando a assinatura não estiver na lista de permissões para usar o Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="7938c-334">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="7938c-335">Lote</span><span class="sxs-lookup"><span data-stu-id="7938c-335">Batch</span></span>
* <span data-ttu-id="7938c-336">Melhoria no tratamento de erro quando você não está conectado a uma conta \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="7938c-336">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="7938c-337">IoT</span><span class="sxs-lookup"><span data-stu-id="7938c-337">IoT</span></span>
* <span data-ttu-id="7938c-338">Foi adicionado o suporte para failover manual</span><span class="sxs-lookup"><span data-stu-id="7938c-338">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="7938c-339">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-339">Network</span></span>
* <span data-ttu-id="7938c-340">Foram adicionados os comandos `network application-gateway waf-policy` para oferecer suporte às regras de WAF personalizadas.</span><span class="sxs-lookup"><span data-stu-id="7938c-340">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="7938c-341">Adicionados os argumentos `--waf-policy` e `--max-capacity` para `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-341">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="7938c-342">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-342">Resource</span></span>
* <span data-ttu-id="7938c-343">Melhoria da mensagem de erro do `deployment create` quando não há nenhum TTY disponível</span><span class="sxs-lookup"><span data-stu-id="7938c-343">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="7938c-344">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-344">Role</span></span>
* <span data-ttu-id="7938c-345">O texto da Ajuda foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="7938c-345">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="7938c-346">Computação</span><span class="sxs-lookup"><span data-stu-id="7938c-346">Compute</span></span>
* <span data-ttu-id="7938c-347">Foi adicionado o suporte para `vm create` para as VMs de uma imagem gerenciada com LUNs de disco de dados que não começam em 0 ou que ignoram números</span><span class="sxs-lookup"><span data-stu-id="7938c-347">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="7938c-348">21 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="7938c-348">May 21, 2019</span></span>

<span data-ttu-id="7938c-349">Versão 2.0.65</span><span class="sxs-lookup"><span data-stu-id="7938c-349">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="7938c-350">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-350">Core</span></span>
* <span data-ttu-id="7938c-351">Foram adicionados comentários melhores para erros de autenticação</span><span class="sxs-lookup"><span data-stu-id="7938c-351">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="7938c-352">Corrigido um problema em que a CLI carregava extensões que não eram compatíveis com a versão do núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-352">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="7938c-353">Corrigido um problema com a inicialização quando `clouds.config` está corrompido</span><span class="sxs-lookup"><span data-stu-id="7938c-353">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-354">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-354">ACR</span></span>
* <span data-ttu-id="7938c-355">Foi adicionado suporte das Identidades Gerenciadas para Tarefas</span><span class="sxs-lookup"><span data-stu-id="7938c-355">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-356">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-356">ACS</span></span>
* <span data-ttu-id="7938c-357">Corrigido o comando `openshift create` quando usado com o cliente AAD do consumidor</span><span class="sxs-lookup"><span data-stu-id="7938c-357">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-358">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-358">AppService</span></span>
* <span data-ttu-id="7938c-359">[PRETERIDO] Preterido o comando `functionapp devops-build` – Será removido na próxima versão</span><span class="sxs-lookup"><span data-stu-id="7938c-359">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="7938c-360">`functionapp devops-pipeline` foi alterado para buscar o log de build do Azure DevOps no modo detalhado</span><span class="sxs-lookup"><span data-stu-id="7938c-360">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="7938c-361">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--use_local_settings` foi removido do comando `functionapp devops-pipeline` – não estava operacional</span><span class="sxs-lookup"><span data-stu-id="7938c-361">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="7938c-362">`webapp up` foi alterado para retornar uma saída JSON se `--logs` não for usado</span><span class="sxs-lookup"><span data-stu-id="7938c-362">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="7938c-363">Foi adicionado suporte para escrever recursos padrão para a configuração local de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="7938c-363">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="7938c-364">Foi adicionado suporte para `webapp up` reimplantar um aplicativo sem usar o argumento `--location`</span><span class="sxs-lookup"><span data-stu-id="7938c-364">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="7938c-365">Corrigido um problema em que o valor do SKU gratuito não funcionava na criação do ASP do SKU gratuito do Linux</span><span class="sxs-lookup"><span data-stu-id="7938c-365">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="7938c-366">BotService</span><span class="sxs-lookup"><span data-stu-id="7938c-366">BotService</span></span>
* <span data-ttu-id="7938c-367">Alterado para permitir todas as capitalizações para parâmetros `--lang` em todos os comandos</span><span class="sxs-lookup"><span data-stu-id="7938c-367">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="7938c-368">Descrição atualizada do módulo de comando</span><span class="sxs-lookup"><span data-stu-id="7938c-368">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="7938c-369">Consumo</span><span class="sxs-lookup"><span data-stu-id="7938c-369">Consumption</span></span>
* <span data-ttu-id="7938c-370">O parâmetro obrigatório ausente foi adicionado para executar `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="7938c-370">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="7938c-371">IoT</span><span class="sxs-lookup"><span data-stu-id="7938c-371">IoT</span></span>
* <span data-ttu-id="7938c-372">Suporte adicionado para listar todas as chaves</span><span class="sxs-lookup"><span data-stu-id="7938c-372">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="7938c-373">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-373">Network</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="7938c-375">O argumento `--nat-gateway` foi adicionado a `network vnet subnet [create|update]` para anexar a um gateway NAT</span><span class="sxs-lookup"><span data-stu-id="7938c-375">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="7938c-376">Corrigido o problema de `dns zone import`, em que os nomes de registro não correspondiam ao tipo de registro</span><span class="sxs-lookup"><span data-stu-id="7938c-376">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="7938c-377">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7938c-377">RDBMS</span></span>
* <span data-ttu-id="7938c-378">Suporte a postgres e mysql adicionado para replicação geográfica</span><span class="sxs-lookup"><span data-stu-id="7938c-378">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="7938c-379">RBAC</span><span class="sxs-lookup"><span data-stu-id="7938c-379">RBAC</span></span>
* <span data-ttu-id="7938c-380">Suporte ao escopo de grupo de gerenciamento adicionado a `role assignment`</span><span class="sxs-lookup"><span data-stu-id="7938c-380">Added support for mangement group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-381">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-381">Storage</span></span>
* <span data-ttu-id="7938c-382">`storage blob sync`: adicionar um comando de sincronização ao armazenamento de blobs</span><span class="sxs-lookup"><span data-stu-id="7938c-382">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="7938c-383">Computação</span><span class="sxs-lookup"><span data-stu-id="7938c-383">Compute</span></span>
* <span data-ttu-id="7938c-384">`--computer-name` foi adicionado a `vm create` para configurar o nome do computador da VM</span><span class="sxs-lookup"><span data-stu-id="7938c-384">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="7938c-385">`--ssh-key-value` foi renomeado para `--ssh-key-values` para `[vm|vmss] create` – Agora, pode aceitar vários valores de chave pública ou caminhos ssh</span><span class="sxs-lookup"><span data-stu-id="7938c-385">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="7938c-386">__Observação__: Isso **não** é uma alteração da falha – `--ssh-key-value` será analisado corretamente, pois corresponde somente a `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="7938c-386">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="7938c-387">O argumento `--type` de `ppg create` foi alterado para ser opcional</span><span class="sxs-lookup"><span data-stu-id="7938c-387">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="7938c-388">6 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="7938c-388">May 6, 2019</span></span>

<span data-ttu-id="7938c-389">Versão 2.0.64</span><span class="sxs-lookup"><span data-stu-id="7938c-389">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-390">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-390">ACS</span></span>
* <span data-ttu-id="7938c-391">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--fqdn` foi removido dos comandos `openshift`</span><span class="sxs-lookup"><span data-stu-id="7938c-391">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="7938c-392">Alterado para usar a versão da API do Red Hat OpenShift no Azure em disponibilidade geral</span><span class="sxs-lookup"><span data-stu-id="7938c-392">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="7938c-393">O sinalizador `customer-admin-group-id` foi adicionado a `openshift create`</span><span class="sxs-lookup"><span data-stu-id="7938c-393">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="7938c-394">[GA] `(PREVIEW)` foi removido da opção `aks create` `--network-policy`</span><span class="sxs-lookup"><span data-stu-id="7938c-394">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-395">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-395">Appservice</span></span>
* <span data-ttu-id="7938c-396">[PRETERIDO] O comando `functionapp devops-build` foi preterido</span><span class="sxs-lookup"><span data-stu-id="7938c-396">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="7938c-397">Renomeado para `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="7938c-397">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="7938c-398">Corrigido ao obter o nome de usuário correto para cloudshell que estava causando a falha em `webapp up`</span><span class="sxs-lookup"><span data-stu-id="7938c-398">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="7938c-399">Documentação `appservice plan --sku` atualizada para refletir o appserviceplans com suporte</span><span class="sxs-lookup"><span data-stu-id="7938c-399">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="7938c-400">Adicionado argumentos opcionais para o grupo de recursos e plano a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="7938c-400">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="7938c-401">Adicionado suporte a `webapp ssh` para respeitar a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="7938c-401">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="7938c-402">Adicionado suporte `appserviceplan create` para a SKU gratuita do Linux</span><span class="sxs-lookup"><span data-stu-id="7938c-402">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="7938c-403">Alterado `webapp up` para ter uma suspensão de 30 segundos depois de definir appsetting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` para lidar com a inicialização a frio kudu</span><span class="sxs-lookup"><span data-stu-id="7938c-403">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="7938c-404">Adicionado suporte para tempo de execução `powershell` a `functionapp create` no Windows</span><span class="sxs-lookup"><span data-stu-id="7938c-404">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="7938c-405">Adicionado o comando `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="7938c-405">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="7938c-406">Lote</span><span class="sxs-lookup"><span data-stu-id="7938c-406">Batch</span></span>
* <span data-ttu-id="7938c-407">Corrigido o bug no validador para as opções `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="7938c-407">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="7938c-408">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="7938c-408">Botservice</span></span>
* <span data-ttu-id="7938c-409">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para criar um Bot de Aplicativo Web vazio por padrão (ou seja, nenhum bot será implantado no Serviço de Aplicativo)</span><span class="sxs-lookup"><span data-stu-id="7938c-409">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="7938c-410">O sinalizador `--echo` foi adicionado ao `bot create` para usar o comportamento antigo com `-v v4`</span><span class="sxs-lookup"><span data-stu-id="7938c-410">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="7938c-411">[ALTERAÇÃO SIGNIFICATIVA] O valor padrão de `--version` foi alterado para `v4`</span><span class="sxs-lookup"><span data-stu-id="7938c-411">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="7938c-412">__OBSERVAÇÃO:__ `bot prepare-publish` ainda usa o padrão antigo</span><span class="sxs-lookup"><span data-stu-id="7938c-412">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="7938c-413">[ALTERAÇÃO SIGNIFICATIVA] `--lang` foi alterado para não definir mais `Csharp` como padrão.</span><span class="sxs-lookup"><span data-stu-id="7938c-413">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="7938c-414">Se o comando exigir `--lang` e ele não for fornecido, o comando será um erro</span><span class="sxs-lookup"><span data-stu-id="7938c-414">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="7938c-415">[ALTERAÇÃO SIGNIFICATIVA] Os argumentos `--appid` e `--password` foram alterados para `bot create` ser obrigatório e agora podem ser criados por meio de `ad app create`</span><span class="sxs-lookup"><span data-stu-id="7938c-415">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="7938c-416">Foi adicionada validação a `--appid` e `--password`</span><span class="sxs-lookup"><span data-stu-id="7938c-416">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="7938c-417">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4` foi alterado para não criar ou usar uma Conta de Armazenamento ou o Application Insights</span><span class="sxs-lookup"><span data-stu-id="7938c-417">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="7938c-418">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v3` foi alterado para exigir uma região em que o Application Insights está disponível</span><span class="sxs-lookup"><span data-stu-id="7938c-418">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="7938c-419">[ALTERAÇÃO SIGNIFICATIVA] O `bot update` foi alterado para afetar somente as propriedades específicas de um bot</span><span class="sxs-lookup"><span data-stu-id="7938c-419">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="7938c-420">[ALTERAÇÃO SIGNIFICATIVA] Os sinalizadores `--lang` foram alterados para aceitar `Javascript` em vez de `Node`</span><span class="sxs-lookup"><span data-stu-id="7938c-420">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="7938c-421">[ALTERAÇÃO SIGNIFICATIVA] O `Node` foi removido como um valor `--lang` permitido</span><span class="sxs-lookup"><span data-stu-id="7938c-421">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="7938c-422">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para não definir mais `SCM_DO_BUILD_DURING_DEPLOYMENT` como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="7938c-422">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="7938c-423">Todas as implantações por meio do Kudu atuarão de acordo com o comportamento padrão</span><span class="sxs-lookup"><span data-stu-id="7938c-423">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="7938c-424">O `bot download` foi alterado para os bots sem arquivos `.bot` para criar o arquivo de configuração específico a um idioma com os valores das Configurações de Aplicativo do bot</span><span class="sxs-lookup"><span data-stu-id="7938c-424">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="7938c-425">Adicionado o suporte `Typescript` para `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="7938c-425">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="7938c-426">Uma mensagem de aviso foi adicionada a `bot prepare-deploy` para os bots `Javascript` e `Typescript` para quando `--code-dir` não contiver `package.json`</span><span class="sxs-lookup"><span data-stu-id="7938c-426">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="7938c-427">O `bot prepare-deploy` foi alterado para retornar `true`, se bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="7938c-427">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="7938c-428">O log detalhado foi adicionado a `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="7938c-428">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="7938c-429">Mais regiões disponíveis do Application Insights foram adicionadas ao `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="7938c-429">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="7938c-430">Configurar</span><span class="sxs-lookup"><span data-stu-id="7938c-430">Configure</span></span>
* <span data-ttu-id="7938c-431">Adicionado suporte para configurações de valor padrão do argumento baseado em pasta</span><span class="sxs-lookup"><span data-stu-id="7938c-431">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="7938c-432">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="7938c-432">Eventhubs</span></span>
* <span data-ttu-id="7938c-433">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="7938c-433">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="7938c-434">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-434">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="7938c-435">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-435">Network</span></span>
* <span data-ttu-id="7938c-436">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--cache` foi substituído por `--defer` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-436">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="7938c-437">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="7938c-437">Policy Insights</span></span>
* <span data-ttu-id="7938c-438">Suporte adicionado a `--expand PolicyEvaluationDetails` para detalhes de avaliação de política de consulta no recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-438">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="7938c-439">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-439">Role</span></span>
* <span data-ttu-id="7938c-440">[PRETERIDO] Alterado argumento ocultar '--password' `create-for-rbac` - suporte será removido em maio de 2019</span><span class="sxs-lookup"><span data-stu-id="7938c-440">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="7938c-441">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="7938c-441">Service Bus</span></span>
* <span data-ttu-id="7938c-442">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="7938c-442">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="7938c-443">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-443">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="7938c-444">`topic [create|update]` foi fixado para permitir suporte a `--max-size` para valores de 10, 20, 40 e 80 GB com a SKU Premium</span><span class="sxs-lookup"><span data-stu-id="7938c-444">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-445">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-445">SQL</span></span>
* <span data-ttu-id="7938c-446">Adicionados os comandos `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="7938c-446">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-447">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-447">VM</span></span>
* <span data-ttu-id="7938c-448">O `--protect-from-scale-in` e o `--protect-from-scale-set-actions` foram adicionados a `vmss update` para habilitar atualizações à política de proteção das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="7938c-448">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="7938c-449">Adicionado a `--instance-id` e `vmss update` para habilitar atualização genérica das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="7938c-449">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="7938c-450">`--instance-id` foi adicionado a `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="7938c-450">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="7938c-451">Adicionado um novo grupo de comandos `ppg` para gerenciar grupos de posicionamento de proximidade</span><span class="sxs-lookup"><span data-stu-id="7938c-451">Added new `ppg` command group for manging Proximity Placement Groups</span></span>
* <span data-ttu-id="7938c-452">Adicionado a `--ppg`, `[vm|vmss] create` e `vm availability-set create` para gerenciar PPGs</span><span class="sxs-lookup"><span data-stu-id="7938c-452">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="7938c-453">Parâmetro `--hyper-v-generation` adicionado a `image create`</span><span class="sxs-lookup"><span data-stu-id="7938c-453">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="7938c-454">23 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="7938c-454">April 23, 2019</span></span>

<span data-ttu-id="7938c-455">Versão 2.0.63</span><span class="sxs-lookup"><span data-stu-id="7938c-455">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-456">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-456">ACS</span></span>
* <span data-ttu-id="7938c-457">Alterado `aks get-credentials` para solicitar substituição dos valores duplicados</span><span class="sxs-lookup"><span data-stu-id="7938c-457">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="7938c-458">Removido `(PREVIEW)` dos comandos de espaços de desenvolvimento "aks use-dev-espaces" e "aks remove-dev-espaces"</span><span class="sxs-lookup"><span data-stu-id="7938c-458">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="7938c-459">AMS</span><span class="sxs-lookup"><span data-stu-id="7938c-459">AMS</span></span>
* <span data-ttu-id="7938c-460">Corrigido o bug com a atualização de filtros de conta e de ativo</span><span class="sxs-lookup"><span data-stu-id="7938c-460">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-461">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-461">AppService</span></span>
* <span data-ttu-id="7938c-462">Adicionado suporte para o ASE e o tempo limite para `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="7938c-462">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="7938c-463">Adicionado suporte para o estabelecimento de CI CD em um pipeline do Azure DevOps de um repositório do Github para aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="7938c-463">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="7938c-464">Adicionado argumento `--github-pat` a `functionapp devops-build create` para aceitar o token de acesso pessoal do Github</span><span class="sxs-lookup"><span data-stu-id="7938c-464">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="7938c-465">Adicionado argumento `--github-repository` a `functionapp devops-build create` para aceitar o repositório Github que contém um código-fonte functionapp</span><span class="sxs-lookup"><span data-stu-id="7938c-465">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="7938c-466">Problema corrigido em que `az webapp up --logs` estava falhando com um erro e atualização da versão .NETCORE padrão para 2.1</span><span class="sxs-lookup"><span data-stu-id="7938c-466">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="7938c-467">Configurações de functionapp desnecessárias removidas durante a criação de um aplicativo de funções com plano de consumo</span><span class="sxs-lookup"><span data-stu-id="7938c-467">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="7938c-468">Alterado `webapp up` para que a cadeia de caracteres padrão asp agora acrescente o número no final para criar um novo ASP com base nas opções de SKU</span><span class="sxs-lookup"><span data-stu-id="7938c-468">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="7938c-469">Adicionado `-b` como uma opção a `webapp up` para iniciar o aplicativo no navegador</span><span class="sxs-lookup"><span data-stu-id="7938c-469">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="7938c-470">Alterado `webapp deployment source config zip` para lidar com a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="7938c-470">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="7938c-471">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="7938c-471">Deployment Manager</span></span>
* <span data-ttu-id="7938c-472">[VERSÃO PRÉVIA] Criar e gerenciar artefatos que dão suporte a distribuições</span><span class="sxs-lookup"><span data-stu-id="7938c-472">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="7938c-473">Laboratório</span><span class="sxs-lookup"><span data-stu-id="7938c-473">Lab</span></span>
* <span data-ttu-id="7938c-474">Corrigido o bug que causa uma saída inicial</span><span class="sxs-lookup"><span data-stu-id="7938c-474">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="7938c-475">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-475">Network</span></span>
* <span data-ttu-id="7938c-476">Adicionada delegação de servidor de nome automática a `dns zone create` no pai durante a criação da zona filho</span><span class="sxs-lookup"><span data-stu-id="7938c-476">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-477">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-477">Resource</span></span>
* <span data-ttu-id="7938c-478">[PRETERIDO] Argumentos `--link-id`, `--target-id` e `--filter-string` preteridos de `resource link`</span><span class="sxs-lookup"><span data-stu-id="7938c-478">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="7938c-479">Use os argumentos `--link`, `--target` e `--filter`</span><span class="sxs-lookup"><span data-stu-id="7938c-479">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="7938c-480">Corrigido o problema em que os comandos `resource link [create|update]` não funcionavam</span><span class="sxs-lookup"><span data-stu-id="7938c-480">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="7938c-481">Corrigido um problema em que a exclusão usando uma ID de recurso poderia causar falha no erro</span><span class="sxs-lookup"><span data-stu-id="7938c-481">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-482">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-482">SQL</span></span>
* <span data-ttu-id="7938c-483">Adicionado suporte para fuso horário personalizado nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="7938c-483">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="7938c-484">Alterado para permitir que o nome do pool Elástico seja usado com `sql db update`</span><span class="sxs-lookup"><span data-stu-id="7938c-484">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="7938c-485">Adicionado o suporte `--no-wait` para `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-485">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="7938c-486">Adicionado o comando `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="7938c-486">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-487">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-487">Storage</span></span>
* <span data-ttu-id="7938c-488">Corrigido o problema com tokens SAS com codificação dupla em `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="7938c-488">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-489">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-489">VM</span></span>
* <span data-ttu-id="7938c-490">Adicionado sinalizador `--skip-shutdown` a `vm|vmss stop` para desligar as VMs sem o desligamento</span><span class="sxs-lookup"><span data-stu-id="7938c-490">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="7938c-491">Adicionado argumento `--storage-account-type` a `sig image-version create` para definir o tipo de conta do perfil de publicação</span><span class="sxs-lookup"><span data-stu-id="7938c-491">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="7938c-492">Adicionado argumento `--target-regions` a `sig image-version create` para permitir definir os tipos de conta de armazenamento específico da região</span><span class="sxs-lookup"><span data-stu-id="7938c-492">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="7938c-493">9 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="7938c-493">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="7938c-494">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-494">Core</span></span>
* <span data-ttu-id="7938c-495">Correção do problema em que algumas extensões mostraram uma versão do `Unknown` e não podiam ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="7938c-495">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-496">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-496">ACR</span></span>
* <span data-ttu-id="7938c-497">Adição de suporte para execução de uma imagem sem contexto</span><span class="sxs-lookup"><span data-stu-id="7938c-497">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="7938c-498">AMS</span><span class="sxs-lookup"><span data-stu-id="7938c-498">AMS</span></span>
* [PRETERIDO]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [ALTERAÇÃO SIGNIFICATIVA]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="7938c-501">Adição de suporte para novos parâmetros de criptografia em `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="7938c-501">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="7938c-502">Adição de novo parâmetro `--filters` a `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="7938c-502">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-503">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-503">AppService</span></span>
* <span data-ttu-id="7938c-504">Adicionado o suporte `--logs` para `webapp up`</span><span class="sxs-lookup"><span data-stu-id="7938c-504">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="7938c-505">Correção de problemas do comando `functionapp devops-build create` de geração de `azure-pipelines.yml`</span><span class="sxs-lookup"><span data-stu-id="7938c-505">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="7938c-506">Melhoria do tratamento de erros e indicadores `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="7938c-506">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="7938c-507">[ALTERAÇÃO SIGNIFICATIVA] Remoção do sinalizador `--local-git` para o comando `devops-build`; a detecção de git local e a manipulação são obrigatórias para a criação de pipelines do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="7938c-507">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="7938c-508">Adição de suporte para a criação de planos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="7938c-508">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="7938c-509">Adição da capacidade de trocar um plano sob um aplicativo de funções usando `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="7938c-509">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="7938c-510">Adição de suporte para configurações de expansão de plano Premium do Azure Functions</span><span class="sxs-lookup"><span data-stu-id="7938c-510">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="7938c-511">CDN</span><span class="sxs-lookup"><span data-stu-id="7938c-511">CDN</span></span>
* <span data-ttu-id="7938c-512">Adição de suporte para `Microsoft_Standard` e `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="7938c-512">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="7938c-513">Comentários</span><span class="sxs-lookup"><span data-stu-id="7938c-513">Feedback</span></span>
* <span data-ttu-id="7938c-514">Alteração de `feedback` para mostrar metadados em comandos executados recentemente</span><span class="sxs-lookup"><span data-stu-id="7938c-514">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="7938c-515">Alteração de `feedback` para solicitar o auxílio do usuário no processo de criação de problema abrindo um navegador e usando um modelo de problema</span><span class="sxs-lookup"><span data-stu-id="7938c-515">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="7938c-516">Alteração do `feedback` para imprimir o corpo do problema ao executar com '--verbose'</span><span class="sxs-lookup"><span data-stu-id="7938c-516">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="7938c-517">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7938c-517">Monitor</span></span>
* <span data-ttu-id="7938c-518">Correção de um problema em que “count” não era um valor permitido com `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-518">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="7938c-519">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-519">Network</span></span>
* <span data-ttu-id="7938c-520">Correção do formato de tabela que não estava sendo exibido com `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="7938c-520">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="7938c-521">Adição dos comandos `list-request-headers` e `list-response-headers` para `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="7938c-521">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="7938c-522">Adição do comando `list-server-variables` para `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="7938c-522">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="7938c-523">Correção de um problema em que a atualização do estado do link em uma porta express-route geraria uma exceção de atributo desconhecido `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="7938c-523">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="7938c-524">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="7938c-524">PrivateDNS</span></span>
* <span data-ttu-id="7938c-525">Adição de `network private-dns` para zonas de DNS privado</span><span class="sxs-lookup"><span data-stu-id="7938c-525">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-526">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-526">Resource</span></span>
* <span data-ttu-id="7938c-527">Correção do problema com `deployment create` e `group deployment create`, em que um arquivo de parâmetros com um conjunto vazio de parâmetros não funcionaria</span><span class="sxs-lookup"><span data-stu-id="7938c-527">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="7938c-528">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-528">Role</span></span>
* <span data-ttu-id="7938c-529">Correção de `create-for-rbac` para lidar corretamente com `--years`</span><span class="sxs-lookup"><span data-stu-id="7938c-529">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="7938c-530">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `role assignment delete` para solicitar ao excluir todas as atribuições na assinatura incondicionalmente</span><span class="sxs-lookup"><span data-stu-id="7938c-530">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-531">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-531">SQL</span></span>
* <span data-ttu-id="7938c-532">Atualização de `sql mi [create|update]` com as propriedades proxyOverride e publicDataEndpointEnabled</span><span class="sxs-lookup"><span data-stu-id="7938c-532">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-533">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-533">Storage</span></span>
* <span data-ttu-id="7938c-534">[ALTERAÇÃO SIGNIFICATIVA] Remoção do resultado de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="7938c-534">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="7938c-535">Adição de `--full-uri` a `storage blob generate-sas` para criar o URI completo para o blob com SAS</span><span class="sxs-lookup"><span data-stu-id="7938c-535">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="7938c-536">Adição de `--file-snapshot` a `storage file copy start` para copiar arquivo do instantâneo</span><span class="sxs-lookup"><span data-stu-id="7938c-536">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="7938c-537">Alteração de `storage blob copy cancel` para mostrar apenas o erro em vez da exceção para NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="7938c-537">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="7938c-538">26 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="7938c-538">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="7938c-539">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-539">Core</span></span>
* <span data-ttu-id="7938c-540">Correção de problemas com incompatibilidade da extensão de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="7938c-540">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="7938c-541">Agora o tratamento de erros encaminha os clientes para a página de problemas</span><span class="sxs-lookup"><span data-stu-id="7938c-541">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="7938c-542">Nuvem</span><span class="sxs-lookup"><span data-stu-id="7938c-542">Cloud</span></span>
* <span data-ttu-id="7938c-543">Erro de “assinatura não encontrada” corrigido em `cloud set`</span><span class="sxs-lookup"><span data-stu-id="7938c-543">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-544">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-544">ACR</span></span>
* <span data-ttu-id="7938c-545">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="7938c-545">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="7938c-546">`--auth-mode` adicionado aos comandos `acr build`, `acr run`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="7938c-546">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="7938c-547">Grupo de comandos “acr task credential” adicionado para gerenciar as credenciais de uma Tarefa</span><span class="sxs-lookup"><span data-stu-id="7938c-547">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="7938c-548">“--no-wait” adicionado ao comando `acr build`</span><span class="sxs-lookup"><span data-stu-id="7938c-548">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-549">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-549">AppService</span></span>
* <span data-ttu-id="7938c-550">Bug corrigido onde `webapp up` não estava lidando corretamente com a execução do diretório vazio ou do cenário de código desconhecido</span><span class="sxs-lookup"><span data-stu-id="7938c-550">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="7938c-551">Bug corrigido onde os slots não funcionavam para `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="7938c-551">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="7938c-552">Serviço de BOT</span><span class="sxs-lookup"><span data-stu-id="7938c-552">BOT Service</span></span>
* <span data-ttu-id="7938c-553">`bot prepare-deploy` adicionado para se preparar para a implantação de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="7938c-553">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="7938c-554">`bot create --kind registration` alterado para mostrar a senha se ela não for fornecida</span><span class="sxs-lookup"><span data-stu-id="7938c-554">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="7938c-555">[ALTERAÇÃO SIGNIFICATIVA] `--endpoint` alterado em `bot create --kind registration` como padrão para uma cadeia de caracteres vazia, em vez de ser requerido</span><span class="sxs-lookup"><span data-stu-id="7938c-555">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="7938c-556">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="7938c-556">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="7938c-557">CDN</span><span class="sxs-lookup"><span data-stu-id="7938c-557">CDN</span></span>
* <span data-ttu-id="7938c-558">Adicionado o suporte ao `--no-wait` para `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="7938c-558">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [ALTERAÇÃO SIGNIFICATIVA]: `cdn endpoint create` alterado para o comportamento de cache da cadeia de consulta padrão.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="7938c-560">Não há mais padrão para "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="7938c-560">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="7938c-561">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="7938c-561">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7938c-562">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="7938c-562">Cosmosdb</span></span>
* <span data-ttu-id="7938c-563">Suporte adicionado para `--enable-multiple-write-locations` na atualização da conta</span><span class="sxs-lookup"><span data-stu-id="7938c-563">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="7938c-564">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7938c-564">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="7938c-565">Interativo</span><span class="sxs-lookup"><span data-stu-id="7938c-565">Interactive</span></span>
* <span data-ttu-id="7938c-566">Incompatibilidade corrigida com a extensão Interativa instalada por meio do azdev</span><span class="sxs-lookup"><span data-stu-id="7938c-566">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="7938c-567">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7938c-567">Monitor</span></span>
* <span data-ttu-id="7938c-568">Alterado para permitir o valor de dimensão `*` para `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-568">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="7938c-569">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-569">Network</span></span>
* <span data-ttu-id="7938c-570">Grupo de comandos `rewrite-rule` adicionado em `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="7938c-570">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="7938c-571">Perfil</span><span class="sxs-lookup"><span data-stu-id="7938c-571">Profile</span></span>
* <span data-ttu-id="7938c-572">Suporte de conta no nível do locatário para a identidade de serviço gerenciado adicionado em `login`</span><span class="sxs-lookup"><span data-stu-id="7938c-572">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="7938c-573">Postgres</span><span class="sxs-lookup"><span data-stu-id="7938c-573">Postgres</span></span> 
* <span data-ttu-id="7938c-574">Adicionados os comandos postgresql `replica` e `restart server`</span><span class="sxs-lookup"><span data-stu-id="7938c-574">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="7938c-575">Alterado para obter o local padrão do grupo de recursos quando não fornecido para criar servidores e adicionar validação para os dias de retenção</span><span class="sxs-lookup"><span data-stu-id="7938c-575">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-576">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-576">Resource</span></span>
* <span data-ttu-id="7938c-577">Saída da tabela aperfeiçoada para `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="7938c-577">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="7938c-578">Corrigido o problema com `deployment [create|validate]` onde o tipo secureObject não era reconhecido</span><span class="sxs-lookup"><span data-stu-id="7938c-578">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="7938c-579">Grafo</span><span class="sxs-lookup"><span data-stu-id="7938c-579">Graph</span></span>
* <span data-ttu-id="7938c-580">Adicionado o suporte ao `--end-date` para `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="7938c-580">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="7938c-581">Suporte adicionado para acrescentar permissões com `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="7938c-581">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="7938c-582">Bug corrigido com `ad app permission list` quando não havia nenhuma permissão</span><span class="sxs-lookup"><span data-stu-id="7938c-582">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="7938c-583">`ad sp delete` alterado para ignorar a exclusão da atribuição de função se a conta atual não tem nenhuma assinatura</span><span class="sxs-lookup"><span data-stu-id="7938c-583">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="7938c-584">`ad app create` alterado para `--identifier-uris` passar para lista vazia como padrão se não fornecido</span><span class="sxs-lookup"><span data-stu-id="7938c-584">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-585">storage</span><span class="sxs-lookup"><span data-stu-id="7938c-585">storage</span></span>
* <span data-ttu-id="7938c-586">`--snapshot` adicionado a `storage file download-batch` para baixar de um instantâneo de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="7938c-586">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="7938c-587">Barra de progresso `storage blob [download-batch|upload-batch]` alterada para ser menos detalhada e indicar o blob atual</span><span class="sxs-lookup"><span data-stu-id="7938c-587">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="7938c-588">Problema corrigido com `storage account update` ao atualizar os parâmetros de criptografia</span><span class="sxs-lookup"><span data-stu-id="7938c-588">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="7938c-589">Problema corrigido onde `storage blob show` falharia ao usar o oauth (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="7938c-589">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-590">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-590">VM</span></span>
* <span data-ttu-id="7938c-591">Adicionado o comando `image update`</span><span class="sxs-lookup"><span data-stu-id="7938c-591">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="7938c-592">12 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="7938c-592">March 12, 2019</span></span>

<span data-ttu-id="7938c-593">Versão 2.0.60</span><span class="sxs-lookup"><span data-stu-id="7938c-593">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="7938c-594">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-594">Core</span></span>

* <span data-ttu-id="7938c-595">Foi corrigido um erro incorreto no `cloud set` sobre assinatura não encontrada.</span><span class="sxs-lookup"><span data-stu-id="7938c-595">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-596">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-596">ACR</span></span>

* <span data-ttu-id="7938c-597">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="7938c-597">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-598">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-598">ACS</span></span>

* <span data-ttu-id="7938c-599">Alteração para ignorar o parâmetro `--listen-address` para `aks browse` se ele não for compatível com kubectl</span><span class="sxs-lookup"><span data-stu-id="7938c-599">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="7938c-600">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-600">AppService</span></span>

* <span data-ttu-id="7938c-601">Adicionado `[webapp|functionapp] deployment list-publishing-credentials` para obter a URL de publicação do Kudu e suas credenciais.</span><span class="sxs-lookup"><span data-stu-id="7938c-601">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="7938c-602">Removida a instrução de impressão errônea de `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="7938c-602">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="7938c-603">Corrigido `functionapp` para definir a imagem correta do tempo de execução nos planos do Serviço de Aplicativo no Linux.</span><span class="sxs-lookup"><span data-stu-id="7938c-603">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="7938c-604">Removida a marca de versão prévia do `webapp up` e adicionadas melhorias ao comando.</span><span class="sxs-lookup"><span data-stu-id="7938c-604">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="7938c-605">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="7938c-605">Botservice</span></span>

* <span data-ttu-id="7938c-606">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="7938c-606">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="7938c-607">Adicionados `Microsoft-BotFramework-AppId` e `Microsoft-BotFramework-AppPassword` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="7938c-607">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="7938c-608">Removidas as aspas simples da saída de comando `bot publish`, no final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="7938c-608">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="7938c-609">Alterado `bot publish` para que seja assíncrono.</span><span class="sxs-lookup"><span data-stu-id="7938c-609">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="7938c-610">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-610">Container</span></span>

* <span data-ttu-id="7938c-611">Adicionado o argumento `--no-wait` para `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="7938c-611">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="7938c-612">EventHub</span><span class="sxs-lookup"><span data-stu-id="7938c-612">EventHub</span></span>

* <span data-ttu-id="7938c-613">Adicionado o sinalizador `--skip-empty-archives` a `eventhub create|update` para dar suporte a arquivos vazios na captura.</span><span class="sxs-lookup"><span data-stu-id="7938c-613">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="7938c-614">Localizar</span><span class="sxs-lookup"><span data-stu-id="7938c-614">Find</span></span>

* <span data-ttu-id="7938c-615">Atualização de funcionalidade principal</span><span class="sxs-lookup"><span data-stu-id="7938c-615">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7938c-616">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7938c-616">HDInsight</span></span>

* <span data-ttu-id="7938c-617">Adicionado o parâmetro `--storage-account-managed-identity` a `hdinsight create` para oferecer suporte ao MSI do ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="7938c-617">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="7938c-618">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-618">Network</span></span>

* <span data-ttu-id="7938c-619">Corrigido o problema com `vpn-connection update`, onde a atualização de uma conexão VPN entre gateways em assinaturas diferentes falharia.</span><span class="sxs-lookup"><span data-stu-id="7938c-619">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="7938c-620">Rdbms</span><span class="sxs-lookup"><span data-stu-id="7938c-620">Rdbms</span></span>

* <span data-ttu-id="7938c-621">Correções secundárias para obter a localização padrão do grupo de recursos, quando não fornecida, para criar servidores e adicionar validação nos dias de retenção.</span><span class="sxs-lookup"><span data-stu-id="7938c-621">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="7938c-622">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-622">Role</span></span>

* <span data-ttu-id="7938c-623">Corrigido `role definition update` para usar ID a fim de resolver a definição corretamente.</span><span class="sxs-lookup"><span data-stu-id="7938c-623">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="7938c-624">Alterado `ad app credential reset` para remover a suposição de que a entidade de serviço do aplicativo já existe.</span><span class="sxs-lookup"><span data-stu-id="7938c-624">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7938c-625">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7938c-625">Service Fabric</span></span>

* <span data-ttu-id="7938c-626">Corrigido o problema com o fato de `sf cluster list` não ser iterável.</span><span class="sxs-lookup"><span data-stu-id="7938c-626">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="7938c-627">26 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="7938c-627">February 26, 2019</span></span>

<span data-ttu-id="7938c-628">Versão 2.0.59</span><span class="sxs-lookup"><span data-stu-id="7938c-628">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="7938c-629">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-629">Core</span></span>

* <span data-ttu-id="7938c-630">Corrigido o problema onde algumas instâncias usando `--subscription NAME` produziriam uma exceção</span><span class="sxs-lookup"><span data-stu-id="7938c-630">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-631">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-631">ACR</span></span>

* <span data-ttu-id="7938c-632">Parâmetro `--target` adicionado para os comandos `acr build`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="7938c-632">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="7938c-633">Melhor tratamento de erros para os comandos de execução quando não conectado ao Azure</span><span class="sxs-lookup"><span data-stu-id="7938c-633">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-634">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-634">ACS</span></span>

* <span data-ttu-id="7938c-635">Opção `--listen-address` adicionada a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="7938c-635">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-636">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-636">AppService</span></span>

* <span data-ttu-id="7938c-637">Adicionado o comando `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="7938c-637">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="7938c-638">Lote</span><span class="sxs-lookup"><span data-stu-id="7938c-638">Batch</span></span>
* <span data-ttu-id="7938c-639">[ALTERAÇÃO SIGNIFICATIVA] Comando `batch pool upgrade os` removido</span><span class="sxs-lookup"><span data-stu-id="7938c-639">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="7938c-640">[ALTERAÇÃO SIGNIFICATIVA] Propriedade `Pacakges` removida das respostas `Application`</span><span class="sxs-lookup"><span data-stu-id="7938c-640">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="7938c-641">Comando `batch application package list` adicionado para listar os pacotes de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="7938c-641">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="7938c-642">[ALTERAÇÃO SIGNIFICATIVA] `--application-id` alterado para `--application-name` em todos os comandos `batch application`,</span><span class="sxs-lookup"><span data-stu-id="7938c-642">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="7938c-643">O argumento `--json-file` foi adicionado aos comandos para a solicitação de resposta da API bruta</span><span class="sxs-lookup"><span data-stu-id="7938c-643">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="7938c-644">Validação atualizada para incluir automaticamente `https://` em todos os pontos de extremidade, se ausente</span><span class="sxs-lookup"><span data-stu-id="7938c-644">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7938c-645">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7938c-645">CosmosDB</span></span>

* <span data-ttu-id="7938c-646">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7938c-646">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="7938c-647">Kusto</span><span class="sxs-lookup"><span data-stu-id="7938c-647">Kusto</span></span>

* <span data-ttu-id="7938c-648">[ALTERAÇÃO SIGNIFICATIVA] Os tipos `hot_cache_period` e `soft_delete_period` foram alterados do banco de dados para o formato de duração ISO8601</span><span class="sxs-lookup"><span data-stu-id="7938c-648">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="7938c-649">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-649">Network</span></span>

* <span data-ttu-id="7938c-650">Adicionado o argumento `--express-route-gateway-bypass` para `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-650">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="7938c-651">Foram adicionados os grupos de comando a partir das extensões `express-route`</span><span class="sxs-lookup"><span data-stu-id="7938c-651">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="7938c-652">Os grupos de comando `express-route gateway` e `express-route port` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="7938c-652">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="7938c-653">Adicionado o argumento `--legacy-mode` para `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-653">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="7938c-654">Os argumentos `--allow-classic-operations` e `--express-route-port` foram adicionados a `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-654">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="7938c-655">Adicionado o argumento `--gateway-default-site` para `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-655">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="7938c-656">Os comandos `ipsec-policy` foram adicionados a `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="7938c-656">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-657">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-657">Resource</span></span>

* <span data-ttu-id="7938c-658">Foi corrigido o problema com `deployment create` em que o campo do tipo diferencia letras maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="7938c-658">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="7938c-659">Foi adicionado o suporte para arquivo de parâmetros de URI a `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="7938c-659">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="7938c-660">Foi adicionado o suporte para parâmetros de URI e definições a `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="7938c-660">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="7938c-661">Foi corrigido o tratamento de parâmetros e regras para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="7938c-661">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="7938c-662">Foi corrigido o problema com `resource show/update/delete/tag/invoke-action` em que as IDs de assinatura cruzada não respeitaram corretamente a ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="7938c-662">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="7938c-663">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-663">Role</span></span>

* <span data-ttu-id="7938c-664">Foi adicionado o suporte para as funções do aplicativo a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-664">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-665">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-665">VM</span></span>

* <span data-ttu-id="7938c-666">Foi corrigido o problema com `vm create where ` – a rede acelerada não foi habilitada por padrão no Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="7938c-666">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="7938c-667">12 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="7938c-667">February 12, 2019</span></span>

<span data-ttu-id="7938c-668">Versão 2.0.58</span><span class="sxs-lookup"><span data-stu-id="7938c-668">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="7938c-669">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-669">Core</span></span>

* <span data-ttu-id="7938c-670">`az --version` agora exibe uma notificação se você tiver pacotes para atualização</span><span class="sxs-lookup"><span data-stu-id="7938c-670">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="7938c-671">A regressão em que `--ids` não pode ser usado com a saída JSON foi corrigida</span><span class="sxs-lookup"><span data-stu-id="7938c-671">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-672">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-672">ACR</span></span>
* <span data-ttu-id="7938c-673">[ALTERAÇÃO SIGNIFICATIVA] O grupo de comandos `acr build-task` foi removido</span><span class="sxs-lookup"><span data-stu-id="7938c-673">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="7938c-674">[ALTERAÇÃO SIGNIFICATIVA] As opções `--tag` e `--manifest` de `acr repository delete` foram removidas</span><span class="sxs-lookup"><span data-stu-id="7938c-674">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-675">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-675">ACS</span></span>
* <span data-ttu-id="7938c-676">Suporte adicionado a `aks [enable-addons|disable-addons]` para nomes que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="7938c-676">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="7938c-677">Suporte adicionado para a operação de atualização do Azure Active Directory usando `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="7938c-677">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="7938c-678">Um esclarecimento informando que `--output` é ignorado para `aks get-credentials` foi adicionado</span><span class="sxs-lookup"><span data-stu-id="7938c-678">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="7938c-679">AMS</span><span class="sxs-lookup"><span data-stu-id="7938c-679">AMS</span></span>
* <span data-ttu-id="7938c-680">Adicionados os comandos `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="7938c-680">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="7938c-681">Adicionados os comandos `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="7938c-681">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-682">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-682">Appservice</span></span>
* <span data-ttu-id="7938c-683">Foi adicionada a capacidade de criar e configurar funções usando contêineres de ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-683">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="7938c-684">Suporte adicionado para a atualização das configurações de aplicativos Web por meio de JSON</span><span class="sxs-lookup"><span data-stu-id="7938c-684">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="7938c-685">A ajuda foi aprimorada para `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="7938c-685">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="7938c-686">Suporte adicionado para o App Insights para auxiliar na criação de aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="7938c-686">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="7938c-687">Os problemas com o SSH do aplicativo Web foram corrigidos</span><span class="sxs-lookup"><span data-stu-id="7938c-687">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="7938c-688">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="7938c-688">Botservice</span></span>
* <span data-ttu-id="7938c-689">A experiência do usuário para `bot publish` foi aprimorada</span><span class="sxs-lookup"><span data-stu-id="7938c-689">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="7938c-690">Foram adicionados avisos de tempos limite ao executar `npm install` durante `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="7938c-690">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="7938c-691">O caractere inválido `.` de `--name` em `az bot create` foi removido</span><span class="sxs-lookup"><span data-stu-id="7938c-691">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="7938c-692">Alteração para interromper a geração aleatória de nomes de recursos durante a criação do Armazenamento do Azure, Plano do Serviço de Aplicativo, Aplicativo Web/de funções e Application Insights</span><span class="sxs-lookup"><span data-stu-id="7938c-692">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="7938c-693">[PRETERIDO] O argumento `--proj-name` foi preterido em favor de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="7938c-693">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="7938c-694">`az bot publish` foi alterado para remover arquivos de implantação do Node.js do IIS buscados, caso eles já não existissem</span><span class="sxs-lookup"><span data-stu-id="7938c-694">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="7938c-695">Foi adicionado o argumento `--keep-node-modules` para `az bot publish` para não excluir a pasta `node_modules` no Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7938c-695">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="7938c-696">O par chave-valor `"publishCommand"` foi adicionado à saída de `az bot create` durante a criação de uma função do Azure ou bot de aplicativo Web</span><span class="sxs-lookup"><span data-stu-id="7938c-696">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="7938c-697">O valor de `"publishCommand"` é um comando `az bot publish` que é automaticamente preenchido com os parâmetros necessários para publicar o bot recém-criado</span><span class="sxs-lookup"><span data-stu-id="7938c-697">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="7938c-698">O `"WEBSITE_NODE_DEFAULT_VERSION"` foi atualizado no modelo do ARM para que os bots de SDK v4 usem 10.14.1 em vez de 8.9.4</span><span class="sxs-lookup"><span data-stu-id="7938c-698">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="7938c-699">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7938c-699">Key Vault</span></span>
* <span data-ttu-id="7938c-700">Foi corrigido o problema com `keyvault secret backup`, em que alguns usuários recebiam um erro `unexpected_keyword` ao usar `--id`</span><span class="sxs-lookup"><span data-stu-id="7938c-700">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="7938c-701">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7938c-701">Monitor</span></span>
* <span data-ttu-id="7938c-702">`monitor metrics alert [create|update]` foi alterado para permitir o valor dimensional `*`</span><span class="sxs-lookup"><span data-stu-id="7938c-702">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="7938c-703">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-703">Network</span></span>
* <span data-ttu-id="7938c-704">`dns zone export` foi alterado para garantir que CNAMEs exportados fossem FQDNs</span><span class="sxs-lookup"><span data-stu-id="7938c-704">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="7938c-705">O parâmetro `--gateway-name` foi adicionado a `nic ip-config address-pool [add|remove]` para dar suporte a pools de endereços de back-end de gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="7938c-705">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="7938c-706">Os argumentos `--traffic-analytics` e `--workspace` foram adicionados a `network watcher flow-log configure` para dar suporte à análise de tráfego por meio de um espaço de trabalho do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="7938c-706">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="7938c-707">`--idle-timeout` e `--floating-ip` foram adicionados a `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-707">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="7938c-708">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="7938c-708">Policy Insights</span></span>
* <span data-ttu-id="7938c-709">Os comandos `policy remediation` foram adicionados para dar suporte a recursos de correção de política de recursos</span><span class="sxs-lookup"><span data-stu-id="7938c-709">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="7938c-710">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7938c-710">RDBMS</span></span>
* <span data-ttu-id="7938c-711">A mensagem e os parâmetros de comando de ajuda foram aprimorados</span><span class="sxs-lookup"><span data-stu-id="7938c-711">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="7938c-712">Redis</span><span class="sxs-lookup"><span data-stu-id="7938c-712">Redis</span></span>
* <span data-ttu-id="7938c-713">Foram adicionados comandos para gerenciar regras de firewall (criar, atualizar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="7938c-713">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="7938c-714">Foram adicionados comandos para gerenciar links do servidor (criar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="7938c-714">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="7938c-715">Foram adicionados comandos para gerenciar o agendamento de patches (criar, atualizar, excluir, mostrar)</span><span class="sxs-lookup"><span data-stu-id="7938c-715">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="7938c-716">Suporte adicionado para Zonas de Disponibilidade e versão mínima de TLS para criar Redis</span><span class="sxs-lookup"><span data-stu-id="7938c-716">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="7938c-717">[ALTERAÇÃO SIGNIFICATIVA] Os comandos `redis update-settings` e `redis list-all` foram removidos</span><span class="sxs-lookup"><span data-stu-id="7938c-717">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="7938c-718">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro para `redis create`: “configurações de locatário” não é aceito no formato chave[=valor]</span><span class="sxs-lookup"><span data-stu-id="7938c-718">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="7938c-719">[PRETERIDO] Uma mensagem de aviso foi adicionada para preterir o comando `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="7938c-719">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="7938c-720">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-720">Role</span></span>
* <span data-ttu-id="7938c-721">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido dos comandos `vm` para esta localização</span><span class="sxs-lookup"><span data-stu-id="7938c-721">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="7938c-722">SQL VM</span><span class="sxs-lookup"><span data-stu-id="7938c-722">SQL VM</span></span>
* <span data-ttu-id="7938c-723">[PRETERIDO] O argumento `--boostrap-acc-pwd` foi preterido devido a um erro de digitação</span><span class="sxs-lookup"><span data-stu-id="7938c-723">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-724">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-724">VM</span></span>
* <span data-ttu-id="7938c-725">`vm list-skus` foi alterado para permitir o uso de `--all` no lugar de `--all true`</span><span class="sxs-lookup"><span data-stu-id="7938c-725">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="7938c-726">Adicionado `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="7938c-726">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="7938c-727">Foi corrigido o bug em que `vmss encryption enable` falhava se fosse executado anteriormente</span><span class="sxs-lookup"><span data-stu-id="7938c-727">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="7938c-728">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido para os comandos `role`</span><span class="sxs-lookup"><span data-stu-id="7938c-728">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="7938c-729">31 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="7938c-729">January 31, 2019</span></span>

<span data-ttu-id="7938c-730">Versão 2.0.57</span><span class="sxs-lookup"><span data-stu-id="7938c-730">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="7938c-731">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-731">Core</span></span>

* <span data-ttu-id="7938c-732">Hotfix para o [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="7938c-732">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="7938c-733">28 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="7938c-733">January 28, 2019</span></span>

<span data-ttu-id="7938c-734">Versão 2.0.56</span><span class="sxs-lookup"><span data-stu-id="7938c-734">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-735">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-735">ACR</span></span>
* <span data-ttu-id="7938c-736">Suporte adicionado para regras de rede virtual/IP</span><span class="sxs-lookup"><span data-stu-id="7938c-736">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-737">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-737">ACS</span></span>
* <span data-ttu-id="7938c-738">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="7938c-738">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="7938c-739">Comandos do OpenShift gerenciado foram adicionados</span><span class="sxs-lookup"><span data-stu-id="7938c-739">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="7938c-740">Suporte adicionado para operações de atualização da entidade de serviço com `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="7938c-740">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="7938c-741">AMS</span><span class="sxs-lookup"><span data-stu-id="7938c-741">AMS</span></span>
* <span data-ttu-id="7938c-742">[ALTERAÇÃO SIGNIFICATIVA] `ams asset get-streaming-locators` renomeado para `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="7938c-742">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="7938c-743">[ALTERAÇÃO SIGNIFICATIVA] `ams streaming-locator get-content-keys` renomeado para `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="7938c-743">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-744">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-744">Appservice</span></span>
* <span data-ttu-id="7938c-745">Suporte adicionado para o App Insights no `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="7938c-745">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="7938c-746">Suporte adicionado para a criação do plano de serviço de aplicativo (incluindo Elástico Premium) para Aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="7938c-746">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="7938c-747">Foram corrigidos os problemas com de configuração de aplicativo com os planos Elástico Premium</span><span class="sxs-lookup"><span data-stu-id="7938c-747">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="7938c-748">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-748">Container</span></span>
* <span data-ttu-id="7938c-749">Adicionado o comando `container start`</span><span class="sxs-lookup"><span data-stu-id="7938c-749">Added `container start` command</span></span>
* <span data-ttu-id="7938c-750">Alteração para permitir o uso de valores decimais para CPU durante a criação do contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-750">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="7938c-751">EventGrid</span><span class="sxs-lookup"><span data-stu-id="7938c-751">EventGrid</span></span>
* <span data-ttu-id="7938c-752">Parâmetro `--deadletter-endpoint` adicionado a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-752">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="7938c-753">Storagequeue e hybridconnection foram adicionados como novos valores para 'event-subscription [create|update] --endpoint-type\`</span><span class="sxs-lookup"><span data-stu-id="7938c-753">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="7938c-754">Os parâmetros `--max-delivery-attempts` e `--event-ttl` foram adicionados a `event-subscription create` para especificar a política de repetição para eventos</span><span class="sxs-lookup"><span data-stu-id="7938c-754">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="7938c-755">Uma mensagem de aviso foi adicionada a `event-subscription [create|update]` quando o webhook como destino for usado para uma assinatura de evento</span><span class="sxs-lookup"><span data-stu-id="7938c-755">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="7938c-756">O parâmetro source-resource-id foi adicionado para todos os comandos relacionados a eventos e marcar todos os outros parâmetros relacionados ao recurso de origem como preteridos</span><span class="sxs-lookup"><span data-stu-id="7938c-756">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7938c-757">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7938c-757">HDInsight</span></span>
* <span data-ttu-id="7938c-758">[ALTERAÇÃO SIGNIFICATIVA] Os parâmetros `--virtual-network` e `--subnet-name` de `hdinsight [application] create` foram removidos</span><span class="sxs-lookup"><span data-stu-id="7938c-758">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="7938c-759">[ALTERAÇÃO SIGNIFICATIVA] `hdinsight create --storage-account` foi alterado para aceitar o nome ou ID da conta de armazenamento, em vez de pontos de extremidade de blob</span><span class="sxs-lookup"><span data-stu-id="7938c-759">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="7938c-760">Parâmetros `--vnet-name` e `--subnet-name` adicionados a `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="7938c-760">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="7938c-761">Suporte adicionado para a criptografia de disco e Enterprise Security Package ao `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="7938c-761">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="7938c-762">Adicionado o comando `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="7938c-762">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="7938c-763">Adicionado o comando `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="7938c-763">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="7938c-764">IoT</span><span class="sxs-lookup"><span data-stu-id="7938c-764">IoT</span></span>
* <span data-ttu-id="7938c-765">O formato de codificação foi adicionado ao comando routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="7938c-765">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="7938c-766">Kusto</span><span class="sxs-lookup"><span data-stu-id="7938c-766">Kusto</span></span>
* <span data-ttu-id="7938c-767">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="7938c-767">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="7938c-768">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7938c-768">Monitor</span></span>
* <span data-ttu-id="7938c-769">A comparação de ID foi alterada para diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="7938c-769">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="7938c-770">Perfil</span><span class="sxs-lookup"><span data-stu-id="7938c-770">Profile</span></span>
* <span data-ttu-id="7938c-771">A conta de nível de locatário foi habilitada para a identidade de serviço gerenciada de `login`</span><span class="sxs-lookup"><span data-stu-id="7938c-771">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="7938c-772">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-772">Network</span></span>
* <span data-ttu-id="7938c-773">Foi corrigido o problema com `express-route update`: em que o argumento `--bandwidth` era ignorado</span><span class="sxs-lookup"><span data-stu-id="7938c-773">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="7938c-774">Foi corrigido o problema com `ddos-protection update` em que definir a compreensão levava ao rastreamento de pilha</span><span class="sxs-lookup"><span data-stu-id="7938c-774">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-775">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-775">Resource</span></span>
* <span data-ttu-id="7938c-776">Suporte adicionado para o arquivo de parâmetros de URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="7938c-776">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="7938c-777">Suporte adicionado para a identidade gerenciada à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="7938c-777">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="7938c-778">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-778">SQL Virtual Machine</span></span>
* <span data-ttu-id="7938c-779">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="7938c-779">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-780">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-780">Storage</span></span>
* <span data-ttu-id="7938c-781">Alteração na correção para atualizar apenas as propriedades que são alteradas no mesmo objeto</span><span class="sxs-lookup"><span data-stu-id="7938c-781">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="7938c-782">#8021 foi corrigido, dados binários são codificados em base 64 quando retornados</span><span class="sxs-lookup"><span data-stu-id="7938c-782">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-783">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-783">VM</span></span>
* <span data-ttu-id="7938c-784">Alteração de `vm encryption enable` para validar o cofre de chaves de criptografia de disco e se esse cofre de chaves de criptografia de chave existe</span><span class="sxs-lookup"><span data-stu-id="7938c-784">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="7938c-785">O sinalizador `--force` foi adicionado a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="7938c-785">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="7938c-786">15 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="7938c-786">January 15, 2019</span></span>

<span data-ttu-id="7938c-787">Versão 2.0.55</span><span class="sxs-lookup"><span data-stu-id="7938c-787">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-788">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-788">ACR</span></span>
* <span data-ttu-id="7938c-789">Alteração para permitir forçar o envio por push de um gráfico Helm que não existe</span><span class="sxs-lookup"><span data-stu-id="7938c-789">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="7938c-790">Alteração para permitir operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="7938c-790">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="7938c-791">[PRETERIDO] O parâmetro `--resource-group` foi preterido nos comandos:</span><span class="sxs-lookup"><span data-stu-id="7938c-791">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="7938c-792">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-792">ACS</span></span>
* <span data-ttu-id="7938c-793">Suporte adicionado para novas regiões ACI</span><span class="sxs-lookup"><span data-stu-id="7938c-793">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-794">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-794">Appservice</span></span>
* <span data-ttu-id="7938c-795">Foi corrigido o problema com o carregamento de certificados para aplicativos que são hospedados em um ASE, em que o RG do ASE e o RG do aplicativo são diferentes</span><span class="sxs-lookup"><span data-stu-id="7938c-795">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="7938c-796">Alteração de `webapp up` para usar a SKU P1V1 como padrão para Linux</span><span class="sxs-lookup"><span data-stu-id="7938c-796">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="7938c-797">`[webapp|functionapp] deployment source config-zip` foi corrigido para mostrar a mensagem de erro adequada quando uma implantação falhar</span><span class="sxs-lookup"><span data-stu-id="7938c-797">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="7938c-798">Adicionado o comando `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="7938c-798">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="7938c-799">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="7938c-799">Botservice</span></span>
* <span data-ttu-id="7938c-800">Atualizações de status de implantação foram adicionadas a `bot create`</span><span class="sxs-lookup"><span data-stu-id="7938c-800">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="7938c-801">Configurar</span><span class="sxs-lookup"><span data-stu-id="7938c-801">Configure</span></span>
* <span data-ttu-id="7938c-802">`none` foi adicionado como um formato de saída configurável</span><span class="sxs-lookup"><span data-stu-id="7938c-802">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7938c-803">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7938c-803">CosmosDB</span></span>
* <span data-ttu-id="7938c-804">Suporte adicionado para criar o banco de dados com taxa de transferência compartilhada</span><span class="sxs-lookup"><span data-stu-id="7938c-804">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7938c-805">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7938c-805">HDInsight</span></span>
* <span data-ttu-id="7938c-806">Foram adicionados comandos para o gerenciamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="7938c-806">Added commands for managing applications</span></span>
* <span data-ttu-id="7938c-807">Foram adicionados comandos para o gerenciamento de ações de script</span><span class="sxs-lookup"><span data-stu-id="7938c-807">Added commands for managing script actions</span></span>
* <span data-ttu-id="7938c-808">Foram adicionados comandos para o gerenciamento do Operations Management Suite (OMS)</span><span class="sxs-lookup"><span data-stu-id="7938c-808">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="7938c-809">Suporte adicionado para listar a utilização regional ao `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="7938c-809">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="7938c-810">[ALTERAÇÃO SIGNIFICATIVA] O tipo de cluster padrão de `hdinsight create` foi removido</span><span class="sxs-lookup"><span data-stu-id="7938c-810">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="7938c-811">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-811">Network</span></span>
* <span data-ttu-id="7938c-812">Adicionados os argumentos `--custom-headers` e `--status-code-ranges` para `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-812">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="7938c-813">Novos tipos de roteamento foram adicionados: Subrede e múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="7938c-813">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="7938c-814">Adicionados os argumentos `--custom-headers` e `--subnets` para `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-814">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="7938c-815">Foi corrigido o problema no qual fornecer `--vnets ""` a `ddos-protection update` causava um erro</span><span class="sxs-lookup"><span data-stu-id="7938c-815">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="7938c-816">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-816">Role</span></span>
* <span data-ttu-id="7938c-817">[PRETERIDO] O argumento `--password` foi preterido para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="7938c-817">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="7938c-818">Como alternativa, use senhas seguras geradas pela CLI</span><span class="sxs-lookup"><span data-stu-id="7938c-818">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="7938c-819">Segurança</span><span class="sxs-lookup"><span data-stu-id="7938c-819">Security</span></span>
* <span data-ttu-id="7938c-820">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="7938c-820">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-821">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-821">Storage</span></span>
* <span data-ttu-id="7938c-822">[ALTERAÇÃO SIGNIFICATIVA] O número padrão de resultados de `storage [blob|file|container|share] list` foi alterado para 5.000.</span><span class="sxs-lookup"><span data-stu-id="7938c-822">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="7938c-823">Use `--num-results *` para o comportamento original de retornar todos os resultados</span><span class="sxs-lookup"><span data-stu-id="7938c-823">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="7938c-824">Parâmetro `--marker` adicionado a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="7938c-824">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="7938c-825">Um marcador de log foi adicionado para a próxima página ao STDERR de `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="7938c-825">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="7938c-826">O comando `storage blob service-properties update` foi adicionado com suporte para sites estáticos</span><span class="sxs-lookup"><span data-stu-id="7938c-826">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-827">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-827">VM</span></span>
* <span data-ttu-id="7938c-828">`vm [disk|unmanaged-disk]` e `vmss disk` foram alterados para que tenham parâmetros mais consistentes</span><span class="sxs-lookup"><span data-stu-id="7938c-828">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="7938c-829">Suporte adicionado para referência cruzada de imagem de locatário a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7938c-829">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="7938c-830">O bug de configuração padrão foi corrigido em `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="7938c-830">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="7938c-831">O argumento `--provision-after-extensions` foi adicionado a `vmss extension set` para definir quais extensões deverão ser provisionadas antes da extensão ser definida</span><span class="sxs-lookup"><span data-stu-id="7938c-831">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="7938c-832">O argumento `--replica-count` foi adicionado a `sig image-version update` para definir a contagem de replicação padrão</span><span class="sxs-lookup"><span data-stu-id="7938c-832">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="7938c-833">Foi corrigido o bug com `image create --source` em que o disco do sistema operacional de origem era confundido com uma VM do mesmo nome, mesmo se a ID de recurso completa fosse fornecida</span><span class="sxs-lookup"><span data-stu-id="7938c-833">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="7938c-834">20 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-834">December 20, 2018</span></span>

<span data-ttu-id="7938c-835">Versão 2.0.54</span><span class="sxs-lookup"><span data-stu-id="7938c-835">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="7938c-836">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-836">Appservice</span></span>
* <span data-ttu-id="7938c-837">Corrigido o problema que causava falha na reimplantação do `webapp up`</span><span class="sxs-lookup"><span data-stu-id="7938c-837">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="7938c-838">Adicionado suporte para listar e restaurar instantâneos de aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="7938c-838">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="7938c-839">Adicionado suporte para o sinalizador `--runtime` para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="7938c-839">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="7938c-840">IoT Central</span><span class="sxs-lookup"><span data-stu-id="7938c-840">IoTCentral</span></span>
* <span data-ttu-id="7938c-841">Corrigida a chamada à API do comando de atualização</span><span class="sxs-lookup"><span data-stu-id="7938c-841">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="7938c-842">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-842">Role</span></span>
* <span data-ttu-id="7938c-843">[ALTERAÇÃO SIGNIFICATIVA] `ad [app|sp] list` alterado para listar somente os 100 primeiros objetos por padrão</span><span class="sxs-lookup"><span data-stu-id="7938c-843">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-844">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-844">SQL</span></span>
* <span data-ttu-id="7938c-845">Adicionado suporte para ordenação personalizada nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="7938c-845">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-846">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-846">VM</span></span>
* <span data-ttu-id="7938c-847">Parâmetro `---os-type` adicionado a `disk create`</span><span class="sxs-lookup"><span data-stu-id="7938c-847">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="7938c-848">18 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-848">December 18, 2018</span></span>

<span data-ttu-id="7938c-849">Versão 2.0.53</span><span class="sxs-lookup"><span data-stu-id="7938c-849">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="7938c-850">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-850">ACR</span></span>
* <span data-ttu-id="7938c-851">Adicionado suporte para importação de imagem de Registros de Contêiner externos</span><span class="sxs-lookup"><span data-stu-id="7938c-851">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="7938c-852">Simplificado o layout da tabela para a lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="7938c-852">Condensed the table layout for task list</span></span>
* <span data-ttu-id="7938c-853">Adicionado suporte para URLs do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="7938c-853">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-854">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-854">ACS</span></span>
* <span data-ttu-id="7938c-855">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="7938c-855">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="7938c-856">Removido “(VISUALIZAÇÃO)” de argumentos do AAD para `aks create`</span><span class="sxs-lookup"><span data-stu-id="7938c-856">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="7938c-857">[PRETERIDO] Comandos `az acs` preteridos.</span><span class="sxs-lookup"><span data-stu-id="7938c-857">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="7938c-858">O serviço ACS será desativado em 31 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="7938c-858">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="7938c-859">Adicionado suporte da Política de Rede durante a criação de novos clusters AKS</span><span class="sxs-lookup"><span data-stu-id="7938c-859">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="7938c-860">Removido o requisito do argumento `--nodepool-name` para `aks scale` se houver apenas um pool de nós</span><span class="sxs-lookup"><span data-stu-id="7938c-860">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-861">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-861">Appservice</span></span>
* <span data-ttu-id="7938c-862">Corrigido o problema em que `webapp config container` não honra o parâmetro `--slot`</span><span class="sxs-lookup"><span data-stu-id="7938c-862">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="7938c-863">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="7938c-863">Botservice</span></span>
* <span data-ttu-id="7938c-864">Suporte adicionado para análise do arquivo `.bot` ao chamar `bot show`</span><span class="sxs-lookup"><span data-stu-id="7938c-864">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="7938c-865">Corrigido o bug de provisionamento do AppInsights</span><span class="sxs-lookup"><span data-stu-id="7938c-865">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="7938c-866">Corrigido o bug de espaço em branco ao lidar com caminhos de arquivo</span><span class="sxs-lookup"><span data-stu-id="7938c-866">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="7938c-867">Reduzidas as chamadas de rede do Kudu</span><span class="sxs-lookup"><span data-stu-id="7938c-867">Reduced Kudu network calls</span></span>
* <span data-ttu-id="7938c-868">Melhorias de UX para comandos gerais</span><span class="sxs-lookup"><span data-stu-id="7938c-868">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="7938c-869">Consumo</span><span class="sxs-lookup"><span data-stu-id="7938c-869">Consumption</span></span>
* <span data-ttu-id="7938c-870">Corrigidos os bugs da API de orçamento ao mostrar notificações</span><span class="sxs-lookup"><span data-stu-id="7938c-870">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7938c-871">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7938c-871">CosmosDB</span></span>
* <span data-ttu-id="7938c-872">Suporte adicionado para atualizar a conta de vários mestres para mestre único</span><span class="sxs-lookup"><span data-stu-id="7938c-872">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="7938c-873">Mapas</span><span class="sxs-lookup"><span data-stu-id="7938c-873">Maps</span></span>
* <span data-ttu-id="7938c-874">Adicionado suporte ao SKU S1 para `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-874">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="7938c-875">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-875">Network</span></span>
* <span data-ttu-id="7938c-876">Adicionado suporte para `--format` e `--log-version` para `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="7938c-876">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="7938c-877">Corrigido o problema com `dns zone update` em que usar "" para limpar a resolução e o registro de redes virtuais não funcionava</span><span class="sxs-lookup"><span data-stu-id="7938c-877">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-878">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-878">Resource</span></span>
* <span data-ttu-id="7938c-879">Corrigido o tratamento do parâmetro de escopo para grupos de gerenciamento do `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-879">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="7938c-880">Adicionado o novo comando `resource wait`</span><span class="sxs-lookup"><span data-stu-id="7938c-880">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-881">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-881">Storage</span></span>
*  <span data-ttu-id="7938c-882">Adicionada a capacidade de atualizar a versão do esquema de log para serviços de armazenamento no `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="7938c-882">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-883">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-883">VM</span></span>
* <span data-ttu-id="7938c-884">Corrigida a falha em `vm identity remove` quando a VM especificada não tem nenhuma identidade de serviço gerenciado atribuída</span><span class="sxs-lookup"><span data-stu-id="7938c-884">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="7938c-885">4 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-885">December 4, 2018</span></span>

<span data-ttu-id="7938c-886">Versão 2.0.52</span><span class="sxs-lookup"><span data-stu-id="7938c-886">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="7938c-887">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-887">Core</span></span>
* <span data-ttu-id="7938c-888">Adicionado suporte para provisionamento de recursos de locatários cruzados para a entidade de serviço de multilocatários</span><span class="sxs-lookup"><span data-stu-id="7938c-888">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="7938c-889">Corrigido o bug onde as ids enviadas por pipe de um comando com a saída tsv eram analisados incorretamente</span><span class="sxs-lookup"><span data-stu-id="7938c-889">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-890">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-890">Appservice</span></span>
* <span data-ttu-id="7938c-891">[VERSÃO PRÉVIA] Adicionado o comando `webapp up` que ajuda a criar e implantar conteúdo em aplicativo</span><span class="sxs-lookup"><span data-stu-id="7938c-891">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="7938c-892">Corrigido um bug no aplicativo com base em contêiner do Windows devido à alteração de back-end</span><span class="sxs-lookup"><span data-stu-id="7938c-892">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="7938c-893">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-893">Network</span></span>
* <span data-ttu-id="7938c-894">Adicionado o argumento `--exclusion` a `application-gateway waf-config set` para dar suporte a exclusões de WAF</span><span class="sxs-lookup"><span data-stu-id="7938c-894">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="7938c-895">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-895">Role</span></span>
* <span data-ttu-id="7938c-896">Adicionado suporte para identificadores personalizados para a credencial de senha</span><span class="sxs-lookup"><span data-stu-id="7938c-896">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="7938c-897">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-897">VM</span></span>
* <span data-ttu-id="7938c-898">[PRETERIDO] Parâmetro `vm extension [show|wait] --expand` preterido</span><span class="sxs-lookup"><span data-stu-id="7938c-898">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="7938c-899">Adicionado parâmetro `--force` a `vm restart` para reimplantar as VMs sem resposta</span><span class="sxs-lookup"><span data-stu-id="7938c-899">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="7938c-900">Alterado `[vm|vmss] create --authentication-type` para aceitar "todos" para criar uma VM com senha e autenticação SSH</span><span class="sxs-lookup"><span data-stu-id="7938c-900">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="7938c-901">Adicionado parâmetro `image create --os-disk-caching` para definir o cache de disco do sistema operacional para uma imagem</span><span class="sxs-lookup"><span data-stu-id="7938c-901">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="7938c-902">20 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-902">November 20, 2018</span></span>

<span data-ttu-id="7938c-903">Versão 2.0.51</span><span class="sxs-lookup"><span data-stu-id="7938c-903">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="7938c-904">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-904">Core</span></span>
* <span data-ttu-id="7938c-905">Logon do MSI alterado para não reutilizar o nome da assinatura na identidade</span><span class="sxs-lookup"><span data-stu-id="7938c-905">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-906">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-906">ACR</span></span>
* <span data-ttu-id="7938c-907">Token de contexto adicionado à etapa da tarefa</span><span class="sxs-lookup"><span data-stu-id="7938c-907">Added context token to task step</span></span>
* <span data-ttu-id="7938c-908">Suporte adicionado para definir segredos na execução do acr para espelhar a tarefa do acr</span><span class="sxs-lookup"><span data-stu-id="7938c-908">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="7938c-909">Suporte aprimorado para `--top` e `--orderby` para os comandos `show-tags` e `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="7938c-909">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-910">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-910">Appservice</span></span>
* <span data-ttu-id="7938c-911">Tempo limite padrão para a implantação do zip alterado para sondar o status aumentado para 5 minutos, também adicionando uma propriedade de tempo limite para personalizar esse valor</span><span class="sxs-lookup"><span data-stu-id="7938c-911">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="7938c-912">Padrão `node_version` atualizado.</span><span class="sxs-lookup"><span data-stu-id="7938c-912">Updated the default `node_version`.</span></span> <span data-ttu-id="7938c-913">Redefinir a ação de troca de slots durante uma troca de duas fases preserva todas as configurações do aplicativo e cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="7938c-913">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="7938c-914">Verificação da SKU no lado do cliente removida para o Linux criar o plano do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="7938c-914">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="7938c-915">Erro corrigido ao tentar obter o status de implantação do zip</span><span class="sxs-lookup"><span data-stu-id="7938c-915">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="7938c-916">Iot Central</span><span class="sxs-lookup"><span data-stu-id="7938c-916">IotCentral</span></span>
* <span data-ttu-id="7938c-917">Verificação de disponibilidade do subdomínio adicionada ao criar um aplicativo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="7938c-917">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="7938c-918">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7938c-918">KeyVault</span></span>
* <span data-ttu-id="7938c-919">Bug corrigido em que os erros podem ter sido ignorados</span><span class="sxs-lookup"><span data-stu-id="7938c-919">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="7938c-920">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-920">Network</span></span>
* <span data-ttu-id="7938c-921">Subcomandos `root-cert` adicionados a `application-gateway` para lidar com os certificados de raiz confiável</span><span class="sxs-lookup"><span data-stu-id="7938c-921">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="7938c-922">Opções `--min-capacity` e `--custom-error-pages` adicionadas a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="7938c-922">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="7938c-923">`--zones` adicionado para suporte da zona de disponibilidade a `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="7938c-923">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="7938c-924">Argumentos `--file-upload-limit`, `--max-request-body-size` e `--request-body-check` a `application-gateway waf-config set` adicionados</span><span class="sxs-lookup"><span data-stu-id="7938c-924">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="7938c-925">Rdbms</span><span class="sxs-lookup"><span data-stu-id="7938c-925">Rdbms</span></span>
* <span data-ttu-id="7938c-926">Comandos vnet do mariadb adicionados</span><span class="sxs-lookup"><span data-stu-id="7938c-926">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="7938c-927">Rbac</span><span class="sxs-lookup"><span data-stu-id="7938c-927">Rbac</span></span>
* <span data-ttu-id="7938c-928">Um problema corrigido ao tentar atualizar credenciais inalteradas em `ad app update`</span><span class="sxs-lookup"><span data-stu-id="7938c-928">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="7938c-929">Avisos de saída adicionados para comunicar alterações de falha em um futuro próximo para `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="7938c-929">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="7938c-930">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-930">Storage</span></span>
* <span data-ttu-id="7938c-931">Melhor manipulação de casos incomuns para os comandos da cópia de armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-931">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="7938c-932">Corrigido o problema em que `storage blob copy start-batch` não usava credenciais de logon quando as contas de origem e destino eram iguais</span><span class="sxs-lookup"><span data-stu-id="7938c-932">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="7938c-933">Bug corrigido com `storage [blob|file] url` em que `sas_token` não foi incorporado na URL</span><span class="sxs-lookup"><span data-stu-id="7938c-933">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="7938c-934">Aviso de alteração da falha adicionado a `[blob|container] list`: produzirá apenas os primeiros 5.000 resultados por padrão</span><span class="sxs-lookup"><span data-stu-id="7938c-934">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-935">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-935">VM</span></span>
* <span data-ttu-id="7938c-936">Suporte adicionado a `[vm|vmss] create --storage-sku` para especificar a SKU da conta de armazenamento para o SO gerenciado e os discos de dados separadamente</span><span class="sxs-lookup"><span data-stu-id="7938c-936">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="7938c-937">Parâmetros do nome da versão alterados de `sig image-version` para `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="7938c-937">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="7938c-938">Argumento `sig image-version` preterido `--image-version-name`, substituído por `--image-version`</span><span class="sxs-lookup"><span data-stu-id="7938c-938">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="7938c-939">Suporte adicionado para usar o disco local do SO a `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="7938c-939">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="7938c-940">Adicionado o suporte ao `--no-wait` para `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="7938c-940">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="7938c-941">Adicionado o comando `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="7938c-941">Added `snapshot wait` command</span></span>
* <span data-ttu-id="7938c-942">Suporte adicionado para usar o nome da instância com `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="7938c-942">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="7938c-943">6 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-943">November 6, 2018</span></span>

<span data-ttu-id="7938c-944">Versão 2.0.50</span><span class="sxs-lookup"><span data-stu-id="7938c-944">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="7938c-945">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-945">Core</span></span>
* <span data-ttu-id="7938c-946">Foi adicionado suporte para o serviço principal sn + autenticação do emissor</span><span class="sxs-lookup"><span data-stu-id="7938c-946">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-947">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-947">ACR</span></span>
* <span data-ttu-id="7938c-948">Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa</span><span class="sxs-lookup"><span data-stu-id="7938c-948">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="7938c-949">Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação</span><span class="sxs-lookup"><span data-stu-id="7938c-949">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-950">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-950">ACS</span></span>
* <span data-ttu-id="7938c-951">[ALTERAÇÃO SIGNIFICATIVA] `enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão</span><span class="sxs-lookup"><span data-stu-id="7938c-951">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="7938c-952">Supervisor</span><span class="sxs-lookup"><span data-stu-id="7938c-952">Advisor</span></span>
* <span data-ttu-id="7938c-953">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="7938c-953">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="7938c-954">AMS</span><span class="sxs-lookup"><span data-stu-id="7938c-954">AMS</span></span>
* <span data-ttu-id="7938c-955">Novos grupos de comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="7938c-955">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="7938c-956">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="7938c-956">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="7938c-957">Adicionados parâmetros de criptografia com suporte para `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="7938c-957">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="7938c-958">O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido</span><span class="sxs-lookup"><span data-stu-id="7938c-958">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="7938c-959">Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="7938c-959">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="7938c-960">Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="7938c-960">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="7938c-961">Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="7938c-961">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="7938c-962">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming locator` foi substituído por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="7938c-962">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="7938c-963">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--content-keys` de `ams streaming locator` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="7938c-963">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="7938c-964">[ALTERAÇÃO SIGNIFICATIVA] `--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="7938c-964">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="7938c-965">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming policy` foi substituído por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="7938c-965">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="7938c-966">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="7938c-966">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="7938c-967">Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="7938c-967">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="7938c-968">Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado</span><span class="sxs-lookup"><span data-stu-id="7938c-968">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="7938c-969">[ALTERAÇÃO SIGNIFICATIVA] `--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="7938c-969">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="7938c-970">Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'.</span><span class="sxs-lookup"><span data-stu-id="7938c-970">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="7938c-971">Um ativo sem rótulo pode ser enviado assim: 'assetName='</span><span class="sxs-lookup"><span data-stu-id="7938c-971">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-972">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-972">AppService</span></span>
* <span data-ttu-id="7938c-973">Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido</span><span class="sxs-lookup"><span data-stu-id="7938c-973">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="7938c-974">Configurar</span><span class="sxs-lookup"><span data-stu-id="7938c-974">Configure</span></span>
* <span data-ttu-id="7938c-975">O YAML foi adicionado às opções de formato de saída</span><span class="sxs-lookup"><span data-stu-id="7938c-975">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="7938c-976">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-976">Container</span></span>
* <span data-ttu-id="7938c-977">Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml</span><span class="sxs-lookup"><span data-stu-id="7938c-977">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="7938c-978">EventHub</span><span class="sxs-lookup"><span data-stu-id="7938c-978">EventHub</span></span>
* <span data-ttu-id="7938c-979">O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-979">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="7938c-980">Interativo</span><span class="sxs-lookup"><span data-stu-id="7938c-980">Interactive</span></span>
* <span data-ttu-id="7938c-981">O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos</span><span class="sxs-lookup"><span data-stu-id="7938c-981">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="7938c-982">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7938c-982">Monitor</span></span>
* <span data-ttu-id="7938c-983">Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) para `--condition` em `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-983">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="7938c-984">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-984">Network</span></span>
* <span data-ttu-id="7938c-985">Os nomes de comandos `network interface-endpoint` foram preteridos em benefício de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="7938c-985">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="7938c-986">Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID</span><span class="sxs-lookup"><span data-stu-id="7938c-986">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="7938c-987">Foi corrigido um problema onde `--ip-tags` não funcionava corretamente com `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="7938c-987">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="7938c-988">Perfil</span><span class="sxs-lookup"><span data-stu-id="7938c-988">Profile</span></span>
* <span data-ttu-id="7938c-989">`--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado</span><span class="sxs-lookup"><span data-stu-id="7938c-989">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="7938c-990">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7938c-990">RDBMS</span></span>
* <span data-ttu-id="7938c-991">Adicionados comandos da réplica mysql</span><span class="sxs-lookup"><span data-stu-id="7938c-991">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-992">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-992">Resource</span></span>
* <span data-ttu-id="7938c-993">Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="7938c-993">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="7938c-994">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-994">Role</span></span>
* <span data-ttu-id="7938c-995">Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais</span><span class="sxs-lookup"><span data-stu-id="7938c-995">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="7938c-996">`ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="7938c-996">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="7938c-997">Suporte adicionado para conceder permissões a aplicativos do AAD</span><span class="sxs-lookup"><span data-stu-id="7938c-997">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-998">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-998">Storage</span></span>
* <span data-ttu-id="7938c-999">Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="7938c-999">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-1000">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1000">VM</span></span>
* <span data-ttu-id="7938c-1001">O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem</span><span class="sxs-lookup"><span data-stu-id="7938c-1001">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="7938c-1002">O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido</span><span class="sxs-lookup"><span data-stu-id="7938c-1002">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="7938c-1003">O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado</span><span class="sxs-lookup"><span data-stu-id="7938c-1003">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="7938c-1004">`vm secret format` foi alterado para exigir a saída json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="7938c-1004">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="7938c-1005">Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido</span><span class="sxs-lookup"><span data-stu-id="7938c-1005">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="7938c-1006">Validação de argumento aprimorado para `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="7938c-1006">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="7938c-1007">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1007">October 23, 2018</span></span>

<span data-ttu-id="7938c-1008">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="7938c-1008">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="7938c-1009">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-1009">Core</span></span>
* <span data-ttu-id="7938c-1010">Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`</span><span class="sxs-lookup"><span data-stu-id="7938c-1010">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="7938c-1011">Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="7938c-1011">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-1012">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-1012">ACR</span></span>
* <span data-ttu-id="7938c-1013">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="7938c-1013">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="7938c-1014">CDN</span><span class="sxs-lookup"><span data-stu-id="7938c-1014">CDN</span></span>
* <span data-ttu-id="7938c-1015">[ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="7938c-1015">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="7938c-1016">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="7938c-1016">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="7938c-1017">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-1017">Container</span></span>
* <span data-ttu-id="7938c-1018">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="7938c-1018">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="7938c-1019">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="7938c-1019">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="7938c-1020">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="7938c-1020">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="7938c-1021">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="7938c-1021">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="7938c-1022">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="7938c-1022">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="7938c-1023">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="7938c-1023">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="7938c-1024">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="7938c-1024">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7938c-1025">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7938c-1025">CosmosDB</span></span>
* <span data-ttu-id="7938c-1026">Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1026">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="7938c-1027">Interativo</span><span class="sxs-lookup"><span data-stu-id="7938c-1027">Interactive</span></span>
* <span data-ttu-id="7938c-1028">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="7938c-1028">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="7938c-1029">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="7938c-1029">IoT Central</span></span>
* <span data-ttu-id="7938c-1030">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="7938c-1030">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="7938c-1031">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="7938c-1031">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="7938c-1032">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7938c-1032">Monitor</span></span>
* <span data-ttu-id="7938c-1033">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="7938c-1033">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="7938c-1034">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="7938c-1034">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="7938c-1035">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="7938c-1035">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="7938c-1036">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="7938c-1036">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="7938c-1037">Adicionado `--namespace` como alias para a opção preterida `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="7938c-1037">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="7938c-1038">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="7938c-1038">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="7938c-1039">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="7938c-1039">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="7938c-1040">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="7938c-1040">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="7938c-1041">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="7938c-1041">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="7938c-1042">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1042">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="7938c-1043">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-1043">Network</span></span>
* <span data-ttu-id="7938c-1044">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="7938c-1044">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="7938c-1045">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="7938c-1045">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="7938c-1046">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7938c-1046">ServiceBus</span></span>
* <span data-ttu-id="7938c-1047">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="7938c-1047">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-1048">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-1048">SQL</span></span>
* <span data-ttu-id="7938c-1049">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="7938c-1049">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-1050">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-1050">Storage</span></span>
* <span data-ttu-id="7938c-1051">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="7938c-1051">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="7938c-1052">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="7938c-1052">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-1053">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1053">VM</span></span>
* <span data-ttu-id="7938c-1054">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1054">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="7938c-1055">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1055">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="7938c-1056">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1056">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="7938c-1057">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1057">October 16, 2018</span></span>

<span data-ttu-id="7938c-1058">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="7938c-1058">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-1059">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1059">VM</span></span>
* <span data-ttu-id="7938c-1060">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="7938c-1060">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="7938c-1061">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1061">October 9, 2018</span></span>

<span data-ttu-id="7938c-1062">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="7938c-1062">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="7938c-1063">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-1063">Core</span></span>
* <span data-ttu-id="7938c-1064">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="7938c-1064">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-1065">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-1065">ACR</span></span>
* <span data-ttu-id="7938c-1066">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="7938c-1066">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-1067">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-1067">ACS</span></span>
* <span data-ttu-id="7938c-1068">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="7938c-1068">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="7938c-1069">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="7938c-1069">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="7938c-1070">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="7938c-1070">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="7938c-1071">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="7938c-1071">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="7938c-1072">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-1072">Container</span></span>
* <span data-ttu-id="7938c-1073">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um tempo de execução específico</span><span class="sxs-lookup"><span data-stu-id="7938c-1073">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="7938c-1074">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="7938c-1074">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="7938c-1075">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="7938c-1075">Event Hub</span></span>
* <span data-ttu-id="7938c-1076">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="7938c-1076">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="7938c-1077">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="7938c-1077">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="7938c-1078">Extensões</span><span class="sxs-lookup"><span data-stu-id="7938c-1078">Extensions</span></span>
* <span data-ttu-id="7938c-1079">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="7938c-1079">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7938c-1080">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7938c-1080">HDInsight</span></span>
* <span data-ttu-id="7938c-1081">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="7938c-1081">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="7938c-1082">IoT</span><span class="sxs-lookup"><span data-stu-id="7938c-1082">IoT</span></span>
* <span data-ttu-id="7938c-1083">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="7938c-1083">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="7938c-1084">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7938c-1084">KeyVault</span></span>
* <span data-ttu-id="7938c-1085">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="7938c-1085">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="7938c-1086">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-1086">Network</span></span>
* <span data-ttu-id="7938c-1087">Corrigido `network dns zone create`: O comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="7938c-1087">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="7938c-1088">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="7938c-1088">See #6052</span></span>
* <span data-ttu-id="7938c-1089">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1089">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="7938c-1090">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="7938c-1090">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="7938c-1091">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="7938c-1091">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="7938c-1092">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="7938c-1092">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="7938c-1093">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="7938c-1093">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="7938c-1094">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="7938c-1094">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="7938c-1095">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-1095">Role</span></span>
* <span data-ttu-id="7938c-1096">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="7938c-1096">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="7938c-1097">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="7938c-1097">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="7938c-1098">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="7938c-1098">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="7938c-1099">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="7938c-1099">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="7938c-1100">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="7938c-1100">Service Bus</span></span>
* <span data-ttu-id="7938c-1101">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="7938c-1101">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-1102">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1102">VM</span></span>
* <span data-ttu-id="7938c-1103">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="7938c-1103">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="7938c-1104">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="7938c-1104">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="7938c-1105">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="7938c-1105">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="7938c-1106">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="7938c-1106">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="7938c-1107">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="7938c-1107">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="7938c-1108">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="7938c-1108">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="7938c-1109">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1109">September 21, 2018</span></span>

<span data-ttu-id="7938c-1110">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="7938c-1110">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-1111">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-1111">ACR</span></span>
* <span data-ttu-id="7938c-1112">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-1112">Added ACR Task commands</span></span>
* <span data-ttu-id="7938c-1113">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="7938c-1113">Added quick run command</span></span>
* <span data-ttu-id="7938c-1114">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="7938c-1114">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="7938c-1115">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-1115">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="7938c-1116">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="7938c-1116">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="7938c-1117">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="7938c-1117">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-1118">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-1118">ACS</span></span>
* <span data-ttu-id="7938c-1119">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="7938c-1119">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="7938c-1120">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="7938c-1120">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-1121">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-1121">AppService</span></span>

* <span data-ttu-id="7938c-1122">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="7938c-1122">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="7938c-1123">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="7938c-1123">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="7938c-1124">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="7938c-1124">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="7938c-1125">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="7938c-1125">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="7938c-1126">Lote</span><span class="sxs-lookup"><span data-stu-id="7938c-1126">Batch</span></span>
* <span data-ttu-id="7938c-1127">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="7938c-1127">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="7938c-1128">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="7938c-1128">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="7938c-1129">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1129">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="7938c-1130">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="7938c-1130">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7938c-1131">Lote AI</span><span class="sxs-lookup"><span data-stu-id="7938c-1131">Batch AI</span></span> 
* <span data-ttu-id="7938c-1132">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1132">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7938c-1133">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="7938c-1133">Cognitive Services</span></span>
* <span data-ttu-id="7938c-1134">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="7938c-1134">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="7938c-1135">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="7938c-1135">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="7938c-1136">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="7938c-1136">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="7938c-1137">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="7938c-1137">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="7938c-1138">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="7938c-1138">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="7938c-1139">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="7938c-1139">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="7938c-1140">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-1140">Container</span></span>
* <span data-ttu-id="7938c-1141">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="7938c-1141">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="7938c-1142">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="7938c-1142">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="7938c-1143">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="7938c-1143">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="7938c-1144">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="7938c-1144">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="7938c-1145">DataLake</span><span class="sxs-lookup"><span data-stu-id="7938c-1145">Datalake</span></span>
* <span data-ttu-id="7938c-1146">Comandos adicionados para regras da rede virtual</span><span class="sxs-lookup"><span data-stu-id="7938c-1146">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="7938c-1147">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="7938c-1147">Interactive Shell</span></span>
* <span data-ttu-id="7938c-1148">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="7938c-1148">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="7938c-1149">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="7938c-1149">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="7938c-1150">IoT</span><span class="sxs-lookup"><span data-stu-id="7938c-1150">IoT</span></span>
* <span data-ttu-id="7938c-1151">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="7938c-1151">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="7938c-1152">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7938c-1152">Key Vault</span></span>
* <span data-ttu-id="7938c-1153">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="7938c-1153">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="7938c-1154">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-1154">Network</span></span>
* <span data-ttu-id="7938c-1155">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="7938c-1155">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="7938c-1156">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="7938c-1156">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="7938c-1157">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="7938c-1157">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="7938c-1158">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="7938c-1158">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="7938c-1159">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="7938c-1159">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="7938c-1160">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="7938c-1160">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="7938c-1161">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="7938c-1161">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="7938c-1162">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="7938c-1162">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="7938c-1163">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="7938c-1163">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="7938c-1164">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="7938c-1164">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="7938c-1165">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="7938c-1165">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="7938c-1166">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="7938c-1166">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="7938c-1167">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="7938c-1167">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="7938c-1168">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="7938c-1168">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="7938c-1169">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="7938c-1169">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="7938c-1170">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="7938c-1170">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="7938c-1171">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="7938c-1171">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="7938c-1172">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="7938c-1172">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="7938c-1173">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7938c-1173">RDBMS</span></span>
* <span data-ttu-id="7938c-1174">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="7938c-1174">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="7938c-1175">Reserva</span><span class="sxs-lookup"><span data-stu-id="7938c-1175">Reservation</span></span>
* <span data-ttu-id="7938c-1176">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="7938c-1176">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="7938c-1177">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="7938c-1177">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="7938c-1178">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="7938c-1178">Manage App</span></span>
* <span data-ttu-id="7938c-1179">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="7938c-1179">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="7938c-1180">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="7938c-1180">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="7938c-1181">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-1181">Role</span></span>
* <span data-ttu-id="7938c-1182">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="7938c-1182">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="7938c-1183">SignalR</span><span class="sxs-lookup"><span data-stu-id="7938c-1183">SignalR</span></span>
* <span data-ttu-id="7938c-1184">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="7938c-1184">First release</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-1185">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-1185">Storage</span></span>
* <span data-ttu-id="7938c-1186">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="7938c-1186">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="7938c-1187">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="7938c-1187">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-1188">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1188">VM</span></span>
* <span data-ttu-id="7938c-1189">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="7938c-1189">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="7938c-1190">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="7938c-1190">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="7938c-1191">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1191">August 28, 2018</span></span>

<span data-ttu-id="7938c-1192">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="7938c-1192">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="7938c-1193">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-1193">Core</span></span>

* <span data-ttu-id="7938c-1194">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="7938c-1194">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="7938c-1195">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="7938c-1195">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-1196">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-1196">ACR</span></span>

* <span data-ttu-id="7938c-1197">Adicionada uma solução alternativa para operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="7938c-1197">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="7938c-1198">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="7938c-1198">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-1199">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-1199">ACS</span></span>

* <span data-ttu-id="7938c-1200">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="7938c-1200">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="7938c-1201">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="7938c-1201">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-1202">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-1202">AppService</span></span>

* <span data-ttu-id="7938c-1203">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="7938c-1203">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="7938c-1204">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="7938c-1204">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="7938c-1205">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="7938c-1205">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="7938c-1206">Backup</span><span class="sxs-lookup"><span data-stu-id="7938c-1206">Backup</span></span>

* <span data-ttu-id="7938c-1207">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="7938c-1207">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="7938c-1208">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="7938c-1208">Bot Service</span></span>

* <span data-ttu-id="7938c-1209">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="7938c-1209">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7938c-1210">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="7938c-1210">Cognitive Services</span></span>

* <span data-ttu-id="7938c-1211">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="7938c-1211">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="7938c-1212">IoT</span><span class="sxs-lookup"><span data-stu-id="7938c-1212">IoT</span></span>

* <span data-ttu-id="7938c-1213">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="7938c-1213">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="7938c-1214">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7938c-1214">Monitor</span></span>

* <span data-ttu-id="7938c-1215">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="7938c-1215">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="7938c-1216">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="7938c-1216">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="7938c-1217">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-1217">Network</span></span>

* <span data-ttu-id="7938c-1218">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="7938c-1218">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-1219">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-1219">Resource</span></span>

* <span data-ttu-id="7938c-1220">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="7938c-1220">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-1221">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-1221">Storage</span></span>

* <span data-ttu-id="7938c-1222">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="7938c-1222">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-1223">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1223">VM</span></span>

* <span data-ttu-id="7938c-1224">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="7938c-1224">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="7938c-1225">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1225">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="7938c-1226">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1226">Auguest 14, 2018</span></span>

<span data-ttu-id="7938c-1227">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="7938c-1227">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="7938c-1228">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-1228">Core</span></span>

* <span data-ttu-id="7938c-1229">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="7938c-1229">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="7938c-1230">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="7938c-1230">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="7938c-1231">Telemetria</span><span class="sxs-lookup"><span data-stu-id="7938c-1231">Telemetry</span></span>

* <span data-ttu-id="7938c-1232">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="7938c-1232">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-1233">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-1233">ACR</span></span>

* <span data-ttu-id="7938c-1234">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="7938c-1234">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="7938c-1235">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="7938c-1235">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-1236">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-1236">ACS</span></span>

* <span data-ttu-id="7938c-1237">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="7938c-1237">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="7938c-1238">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="7938c-1238">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="7938c-1239">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="7938c-1239">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="7938c-1240">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="7938c-1240">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="7938c-1241">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="7938c-1241">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="7938c-1242">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-1242">AppService</span></span>

* <span data-ttu-id="7938c-1243">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="7938c-1243">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="7938c-1244">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="7938c-1244">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="7938c-1245">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7938c-1245">BatchAI</span></span>

* <span data-ttu-id="7938c-1246">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="7938c-1246">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="7938c-1247">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-1247">Container</span></span>

* <span data-ttu-id="7938c-1248">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-1248">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="7938c-1249">IoT</span><span class="sxs-lookup"><span data-stu-id="7938c-1249">IoT</span></span>

* <span data-ttu-id="7938c-1250">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="7938c-1250">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="7938c-1251">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="7938c-1251">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="7938c-1252">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="7938c-1252">Iot Central</span></span>

* <span data-ttu-id="7938c-1253">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="7938c-1253">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="7938c-1254">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7938c-1254">KeyVault</span></span>


* <span data-ttu-id="7938c-1255">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="7938c-1255">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="7938c-1256">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="7938c-1256">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="7938c-1257">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="7938c-1257">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="7938c-1258">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="7938c-1258">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="7938c-1259">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="7938c-1259">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="7938c-1260">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="7938c-1260">Relay</span></span>

* <span data-ttu-id="7938c-1261">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="7938c-1261">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-1262">Sql</span><span class="sxs-lookup"><span data-stu-id="7938c-1262">Sql</span></span>

* <span data-ttu-id="7938c-1263">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="7938c-1263">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-1264">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-1264">Storage</span></span>

* <span data-ttu-id="7938c-1265">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="7938c-1265">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="7938c-1266">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="7938c-1266">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="7938c-1267">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="7938c-1267">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="7938c-1268">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="7938c-1268">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="7938c-1269">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-1269">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-1270">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1270">VM</span></span>

* <span data-ttu-id="7938c-1271">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="7938c-1271">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="7938c-1272">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1272">July 31, 2018</span></span>

<span data-ttu-id="7938c-1273">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="7938c-1273">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-1274">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-1274">ACR</span></span>

* <span data-ttu-id="7938c-1275">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="7938c-1275">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="7938c-1276">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="7938c-1276">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-1277">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-1277">ACS</span></span>

* <span data-ttu-id="7938c-1278">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="7938c-1278">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="7938c-1279">Lote</span><span class="sxs-lookup"><span data-stu-id="7938c-1279">Batch</span></span>

* <span data-ttu-id="7938c-1280">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="7938c-1280">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="7938c-1281">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-1281">Container</span></span>

* <span data-ttu-id="7938c-1282">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="7938c-1282">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="7938c-1283">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-1283">Network</span></span>

* <span data-ttu-id="7938c-1284">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="7938c-1284">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="7938c-1285">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-1285">Resource</span></span>

* <span data-ttu-id="7938c-1286">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="7938c-1286">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="7938c-1287">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="7938c-1287">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="7938c-1288">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-1288">Role</span></span>

* <span data-ttu-id="7938c-1289">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="7938c-1289">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="7938c-1290">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="7938c-1290">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="7938c-1291">Search</span><span class="sxs-lookup"><span data-stu-id="7938c-1291">Search</span></span>

* <span data-ttu-id="7938c-1292">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="7938c-1292">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="7938c-1293">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="7938c-1293">Service Bus</span></span>

* <span data-ttu-id="7938c-1294">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="7938c-1294">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="7938c-1295">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="7938c-1295">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="7938c-1296">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="7938c-1296">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="7938c-1297">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="7938c-1297">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-1298">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-1298">Storage</span></span>

* <span data-ttu-id="7938c-1299">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="7938c-1299">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="7938c-1300">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="7938c-1300">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-1301">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1301">VM</span></span>

* <span data-ttu-id="7938c-1302">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="7938c-1302">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="7938c-1303">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="7938c-1303">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="7938c-1304">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1304">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="7938c-1305">[ALTERAÇÃO SIGNIFICATIVA] `[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="7938c-1305">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="7938c-1306">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1306">July 18, 2018</span></span>

<span data-ttu-id="7938c-1307">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="7938c-1307">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="7938c-1308">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-1308">Core</span></span>

* <span data-ttu-id="7938c-1309">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="7938c-1309">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="7938c-1310">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="7938c-1310">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="7938c-1311">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="7938c-1311">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-1312">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-1312">ACR</span></span>

* <span data-ttu-id="7938c-1313">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="7938c-1313">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="7938c-1314">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="7938c-1314">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="7938c-1315">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="7938c-1315">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="7938c-1316">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="7938c-1316">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-1317">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-1317">ACS</span></span>

* <span data-ttu-id="7938c-1318">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="7938c-1318">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-1319">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-1319">AppService</span></span>

* <span data-ttu-id="7938c-1320">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="7938c-1320">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="7938c-1321">Lote</span><span class="sxs-lookup"><span data-stu-id="7938c-1321">Batch</span></span>

* <span data-ttu-id="7938c-1322">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="7938c-1322">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="7938c-1323">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="7938c-1323">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7938c-1324">Lote AI</span><span class="sxs-lookup"><span data-stu-id="7938c-1324">Batch AI</span></span>

* <span data-ttu-id="7938c-1325">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="7938c-1325">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="7938c-1326">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-1326">Container</span></span>

* <span data-ttu-id="7938c-1327">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="7938c-1327">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="7938c-1328">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="7938c-1328">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="7938c-1329">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-1329">Network</span></span>

* <span data-ttu-id="7938c-1330">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="7938c-1330">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="7938c-1331">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="7938c-1331">Added `network nic wait`</span></span>
* <span data-ttu-id="7938c-1332">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="7938c-1332">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="7938c-1333">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="7938c-1333">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="7938c-1334">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-1334">Resource</span></span>

* <span data-ttu-id="7938c-1335">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="7938c-1335">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="7938c-1336">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="7938c-1336">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="7938c-1337">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="7938c-1337">Added `deployment wait` command</span></span>
* <span data-ttu-id="7938c-1338">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="7938c-1338">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-1339">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-1339">SQL</span></span>

* <span data-ttu-id="7938c-1340">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1340">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="7938c-1341">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="7938c-1341">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="7938c-1342">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="7938c-1342">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-1343">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-1343">Storage</span></span>

* <span data-ttu-id="7938c-1344">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="7938c-1344">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-1345">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1345">VM</span></span>

* <span data-ttu-id="7938c-1346">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="7938c-1346">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="7938c-1347">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="7938c-1347">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="7938c-1348">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="7938c-1348">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="7938c-1349">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1349">July 3, 2018</span></span>

<span data-ttu-id="7938c-1350">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="7938c-1350">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="7938c-1351">AKS</span><span class="sxs-lookup"><span data-stu-id="7938c-1351">AKS</span></span>

* <span data-ttu-id="7938c-1352">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="7938c-1352">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="7938c-1353">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1353">July 3, 2018</span></span>

<span data-ttu-id="7938c-1354">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="7938c-1354">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="7938c-1355">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-1355">Core</span></span>

* <span data-ttu-id="7938c-1356">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="7938c-1356">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-1357">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-1357">ACR</span></span>

* <span data-ttu-id="7938c-1358">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="7938c-1358">Added polling build status</span></span>
* <span data-ttu-id="7938c-1359">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="7938c-1359">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="7938c-1360">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="7938c-1360">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-1361">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-1361">ACS</span></span>

* <span data-ttu-id="7938c-1362">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="7938c-1362">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="7938c-1363">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="7938c-1363">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="7938c-1364">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="7938c-1364">Updated options for `aks browse` command.</span></span> <span data-ttu-id="7938c-1365">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="7938c-1365">Added `--listen-port` support</span></span>
* <span data-ttu-id="7938c-1366">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="7938c-1366">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="7938c-1367">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="7938c-1367">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="7938c-1368">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="7938c-1368">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-1369">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-1369">AppService</span></span>

* <span data-ttu-id="7938c-1370">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="7938c-1370">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="7938c-1371">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="7938c-1371">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="7938c-1372">Backup</span><span class="sxs-lookup"><span data-stu-id="7938c-1372">Backup</span></span>

* <span data-ttu-id="7938c-1373">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="7938c-1373">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="7938c-1374">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7938c-1374">BatchAI</span></span>

* <span data-ttu-id="7938c-1375">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="7938c-1375">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="7938c-1376">Nuvem</span><span class="sxs-lookup"><span data-stu-id="7938c-1376">Cloud</span></span>

* <span data-ttu-id="7938c-1377">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="7938c-1377">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="7938c-1378">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-1378">Container</span></span>

* <span data-ttu-id="7938c-1379">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="7938c-1379">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="7938c-1380">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="7938c-1380">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="7938c-1381">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="7938c-1381">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="7938c-1382">Extensão</span><span class="sxs-lookup"><span data-stu-id="7938c-1382">Extension</span></span>

* <span data-ttu-id="7938c-1383">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="7938c-1383">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="7938c-1384">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-1384">Network</span></span>

* <span data-ttu-id="7938c-1385">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="7938c-1385">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="7938c-1386">Rdbms</span><span class="sxs-lookup"><span data-stu-id="7938c-1386">Rdbms</span></span>

* <span data-ttu-id="7938c-1387">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="7938c-1387">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-1388">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-1388">Resource</span></span>

* <span data-ttu-id="7938c-1389">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="7938c-1389">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-1390">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1390">VM</span></span>

* <span data-ttu-id="7938c-1391">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="7938c-1391">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="7938c-1392">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1392">June 25, 2018</span></span>

<span data-ttu-id="7938c-1393">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="7938c-1393">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="7938c-1394">CLI</span><span class="sxs-lookup"><span data-stu-id="7938c-1394">CLI</span></span>

* <span data-ttu-id="7938c-1395">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="7938c-1395">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="7938c-1396">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1396">June 19, 2018</span></span>

<span data-ttu-id="7938c-1397">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="7938c-1397">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="7938c-1398">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-1398">Core</span></span>

* <span data-ttu-id="7938c-1399">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="7938c-1399">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-1400">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-1400">ACR</span></span>

* <span data-ttu-id="7938c-1401">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="7938c-1401">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="7938c-1402">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="7938c-1402">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-1403">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-1403">ACS</span></span>

* <span data-ttu-id="7938c-1404">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="7938c-1404">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="7938c-1405">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="7938c-1405">Added `--update` support</span></span>
* <span data-ttu-id="7938c-1406">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="7938c-1406">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="7938c-1407">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="7938c-1407">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="7938c-1408">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="7938c-1408">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="7938c-1409">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="7938c-1409">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="7938c-1410">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="7938c-1410">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="7938c-1411">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="7938c-1411">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-1412">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-1412">AppService</span></span>

* <span data-ttu-id="7938c-1413">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="7938c-1413">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="7938c-1414">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="7938c-1414">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="7938c-1415">Lote</span><span class="sxs-lookup"><span data-stu-id="7938c-1415">Batch</span></span>

* <span data-ttu-id="7938c-1416">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="7938c-1416">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7938c-1417">Lote AI</span><span class="sxs-lookup"><span data-stu-id="7938c-1417">Batch AI</span></span>

* <span data-ttu-id="7938c-1418">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="7938c-1418">Added support for workspaces.</span></span> <span data-ttu-id="7938c-1419">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="7938c-1419">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="7938c-1420">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="7938c-1420">Added support for experiments.</span></span> <span data-ttu-id="7938c-1421">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="7938c-1421">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="7938c-1422">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="7938c-1422">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="7938c-1423">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="7938c-1423">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="7938c-1424">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="7938c-1424">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="7938c-1425">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="7938c-1425">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="7938c-1426">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="7938c-1426">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="7938c-1427">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="7938c-1427">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="7938c-1428">[ALTERAÇÃO SIGNIFICATIVA] `--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="7938c-1428">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="7938c-1429">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="7938c-1429">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="7938c-1430">[ALTERAÇÃO SIGNIFICATIVA] `--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="7938c-1430">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="7938c-1431">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="7938c-1431">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="7938c-1432">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="7938c-1432">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="7938c-1433">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="7938c-1433">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="7938c-1434">[ALTERAÇÃO SIGNIFICATIVA] `--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1434">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="7938c-1435">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="7938c-1435">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="7938c-1436">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="7938c-1436">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="7938c-1437">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="7938c-1437">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="7938c-1438">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="7938c-1438">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="7938c-1439">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="7938c-1439">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="7938c-1440">Mapas</span><span class="sxs-lookup"><span data-stu-id="7938c-1440">Maps</span></span>

* <span data-ttu-id="7938c-1441">[ALTERAÇÃO SIGNIFICATIVA] `maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="7938c-1441">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="7938c-1442">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-1442">Network</span></span>

* <span data-ttu-id="7938c-1443">Foi adicionado suporte a `https` para `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="7938c-1443">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="7938c-1444">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="7938c-1444">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="7938c-1445">#6502</span><span class="sxs-lookup"><span data-stu-id="7938c-1445">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="7938c-1446">Reservas</span><span class="sxs-lookup"><span data-stu-id="7938c-1446">Reservations</span></span>

* <span data-ttu-id="7938c-1447">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="7938c-1447">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="7938c-1448">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="7938c-1448">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="7938c-1449">[ALTERAÇÃO SIGNIFICATIVA] `kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="7938c-1449">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="7938c-1450">[ALTERAÇÃO SIGNIFICATIVA] `capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="7938c-1450">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="7938c-1451">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="7938c-1451">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="7938c-1452">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="7938c-1452">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="7938c-1453">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-1453">Role</span></span>

* <span data-ttu-id="7938c-1454">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="7938c-1454">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-1455">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-1455">SQL</span></span>

* <span data-ttu-id="7938c-1456">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="7938c-1456">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-1457">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-1457">Storage</span></span>

* <span data-ttu-id="7938c-1458">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="7938c-1458">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-1459">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1459">VM</span></span>

* <span data-ttu-id="7938c-1460">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1460">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="7938c-1461">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="7938c-1461">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="7938c-1462">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="7938c-1462">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="7938c-1463">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1463">June 13, 2018</span></span>

<span data-ttu-id="7938c-1464">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="7938c-1464">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="7938c-1465">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-1465">Core</span></span>

* <span data-ttu-id="7938c-1466">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="7938c-1466">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="7938c-1467">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1467">June 13, 2018</span></span>

<span data-ttu-id="7938c-1468">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="7938c-1468">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="7938c-1469">AKS</span><span class="sxs-lookup"><span data-stu-id="7938c-1469">AKS</span></span>

* <span data-ttu-id="7938c-1470">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1470">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="7938c-1471">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="7938c-1471">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="7938c-1472">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1472">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="7938c-1473">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1473">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="7938c-1474">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1474">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-1475">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-1475">AppService</span></span>

* <span data-ttu-id="7938c-1476">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="7938c-1476">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="7938c-1477">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1477">June 5, 2018</span></span>

<span data-ttu-id="7938c-1478">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="7938c-1478">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="7938c-1479">Interativo</span><span class="sxs-lookup"><span data-stu-id="7938c-1479">Interactive</span></span>

* <span data-ttu-id="7938c-1480">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="7938c-1480">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="7938c-1481">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1481">June 5, 2018</span></span>

<span data-ttu-id="7938c-1482">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="7938c-1482">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="7938c-1483">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-1483">Core</span></span>

* <span data-ttu-id="7938c-1484">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="7938c-1484">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="7938c-1485">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="7938c-1485">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-1486">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-1486">ACR</span></span>

* <span data-ttu-id="7938c-1487">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="7938c-1487">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="7938c-1488">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="7938c-1488">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="7938c-1489">AKS</span><span class="sxs-lookup"><span data-stu-id="7938c-1489">AKS</span></span>

* <span data-ttu-id="7938c-1490">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="7938c-1490">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="7938c-1491">Lote</span><span class="sxs-lookup"><span data-stu-id="7938c-1491">Batch</span></span>

* <span data-ttu-id="7938c-1492">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="7938c-1492">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="7938c-1493">IOT</span><span class="sxs-lookup"><span data-stu-id="7938c-1493">IOT</span></span>

* <span data-ttu-id="7938c-1494">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="7938c-1494">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="7938c-1495">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-1495">Network</span></span>

* <span data-ttu-id="7938c-1496">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="7938c-1496">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="7938c-1497">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="7938c-1497">Policy Insights</span></span>

* <span data-ttu-id="7938c-1498">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="7938c-1498">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="7938c-1499">ARM</span><span class="sxs-lookup"><span data-stu-id="7938c-1499">ARM</span></span>

* <span data-ttu-id="7938c-1500">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="7938c-1500">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-1501">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-1501">SQL</span></span>

* <span data-ttu-id="7938c-1502">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="7938c-1502">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="7938c-1503">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="7938c-1503">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="7938c-1504">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-1504">Storage</span></span>

* <span data-ttu-id="7938c-1505">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="7938c-1505">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-1506">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1506">VM</span></span>

* <span data-ttu-id="7938c-1507">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="7938c-1507">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="7938c-1508">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1508">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="7938c-1509">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1509">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="7938c-1510">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1510">May 22, 2018</span></span>

<span data-ttu-id="7938c-1511">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="7938c-1511">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="7938c-1512">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-1512">Core</span></span>

* <span data-ttu-id="7938c-1513">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="7938c-1513">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-1514">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-1514">ACS</span></span>

* <span data-ttu-id="7938c-1515">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="7938c-1515">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="7938c-1516">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="7938c-1516">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-1517">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-1517">AppService</span></span>

* <span data-ttu-id="7938c-1518">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="7938c-1518">Improved generic update commands</span></span>
* <span data-ttu-id="7938c-1519">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="7938c-1519">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="7938c-1520">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-1520">Container</span></span>

* <span data-ttu-id="7938c-1521">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="7938c-1521">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="7938c-1522">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-1522">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="7938c-1523">Extensão</span><span class="sxs-lookup"><span data-stu-id="7938c-1523">Extension</span></span>

* <span data-ttu-id="7938c-1524">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="7938c-1524">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="7938c-1525">Interativo</span><span class="sxs-lookup"><span data-stu-id="7938c-1525">Interactive</span></span>

* <span data-ttu-id="7938c-1526">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="7938c-1526">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="7938c-1527">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="7938c-1527">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="7938c-1528">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7938c-1528">KeyVault</span></span>

* <span data-ttu-id="7938c-1529">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="7938c-1529">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="7938c-1530">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-1530">Network</span></span>

* <span data-ttu-id="7938c-1531">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="7938c-1531">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="7938c-1532">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="7938c-1532">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-1533">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-1533">SQL</span></span>

* <span data-ttu-id="7938c-1534">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="7938c-1534">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="7938c-1535">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="7938c-1535">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="7938c-1536">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="7938c-1536">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="7938c-1537">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7938c-1537">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="7938c-1538">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="7938c-1538">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="7938c-1539">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="7938c-1539">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="7938c-1540">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="7938c-1540">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="7938c-1541">`edition`.</span><span class="sxs-lookup"><span data-stu-id="7938c-1541">`edition`.</span></span> <span data-ttu-id="7938c-1542">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="7938c-1542">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="7938c-1543">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="7938c-1543">`elasticPoolName`.</span></span> <span data-ttu-id="7938c-1544">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="7938c-1544">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="7938c-1545">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="7938c-1545">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="7938c-1546">`edition`.</span><span class="sxs-lookup"><span data-stu-id="7938c-1546">`edition`.</span></span> <span data-ttu-id="7938c-1547">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="7938c-1547">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="7938c-1548">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="7938c-1548">`dtu`.</span></span> <span data-ttu-id="7938c-1549">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="7938c-1549">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="7938c-1550">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="7938c-1550">`databaseDtuMin`.</span></span> <span data-ttu-id="7938c-1551">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="7938c-1551">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="7938c-1552">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="7938c-1552">`databaseDtuMax`.</span></span> <span data-ttu-id="7938c-1553">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="7938c-1553">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="7938c-1554">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="7938c-1554">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="7938c-1555">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="7938c-1555">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-1556">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-1556">Storage</span></span>

* <span data-ttu-id="7938c-1557">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="7938c-1557">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="7938c-1558">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="7938c-1558">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-1559">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1559">VM</span></span>

* <span data-ttu-id="7938c-1560">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="7938c-1560">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="7938c-1561">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="7938c-1561">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="7938c-1562">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="7938c-1562">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="7938c-1563">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="7938c-1563">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="7938c-1564">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="7938c-1564">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="7938c-1565">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1565">May 7, 2018</span></span>

<span data-ttu-id="7938c-1566">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="7938c-1566">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="7938c-1567">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-1567">Core</span></span>

* <span data-ttu-id="7938c-1568">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="7938c-1568">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="7938c-1569">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="7938c-1569">Added limited support for positional arguments</span></span>
* <span data-ttu-id="7938c-1570">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="7938c-1570">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="7938c-1571">#5591</span><span class="sxs-lookup"><span data-stu-id="7938c-1571">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="7938c-1572">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="7938c-1572">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="7938c-1573">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="7938c-1573">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="7938c-1574">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="7938c-1574">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="7938c-1575">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="7938c-1575">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="7938c-1576">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="7938c-1576">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-1577">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-1577">ACR</span></span>

* <span data-ttu-id="7938c-1578">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-1578">Added ACR Build commands</span></span>
* <span data-ttu-id="7938c-1579">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="7938c-1579">Improved resource not found error messages</span></span>
* <span data-ttu-id="7938c-1580">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="7938c-1580">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="7938c-1581">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="7938c-1581">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="7938c-1582">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="7938c-1582">Improved repository commands error messages</span></span>
* <span data-ttu-id="7938c-1583">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="7938c-1583">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-1584">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-1584">ACS</span></span>

* <span data-ttu-id="7938c-1585">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="7938c-1585">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="7938c-1586">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="7938c-1586">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="7938c-1587">AMS</span><span class="sxs-lookup"><span data-stu-id="7938c-1587">AMS</span></span>

* <span data-ttu-id="7938c-1588">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="7938c-1588">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-1589">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-1589">Appservice</span></span>

* <span data-ttu-id="7938c-1590">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="7938c-1590">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="7938c-1591">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="7938c-1591">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="7938c-1592">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="7938c-1592">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="7938c-1593">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="7938c-1593">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7938c-1594">Lote AI</span><span class="sxs-lookup"><span data-stu-id="7938c-1594">Batch AI</span></span>

* <span data-ttu-id="7938c-1595">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="7938c-1595">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7938c-1596">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="7938c-1596">Cognitive Services</span></span>

* <span data-ttu-id="7938c-1597">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="7938c-1597">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="7938c-1598">Consumo</span><span class="sxs-lookup"><span data-stu-id="7938c-1598">Consumption</span></span>

* <span data-ttu-id="7938c-1599">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="7938c-1599">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="7938c-1600">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-1600">Container</span></span>

* <span data-ttu-id="7938c-1601">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="7938c-1601">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="7938c-1602">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7938c-1602">Cosmos DB</span></span>

* <span data-ttu-id="7938c-1603">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7938c-1603">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="7938c-1604">DMS</span><span class="sxs-lookup"><span data-stu-id="7938c-1604">DMS</span></span>

* <span data-ttu-id="7938c-1605">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="7938c-1605">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="7938c-1606">Extensão</span><span class="sxs-lookup"><span data-stu-id="7938c-1606">Extension</span></span>

* <span data-ttu-id="7938c-1607">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="7938c-1607">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="7938c-1608">Interativo</span><span class="sxs-lookup"><span data-stu-id="7938c-1608">Interactive</span></span>

* <span data-ttu-id="7938c-1609">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="7938c-1609">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="7938c-1610">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="7938c-1610">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="7938c-1611">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="7938c-1611">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="7938c-1612">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="7938c-1612">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="7938c-1613">Laboratório</span><span class="sxs-lookup"><span data-stu-id="7938c-1613">Lab</span></span>

* <span data-ttu-id="7938c-1614">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="7938c-1614">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="7938c-1615">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-1615">Network</span></span>

* <span data-ttu-id="7938c-1616">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="7938c-1616">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="7938c-1617">Perfil</span><span class="sxs-lookup"><span data-stu-id="7938c-1617">Profile</span></span>

* <span data-ttu-id="7938c-1618">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="7938c-1618">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="7938c-1619">[ALTERAÇÃO SIGNIFICATIVA] `--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="7938c-1619">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="7938c-1620">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="7938c-1620">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="7938c-1621">Redis</span><span class="sxs-lookup"><span data-stu-id="7938c-1621">Redis</span></span>

* <span data-ttu-id="7938c-1622">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="7938c-1622">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="7938c-1623">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="7938c-1623">Deprecated `redis list-all`.</span></span> <span data-ttu-id="7938c-1624">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="7938c-1624">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="7938c-1625">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="7938c-1625">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="7938c-1626">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="7938c-1626">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="7938c-1627">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-1627">Role</span></span>

* <span data-ttu-id="7938c-1628">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="7938c-1628">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-1629">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-1629">Storage</span></span>

* <span data-ttu-id="7938c-1630">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="7938c-1630">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="7938c-1631">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="7938c-1631">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="7938c-1632">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="7938c-1632">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="7938c-1633">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="7938c-1633">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="7938c-1634">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="7938c-1634">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-1635">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1635">VM</span></span>

* <span data-ttu-id="7938c-1636">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="7938c-1636">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="7938c-1637">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="7938c-1637">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="7938c-1638">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="7938c-1638">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="7938c-1639">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="7938c-1639">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="7938c-1640">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="7938c-1640">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="7938c-1641">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="7938c-1641">Added write accelerator support</span></span>
* <span data-ttu-id="7938c-1642">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="7938c-1642">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="7938c-1643">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="7938c-1643">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="7938c-1644">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="7938c-1644">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="7938c-1645">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1645">April 10, 2018</span></span>

<span data-ttu-id="7938c-1646">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="7938c-1646">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-1647">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-1647">ACR</span></span>

* <span data-ttu-id="7938c-1648">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="7938c-1648">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-1649">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-1649">ACS</span></span>

* <span data-ttu-id="7938c-1650">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="7938c-1650">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-1651">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-1651">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="7938c-1653">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="7938c-1653">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="7938c-1654">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7938c-1654">BatchAI</span></span>

* <span data-ttu-id="7938c-1655">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="7938c-1655">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="7938c-1656">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="7938c-1656">Job level mounting</span></span>
  - <span data-ttu-id="7938c-1657">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="7938c-1657">Environment variables with secret values</span></span>
  - <span data-ttu-id="7938c-1658">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="7938c-1658">Performance counters settings</span></span>
  - <span data-ttu-id="7938c-1659">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="7938c-1659">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="7938c-1660">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="7938c-1660">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="7938c-1661">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="7938c-1661">Usage and limits reporting</span></span>
  - <span data-ttu-id="7938c-1662">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="7938c-1662">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="7938c-1663">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="7938c-1663">Support for custom images</span></span>
  - <span data-ttu-id="7938c-1664">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="7938c-1664">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="7938c-1665">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="7938c-1665">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="7938c-1666">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="7938c-1666">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="7938c-1667">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="7938c-1667">National clouds are supported</span></span>
* <span data-ttu-id="7938c-1668">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="7938c-1668">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="7938c-1669">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="7938c-1669">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="7938c-1670">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="7938c-1670">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="7938c-1671">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="7938c-1671">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="7938c-1672">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="7938c-1672">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="7938c-1673">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="7938c-1673">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="7938c-1674">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="7938c-1674">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="7938c-1675">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="7938c-1675">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="7938c-1676">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="7938c-1676">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="7938c-1677">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1677">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="7938c-1678">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="7938c-1678">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="7938c-1679">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="7938c-1679">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="7938c-1680">[ALTERAÇÃO SIGNIFICATIVA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1680">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="7938c-1681">Cobrança</span><span class="sxs-lookup"><span data-stu-id="7938c-1681">Billing</span></span>

* <span data-ttu-id="7938c-1682">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="7938c-1682">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="7938c-1683">Consumo</span><span class="sxs-lookup"><span data-stu-id="7938c-1683">Consumption</span></span>

* <span data-ttu-id="7938c-1684">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="7938c-1684">Added `marketplace` commands</span></span>
* <span data-ttu-id="7938c-1685">[ALTERAÇÃO SIGNIFICATIVA] `reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="7938c-1685">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="7938c-1686">[ALTERAÇÃO SIGNIFICATIVA] `reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="7938c-1686">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="7938c-1687">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="7938c-1687">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="7938c-1688">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="7938c-1688">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="7938c-1689">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="7938c-1689">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="7938c-1690">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-1690">Container</span></span>

* <span data-ttu-id="7938c-1691">Adição dos parâmetros de montagem de volume de repositório git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="7938c-1691">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="7938c-1692">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="7938c-1692">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="7938c-1693">Extensão</span><span class="sxs-lookup"><span data-stu-id="7938c-1693">Extension</span></span>

* <span data-ttu-id="7938c-1694">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="7938c-1694">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="7938c-1695">Interativo</span><span class="sxs-lookup"><span data-stu-id="7938c-1695">Interactive</span></span>

* <span data-ttu-id="7938c-1696">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="7938c-1696">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="7938c-1697">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="7938c-1697">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="7938c-1698">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="7938c-1698">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="7938c-1699">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-1699">Network</span></span>

* <span data-ttu-id="7938c-1700">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="7938c-1700">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="7938c-1701">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="7938c-1701">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="7938c-1702">#4910</span><span class="sxs-lookup"><span data-stu-id="7938c-1702">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="7938c-1703">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="7938c-1703">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="7938c-1704">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="7938c-1704">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="7938c-1705">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-1705">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="7938c-1706">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-1706">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="7938c-1707">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="7938c-1707">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="7938c-1708">Perfil</span><span class="sxs-lookup"><span data-stu-id="7938c-1708">Profile</span></span>

* <span data-ttu-id="7938c-1709">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="7938c-1709">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="7938c-1710">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="7938c-1710">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="7938c-1711">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7938c-1711">RDBMS</span></span>

* <span data-ttu-id="7938c-1712">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="7938c-1712">Added `georestore` command</span></span>
* <span data-ttu-id="7938c-1713">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1713">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-1714">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-1714">Resource</span></span>

* <span data-ttu-id="7938c-1715">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1715">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="7938c-1716">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="7938c-1716">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-1717">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-1717">SQL</span></span>

* <span data-ttu-id="7938c-1718">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="7938c-1718">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-1719">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-1719">Storage</span></span>

* <span data-ttu-id="7938c-1720">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="7938c-1720">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-1721">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1721">VM</span></span>

* <span data-ttu-id="7938c-1722">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1722">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="7938c-1723">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="7938c-1723">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="7938c-1725">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1725">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="7938c-1726">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="7938c-1726">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="7938c-1727">#5718</span><span class="sxs-lookup"><span data-stu-id="7938c-1727">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="7938c-1728">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="7938c-1728">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="7938c-1729">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1729">March 27, 2018</span></span>

<span data-ttu-id="7938c-1730">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="7938c-1730">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="7938c-1731">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-1731">Core</span></span>

* <span data-ttu-id="7938c-1732">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="7938c-1732">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-1733">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-1733">ACS</span></span>

* <span data-ttu-id="7938c-1734">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="7938c-1734">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-1735">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-1735">Appservice</span></span>

* <span data-ttu-id="7938c-1736">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="7938c-1736">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="7938c-1737">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="7938c-1737">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="7938c-1738">Backup</span><span class="sxs-lookup"><span data-stu-id="7938c-1738">Backup</span></span>

* <span data-ttu-id="7938c-1739">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="7938c-1739">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="7938c-1740">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="7938c-1740">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="7938c-1741">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="7938c-1741">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="7938c-1742">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="7938c-1742">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="7938c-1743">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-1743">Container</span></span>

* <span data-ttu-id="7938c-1744">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="7938c-1744">Added `container exec` command.</span></span> <span data-ttu-id="7938c-1745">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="7938c-1745">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="7938c-1746">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-1746">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="7938c-1747">Extensão</span><span class="sxs-lookup"><span data-stu-id="7938c-1747">Extension</span></span>

* <span data-ttu-id="7938c-1748">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="7938c-1748">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="7938c-1749">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="7938c-1749">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="7938c-1750">[ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="7938c-1750">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="7938c-1751">Interativo</span><span class="sxs-lookup"><span data-stu-id="7938c-1751">Interactive</span></span>

* <span data-ttu-id="7938c-1752">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="7938c-1752">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="7938c-1753">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="7938c-1753">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="7938c-1754">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="7938c-1754">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="7938c-1755">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="7938c-1755">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="7938c-1756">Laboratório</span><span class="sxs-lookup"><span data-stu-id="7938c-1756">Lab</span></span>

* <span data-ttu-id="7938c-1757">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="7938c-1757">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="7938c-1758">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7938c-1758">Monitor</span></span>

* <span data-ttu-id="7938c-1759">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="7938c-1759">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="7938c-1760">Corrigido [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="7938c-1760">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="7938c-1761">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="7938c-1761">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="7938c-1762">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-1762">Network</span></span>

* <span data-ttu-id="7938c-1763">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="7938c-1763">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="7938c-1764">Perfil</span><span class="sxs-lookup"><span data-stu-id="7938c-1764">Profile</span></span>

* <span data-ttu-id="7938c-1765">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="7938c-1765">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="7938c-1766">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7938c-1766">RDBMS</span></span>

* <span data-ttu-id="7938c-1767">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="7938c-1767">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-1768">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-1768">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="7938c-1770">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-1770">Role</span></span>

* <span data-ttu-id="7938c-1771">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1771">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="7938c-1772">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="7938c-1772">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="7938c-1773">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="7938c-1773">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="7938c-1774">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="7938c-1774">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="7938c-1775">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="7938c-1775">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-1776">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-1776">Storage</span></span>

* <span data-ttu-id="7938c-1777">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="7938c-1777">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="7938c-1778">Corrigido [#4049](https://github.com/Azure/azure-cli/issues/4049): problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="7938c-1778">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-1779">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1779">VM</span></span>

* <span data-ttu-id="7938c-1780">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="7938c-1780">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="7938c-1781">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="7938c-1781">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="7938c-1782">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="7938c-1782">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="7938c-1783">[ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="7938c-1783">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="7938c-1784">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1784">March 13, 2018</span></span>

<span data-ttu-id="7938c-1785">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="7938c-1785">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-1786">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-1786">ACR</span></span>

* <span data-ttu-id="7938c-1787">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="7938c-1787">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="7938c-1788">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="7938c-1788">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="7938c-1789">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="7938c-1789">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-1790">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-1790">ACS</span></span>

* <span data-ttu-id="7938c-1791">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="7938c-1791">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="7938c-1792">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="7938c-1792">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="7938c-1793">Supervisor</span><span class="sxs-lookup"><span data-stu-id="7938c-1793">Advisor</span></span>

* <span data-ttu-id="7938c-1794">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="7938c-1794">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="7938c-1795">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="7938c-1795">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="7938c-1796">[ALTERAÇÃO SIGNIFICATIVA] `advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="7938c-1796">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="7938c-1797">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="7938c-1797">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="7938c-1798">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="7938c-1798">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-1799">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-1799">Appservice</span></span>

* <span data-ttu-id="7938c-1800">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="7938c-1800">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="7938c-1801">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="7938c-1801">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="7938c-1802">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="7938c-1802">Eventhubs</span></span>

* <span data-ttu-id="7938c-1803">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="7938c-1803">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="7938c-1804">Extensão</span><span class="sxs-lookup"><span data-stu-id="7938c-1804">Extension</span></span>

* <span data-ttu-id="7938c-1805">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="7938c-1805">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="7938c-1806">Interativo</span><span class="sxs-lookup"><span data-stu-id="7938c-1806">Interactive</span></span>

* <span data-ttu-id="7938c-1807">Corrigido [#5625](https://github.com/Azure/azure-cli/issues/5625): manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="7938c-1807">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="7938c-1808">Corrigido [#3016](https://github.com/Azure/azure-cli/issues/3016): histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="7938c-1808">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="7938c-1809">Corrigido [#5688](https://github.com/Azure/azure-cli/issues/5688): as conclusões não aparecerão se o carregamento da tabela de comando encontrar uma exceção</span><span class="sxs-lookup"><span data-stu-id="7938c-1809">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="7938c-1810">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="7938c-1810">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="7938c-1811">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7938c-1811">Monitor</span></span>

* <span data-ttu-id="7938c-1812">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="7938c-1812">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="7938c-1813">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="7938c-1813">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="7938c-1814">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="7938c-1814">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="7938c-1815">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="7938c-1815">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="7938c-1816">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-1816">Network</span></span>

* <span data-ttu-id="7938c-1817">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1817">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="7938c-1818">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="7938c-1818">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="7938c-1819">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="7938c-1819">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="7938c-1820">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="7938c-1820">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="7938c-1821">Perfil</span><span class="sxs-lookup"><span data-stu-id="7938c-1821">Profile</span></span>

* <span data-ttu-id="7938c-1822">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="7938c-1822">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="7938c-1823">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="7938c-1823">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="7938c-1824">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7938c-1824">RDBMS</span></span>

* <span data-ttu-id="7938c-1825">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="7938c-1825">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="7938c-1826">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="7938c-1826">Service Bus</span></span>

* <span data-ttu-id="7938c-1827">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="7938c-1827">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-1828">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-1828">Storage</span></span>

* <span data-ttu-id="7938c-1829">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="7938c-1829">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="7938c-1830">Corrigido [#5286](https://github.com/Azure/azure-cli/issues/5286): os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="7938c-1830">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-1831">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1831">VM</span></span>

* <span data-ttu-id="7938c-1832">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="7938c-1832">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="7938c-1833">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="7938c-1833">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="7938c-1834">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="7938c-1834">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="7938c-1835">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="7938c-1835">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="7938c-1836">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1836">February 27, 2018</span></span>

<span data-ttu-id="7938c-1837">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="7938c-1837">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="7938c-1838">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-1838">Core</span></span>

* <span data-ttu-id="7938c-1839">Corrigido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="7938c-1839">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="7938c-1840">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="7938c-1840">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="7938c-1841">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="7938c-1841">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-1842">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-1842">ACS</span></span>

* <span data-ttu-id="7938c-1843">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="7938c-1843">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="7938c-1844">Problema corrigido: permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="7938c-1844">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="7938c-1845">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="7938c-1845">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="7938c-1846">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="7938c-1846">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-1847">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-1847">Appservice</span></span>

* <span data-ttu-id="7938c-1848">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="7938c-1848">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="7938c-1849">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="7938c-1849">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7938c-1850">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="7938c-1850">Cognitive Services</span></span>

* <span data-ttu-id="7938c-1851">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="7938c-1851">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="7938c-1852">Consumo</span><span class="sxs-lookup"><span data-stu-id="7938c-1852">Consumption</span></span>

* <span data-ttu-id="7938c-1853">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="7938c-1853">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="7938c-1854">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="7938c-1854">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="7938c-1855">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-1855">Container</span></span>

* <span data-ttu-id="7938c-1856">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="7938c-1856">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="7938c-1857">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-1857">Network</span></span>

* <span data-ttu-id="7938c-1858">Corrigido [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="7938c-1858">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-1859">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-1859">Resource</span></span>

* <span data-ttu-id="7938c-1860">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="7938c-1860">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="7938c-1861">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-1861">Role</span></span>

* <span data-ttu-id="7938c-1862">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="7938c-1862">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-1863">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-1863">SQL</span></span>

* <span data-ttu-id="7938c-1864">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="7938c-1864">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-1865">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-1865">Storage</span></span>

* <span data-ttu-id="7938c-1866">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="7938c-1866">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-1867">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1867">VM</span></span>

* <span data-ttu-id="7938c-1868">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="7938c-1868">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="7938c-1869">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1869">February 13, 2018</span></span>

<span data-ttu-id="7938c-1870">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="7938c-1870">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="7938c-1871">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-1871">Core</span></span>

* <span data-ttu-id="7938c-1872">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="7938c-1872">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-1873">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-1873">ACS</span></span>

* <span data-ttu-id="7938c-1874">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="7938c-1874">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="7938c-1875">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1875">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="7938c-1876">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="7938c-1876">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="7938c-1877">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="7938c-1877">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="7938c-1878">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="7938c-1878">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="7938c-1879">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="7938c-1879">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="7938c-1880">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="7938c-1880">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="7938c-1881">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="7938c-1881">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-1882">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-1882">Appservice</span></span>

* <span data-ttu-id="7938c-1883">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="7938c-1883">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="7938c-1884">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="7938c-1884">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="7938c-1885">CDN</span><span class="sxs-lookup"><span data-stu-id="7938c-1885">CDN</span></span>

* <span data-ttu-id="7938c-1886">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="7938c-1886">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="7938c-1887">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-1887">Container</span></span>

* <span data-ttu-id="7938c-1888">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="7938c-1888">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="7938c-1889">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-1889">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7938c-1890">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7938c-1890">CosmosDB</span></span>

* <span data-ttu-id="7938c-1891">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="7938c-1891">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="7938c-1892">Extensão</span><span class="sxs-lookup"><span data-stu-id="7938c-1892">Extension</span></span>

* <span data-ttu-id="7938c-1893">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-1893">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="7938c-1894">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-1894">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="7938c-1895">Comentários</span><span class="sxs-lookup"><span data-stu-id="7938c-1895">Feedback</span></span>

* <span data-ttu-id="7938c-1896">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="7938c-1896">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="7938c-1897">Interativo</span><span class="sxs-lookup"><span data-stu-id="7938c-1897">Interactive</span></span>

* <span data-ttu-id="7938c-1898">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="7938c-1898">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="7938c-1899">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="7938c-1899">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="7938c-1900">IoT</span><span class="sxs-lookup"><span data-stu-id="7938c-1900">IoT</span></span>

* <span data-ttu-id="7938c-1901">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="7938c-1901">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="7938c-1902">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="7938c-1902">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="7938c-1903">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-1903">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="7938c-1904">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="7938c-1904">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="7938c-1905">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7938c-1905">Monitor</span></span>

* <span data-ttu-id="7938c-1906">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1906">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="7938c-1907">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-1907">Network</span></span>

* <span data-ttu-id="7938c-1908">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="7938c-1908">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="7938c-1909">Perfil</span><span class="sxs-lookup"><span data-stu-id="7938c-1909">Profile</span></span>

* <span data-ttu-id="7938c-1910">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="7938c-1910">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-1911">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-1911">Resource</span></span>

* <span data-ttu-id="7938c-1912">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="7938c-1912">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="7938c-1913">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-1913">Role</span></span>

* <span data-ttu-id="7938c-1914">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="7938c-1914">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-1915">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-1915">SQL</span></span>

* <span data-ttu-id="7938c-1916">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="7938c-1916">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="7938c-1917">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="7938c-1917">Added `sql db rename`</span></span>
* <span data-ttu-id="7938c-1918">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="7938c-1918">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-1919">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-1919">Storage</span></span>

* <span data-ttu-id="7938c-1920">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="7938c-1920">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-1921">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1921">VM</span></span>

* <span data-ttu-id="7938c-1922">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="7938c-1922">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="7938c-1923">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="7938c-1923">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="7938c-1924">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="7938c-1924">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="7938c-1925">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1925">January 31, 2018</span></span>

<span data-ttu-id="7938c-1926">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="7938c-1926">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="7938c-1927">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-1927">Core</span></span>

* <span data-ttu-id="7938c-1928">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="7938c-1928">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="7938c-1929">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="7938c-1929">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="7938c-1930">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="7938c-1930">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="7938c-1931">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="7938c-1931">Use `--verbose` to see</span></span>
* <span data-ttu-id="7938c-1932">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="7938c-1932">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-1933">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-1933">ACS</span></span>

* <span data-ttu-id="7938c-1934">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="7938c-1934">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="7938c-1935">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="7938c-1935">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-1936">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-1936">Appservice</span></span>

* <span data-ttu-id="7938c-1937">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="7938c-1937">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="7938c-1938">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="7938c-1938">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="7938c-1939">CDN</span><span class="sxs-lookup"><span data-stu-id="7938c-1939">CDN</span></span>

* <span data-ttu-id="7938c-1940">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1940">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7938c-1941">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7938c-1941">CosmosDB</span></span>

* <span data-ttu-id="7938c-1942">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="7938c-1942">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="7938c-1943">Interativo</span><span class="sxs-lookup"><span data-stu-id="7938c-1943">Interactive</span></span>

* <span data-ttu-id="7938c-1944">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="7938c-1944">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="7938c-1945">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-1945">Network</span></span>

* <span data-ttu-id="7938c-1946">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1946">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="7938c-1947">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="7938c-1947">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="7938c-1948">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1948">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="7938c-1949">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1949">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="7938c-1950">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="7938c-1950">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="7938c-1951">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="7938c-1951">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="7938c-1952">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="7938c-1952">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="7938c-1953">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="7938c-1953">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="7938c-1954">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="7938c-1954">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="7938c-1955">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="7938c-1955">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="7938c-1956">Perfil</span><span class="sxs-lookup"><span data-stu-id="7938c-1956">Profile</span></span>

* <span data-ttu-id="7938c-1957">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="7938c-1957">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-1958">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-1958">Resource</span></span>

* <span data-ttu-id="7938c-1959">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="7938c-1959">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-1960">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-1960">Storage</span></span>

* <span data-ttu-id="7938c-1961">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="7938c-1961">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="7938c-1962">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="7938c-1962">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="7938c-1963">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="7938c-1963">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="7938c-1964">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="7938c-1964">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="7938c-1965">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="7938c-1965">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-1966">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-1966">VM</span></span>

* <span data-ttu-id="7938c-1967">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="7938c-1967">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="7938c-1968">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="7938c-1968">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="7938c-1969">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="7938c-1969">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="7938c-1970">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7938c-1970">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="7938c-1971">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="7938c-1971">January 17, 2018</span></span>

<span data-ttu-id="7938c-1972">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="7938c-1972">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-1973">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-1973">ACR</span></span>

* <span data-ttu-id="7938c-1974">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="7938c-1974">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="7938c-1975">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="7938c-1975">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-1976">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-1976">ACS</span></span>

* <span data-ttu-id="7938c-1977">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="7938c-1977">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="7938c-1978">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="7938c-1978">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-1979">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-1979">Appservice</span></span>

* <span data-ttu-id="7938c-1980">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="7938c-1980">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="7938c-1981">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="7938c-1981">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="7938c-1982">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="7938c-1982">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="7938c-1983">Backup</span><span class="sxs-lookup"><span data-stu-id="7938c-1983">Backup</span></span>

* <span data-ttu-id="7938c-1984">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="7938c-1984">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="7938c-1985">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="7938c-1985">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="7938c-1986">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="7938c-1986">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="7938c-1987">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="7938c-1987">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="7938c-1988">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="7938c-1988">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="7938c-1989">Lote</span><span class="sxs-lookup"><span data-stu-id="7938c-1989">Batch</span></span>

* <span data-ttu-id="7938c-1990">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="7938c-1990">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="7938c-1991">Nuvem</span><span class="sxs-lookup"><span data-stu-id="7938c-1991">Cloud</span></span>

* <span data-ttu-id="7938c-1992">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="7938c-1992">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="7938c-1993">Consumo</span><span class="sxs-lookup"><span data-stu-id="7938c-1993">Consumption</span></span>

* <span data-ttu-id="7938c-1994">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="7938c-1994">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="7938c-1995">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="7938c-1995">Event Grid</span></span>

* <span data-ttu-id="7938c-1996">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="7938c-1996">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="7938c-1997">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="7938c-1997">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="7938c-1998">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="7938c-1998">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="7938c-1999">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="7938c-1999">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="7938c-2000">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="7938c-2000">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="7938c-2001">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="7938c-2001">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="7938c-2002">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="7938c-2002">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="7938c-2003">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="7938c-2003">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="7938c-2004">Interativo</span><span class="sxs-lookup"><span data-stu-id="7938c-2004">Interactive</span></span>

* <span data-ttu-id="7938c-2005">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="7938c-2005">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="7938c-2006">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="7938c-2006">Fixed errors on startup</span></span>
* <span data-ttu-id="7938c-2007">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="7938c-2007">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="7938c-2008">IoT</span><span class="sxs-lookup"><span data-stu-id="7938c-2008">IoT</span></span>

* <span data-ttu-id="7938c-2009">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="7938c-2009">Added support for device provisioning service</span></span>
* <span data-ttu-id="7938c-2010">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="7938c-2010">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="7938c-2011">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="7938c-2011">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="7938c-2012">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7938c-2012">Monitor</span></span>

* <span data-ttu-id="7938c-2013">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="7938c-2013">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="7938c-2014">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2014">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="7938c-2015">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="7938c-2015">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="7938c-2016">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-2016">Network</span></span>

* <span data-ttu-id="7938c-2017">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="7938c-2017">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="7938c-2018">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-2018">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="7938c-2019">Perfil</span><span class="sxs-lookup"><span data-stu-id="7938c-2019">Profile</span></span>

* <span data-ttu-id="7938c-2020">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="7938c-2020">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="7938c-2021">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-2021">Role</span></span>

* <span data-ttu-id="7938c-2022">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="7938c-2022">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7938c-2023">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7938c-2023">Service Fabric</span></span>

* <span data-ttu-id="7938c-2024">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="7938c-2024">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="7938c-2025">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="7938c-2025">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-2026">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-2026">VM</span></span>

* <span data-ttu-id="7938c-2027">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="7938c-2027">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="7938c-2028">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="7938c-2028">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="7938c-2029">[ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="7938c-2029">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="7938c-2030">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="7938c-2030">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="7938c-2031">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="7938c-2031">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="7938c-2032">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2032">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="7938c-2033">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2033">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="7938c-2034">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="7938c-2034">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="7938c-2035">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="7938c-2035">December 19, 2017</span></span>

<span data-ttu-id="7938c-2036">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="7938c-2036">Version 2.0.23</span></span>

* <span data-ttu-id="7938c-2037">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="7938c-2037">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="7938c-2038">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-2038">Container</span></span>

* <span data-ttu-id="7938c-2039">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-2039">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="7938c-2040">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-2040">Network</span></span>

* <span data-ttu-id="7938c-2041">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-2041">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="7938c-2042">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-2042">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-2043">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-2043">Storage</span></span>

* <span data-ttu-id="7938c-2044">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="7938c-2044">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-2045">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-2045">VM</span></span>

* <span data-ttu-id="7938c-2046">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="7938c-2046">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="7938c-2047">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="7938c-2047">December 5, 2017</span></span>

<span data-ttu-id="7938c-2048">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="7938c-2048">Version 2.0.22</span></span>

* <span data-ttu-id="7938c-2049">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="7938c-2049">Removed `az component` commands.</span></span> <span data-ttu-id="7938c-2050">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="7938c-2050">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="7938c-2051">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-2051">Core</span></span>
* <span data-ttu-id="7938c-2052">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="7938c-2052">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="7938c-2053">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="7938c-2053">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-2054">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-2054">ACS</span></span>

* <span data-ttu-id="7938c-2055">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="7938c-2055">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="7938c-2056">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2056">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="7938c-2057">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="7938c-2057">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="7938c-2058">Supervisor</span><span class="sxs-lookup"><span data-stu-id="7938c-2058">Advisor</span></span>

* <span data-ttu-id="7938c-2059">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="7938c-2059">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-2060">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-2060">Appservice</span></span>

* <span data-ttu-id="7938c-2061">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="7938c-2061">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="7938c-2062">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="7938c-2062">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="7938c-2063">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="7938c-2063">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="7938c-2064">Consumo</span><span class="sxs-lookup"><span data-stu-id="7938c-2064">Consumption</span></span>

* <span data-ttu-id="7938c-2065">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="7938c-2065">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="7938c-2066">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-2066">Container</span></span>

* <span data-ttu-id="7938c-2067">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="7938c-2067">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="7938c-2068">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7938c-2068">Monitor</span></span>

* <span data-ttu-id="7938c-2069">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="7938c-2069">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-2070">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-2070">Resource</span></span>

* <span data-ttu-id="7938c-2071">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="7938c-2071">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="7938c-2072">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-2072">Role</span></span>

* <span data-ttu-id="7938c-2073">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="7938c-2073">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="7938c-2074">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="7938c-2074">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="7938c-2075">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="7938c-2075">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-2076">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-2076">SQL</span></span>

* <span data-ttu-id="7938c-2077">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="7938c-2077">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="7938c-2078">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="7938c-2078">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-2079">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-2079">VM</span></span>

* <span data-ttu-id="7938c-2080">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="7938c-2080">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="7938c-2081">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="7938c-2081">November 14, 2017</span></span>

<span data-ttu-id="7938c-2082">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="7938c-2082">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-2083">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-2083">ACR</span></span>

* <span data-ttu-id="7938c-2084">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="7938c-2084">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="7938c-2085">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-2085">ACS</span></span>

* <span data-ttu-id="7938c-2086">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="7938c-2086">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="7938c-2087">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2087">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="7938c-2088">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="7938c-2088">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="7938c-2089">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="7938c-2089">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="7938c-2090">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="7938c-2090">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-2091">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-2091">Appservice</span></span>

* <span data-ttu-id="7938c-2092">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="7938c-2092">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="7938c-2093">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="7938c-2093">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="7938c-2094">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="7938c-2094">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="7938c-2095">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="7938c-2095">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="7938c-2096">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="7938c-2096">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="7938c-2097">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="7938c-2097">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="7938c-2098">Lote</span><span class="sxs-lookup"><span data-stu-id="7938c-2098">Batch</span></span>

* <span data-ttu-id="7938c-2099">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="7938c-2099">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="7938c-2100">Batchai</span><span class="sxs-lookup"><span data-stu-id="7938c-2100">Batchai</span></span>

* <span data-ttu-id="7938c-2101">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2101">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="7938c-2102">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2102">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="7938c-2103">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="7938c-2103">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="7938c-2104">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2104">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="7938c-2105">Nuvem</span><span class="sxs-lookup"><span data-stu-id="7938c-2105">Cloud</span></span>

* <span data-ttu-id="7938c-2106">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="7938c-2106">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="7938c-2107">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-2107">Container</span></span>

* <span data-ttu-id="7938c-2108">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="7938c-2108">Added support to open multiple ports</span></span>
* <span data-ttu-id="7938c-2109">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="7938c-2109">Added container group restart policy</span></span>
* <span data-ttu-id="7938c-2110">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="7938c-2110">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="7938c-2111">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="7938c-2111">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7938c-2112">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7938c-2112">Data Lake Analytics</span></span>

* <span data-ttu-id="7938c-2113">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="7938c-2113">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7938c-2114">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7938c-2114">Data Lake Store</span></span>

* <span data-ttu-id="7938c-2115">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="7938c-2115">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="7938c-2116">Extensão</span><span class="sxs-lookup"><span data-stu-id="7938c-2116">Extension</span></span>

* <span data-ttu-id="7938c-2117">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="7938c-2117">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="7938c-2118">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="7938c-2118">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="7938c-2119">IoT</span><span class="sxs-lookup"><span data-stu-id="7938c-2119">IoT</span></span>

* <span data-ttu-id="7938c-2120">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="7938c-2120">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="7938c-2121">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7938c-2121">Monitor</span></span>

* <span data-ttu-id="7938c-2122">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="7938c-2122">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="7938c-2123">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-2123">Network</span></span>

* <span data-ttu-id="7938c-2124">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="7938c-2124">Added support for CAA DNS records</span></span>
* <span data-ttu-id="7938c-2125">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="7938c-2125">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="7938c-2126">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="7938c-2126">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="7938c-2127">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="7938c-2127">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="7938c-2128">Reservas</span><span class="sxs-lookup"><span data-stu-id="7938c-2128">Reservations</span></span>

* <span data-ttu-id="7938c-2129">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="7938c-2129">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-2130">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-2130">Resource</span></span>

* <span data-ttu-id="7938c-2131">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-2131">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-2132">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-2132">SQL</span></span>

* <span data-ttu-id="7938c-2133">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-2133">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-2134">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-2134">Storage</span></span>

* <span data-ttu-id="7938c-2135">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="7938c-2135">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="7938c-2136">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="7938c-2136">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="7938c-2137">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="7938c-2137">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="7938c-2138">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="7938c-2138">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="7938c-2139">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="7938c-2139">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="7938c-2140">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="7938c-2140">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="7938c-2141">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-2141">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-2142">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-2142">VM</span></span>

* <span data-ttu-id="7938c-2143">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="7938c-2143">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="7938c-2144">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="7938c-2144">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="7938c-2145">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="7938c-2145">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="7938c-2146">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="7938c-2146">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="7938c-2147">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="7938c-2147">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="7938c-2148">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="7938c-2148">October 24, 2017</span></span>

<span data-ttu-id="7938c-2149">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="7938c-2149">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="7938c-2150">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-2150">Core</span></span>

* <span data-ttu-id="7938c-2151">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="7938c-2151">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-2152">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-2152">ACR</span></span>

* <span data-ttu-id="7938c-2153">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="7938c-2153">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="7938c-2154">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="7938c-2154">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="7938c-2155">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="7938c-2155">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-2156">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-2156">ACS</span></span>

* <span data-ttu-id="7938c-2157">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="7938c-2157">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="7938c-2158">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="7938c-2158">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-2159">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-2159">Appservice</span></span>

* <span data-ttu-id="7938c-2160">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="7938c-2160">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="7938c-2161">Componente</span><span class="sxs-lookup"><span data-stu-id="7938c-2161">Component</span></span>

* <span data-ttu-id="7938c-2162">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="7938c-2162">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="7938c-2163">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7938c-2163">Monitor</span></span>

* <span data-ttu-id="7938c-2164">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="7938c-2164">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-2165">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-2165">Resource</span></span>

* <span data-ttu-id="7938c-2166">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="7938c-2166">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="7938c-2167">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="7938c-2167">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-2168">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-2168">VM</span></span>

* <span data-ttu-id="7938c-2169">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2169">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="7938c-2170">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="7938c-2170">October 9, 2017</span></span>

<span data-ttu-id="7938c-2171">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="7938c-2171">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="7938c-2172">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-2172">Core</span></span>

* <span data-ttu-id="7938c-2173">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="7938c-2173">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-2174">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-2174">Appservice</span></span>

* <span data-ttu-id="7938c-2175">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="7938c-2175">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="7938c-2176">Lote</span><span class="sxs-lookup"><span data-stu-id="7938c-2176">Batch</span></span>

* <span data-ttu-id="7938c-2177">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="7938c-2177">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="7938c-2178">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="7938c-2178">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="7938c-2179">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="7938c-2179">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="7938c-2180">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="7938c-2180">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="7938c-2181">Batchai</span><span class="sxs-lookup"><span data-stu-id="7938c-2181">Batchai</span></span>

* <span data-ttu-id="7938c-2182">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="7938c-2182">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="7938c-2183">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7938c-2183">Keyvault</span></span>

* <span data-ttu-id="7938c-2184">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="7938c-2184">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="7938c-2185">(#4448)</span><span class="sxs-lookup"><span data-stu-id="7938c-2185">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="7938c-2186">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-2186">Network</span></span>

* <span data-ttu-id="7938c-2187">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="7938c-2187">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="7938c-2188">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="7938c-2188">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-2189">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-2189">Resource</span></span>

* <span data-ttu-id="7938c-2190">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="7938c-2190">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="7938c-2191">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="7938c-2191">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="7938c-2192">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="7938c-2192">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="7938c-2193">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-2193">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-2194">Sql</span><span class="sxs-lookup"><span data-stu-id="7938c-2194">Sql</span></span>

* <span data-ttu-id="7938c-2195">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="7938c-2195">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="7938c-2196">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="7938c-2196">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="7938c-2197">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="7938c-2197">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-2198">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-2198">Storage</span></span>

* <span data-ttu-id="7938c-2199">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="7938c-2199">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-2200">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-2200">Vm</span></span>

* <span data-ttu-id="7938c-2201">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="7938c-2201">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="7938c-2202">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2202">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="7938c-2203">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="7938c-2203">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="7938c-2204">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2204">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="7938c-2205">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2205">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="7938c-2206">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="7938c-2206">September 22, 2017</span></span>

<span data-ttu-id="7938c-2207">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="7938c-2207">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-2208">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-2208">Resource</span></span>

* <span data-ttu-id="7938c-2209">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="7938c-2209">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="7938c-2210">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="7938c-2210">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="7938c-2211">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2211">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="7938c-2212">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="7938c-2212">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="7938c-2213">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-2213">Network</span></span>

* <span data-ttu-id="7938c-2214">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="7938c-2214">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="7938c-2215">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="7938c-2215">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="7938c-2216">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7938c-2216">Added `asg` application security group commands</span></span>
* <span data-ttu-id="7938c-2217">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-2217">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="7938c-2218">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-2218">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="7938c-2219">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-2219">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="7938c-2220">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="7938c-2220">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-2221">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-2221">Storage</span></span>

* <span data-ttu-id="7938c-2222">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="7938c-2222">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="7938c-2223">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="7938c-2223">Eventgrid</span></span>

* <span data-ttu-id="7938c-2224">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="7938c-2224">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-2225">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-2225">SQL</span></span>

* <span data-ttu-id="7938c-2226">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="7938c-2226">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="7938c-2227">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="7938c-2227">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="7938c-2228">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-2228">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="7938c-2229">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7938c-2229">Keyvault</span></span>

* <span data-ttu-id="7938c-2230">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="7938c-2230">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-2231">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-2231">VM</span></span>

* <span data-ttu-id="7938c-2232">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2232">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="7938c-2233">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="7938c-2233">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="7938c-2234">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2234">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="7938c-2235">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="7938c-2235">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="7938c-2236">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="7938c-2236">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="7938c-2237">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="7938c-2237">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-2238">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-2238">ACS</span></span>

* <span data-ttu-id="7938c-2239">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-2239">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-2240">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-2240">Appservice</span></span>

* <span data-ttu-id="7938c-2241">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="7938c-2241">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="7938c-2242">Backup</span><span class="sxs-lookup"><span data-stu-id="7938c-2242">Backup</span></span>

* <span data-ttu-id="7938c-2243">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="7938c-2243">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="7938c-2244">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="7938c-2244">September 11, 2017</span></span>

<span data-ttu-id="7938c-2245">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="7938c-2245">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="7938c-2246">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-2246">Core</span></span>

* <span data-ttu-id="7938c-2247">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="7938c-2247">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="7938c-2248">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="7938c-2248">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-2249">Acs</span><span class="sxs-lookup"><span data-stu-id="7938c-2249">Acs</span></span>

* <span data-ttu-id="7938c-2250">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="7938c-2250">Added `acs list-locations` command</span></span>
* <span data-ttu-id="7938c-2251">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="7938c-2251">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-2252">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-2252">Appservice</span></span>

* <span data-ttu-id="7938c-2253">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="7938c-2253">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="7938c-2254">CDN</span><span class="sxs-lookup"><span data-stu-id="7938c-2254">CDN</span></span>

* <span data-ttu-id="7938c-2255">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2255">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="7938c-2256">Extensão</span><span class="sxs-lookup"><span data-stu-id="7938c-2256">Extension</span></span>

* <span data-ttu-id="7938c-2257">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="7938c-2257">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="7938c-2258">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7938c-2258">Keyvault</span></span>

* <span data-ttu-id="7938c-2259">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="7938c-2259">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="7938c-2260">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-2260">Network</span></span>

* <span data-ttu-id="7938c-2261">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="7938c-2261">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="7938c-2262">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="7938c-2262">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="7938c-2263">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="7938c-2263">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="7938c-2264">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2264">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="7938c-2265">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2265">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-2266">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-2266">Resource</span></span>

* <span data-ttu-id="7938c-2267">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="7938c-2267">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="7938c-2268">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2268">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="7938c-2269">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="7938c-2269">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="7938c-2270">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="7938c-2270">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-2271">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-2271">SQL</span></span>

* <span data-ttu-id="7938c-2272">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="7938c-2272">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-2273">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-2273">VM</span></span>

* <span data-ttu-id="7938c-2274">Corrigido: não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="7938c-2274">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="7938c-2275">Corrigido: usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="7938c-2275">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="7938c-2276">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2276">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="7938c-2277">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="7938c-2277">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="7938c-2278">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="7938c-2278">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="7938c-2279">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="7938c-2279">August 31, 2017</span></span>

<span data-ttu-id="7938c-2280">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="7938c-2280">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="7938c-2281">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7938c-2281">Keyvault</span></span>

* <span data-ttu-id="7938c-2282">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="7938c-2282">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="7938c-2283">Sf</span><span class="sxs-lookup"><span data-stu-id="7938c-2283">Sf</span></span>

* <span data-ttu-id="7938c-2284">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="7938c-2284">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-2285">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-2285">Storage</span></span>

* <span data-ttu-id="7938c-2286">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="7938c-2286">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="7938c-2287">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="7938c-2287">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="7938c-2288">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="7938c-2288">August 28, 2017</span></span>

<span data-ttu-id="7938c-2289">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="7938c-2289">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="7938c-2290">CLI</span><span class="sxs-lookup"><span data-stu-id="7938c-2290">CLI</span></span>

* <span data-ttu-id="7938c-2291">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="7938c-2291">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-2292">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-2292">ACS</span></span>

* <span data-ttu-id="7938c-2293">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="7938c-2293">Corrected preview regions</span></span>
* <span data-ttu-id="7938c-2294">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="7938c-2294">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="7938c-2295">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="7938c-2295">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-2296">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-2296">Appservice</span></span>

* <span data-ttu-id="7938c-2297">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="7938c-2297">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="7938c-2298">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="7938c-2298">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="7938c-2299">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="7938c-2299">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="7938c-2300">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="7938c-2300">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="7938c-2301">Corrigido: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="7938c-2301">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="7938c-2302">IoT</span><span class="sxs-lookup"><span data-stu-id="7938c-2302">IoT</span></span>

* <span data-ttu-id="7938c-2303">Corrigido #3934: a criação de uma política não limpa mais as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="7938c-2303">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="7938c-2304">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-2304">Network</span></span>

* <span data-ttu-id="7938c-2305">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="7938c-2305">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="7938c-2306">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-2306">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="7938c-2307">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7938c-2307">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="7938c-2308">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2308">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="7938c-2309">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2309">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="7938c-2310">Perfil</span><span class="sxs-lookup"><span data-stu-id="7938c-2310">Profile</span></span>

* <span data-ttu-id="7938c-2311">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7938c-2311">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7938c-2312">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7938c-2312">Service Fabric</span></span>

* <span data-ttu-id="7938c-2313">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="7938c-2313">Preview release</span></span>
* <span data-ttu-id="7938c-2314">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="7938c-2314">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="7938c-2315">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="7938c-2315">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="7938c-2316">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="7938c-2316">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-2317">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-2317">Storage</span></span>

* <span data-ttu-id="7938c-2318">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="7938c-2318">Enabled setting blob tier</span></span>
* <span data-ttu-id="7938c-2319">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="7938c-2319">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="7938c-2320">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="7938c-2320">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="7938c-2321">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="7938c-2321">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="7938c-2322">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="7938c-2322">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="7938c-2323">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="7938c-2323">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-2324">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-2324">VM</span></span>

* <span data-ttu-id="7938c-2325">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="7938c-2325">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="7938c-2326">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="7938c-2326">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="7938c-2327">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2327">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="7938c-2328">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="7938c-2328">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="7938c-2329">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="7938c-2329">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="7938c-2330">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2330">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="7938c-2331">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="7938c-2331">August 15, 2017</span></span>

<span data-ttu-id="7938c-2332">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="7938c-2332">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-2333">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-2333">ACS</span></span>

* <span data-ttu-id="7938c-2334">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="7938c-2334">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-2335">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-2335">Appservice</span></span>

* <span data-ttu-id="7938c-2336">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="7938c-2336">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="7938c-2337">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="7938c-2337">Event Grid</span></span>

* <span data-ttu-id="7938c-2338">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="7938c-2338">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="7938c-2339">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="7938c-2339">August 11, 2017</span></span>

<span data-ttu-id="7938c-2340">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="7938c-2340">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-2341">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-2341">ACS</span></span>

* <span data-ttu-id="7938c-2342">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="7938c-2342">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="7938c-2343">Lote</span><span class="sxs-lookup"><span data-stu-id="7938c-2343">Batch</span></span>

* <span data-ttu-id="7938c-2344">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="7938c-2344">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="7938c-2345">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="7938c-2345">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="7938c-2346">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-2346">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="7938c-2347">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://”</span><span class="sxs-lookup"><span data-stu-id="7938c-2347">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="7938c-2348">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="7938c-2348">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="7938c-2349">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="7938c-2349">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="7938c-2350">Componente</span><span class="sxs-lookup"><span data-stu-id="7938c-2350">Component</span></span>

* <span data-ttu-id="7938c-2351">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="7938c-2351">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="7938c-2352">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-2352">Container</span></span>

* <span data-ttu-id="7938c-2353">`create`: corrigido o problema em que o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="7938c-2353">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="7938c-2354">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7938c-2354">Data Lake Store</span></span>

* <span data-ttu-id="7938c-2355">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="7938c-2355">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="7938c-2356">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="7938c-2356">Event Grid</span></span>

* <span data-ttu-id="7938c-2357">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="7938c-2357">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="7938c-2358">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-2358">Network</span></span>

* <span data-ttu-id="7938c-2359">`lb`: corrigido o problema em que os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="7938c-2359">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="7938c-2360">`application-gateway {subresource} delete`: corrigido o problema em que `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="7938c-2360">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="7938c-2361">`application-gateway http-settings update`: corrigido o problema em que `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="7938c-2361">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="7938c-2362">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="7938c-2362">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="7938c-2363">Perfil</span><span class="sxs-lookup"><span data-stu-id="7938c-2363">Profile</span></span>

* <span data-ttu-id="7938c-2364">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="7938c-2364">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-2365">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-2365">Storage</span></span>

* <span data-ttu-id="7938c-2366">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="7938c-2366">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-2367">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-2367">VM</span></span>

* <span data-ttu-id="7938c-2368">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="7938c-2368">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="7938c-2369">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="7938c-2369">Exposed `list-skus` command</span></span>
* <span data-ttu-id="7938c-2370">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="7938c-2370">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="7938c-2371">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="7938c-2371">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="7938c-2372">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="7938c-2372">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="7938c-2373">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="7938c-2373">July 28, 2017</span></span>

<span data-ttu-id="7938c-2374">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="7938c-2374">Version 2.0.12</span></span>

* <span data-ttu-id="7938c-2375">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-2375">Added container commands</span></span>
* <span data-ttu-id="7938c-2376">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="7938c-2376">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="7938c-2377">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-2377">Core</span></span>

* <span data-ttu-id="7938c-2378">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="7938c-2378">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="7938c-2379">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="7938c-2379">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="7938c-2380">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="7938c-2380">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="7938c-2381">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="7938c-2381">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="7938c-2382">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="7938c-2382">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="7938c-2383">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="7938c-2383">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="7938c-2384">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="7938c-2384">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="7938c-2385">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="7938c-2385">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="7938c-2386">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="7938c-2386">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="7938c-2387">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="7938c-2387">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="7938c-2388">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="7938c-2388">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="7938c-2389">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="7938c-2389">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="7938c-2390">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="7938c-2390">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="7938c-2391">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="7938c-2391">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="7938c-2392">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="7938c-2392">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="7938c-2393">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="7938c-2393">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="7938c-2394">ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-2394">ACR</span></span>

* <span data-ttu-id="7938c-2395">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="7938c-2395">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="7938c-2396">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="7938c-2396">Support SKU update for managed registries</span></span>
* <span data-ttu-id="7938c-2397">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="7938c-2397">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="7938c-2398">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-2398">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="7938c-2399">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-2399">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="7938c-2400">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="7938c-2400">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-2401">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-2401">ACS</span></span>

* <span data-ttu-id="7938c-2402">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="7938c-2402">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-2403">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-2403">Appservice</span></span>

* <span data-ttu-id="7938c-2404">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="7938c-2404">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="7938c-2405">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="7938c-2405">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="7938c-2406">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="7938c-2406">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="7938c-2407">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="7938c-2407">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="7938c-2408">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="7938c-2408">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="7938c-2409">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="7938c-2409">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="7938c-2410">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="7938c-2410">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="7938c-2411">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="7938c-2411">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="7938c-2412">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="7938c-2412">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="7938c-2413">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="7938c-2413">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="7938c-2414">Lote</span><span class="sxs-lookup"><span data-stu-id="7938c-2414">Batch</span></span>

* <span data-ttu-id="7938c-2415">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="7938c-2415">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="7938c-2416">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="7938c-2416">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="7938c-2417">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="7938c-2417">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="7938c-2418">CDN</span><span class="sxs-lookup"><span data-stu-id="7938c-2418">CDN</span></span>

* <span data-ttu-id="7938c-2419">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="7938c-2419">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="7938c-2420">Nuvem</span><span class="sxs-lookup"><span data-stu-id="7938c-2420">Cloud</span></span>

* <span data-ttu-id="7938c-2421">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="7938c-2421">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="7938c-2422">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="7938c-2422">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="7938c-2423">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="7938c-2423">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="7938c-2424">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="7938c-2424">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="7938c-2425">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="7938c-2425">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7938c-2426">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7938c-2426">CosmosDB</span></span>

* <span data-ttu-id="7938c-2427">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="7938c-2427">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="7938c-2428">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="7938c-2428">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7938c-2429">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7938c-2429">Data Lake Analytics</span></span>

* <span data-ttu-id="7938c-2430">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="7938c-2430">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="7938c-2431">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="7938c-2431">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="7938c-2432">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="7938c-2432">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7938c-2433">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7938c-2433">Data Lake Store</span></span>

* <span data-ttu-id="7938c-2434">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="7938c-2434">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="7938c-2435">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="7938c-2435">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="7938c-2436">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="7938c-2436">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="7938c-2437">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7938c-2437">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="7938c-2438">Interativo</span><span class="sxs-lookup"><span data-stu-id="7938c-2438">Interactive</span></span>

* <span data-ttu-id="7938c-2439">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="7938c-2439">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="7938c-2440">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="7938c-2440">Increased test coverage</span></span>
* <span data-ttu-id="7938c-2441">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="7938c-2441">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="7938c-2442">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="7938c-2442">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="7938c-2443">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="7938c-2443">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="7938c-2444">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="7938c-2444">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="7938c-2445">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="7938c-2445">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="7938c-2446">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="7938c-2446">Added `--progress` flag</span></span>
* <span data-ttu-id="7938c-2447">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="7938c-2447">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="7938c-2448">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="7938c-2448">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="7938c-2449">IoT</span><span class="sxs-lookup"><span data-stu-id="7938c-2449">IoT</span></span>

* <span data-ttu-id="7938c-2450">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="7938c-2450">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="7938c-2451">(#3934)</span><span class="sxs-lookup"><span data-stu-id="7938c-2451">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="7938c-2452">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="7938c-2452">Key vault</span></span>

* <span data-ttu-id="7938c-2453">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="7938c-2453">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="7938c-2454">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="7938c-2454">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="7938c-2455">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="7938c-2455">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="7938c-2456">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="7938c-2456">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="7938c-2457">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="7938c-2457">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="7938c-2458">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="7938c-2458">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="7938c-2459">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="7938c-2459">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="7938c-2460">(#3307)</span><span class="sxs-lookup"><span data-stu-id="7938c-2460">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="7938c-2461">Laboratório</span><span class="sxs-lookup"><span data-stu-id="7938c-2461">Lab</span></span>

* <span data-ttu-id="7938c-2462">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="7938c-2462">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="7938c-2463">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="7938c-2463">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="7938c-2464">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7938c-2464">Monitor</span></span>

* <span data-ttu-id="7938c-2465">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="7938c-2465">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="7938c-2466">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="7938c-2466">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="7938c-2467">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="7938c-2467">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="7938c-2468">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="7938c-2468">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="7938c-2469">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="7938c-2469">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="7938c-2470">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="7938c-2470">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="7938c-2471">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="7938c-2471">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="7938c-2472">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="7938c-2472">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="7938c-2473">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="7938c-2473">`location` no longer required</span></span>
  * <span data-ttu-id="7938c-2474">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="7938c-2474">Add name and ID support for target</span></span>
  * <span data-ttu-id="7938c-2475">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="7938c-2475">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="7938c-2476">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="7938c-2476">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="7938c-2477">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="7938c-2477">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="7938c-2478">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="7938c-2478">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="7938c-2479">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="7938c-2479">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="7938c-2480">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="7938c-2480">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="7938c-2481">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-2481">Network</span></span>

* <span data-ttu-id="7938c-2482">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="7938c-2482">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="7938c-2483">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="7938c-2483">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="7938c-2484">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="7938c-2484">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="7938c-2485">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="7938c-2485">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="7938c-2486">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="7938c-2486">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="7938c-2487">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="7938c-2487">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="7938c-2488">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="7938c-2488">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="7938c-2489">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="7938c-2489">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="7938c-2490">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="7938c-2490">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="7938c-2491">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="7938c-2491">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="7938c-2492">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2492">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="7938c-2493">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="7938c-2493">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="7938c-2494">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="7938c-2494">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="7938c-2495">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="7938c-2495">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="7938c-2496">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="7938c-2496">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="7938c-2497">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2497">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="7938c-2498">Adicionado o suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para --dns-servers</span><span class="sxs-lookup"><span data-stu-id="7938c-2498">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="7938c-2499">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="7938c-2499">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="7938c-2500">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="7938c-2500">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="7938c-2501">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2501">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="7938c-2502">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="7938c-2502">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="7938c-2503">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="7938c-2503">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="7938c-2504">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="7938c-2504">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="7938c-2505">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="7938c-2505">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="7938c-2506">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="7938c-2506">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="7938c-2507">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="7938c-2507">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="7938c-2508">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="7938c-2508">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="7938c-2509">Perfil</span><span class="sxs-lookup"><span data-stu-id="7938c-2509">Profile</span></span>

* <span data-ttu-id="7938c-2510">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="7938c-2510">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="7938c-2511">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="7938c-2511">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="7938c-2512">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="7938c-2512">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="7938c-2513">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="7938c-2513">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="7938c-2514">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="7938c-2514">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="7938c-2515">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7938c-2515">RDBMS</span></span>

* <span data-ttu-id="7938c-2516">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="7938c-2516">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="7938c-2517">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="7938c-2517">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="7938c-2518">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="7938c-2518">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="7938c-2519">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="7938c-2519">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-2520">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-2520">Resource</span></span>

* <span data-ttu-id="7938c-2521">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2521">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="7938c-2522">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="7938c-2522">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="7938c-2523">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="7938c-2523">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="7938c-2524">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="7938c-2524">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="7938c-2525">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="7938c-2525">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="7938c-2526">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="7938c-2526">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="7938c-2527">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="7938c-2527">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="7938c-2528">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="7938c-2528">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="7938c-2529">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-2529">Role</span></span>

* <span data-ttu-id="7938c-2530">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="7938c-2530">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="7938c-2531">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="7938c-2531">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="7938c-2532">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="7938c-2532">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="7938c-2533">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="7938c-2533">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="7938c-2534">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="7938c-2534">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7938c-2535">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7938c-2535">Service Fabric</span></span>
* <span data-ttu-id="7938c-2536">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="7938c-2536">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="7938c-2537">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="7938c-2537">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="7938c-2538">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="7938c-2538">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-2539">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-2539">SQL</span></span>

* <span data-ttu-id="7938c-2540">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="7938c-2540">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="7938c-2541">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="7938c-2541">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="7938c-2542">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="7938c-2542">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-2543">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-2543">Storage</span></span>

* <span data-ttu-id="7938c-2544">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="7938c-2544">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="7938c-2545">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="7938c-2545">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="7938c-2546">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="7938c-2546">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="7938c-2547">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="7938c-2547">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="7938c-2548">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="7938c-2548">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="7938c-2549">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="7938c-2549">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-2550">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-2550">VM</span></span>

* <span data-ttu-id="7938c-2551">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="7938c-2551">Support configuring nsg</span></span>
* <span data-ttu-id="7938c-2552">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="7938c-2552">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="7938c-2553">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="7938c-2553">Support managed service identities</span></span>
* <span data-ttu-id="7938c-2554">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="7938c-2554">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="7938c-2555">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="7938c-2555">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="7938c-2556">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="7938c-2556">May 10, 2017</span></span>

<span data-ttu-id="7938c-2557">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="7938c-2557">Version 2.0.6</span></span>

* <span data-ttu-id="7938c-2558">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7938c-2558">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="7938c-2559">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="7938c-2559">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="7938c-2560">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7938c-2560">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="7938c-2561">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="7938c-2561">Include Cognitive Services module</span></span>
* <span data-ttu-id="7938c-2562">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7938c-2562">Include Service Fabric module</span></span>
* <span data-ttu-id="7938c-2563">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="7938c-2563">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="7938c-2564">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="7938c-2564">Add support for CDN commands</span></span>
* <span data-ttu-id="7938c-2565">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="7938c-2565">Remove Container module</span></span>
* <span data-ttu-id="7938c-2566">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="7938c-2566">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="7938c-2567">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="7938c-2567">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="7938c-2568">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-2568">Core</span></span>

* <span data-ttu-id="7938c-2569">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="7938c-2569">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="7938c-2570">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="7938c-2570">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="7938c-2571">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="7938c-2571">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="7938c-2572">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="7938c-2572">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="7938c-2573">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="7938c-2573">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="7938c-2574">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="7938c-2574">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="7938c-2575">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="7938c-2575">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="7938c-2576">núcleo: permitir que o caminho do arquivo accessTokens.json seja configurável por meio de uma variável de ambiente ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="7938c-2576">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="7938c-2577">núcleo: permitir que padrões configurados sejam aplicados em argumentos opcionais ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="7938c-2577">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="7938c-2578">núcleo: desempenho aprimorado</span><span class="sxs-lookup"><span data-stu-id="7938c-2578">core: Improved performance</span></span>
* <span data-ttu-id="7938c-2579">núcleo: certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="7938c-2579">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="7938c-2580">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="7938c-2580">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-2581">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-2581">ACS</span></span>

* <span data-ttu-id="7938c-2582">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7938c-2582">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="7938c-2583">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="7938c-2583">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="7938c-2584">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="7938c-2584">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="7938c-2585">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="7938c-2585">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-2586">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-2586">AppService</span></span>

* <span data-ttu-id="7938c-2587">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="7938c-2587">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="7938c-2588">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="7938c-2588">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="7938c-2589">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="7938c-2589">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="7938c-2590">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="7938c-2590">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="7938c-2591">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="7938c-2591">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="7938c-2592">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="7938c-2592">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="7938c-2593">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="7938c-2593">support slot swap with preview</span></span>
* <span data-ttu-id="7938c-2594">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="7938c-2594">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="7938c-2595">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="7938c-2595">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7938c-2596">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7938c-2596">CosmosDB</span></span>

* <span data-ttu-id="7938c-2597">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7938c-2597">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="7938c-2598">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="7938c-2598">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="7938c-2599">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="7938c-2599">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="7938c-2600">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="7938c-2600">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7938c-2601">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7938c-2601">Data Lake Analytics</span></span>

* <span data-ttu-id="7938c-2602">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="7938c-2602">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="7938c-2603">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="7938c-2603">Add support for new catalog item type: package.</span></span> <span data-ttu-id="7938c-2604">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="7938c-2604">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="7938c-2605">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="7938c-2605">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="7938c-2606">Tabela</span><span class="sxs-lookup"><span data-stu-id="7938c-2606">Table</span></span>
  * <span data-ttu-id="7938c-2607">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="7938c-2607">Table valued function</span></span>
  * <span data-ttu-id="7938c-2608">Visualizar</span><span class="sxs-lookup"><span data-stu-id="7938c-2608">View</span></span>
  * <span data-ttu-id="7938c-2609">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="7938c-2609">Table Statistics.</span></span> <span data-ttu-id="7938c-2610">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="7938c-2610">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7938c-2611">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7938c-2611">Data Lake Store</span></span>

* <span data-ttu-id="7938c-2612">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="7938c-2612">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="7938c-2613">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="7938c-2613">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="7938c-2614">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="7938c-2614">missed help for access show.</span></span> <span data-ttu-id="7938c-2615">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="7938c-2615">adding it.</span></span> <span data-ttu-id="7938c-2616">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="7938c-2616">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="7938c-2617">Localizar</span><span class="sxs-lookup"><span data-stu-id="7938c-2617">Find</span></span>

* <span data-ttu-id="7938c-2618">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="7938c-2618">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="7938c-2619">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7938c-2619">KeyVault</span></span>

* <span data-ttu-id="7938c-2620">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="7938c-2620">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="7938c-2621">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois estes parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="7938c-2621">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="7938c-2622">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="7938c-2622">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="7938c-2623">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="7938c-2623">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="7938c-2624">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="7938c-2624">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="7938c-2625">Laboratório</span><span class="sxs-lookup"><span data-stu-id="7938c-2625">Lab</span></span>

* <span data-ttu-id="7938c-2626">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="7938c-2626">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="7938c-2627">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="7938c-2627">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="7938c-2628">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="7938c-2628">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="7938c-2629">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="7938c-2629">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="7938c-2630">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="7938c-2630">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="7938c-2631">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7938c-2631">Monitor</span></span>

* <span data-ttu-id="7938c-2632">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="7938c-2632">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="7938c-2633">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="7938c-2633">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="7938c-2634">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-2634">Network</span></span>

* <span data-ttu-id="7938c-2635">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="7938c-2635">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="7938c-2636">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2636">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="7938c-2637">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7938c-2637">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="7938c-2638">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7938c-2638">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="7938c-2639">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="7938c-2639">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="7938c-2640">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="7938c-2640">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="7938c-2641">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="7938c-2641">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="7938c-2642">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="7938c-2642">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="7938c-2643">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="7938c-2643">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="7938c-2644">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="7938c-2644">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="7938c-2645">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="7938c-2645">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="7938c-2646">BC: corrigido um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2646">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="7938c-2647">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="7938c-2647">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="7938c-2648">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="7938c-2648">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="7938c-2649">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="7938c-2649">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="7938c-2650">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="7938c-2650">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="7938c-2651">Perfil</span><span class="sxs-lookup"><span data-stu-id="7938c-2651">Profile</span></span>

* <span data-ttu-id="7938c-2652">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="7938c-2652">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="7938c-2653">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="7938c-2653">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="7938c-2654">Redis</span><span class="sxs-lookup"><span data-stu-id="7938c-2654">Redis</span></span>

* <span data-ttu-id="7938c-2655">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="7938c-2655">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="7938c-2656">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="7938c-2656">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="7938c-2657">Recurso</span><span class="sxs-lookup"><span data-stu-id="7938c-2657">Resource</span></span>

* <span data-ttu-id="7938c-2658">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="7938c-2658">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="7938c-2659">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="7938c-2659">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="7938c-2660">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="7938c-2660">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="7938c-2661">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="7938c-2661">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="7938c-2662">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="7938c-2662">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="7938c-2663">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="7938c-2663">Add docs for az lock update.</span></span> <span data-ttu-id="7938c-2664">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="7938c-2664">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="7938c-2665">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="7938c-2665">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="7938c-2666">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="7938c-2666">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="7938c-2667">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="7938c-2667">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="7938c-2668">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="7938c-2668">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="7938c-2669">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="7938c-2669">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="7938c-2670">Função</span><span class="sxs-lookup"><span data-stu-id="7938c-2670">Role</span></span>

* <span data-ttu-id="7938c-2671">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="7938c-2671">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="7938c-2672">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="7938c-2672">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="7938c-2673">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="7938c-2673">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="7938c-2674">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="7938c-2674">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="7938c-2675">SQL</span><span class="sxs-lookup"><span data-stu-id="7938c-2675">SQL</span></span>

* <span data-ttu-id="7938c-2676">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="7938c-2676">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="7938c-2677">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="7938c-2677">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="7938c-2678">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-2678">Storage</span></span>

* <span data-ttu-id="7938c-2679">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="7938c-2679">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="7938c-2680">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="7938c-2680">Add support for incremental blob copy</span></span>
* <span data-ttu-id="7938c-2681">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="7938c-2681">Add support for large block blob upload</span></span>
* <span data-ttu-id="7938c-2682">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="7938c-2682">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-2683">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-2683">VM</span></span>

* <span data-ttu-id="7938c-2684">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="7938c-2684">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="7938c-2685">observação: em comandos da VM em nuvens soberanas, evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="7938c-2685">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="7938c-2686">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="7938c-2686">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="7938c-2687">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="7938c-2687">az vm/vmss disk</span></span>
  3. <span data-ttu-id="7938c-2688">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="7938c-2688">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="7938c-2689">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="7938c-2689">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="7938c-2690">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="7938c-2690">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="7938c-2691">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="7938c-2691">April 3, 2017</span></span>

<span data-ttu-id="7938c-2692">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="7938c-2692">Version 2.0.2</span></span>

<span data-ttu-id="7938c-2693">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="7938c-2693">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="7938c-2694">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7938c-2694">Core</span></span>

* <span data-ttu-id="7938c-2695">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="7938c-2695">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="7938c-2696">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="7938c-2696">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="7938c-2697">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="7938c-2697">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="7938c-2698">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="7938c-2698">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="7938c-2699">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="7938c-2699">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="7938c-2700">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="7938c-2700">Add prompting for missing template parameters.</span></span> <span data-ttu-id="7938c-2701">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="7938c-2701">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="7938c-2702">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="7938c-2702">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="7938c-2703">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="7938c-2703">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="7938c-2704">ACS</span><span class="sxs-lookup"><span data-stu-id="7938c-2704">ACS</span></span>

* <span data-ttu-id="7938c-2705">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="7938c-2705">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="7938c-2706">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="7938c-2706">Add support for ssh key password prompting.</span></span> <span data-ttu-id="7938c-2707">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="7938c-2707">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="7938c-2708">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="7938c-2708">Add support for windows clusters.</span></span> <span data-ttu-id="7938c-2709">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="7938c-2709">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="7938c-2710">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="7938c-2710">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="7938c-2711">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="7938c-2711">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="7938c-2712">AppService</span><span class="sxs-lookup"><span data-stu-id="7938c-2712">AppService</span></span>

* <span data-ttu-id="7938c-2713">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="7938c-2713">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="7938c-2714">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="7938c-2714">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="7938c-2715">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="7938c-2715">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="7938c-2716">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="7938c-2716">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="7938c-2717">DataLake</span><span class="sxs-lookup"><span data-stu-id="7938c-2717">DataLake</span></span>

* <span data-ttu-id="7938c-2718">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7938c-2718">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="7938c-2719">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7938c-2719">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="7938c-2720">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="7938c-2720">DocuemntDB</span></span>

* <span data-ttu-id="7938c-2721">DocumentDB: adicionado suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="7938c-2721">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="7938c-2722">VM</span><span class="sxs-lookup"><span data-stu-id="7938c-2722">VM</span></span>

* <span data-ttu-id="7938c-2723">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="7938c-2723">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="7938c-2724">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="7938c-2724">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="7938c-2725">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="7938c-2725">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="7938c-2726">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="7938c-2726">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="7938c-2727">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="7938c-2727">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="7938c-2728">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="7938c-2728">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="7938c-2729">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="7938c-2729">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="7938c-2730">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="7938c-2730">February 27, 2017</span></span>

<span data-ttu-id="7938c-2731">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="7938c-2731">Version 2.0.0</span></span>

<span data-ttu-id="7938c-2732">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="7938c-2732">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="7938c-2733">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="7938c-2733">Container Service (acs)</span></span>
- <span data-ttu-id="7938c-2734">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="7938c-2734">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="7938c-2735">Rede</span><span class="sxs-lookup"><span data-stu-id="7938c-2735">Networking</span></span>
- <span data-ttu-id="7938c-2736">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7938c-2736">Storage</span></span>

<span data-ttu-id="7938c-2737">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="7938c-2737">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="7938c-2738">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="7938c-2738">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="7938c-2739">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="7938c-2739">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="7938c-2740">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="7938c-2740">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="7938c-2741">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="7938c-2741">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="7938c-2742">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="7938c-2742">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="7938c-2743">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="7938c-2743">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="7938c-2744">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="7938c-2744">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="7938c-2745">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="7938c-2745">Provide feedback from the command line with the `az feedback` command</span></span>

