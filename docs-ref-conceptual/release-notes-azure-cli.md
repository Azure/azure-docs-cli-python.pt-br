---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 08/27/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 156ff2e6d011104ebbb1608ff33bad8ebb6396ed
ms.sourcegitcommit: df2be5609a6cbeecb9f8ef0928a9fabfb207e7f9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "70047281"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="48688-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="48688-103">Azure CLI release notes</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="48688-104">27 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="48688-104">August 27, 2019</span></span>

<span data-ttu-id="48688-105">Versão 2.0.72</span><span class="sxs-lookup"><span data-stu-id="48688-105">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="48688-106">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-106">ACR</span></span>

* <span data-ttu-id="48688-107">[ALTERAÇÃO DA FALHA] Remoção do suporte para o SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="48688-107">[BREAKING CHNAGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="48688-108">Gerenciamento de API</span><span class="sxs-lookup"><span data-stu-id="48688-108">API Management</span></span>

* <span data-ttu-id="48688-109">[VERSÃO PRÉVIA] Adição do grupo de comandos `apim`</span><span class="sxs-lookup"><span data-stu-id="48688-109">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-110">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-110">AppService</span></span>

* <span data-ttu-id="48688-111">Correção do problema com o comando `webapp webjob continuous start` ao especificar um slot</span><span class="sxs-lookup"><span data-stu-id="48688-111">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="48688-112">Alteração de `webapp up` para detectar a pasta `env` e removê-la do arquivo usado para implantação</span><span class="sxs-lookup"><span data-stu-id="48688-112">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="48688-113">Keyvault</span><span class="sxs-lookup"><span data-stu-id="48688-113">Keyvault</span></span>

* <span data-ttu-id="48688-114">Correção de um bug no `keyvault secret set` que ignorava o argumento `--expires`</span><span class="sxs-lookup"><span data-stu-id="48688-114">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="48688-115">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-115">Network</span></span>

* <span data-ttu-id="48688-116">Adição de suporte para endereços IPv6 a argumentos `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="48688-116">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="48688-117">Adição de novos comandos `network private-endpoint [create|update|list-types]` para o gerenciamento de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="48688-117">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="48688-118">Adição do grupo de comandos `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="48688-118">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="48688-119">Adicionados os argumentos `--private-endpoint-network-policies` e `--private-link-service-network-policies` para `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="48688-119">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="48688-120">RBAC</span><span class="sxs-lookup"><span data-stu-id="48688-120">RBAC</span></span>

* <span data-ttu-id="48688-121">Correção de um problema com `ad app update --homepage` em que a página inicial não era atualizada</span><span class="sxs-lookup"><span data-stu-id="48688-121">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="48688-122">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="48688-122">ServiceFabric</span></span>

* <span data-ttu-id="48688-123">Adição de suporte para nomes de Key Vault grafados com maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="48688-123">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="48688-124">Correção de um problema ao usar certificados no Key Vault</span><span class="sxs-lookup"><span data-stu-id="48688-124">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="48688-125">Correção de um problema com o uso de arquivos de certificado PFX</span><span class="sxs-lookup"><span data-stu-id="48688-125">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="48688-126">Correção de um problema com `sf cluster certificate add` quando o grupo de recursos do Key Vault não era especificado</span><span class="sxs-lookup"><span data-stu-id="48688-126">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="48688-127">Correção de um problema em que `sf cluster set` não funcionava</span><span class="sxs-lookup"><span data-stu-id="48688-127">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="48688-128">SignalR</span><span class="sxs-lookup"><span data-stu-id="48688-128">SignalR</span></span>

* <span data-ttu-id="48688-129">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="48688-129">Added new commands:</span></span>
  * <span data-ttu-id="48688-130">`signalr cors`: gerenciar CORS do SignalR</span><span class="sxs-lookup"><span data-stu-id="48688-130">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="48688-131">`signalr restart`: reiniciar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="48688-131">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="48688-132">`signalr update`: atualizar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="48688-132">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="48688-133">Adicionado o argumento `--service-mode` para `signalr create`</span><span class="sxs-lookup"><span data-stu-id="48688-133">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="48688-134">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-134">Storage</span></span>

* <span data-ttu-id="48688-135">Adicionado o comando `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="48688-135">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="48688-136">13 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="48688-136">August 13, 2019</span></span>

<span data-ttu-id="48688-137">Versão 2.0.71</span><span class="sxs-lookup"><span data-stu-id="48688-137">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-138">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-138">AppService</span></span>

* <span data-ttu-id="48688-139">Um problema de falha de slots com os comandos `webapp webjob continuous` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="48688-139">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="48688-140">BotService</span><span class="sxs-lookup"><span data-stu-id="48688-140">BotService</span></span>

* <span data-ttu-id="48688-141">[ALTERAÇÃO SIGNIFICATIVA] O suporte para a criação de bots SDK v3 foi removido</span><span class="sxs-lookup"><span data-stu-id="48688-141">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="48688-142">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="48688-142">CognitiveServices</span></span>

* <span data-ttu-id="48688-143">Adicionados os comandos `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="48688-143">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="48688-144">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="48688-144">Cosmos DB</span></span>

* <span data-ttu-id="48688-145">Removido o aviso ao atualizar vários locais de gravação</span><span class="sxs-lookup"><span data-stu-id="48688-145">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="48688-146">Foram adicionados os comandos CRUD para o CosmosDB SQL, MongoDB, Cassandra, Gremlin e Recursos de tabela e taxa de transferência do recurso</span><span class="sxs-lookup"><span data-stu-id="48688-146">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="48688-147">HDInsight</span><span class="sxs-lookup"><span data-stu-id="48688-147">HDInsight</span></span>

<span data-ttu-id="48688-148">Esta versão contém um grande número de alterações da falha.</span><span class="sxs-lookup"><span data-stu-id="48688-148">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="48688-149">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="48688-149">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="48688-150">`--storage-default-container` renomeado para `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="48688-150">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="48688-151">`--storage-default-filesystem` renomeado para `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="48688-151">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="48688-152">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--name` de `application create` foi alterado para representar o nome do aplicativo em vez do nome do cluster</span><span class="sxs-lookup"><span data-stu-id="48688-152">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="48688-153">O argumento `--cluster-name` foi adicionado a `application create` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="48688-153">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="48688-154">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `application create`:</span><span class="sxs-lookup"><span data-stu-id="48688-154">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="48688-155">`--application-type` renomeado para `--type`</span><span class="sxs-lookup"><span data-stu-id="48688-155">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="48688-156">`--marketplace-identifier` renomeado para `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="48688-156">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="48688-157">`--https-endpoint-access-mode` renomeado para `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="48688-157">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="48688-158">Renomeado de `--https-endpoint-destination-port` para `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="48688-158">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="48688-159">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros removidos para `application create`:</span><span class="sxs-lookup"><span data-stu-id="48688-159">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="48688-160">[ALTERAÇÃO DA FALHA] Renomeado de `--target-instance-count` para `--workernode-count` para `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="48688-160">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="48688-161">[ALTERAÇÃO SIGNIFICATIVA] Todos os comandos no grupo `hdinsight script-action` foram alterados para usar o parâmetro `--name` como o nome da ação de script.</span><span class="sxs-lookup"><span data-stu-id="48688-161">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="48688-162">O argumento `--cluster-name` foi adicionado a todos os comandos `hdinsight script-action` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="48688-162">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="48688-163">[ALTERAÇÃO SIGNIFICATIVA] Renomeado de `--script-execution-id` para `--execution-id` para todos os comandos `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="48688-163">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="48688-164">[ALTERAÇÃO SIGNIFICATIVA] `hdinsight script-action show` renomeado para `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="48688-164">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="48688-165">[ALTERAÇÃO DA FALHA] Os parâmetros foram alterados para `hdinsight script-action execute --roles` para serem separados por espaços em vez de separados por vírgula</span><span class="sxs-lookup"><span data-stu-id="48688-165">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="48688-166">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro `--persisted` de `hdinsight script-action list` foi removido</span><span class="sxs-lookup"><span data-stu-id="48688-166">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="48688-167">O parâmetro `hdinsight create --cluster-configurations` foi alterado para aceitar um caminho para um arquivo JSON local ou uma cadeia de caracteres JSON</span><span class="sxs-lookup"><span data-stu-id="48688-167">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="48688-168">Adicionado o comando `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="48688-168">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="48688-169">Alterado `hdinsight monitor enable --workspace` para aceitar uma ID do workspace ou nome do workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="48688-169">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="48688-170">O argumento `hdinsight monitor enable --primary-key`, que será necessário caso uma ID do workspace seja fornecida como o parâmetro, foi adicionado</span><span class="sxs-lookup"><span data-stu-id="48688-170">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="48688-171">Foram adicionados mais exemplos e atualização das descrições das mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="48688-171">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="48688-172">Interativo</span><span class="sxs-lookup"><span data-stu-id="48688-172">Interactive</span></span>

* <span data-ttu-id="48688-173">Um erro no carregamento foi corrigido</span><span class="sxs-lookup"><span data-stu-id="48688-173">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="48688-174">kubernetes</span><span class="sxs-lookup"><span data-stu-id="48688-174">Kubernetes</span></span>

* <span data-ttu-id="48688-175">Alterado para usar `https` se a porta do contêiner do painel estiver usando `https`</span><span class="sxs-lookup"><span data-stu-id="48688-175">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="48688-176">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-176">Network</span></span>

* <span data-ttu-id="48688-177">O argumento `--yes` foi adicionado a `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="48688-177">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="48688-178">Perfil</span><span class="sxs-lookup"><span data-stu-id="48688-178">Profile</span></span>

* <span data-ttu-id="48688-179">O argumento `--resource-type` foi adicionado a `account get-access-token` para obter tokens de acesso de recurso</span><span class="sxs-lookup"><span data-stu-id="48688-179">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="48688-180">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="48688-180">ServiceFabric</span></span>

* <span data-ttu-id="48688-181">Todas as versões de sistema operacional com suporte para criação do cluster sf foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="48688-181">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="48688-182">Foi corrigido o bug de validação do certificado primário</span><span class="sxs-lookup"><span data-stu-id="48688-182">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="48688-183">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-183">Storage</span></span>

* <span data-ttu-id="48688-184">Adicionado o comando `storage copy`</span><span class="sxs-lookup"><span data-stu-id="48688-184">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="48688-185">30 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="48688-185">July 30, 2019</span></span>

<span data-ttu-id="48688-186">Versão 2.0.70</span><span class="sxs-lookup"><span data-stu-id="48688-186">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="48688-187">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-187">ACR</span></span>

* <span data-ttu-id="48688-188">Corrigido o problema #9952 (uma regressão no comando `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="48688-188">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="48688-189">Removido o nome da imagem do construtor padrão em `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="48688-189">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-190">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-190">Appservice</span></span>

* <span data-ttu-id="48688-191">Alterado `webapp config ssl` para mostrar uma mensagem se um recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="48688-191">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="48688-192">Corrigido o problema em que `functionapp create` não aceita o tipo de conta de armazenamento `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="48688-192">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="48688-193">Corrigido um problema em que `webapp up` falharia se fosse executado usando versões mais antigas do Python</span><span class="sxs-lookup"><span data-stu-id="48688-193">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="48688-194">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-194">Network</span></span>

* <span data-ttu-id="48688-195">Removido parâmetro inválido `--ids` de `network nic ip-config add` (corrige o #9861)</span><span class="sxs-lookup"><span data-stu-id="48688-195">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="48688-196">Corrige o #9604.</span><span class="sxs-lookup"><span data-stu-id="48688-196">Fixes #9604.</span></span> <span data-ttu-id="48688-197">Adicionado o parâmetro `--root-certs` ao `network application-gateway http-settings [create|update]` para dar suporte a certificados raiz confiáveis associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="48688-197">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="48688-198">Fixado argumento `--subscription` para `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="48688-198">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="48688-199">RBAC</span><span class="sxs-lookup"><span data-stu-id="48688-199">RBAC</span></span>

* <span data-ttu-id="48688-200">Adicionado o comando `user update`</span><span class="sxs-lookup"><span data-stu-id="48688-200">Added `user update` command</span></span>
* <span data-ttu-id="48688-201">[PRETERIDO] Preterido `--upn-or-object-id` de comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="48688-201">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="48688-202">Usar argumento de substituição `--id`</span><span class="sxs-lookup"><span data-stu-id="48688-202">Use replacement argument `--id`</span></span>
* <span data-ttu-id="48688-203">Adicionado argumento `--id` para comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="48688-203">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="48688-204">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-204">SQL</span></span>

* <span data-ttu-id="48688-205">Adicionados comandos de gerenciamento para chaves de instância gerenciada e protetor de TDE</span><span class="sxs-lookup"><span data-stu-id="48688-205">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="48688-206">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-206">Storage</span></span>

* <span data-ttu-id="48688-207">Adicionado o comando `storage remove`</span><span class="sxs-lookup"><span data-stu-id="48688-207">Added `storage remove` command</span></span>
* <span data-ttu-id="48688-208">Corrigido um problema com `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="48688-208">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="48688-209">VM</span><span class="sxs-lookup"><span data-stu-id="48688-209">VM</span></span>

* <span data-ttu-id="48688-210">Alterado `list-skus` para usar versão de API mais recente a fim de externar detalhes de zona</span><span class="sxs-lookup"><span data-stu-id="48688-210">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="48688-211">Alterado o padrão de `--single-placement-group` para `false` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="48688-211">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="48688-212">Adicionada a capacidade de selecionar SKUs de armazenamento ZRS para `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="48688-212">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="48688-213">Adicionado novo grupo de comandos `vm host` para dar suporte a hosts dedicados</span><span class="sxs-lookup"><span data-stu-id="48688-213">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="48688-214">Adicionados parâmetros `--host` e `--host-group` em `vm create` para definir o host dedicado da VM</span><span class="sxs-lookup"><span data-stu-id="48688-214">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="48688-215">16 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="48688-215">July 16, 2019</span></span>

<span data-ttu-id="48688-216">Versão 2.0.69</span><span class="sxs-lookup"><span data-stu-id="48688-216">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-217">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-217">Appservice</span></span>

* <span data-ttu-id="48688-218">Os comandos `webapp identity` foram alterados para retornar uma mensagem de erro apropriada se o nome do aplicativo ou ResourceGroupName for inválido</span><span class="sxs-lookup"><span data-stu-id="48688-218">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="48688-219">`webapp list` corrigido para retornar o valor correto para numberOfSites se nenhum ResourceGroup foi fornecido</span><span class="sxs-lookup"><span data-stu-id="48688-219">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="48688-220">Corrigidos os efeitos colaterais de `appservice plan create` e `webapp create`</span><span class="sxs-lookup"><span data-stu-id="48688-220">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="48688-221">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-221">Core</span></span>

* <span data-ttu-id="48688-222">Corrigido um problema em que `--subscription` aparecia apesar de não ser aplicável</span><span class="sxs-lookup"><span data-stu-id="48688-222">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="48688-223">Lote</span><span class="sxs-lookup"><span data-stu-id="48688-223">Batch</span></span>

* <span data-ttu-id="48688-224">[ALTERAÇÃO SIGNIFICATIVA] `batch pool node-agent-skus list` foi substituído por `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="48688-224">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="48688-225">Adicionado suporte para regras de segurança bloqueando o acesso de rede a um pool com base na porta de origem do tráfego ao usar a opção `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="48688-225">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="48688-226">Suporte adicionado para executar a tarefa no diretório de trabalho de contêiner ou no diretório de trabalho de tarefa em lotes ao usar a opção `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="48688-226">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="48688-227">Corrigido o erro na opção `--application-package-references` de `batch pool create` em que ela funcionaria apenas com padrões</span><span class="sxs-lookup"><span data-stu-id="48688-227">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="48688-228">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="48688-228">Eventhubs</span></span>

* <span data-ttu-id="48688-229">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="48688-229">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="48688-230">RDBMS</span><span class="sxs-lookup"><span data-stu-id="48688-230">RDBMS</span></span>

* <span data-ttu-id="48688-231">Adicionado um parâmetro opcional para especificar a réplica de SKU para criar o comando de réplica</span><span class="sxs-lookup"><span data-stu-id="48688-231">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="48688-232">Corrigido o problema com a falha no teste de CI com a criação de réplica de MySQL</span><span class="sxs-lookup"><span data-stu-id="48688-232">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="48688-233">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="48688-233">Relay</span></span>

* <span data-ttu-id="48688-234">Corrigido o problema com a conexão híbrida quando a autorização do cliente desabilitava [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="48688-234">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="48688-235">Parâmetro `--requires-transport-security` adicionado a `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="48688-235">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="48688-236">Barramento de serviço</span><span class="sxs-lookup"><span data-stu-id="48688-236">Servicebus</span></span>

* <span data-ttu-id="48688-237">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="48688-237">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="48688-238">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-238">Storage</span></span>

* <span data-ttu-id="48688-239">Habilitar AADDS de arquivos para atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-239">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="48688-240">Problema corrigido `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="48688-240">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="48688-241">2 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="48688-241">July 2, 2019</span></span>

<span data-ttu-id="48688-242">Versão 2.0.68</span><span class="sxs-lookup"><span data-stu-id="48688-242">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="48688-243">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-243">Core</span></span>

* <span data-ttu-id="48688-244">Agora, os módulos de comando são consolidados em um único Python distribuível.</span><span class="sxs-lookup"><span data-stu-id="48688-244">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="48688-245">Isso substitui o uso direto de muitos pacotes `azure-cli-` no PyPI.</span><span class="sxs-lookup"><span data-stu-id="48688-245">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="48688-246">Assim, o tamanho da instalação será reduzido e apenas os usuários que tiverem instalado diretamente por meio do `pip` serão afetados.</span><span class="sxs-lookup"><span data-stu-id="48688-246">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="48688-247">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-247">ACR</span></span>

* <span data-ttu-id="48688-248">Foi adicionado o suporte para gatilhos de temporizador para tarefa</span><span class="sxs-lookup"><span data-stu-id="48688-248">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-249">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-249">Appservice</span></span>

* <span data-ttu-id="48688-250">O `functionapp create` foi alterado para habilitar o Application Insights por padrão</span><span class="sxs-lookup"><span data-stu-id="48688-250">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="48688-251">[ALTERAÇÃO SIGNIFICATIVA] Foi removido o comando `functionapp devops-build` preterido.</span><span class="sxs-lookup"><span data-stu-id="48688-251">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="48688-252">Agora, use o novo comando `az functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="48688-252">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="48688-253">Foi adicionado o suporte ao plano de aplicativo de funções Consumo em Linux ao `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="48688-253">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="48688-254">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="48688-254">Cosmos DB</span></span>

* <span data-ttu-id="48688-255">Foi adicionado o suporte para desabilitar a TTL</span><span class="sxs-lookup"><span data-stu-id="48688-255">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="48688-256">DLS</span><span class="sxs-lookup"><span data-stu-id="48688-256">DLS</span></span>

* <span data-ttu-id="48688-257">Versão atualizada do ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="48688-257">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="48688-258">Comentários</span><span class="sxs-lookup"><span data-stu-id="48688-258">Feedback</span></span>

* <span data-ttu-id="48688-259">Ao relatar um comando de extensão com falha, agora, o `az feedback` tenta abrir o navegador na URL do projeto/repositório da extensão por meio do índice</span><span class="sxs-lookup"><span data-stu-id="48688-259">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="48688-260">HDInsight</span><span class="sxs-lookup"><span data-stu-id="48688-260">HDInsight</span></span>

* <span data-ttu-id="48688-261">[ALTERAÇÃO SIGNIFICATIVA] O nome do grupo de comandos `oms` foi alterado para `monitor`</span><span class="sxs-lookup"><span data-stu-id="48688-261">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="48688-262">[ALTERAÇÃO SIGNIFICATIVA] `--http-password/-p` tornou-se um parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="48688-262">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="48688-263">Foram adicionados preenchedores para o preenchedor dos parâmetros `--cluster-admin-account` e `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="48688-263">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="48688-264">O parâmetro `cluster-users-group-dns` foi alterado para ser obrigatório quando `—esp` estiver presente</span><span class="sxs-lookup"><span data-stu-id="48688-264">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="48688-265">Foi adicionado um tempo limite para todos os preenchedores automáticos de argumento existentes</span><span class="sxs-lookup"><span data-stu-id="48688-265">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="48688-266">Foi adicionado um tempo limite para transformar o nome do recurso na ID de recurso</span><span class="sxs-lookup"><span data-stu-id="48688-266">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="48688-267">Os preenchedores automáticos foram alterados para selecionar recursos de qualquer grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="48688-267">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="48688-268">Pode ser um grupo de recursos diferente daquele especificado com `-g`</span><span class="sxs-lookup"><span data-stu-id="48688-268">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="48688-269">Foi adicionado o suporte para os parâmetros `--sub-domain-suffix` e `--disable_gateway_auth` no comando `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="48688-269">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="48688-270">Serviços gerenciados</span><span class="sxs-lookup"><span data-stu-id="48688-270">Managed Services</span></span>

* <span data-ttu-id="48688-271">Introdução ao módulo de comando de serviço gerenciado em versão prévia</span><span class="sxs-lookup"><span data-stu-id="48688-271">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="48688-272">Perfil</span><span class="sxs-lookup"><span data-stu-id="48688-272">Profile</span></span>
* <span data-ttu-id="48688-273">Suprimir o argumento `--subscription` para o comando de logoff</span><span class="sxs-lookup"><span data-stu-id="48688-273">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="48688-274">RBAC</span><span class="sxs-lookup"><span data-stu-id="48688-274">RBAC</span></span>

* <span data-ttu-id="48688-275">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--password` foi removido de `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="48688-275">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="48688-276">Foi adicionado o parâmetro `--assignee-principal-type` ao comando `create` para evitar falhas intermitentes causadas pela latência de replicação do servidor do AAD Graph</span><span class="sxs-lookup"><span data-stu-id="48688-276">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="48688-277">Foi corrigida uma falha em `ad signed-in-user` ao listar objetos de propriedade</span><span class="sxs-lookup"><span data-stu-id="48688-277">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="48688-278">Foi corrigido um problema em que o `ad sp` não localizava o aplicativo certo de uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="48688-278">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="48688-279">RDBMS</span><span class="sxs-lookup"><span data-stu-id="48688-279">RDBMS</span></span>

* <span data-ttu-id="48688-280">Foi adicionado o suporte à replicação para o MariaDB</span><span class="sxs-lookup"><span data-stu-id="48688-280">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="48688-281">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-281">SQL</span></span>

* <span data-ttu-id="48688-282">Valores permitidos documentados para `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="48688-282">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="48688-283">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-283">Storage</span></span>

* <span data-ttu-id="48688-284">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="48688-284">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="48688-285">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="48688-285">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="48688-286">VM</span><span class="sxs-lookup"><span data-stu-id="48688-286">VM</span></span>

* <span data-ttu-id="48688-287">Foi corrigido o bug em que o `vmss create` retornava uma mensagem de erro quando era executado com `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="48688-287">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="48688-288">Foi removida a validação do lado do cliente de `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="48688-288">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="48688-289">Não falha quando `--single-placement-group` é definido como `true` e `--instance-count` é maior que 100 ou quando são especificadas zonas de disponibilidade, mas deixa essa validação para o serviço de computação</span><span class="sxs-lookup"><span data-stu-id="48688-289">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="48688-290">Foi corrigido o bug em que o `[vm|vmss] extension image list` falhava quando era usado com `--latest`</span><span class="sxs-lookup"><span data-stu-id="48688-290">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="48688-291">18 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="48688-291">June 18, 2019</span></span>

<span data-ttu-id="48688-292">Versão 2.0.67</span><span class="sxs-lookup"><span data-stu-id="48688-292">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="48688-293">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-293">Core</span></span>

<span data-ttu-id="48688-294">Esta versão apresenta uma nova marca [Versão prévia] para comunicar com mais clareza aos clientes quando um comando, um grupo de comandos ou um argumento está no status de versão prévia.</span><span class="sxs-lookup"><span data-stu-id="48688-294">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="48688-295">Anteriormente, essa informação era transmitida no texto de ajuda ou, implicitamente, pelo número da versão do módulo de comando.</span><span class="sxs-lookup"><span data-stu-id="48688-295">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="48688-296">A CLI removerá os números de versão dos pacotes individuais no futuro.</span><span class="sxs-lookup"><span data-stu-id="48688-296">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="48688-297">Se um comando estiver em versão prévia, todos os seus argumentos também estarão.</span><span class="sxs-lookup"><span data-stu-id="48688-297">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="48688-298">Se um grupo de comandos for rotulado com o status de versão prévia, então todos os seus comandos e argumentos também serão considerados em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="48688-298">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="48688-299">Como resultado dessa alteração, diversos grupos de comandos podem parecer surgir "de repente" com o status de versão prévia com esta liberação.</span><span class="sxs-lookup"><span data-stu-id="48688-299">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="48688-300">O que realmente aconteceu é que a maioria dos pacotes já estava com status de versão prévia, mas estão sendo consideradas GA com esta liberação</span><span class="sxs-lookup"><span data-stu-id="48688-300">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="48688-301">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-301">ACR</span></span>
* <span data-ttu-id="48688-302">Adicionado o comando 'acr check-health'</span><span class="sxs-lookup"><span data-stu-id="48688-302">Added 'acr check-health' command</span></span>
* <span data-ttu-id="48688-303">Melhorado o tratamento de erro para tokens do AAD e para recuperar comandos externos</span><span class="sxs-lookup"><span data-stu-id="48688-303">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="48688-304">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-304">ACS</span></span>
* <span data-ttu-id="48688-305">Comandos preteridos do ACS agora ficam ocultos da exibição da ajuda</span><span class="sxs-lookup"><span data-stu-id="48688-305">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="48688-306">AMS</span><span class="sxs-lookup"><span data-stu-id="48688-306">AMS</span></span>
* <span data-ttu-id="48688-307">[ALTERAÇÃO SIGNIFICATIVA] Alterada para retornar cadeias de caracteres de tempo da ISO 8601 para archive-window-length e key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="48688-307">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-308">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-308">AppService</span></span>
* <span data-ttu-id="48688-309">Adicionado roteamento com base no local para `webapp deleted list` e `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="48688-309">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="48688-310">Corrigido problema em que a URL de destino registrada do webapp ("Não é possível iniciar o aplicativo em...") não era clicável no Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="48688-310">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="48688-311">Corrigido um problema em que a criação de aplicativos com algumas SKUs falhava com um erro de AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="48688-311">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="48688-312">Adicionada a pré-validação para o `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="48688-312">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="48688-313">Corrigido o `[webapp|functionapp] traffic-routing` para usar o actionHostName correto</span><span class="sxs-lookup"><span data-stu-id="48688-313">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="48688-314">Adicionado o suporte de slot para comandos `functionapp`</span><span class="sxs-lookup"><span data-stu-id="48688-314">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="48688-315">Lote</span><span class="sxs-lookup"><span data-stu-id="48688-315">Batch</span></span>
* <span data-ttu-id="48688-316">Corrigida a regressão de autenticação do AAD causada pela geração de relatórios de erros superagressiva para autenticação de chave compartilhada</span><span class="sxs-lookup"><span data-stu-id="48688-316">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="48688-317">BatchAI</span><span class="sxs-lookup"><span data-stu-id="48688-317">BatchAI</span></span>
* <span data-ttu-id="48688-318">Agora os comandos do BatchAI estão preteridos e ocultos</span><span class="sxs-lookup"><span data-stu-id="48688-318">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="48688-319">BotService</span><span class="sxs-lookup"><span data-stu-id="48688-319">BotService</span></span>
* <span data-ttu-id="48688-320">Adição das mensagens de aviso "suporte descontinuado"/"modo de manutenção" para os comandos compatíveis com a v3 do SDK</span><span class="sxs-lookup"><span data-stu-id="48688-320">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48688-321">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48688-321">CosmosDB</span></span>
* <span data-ttu-id="48688-322">[PRETERIDO] Preterido o comando `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="48688-322">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="48688-323">Adicionado o comando `cosmosdb keys list` – substitui o `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="48688-323">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="48688-324">`cosmsodb create/update`: Adicionado novo formato para --location a fim de permitir a configuração da propriedade "isZoneRedundant".</span><span class="sxs-lookup"><span data-stu-id="48688-324">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="48688-325">Formato antigo preterido</span><span class="sxs-lookup"><span data-stu-id="48688-325">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="48688-326">EventGrid</span><span class="sxs-lookup"><span data-stu-id="48688-326">EventGrid</span></span>
* <span data-ttu-id="48688-327">Adicionados comandos do `eventgrid domain` para operações de CRUD no domínio</span><span class="sxs-lookup"><span data-stu-id="48688-327">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="48688-328">Adicionados comandos do `eventgrid domain topic` para operações de CRUD nos tópicos do domínio</span><span class="sxs-lookup"><span data-stu-id="48688-328">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="48688-329">Adicionado argumento do `--odata-query` ao `eventgrid [topic|event-subscription] list` para filtrar os resultados usando a sintaxe do OData</span><span class="sxs-lookup"><span data-stu-id="48688-329">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="48688-330">`event-subscription create/update`: Adicionado o servicebusqueue como novos valores para o parâmetro `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="48688-330">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="48688-331">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para `--included-event-types All` com `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-331">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="48688-332">HDInsight</span><span class="sxs-lookup"><span data-stu-id="48688-332">HDInsight</span></span>
* <span data-ttu-id="48688-333">Adicionado suporte para o parâmetro `--ssh-public-key` no comando `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="48688-333">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="48688-334">IoT</span><span class="sxs-lookup"><span data-stu-id="48688-334">IoT</span></span>
* <span data-ttu-id="48688-335">Adicionado suporte para regenerar as chaves da política de autorização</span><span class="sxs-lookup"><span data-stu-id="48688-335">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="48688-336">Adicionados SDK e suporte para o serviço de provisionamento de repositórios do DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="48688-336">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="48688-337">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-337">Network</span></span>
* <span data-ttu-id="48688-338">Adicionado suporte de zona para o Gateway da NAT</span><span class="sxs-lookup"><span data-stu-id="48688-338">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="48688-339">Adicionado o comando `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="48688-339">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="48688-340">Corrigido o problema com o `dns zone import` em que os usuários não conseguiam importar registros do curinga A</span><span class="sxs-lookup"><span data-stu-id="48688-340">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="48688-341">Corrigido o problema com o `watcher flow-log configure` em que o registro de fluxo não podia ser habilitado em determinadas regiões</span><span class="sxs-lookup"><span data-stu-id="48688-341">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="48688-342">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-342">Resource</span></span>
* <span data-ttu-id="48688-343">Adicionado o comando do `az rest` para fazer chamadas REST</span><span class="sxs-lookup"><span data-stu-id="48688-343">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="48688-344">Corrigido o erro ao usar o `policy assignment list` com um grupo de recursos ou o nível de assinatura `--scope`</span><span class="sxs-lookup"><span data-stu-id="48688-344">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="48688-345">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="48688-345">ServiceBus</span></span>
* <span data-ttu-id="48688-346">Corrigido o problema com o `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="48688-346">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="48688-347">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-347">SQL</span></span>
* <span data-ttu-id="48688-348">Alterado o `--location` para ser opcional para `sql [server|mi] create` – usa o local do grupo de recursos se não especificado</span><span class="sxs-lookup"><span data-stu-id="48688-348">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="48688-349">Corrigido o erro "objeto 'NoneType' não é iterável" para `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="48688-349">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="48688-350">SQLVm</span><span class="sxs-lookup"><span data-stu-id="48688-350">SQLVm</span></span>
* <span data-ttu-id="48688-351">[ALTERAÇÃO DA FALHA] Alterado `sql vm create` para exigir o parâmetro `--license-type`</span><span class="sxs-lookup"><span data-stu-id="48688-351">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="48688-352">Alterado para permitir a configuração da SKU da imagem do SQL ao criar ou atualizar uma VM do SQL</span><span class="sxs-lookup"><span data-stu-id="48688-352">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="48688-353">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-353">Storage</span></span>
* <span data-ttu-id="48688-354">Corrigido o problema com a chave de conta ignorada para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="48688-354">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="48688-355">Corrigido o problema com o `storage blob sync` no Linux</span><span class="sxs-lookup"><span data-stu-id="48688-355">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="48688-356">VM</span><span class="sxs-lookup"><span data-stu-id="48688-356">VM</span></span>
* <span data-ttu-id="48688-357">[VERSÃO PRÉVIA] Adicionados os comandos `vm image template` para criar imagens de VM</span><span class="sxs-lookup"><span data-stu-id="48688-357">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="48688-358">4 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="48688-358">June 4, 2019</span></span>

<span data-ttu-id="48688-359">Versão 2.0.66</span><span class="sxs-lookup"><span data-stu-id="48688-359">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="48688-360">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-360">Core</span></span>
* <span data-ttu-id="48688-361">Foi corrigido o bug em que os comandos falhavam quando `--output yaml` era usado com `--query`</span><span class="sxs-lookup"><span data-stu-id="48688-361">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="48688-362">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-362">ACR</span></span>
* <span data-ttu-id="48688-363">Foi adicionado o grupo de comando 'pack acr' para a criação de Tarefas de build rápida usando Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="48688-363">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="48688-364">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-364">ACS</span></span>
* <span data-ttu-id="48688-365">Permitir a opção de habilitar/desabilitar o complemento kube-dashboard do AKS</span><span class="sxs-lookup"><span data-stu-id="48688-365">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="48688-366">Imprimir uma mensagem amigável quando a assinatura não estiver na lista de permissões para usar o Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="48688-366">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="48688-367">Lote</span><span class="sxs-lookup"><span data-stu-id="48688-367">Batch</span></span>
* <span data-ttu-id="48688-368">Melhoria no tratamento de erro quando você não está conectado a uma conta \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="48688-368">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="48688-369">IoT</span><span class="sxs-lookup"><span data-stu-id="48688-369">IoT</span></span>
* <span data-ttu-id="48688-370">Foi adicionado o suporte para failover manual</span><span class="sxs-lookup"><span data-stu-id="48688-370">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="48688-371">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-371">Network</span></span>
* <span data-ttu-id="48688-372">Foram adicionados os comandos `network application-gateway waf-policy` para oferecer suporte às regras de WAF personalizadas.</span><span class="sxs-lookup"><span data-stu-id="48688-372">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="48688-373">Adicionados os argumentos `--waf-policy` e `--max-capacity` para `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-373">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="48688-374">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-374">Resource</span></span>
* <span data-ttu-id="48688-375">Melhoria da mensagem de erro do `deployment create` quando não há nenhum TTY disponível</span><span class="sxs-lookup"><span data-stu-id="48688-375">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="48688-376">Função</span><span class="sxs-lookup"><span data-stu-id="48688-376">Role</span></span>
* <span data-ttu-id="48688-377">O texto da Ajuda foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="48688-377">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="48688-378">Computação</span><span class="sxs-lookup"><span data-stu-id="48688-378">Compute</span></span>
* <span data-ttu-id="48688-379">Foi adicionado o suporte para `vm create` para as VMs de uma imagem gerenciada com LUNs de disco de dados que não começam em 0 ou que ignoram números</span><span class="sxs-lookup"><span data-stu-id="48688-379">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="48688-380">21 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="48688-380">May 21, 2019</span></span>

<span data-ttu-id="48688-381">Versão 2.0.65</span><span class="sxs-lookup"><span data-stu-id="48688-381">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="48688-382">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-382">Core</span></span>
* <span data-ttu-id="48688-383">Foram adicionados comentários melhores para erros de autenticação</span><span class="sxs-lookup"><span data-stu-id="48688-383">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="48688-384">Corrigido um problema em que a CLI carregava extensões que não eram compatíveis com a versão do núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-384">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="48688-385">Corrigido um problema com a inicialização quando `clouds.config` está corrompido</span><span class="sxs-lookup"><span data-stu-id="48688-385">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="48688-386">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-386">ACR</span></span>
* <span data-ttu-id="48688-387">Foi adicionado suporte das Identidades Gerenciadas para Tarefas</span><span class="sxs-lookup"><span data-stu-id="48688-387">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="48688-388">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-388">ACS</span></span>
* <span data-ttu-id="48688-389">Corrigido o comando `openshift create` quando usado com o cliente AAD do consumidor</span><span class="sxs-lookup"><span data-stu-id="48688-389">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-390">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-390">AppService</span></span>
* <span data-ttu-id="48688-391">[PRETERIDO] Preterido o comando `functionapp devops-build` – Será removido na próxima versão</span><span class="sxs-lookup"><span data-stu-id="48688-391">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="48688-392">`functionapp devops-pipeline` foi alterado para buscar o log de build do Azure DevOps no modo detalhado</span><span class="sxs-lookup"><span data-stu-id="48688-392">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="48688-393">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--use_local_settings` foi removido do comando `functionapp devops-pipeline` – não estava operacional</span><span class="sxs-lookup"><span data-stu-id="48688-393">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="48688-394">`webapp up` foi alterado para retornar uma saída JSON se `--logs` não for usado</span><span class="sxs-lookup"><span data-stu-id="48688-394">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="48688-395">Foi adicionado suporte para escrever recursos padrão para a configuração local de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="48688-395">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="48688-396">Foi adicionado suporte para `webapp up` reimplantar um aplicativo sem usar o argumento `--location`</span><span class="sxs-lookup"><span data-stu-id="48688-396">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="48688-397">Corrigido um problema em que o valor do SKU gratuito não funcionava na criação do ASP do SKU gratuito do Linux</span><span class="sxs-lookup"><span data-stu-id="48688-397">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="48688-398">BotService</span><span class="sxs-lookup"><span data-stu-id="48688-398">BotService</span></span>
* <span data-ttu-id="48688-399">Alterado para permitir todas as capitalizações para parâmetros `--lang` em todos os comandos</span><span class="sxs-lookup"><span data-stu-id="48688-399">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="48688-400">Descrição atualizada do módulo de comando</span><span class="sxs-lookup"><span data-stu-id="48688-400">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="48688-401">Consumo</span><span class="sxs-lookup"><span data-stu-id="48688-401">Consumption</span></span>
* <span data-ttu-id="48688-402">O parâmetro obrigatório ausente foi adicionado para executar `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="48688-402">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="48688-403">IoT</span><span class="sxs-lookup"><span data-stu-id="48688-403">IoT</span></span>
* <span data-ttu-id="48688-404">Suporte adicionado para listar todas as chaves</span><span class="sxs-lookup"><span data-stu-id="48688-404">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="48688-405">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-405">Network</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="48688-407">O argumento `--nat-gateway` foi adicionado a `network vnet subnet [create|update]` para anexar a um gateway NAT</span><span class="sxs-lookup"><span data-stu-id="48688-407">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="48688-408">Corrigido o problema de `dns zone import`, em que os nomes de registro não correspondiam ao tipo de registro</span><span class="sxs-lookup"><span data-stu-id="48688-408">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="48688-409">RDBMS</span><span class="sxs-lookup"><span data-stu-id="48688-409">RDBMS</span></span>
* <span data-ttu-id="48688-410">Suporte a postgres e mysql adicionado para replicação geográfica</span><span class="sxs-lookup"><span data-stu-id="48688-410">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="48688-411">RBAC</span><span class="sxs-lookup"><span data-stu-id="48688-411">RBAC</span></span>
* <span data-ttu-id="48688-412">Suporte ao escopo de grupo de gerenciamento adicionado a `role assignment`</span><span class="sxs-lookup"><span data-stu-id="48688-412">Added support for mangement group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="48688-413">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-413">Storage</span></span>
* <span data-ttu-id="48688-414">`storage blob sync`: adicionar um comando de sincronização ao armazenamento de blobs</span><span class="sxs-lookup"><span data-stu-id="48688-414">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="48688-415">Computação</span><span class="sxs-lookup"><span data-stu-id="48688-415">Compute</span></span>
* <span data-ttu-id="48688-416">`--computer-name` foi adicionado a `vm create` para configurar o nome do computador da VM</span><span class="sxs-lookup"><span data-stu-id="48688-416">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="48688-417">`--ssh-key-value` foi renomeado para `--ssh-key-values` para `[vm|vmss] create` – Agora, pode aceitar vários valores de chave pública ou caminhos ssh</span><span class="sxs-lookup"><span data-stu-id="48688-417">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="48688-418">__Observação__: Isso **não** é uma alteração da falha – `--ssh-key-value` será analisado corretamente, pois corresponde somente a `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="48688-418">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="48688-419">O argumento `--type` de `ppg create` foi alterado para ser opcional</span><span class="sxs-lookup"><span data-stu-id="48688-419">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="48688-420">6 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="48688-420">May 6, 2019</span></span>

<span data-ttu-id="48688-421">Versão 2.0.64</span><span class="sxs-lookup"><span data-stu-id="48688-421">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="48688-422">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-422">ACS</span></span>
* <span data-ttu-id="48688-423">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--fqdn` foi removido dos comandos `openshift`</span><span class="sxs-lookup"><span data-stu-id="48688-423">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="48688-424">Alterado para usar a versão da API do Red Hat OpenShift no Azure em disponibilidade geral</span><span class="sxs-lookup"><span data-stu-id="48688-424">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="48688-425">O sinalizador `customer-admin-group-id` foi adicionado a `openshift create`</span><span class="sxs-lookup"><span data-stu-id="48688-425">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="48688-426">[GA] `(PREVIEW)` foi removido da opção `aks create` `--network-policy`</span><span class="sxs-lookup"><span data-stu-id="48688-426">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-427">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-427">Appservice</span></span>
* <span data-ttu-id="48688-428">[PRETERIDO] O comando `functionapp devops-build` foi preterido</span><span class="sxs-lookup"><span data-stu-id="48688-428">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="48688-429">Renomeado para `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="48688-429">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="48688-430">Corrigido ao obter o nome de usuário correto para cloudshell que estava causando a falha em `webapp up`</span><span class="sxs-lookup"><span data-stu-id="48688-430">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="48688-431">Documentação `appservice plan --sku` atualizada para refletir o appserviceplans com suporte</span><span class="sxs-lookup"><span data-stu-id="48688-431">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="48688-432">Adicionado argumentos opcionais para o grupo de recursos e plano a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="48688-432">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="48688-433">Adicionado suporte a `webapp ssh` para respeitar a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="48688-433">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="48688-434">Adicionado suporte `appserviceplan create` para a SKU gratuita do Linux</span><span class="sxs-lookup"><span data-stu-id="48688-434">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="48688-435">Alterado `webapp up` para ter uma suspensão de 30 segundos depois de definir appsetting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` para lidar com a inicialização a frio kudu</span><span class="sxs-lookup"><span data-stu-id="48688-435">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="48688-436">Adicionado suporte para tempo de execução `powershell` a `functionapp create` no Windows</span><span class="sxs-lookup"><span data-stu-id="48688-436">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="48688-437">Adicionado o comando `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="48688-437">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="48688-438">Lote</span><span class="sxs-lookup"><span data-stu-id="48688-438">Batch</span></span>
* <span data-ttu-id="48688-439">Corrigido o bug no validador para as opções `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="48688-439">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="48688-440">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="48688-440">Botservice</span></span>
* <span data-ttu-id="48688-441">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para criar um Bot de Aplicativo Web vazio por padrão (ou seja, nenhum bot será implantado no Serviço de Aplicativo)</span><span class="sxs-lookup"><span data-stu-id="48688-441">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="48688-442">O sinalizador `--echo` foi adicionado ao `bot create` para usar o comportamento antigo com `-v v4`</span><span class="sxs-lookup"><span data-stu-id="48688-442">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="48688-443">[ALTERAÇÃO SIGNIFICATIVA] O valor padrão de `--version` foi alterado para `v4`</span><span class="sxs-lookup"><span data-stu-id="48688-443">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="48688-444">__OBSERVAÇÃO:__ `bot prepare-publish` ainda usa o padrão antigo</span><span class="sxs-lookup"><span data-stu-id="48688-444">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="48688-445">[ALTERAÇÃO SIGNIFICATIVA] `--lang` foi alterado para não definir mais `Csharp` como padrão.</span><span class="sxs-lookup"><span data-stu-id="48688-445">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="48688-446">Se o comando exigir `--lang` e ele não for fornecido, o comando será um erro</span><span class="sxs-lookup"><span data-stu-id="48688-446">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="48688-447">[ALTERAÇÃO SIGNIFICATIVA] Os argumentos `--appid` e `--password` foram alterados para `bot create` ser obrigatório e agora podem ser criados por meio de `ad app create`</span><span class="sxs-lookup"><span data-stu-id="48688-447">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="48688-448">Foi adicionada validação a `--appid` e `--password`</span><span class="sxs-lookup"><span data-stu-id="48688-448">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="48688-449">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4` foi alterado para não criar ou usar uma Conta de Armazenamento ou o Application Insights</span><span class="sxs-lookup"><span data-stu-id="48688-449">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="48688-450">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v3` foi alterado para exigir uma região em que o Application Insights está disponível</span><span class="sxs-lookup"><span data-stu-id="48688-450">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="48688-451">[ALTERAÇÃO SIGNIFICATIVA] O `bot update` foi alterado para afetar somente as propriedades específicas de um bot</span><span class="sxs-lookup"><span data-stu-id="48688-451">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="48688-452">[ALTERAÇÃO SIGNIFICATIVA] Os sinalizadores `--lang` foram alterados para aceitar `Javascript` em vez de `Node`</span><span class="sxs-lookup"><span data-stu-id="48688-452">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="48688-453">[ALTERAÇÃO SIGNIFICATIVA] O `Node` foi removido como um valor `--lang` permitido</span><span class="sxs-lookup"><span data-stu-id="48688-453">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="48688-454">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para não definir mais `SCM_DO_BUILD_DURING_DEPLOYMENT` como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="48688-454">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="48688-455">Todas as implantações por meio do Kudu atuarão de acordo com o comportamento padrão</span><span class="sxs-lookup"><span data-stu-id="48688-455">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="48688-456">O `bot download` foi alterado para os bots sem arquivos `.bot` para criar o arquivo de configuração específico a um idioma com os valores das Configurações de Aplicativo do bot</span><span class="sxs-lookup"><span data-stu-id="48688-456">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="48688-457">Adicionado o suporte `Typescript` para `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="48688-457">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="48688-458">Uma mensagem de aviso foi adicionada a `bot prepare-deploy` para os bots `Javascript` e `Typescript` para quando `--code-dir` não contiver `package.json`</span><span class="sxs-lookup"><span data-stu-id="48688-458">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="48688-459">O `bot prepare-deploy` foi alterado para retornar `true`, se bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="48688-459">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="48688-460">O log detalhado foi adicionado a `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="48688-460">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="48688-461">Mais regiões disponíveis do Application Insights foram adicionadas ao `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="48688-461">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="48688-462">Configurar</span><span class="sxs-lookup"><span data-stu-id="48688-462">Configure</span></span>
* <span data-ttu-id="48688-463">Adicionado suporte para configurações de valor padrão do argumento baseado em pasta</span><span class="sxs-lookup"><span data-stu-id="48688-463">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="48688-464">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="48688-464">Eventhubs</span></span>
* <span data-ttu-id="48688-465">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="48688-465">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="48688-466">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-466">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="48688-467">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-467">Network</span></span>
* <span data-ttu-id="48688-468">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--cache` foi substituído por `--defer` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-468">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="48688-469">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="48688-469">Policy Insights</span></span>
* <span data-ttu-id="48688-470">Suporte adicionado a `--expand PolicyEvaluationDetails` para detalhes de avaliação de política de consulta no recurso</span><span class="sxs-lookup"><span data-stu-id="48688-470">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="48688-471">Função</span><span class="sxs-lookup"><span data-stu-id="48688-471">Role</span></span>
* <span data-ttu-id="48688-472">[PRETERIDO] Alterado argumento ocultar '--password' `create-for-rbac` - suporte será removido em maio de 2019</span><span class="sxs-lookup"><span data-stu-id="48688-472">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="48688-473">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="48688-473">Service Bus</span></span>
* <span data-ttu-id="48688-474">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="48688-474">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="48688-475">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-475">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="48688-476">`topic [create|update]` foi fixado para permitir suporte a `--max-size` para valores de 10, 20, 40 e 80 GB com a SKU Premium</span><span class="sxs-lookup"><span data-stu-id="48688-476">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="48688-477">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-477">SQL</span></span>
* <span data-ttu-id="48688-478">Adicionados os comandos `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="48688-478">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="48688-479">VM</span><span class="sxs-lookup"><span data-stu-id="48688-479">VM</span></span>
* <span data-ttu-id="48688-480">O `--protect-from-scale-in` e o `--protect-from-scale-set-actions` foram adicionados a `vmss update` para habilitar atualizações à política de proteção das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="48688-480">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="48688-481">Adicionado a `--instance-id` e `vmss update` para habilitar atualização genérica das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="48688-481">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="48688-482">`--instance-id` foi adicionado a `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="48688-482">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="48688-483">Adicionado um novo grupo de comandos `ppg` para gerenciar grupos de posicionamento de proximidade</span><span class="sxs-lookup"><span data-stu-id="48688-483">Added new `ppg` command group for manging Proximity Placement Groups</span></span>
* <span data-ttu-id="48688-484">Adicionado a `--ppg`, `[vm|vmss] create` e `vm availability-set create` para gerenciar PPGs</span><span class="sxs-lookup"><span data-stu-id="48688-484">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="48688-485">Parâmetro `--hyper-v-generation` adicionado a `image create`</span><span class="sxs-lookup"><span data-stu-id="48688-485">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="48688-486">23 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="48688-486">April 23, 2019</span></span>

<span data-ttu-id="48688-487">Versão 2.0.63</span><span class="sxs-lookup"><span data-stu-id="48688-487">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="48688-488">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-488">ACS</span></span>
* <span data-ttu-id="48688-489">Alterado `aks get-credentials` para solicitar substituição dos valores duplicados</span><span class="sxs-lookup"><span data-stu-id="48688-489">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="48688-490">Removido `(PREVIEW)` dos comandos de espaços de desenvolvimento "aks use-dev-espaces" e "aks remove-dev-espaces"</span><span class="sxs-lookup"><span data-stu-id="48688-490">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="48688-491">AMS</span><span class="sxs-lookup"><span data-stu-id="48688-491">AMS</span></span>
* <span data-ttu-id="48688-492">Corrigido o bug com a atualização de filtros de conta e de ativo</span><span class="sxs-lookup"><span data-stu-id="48688-492">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-493">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-493">AppService</span></span>
* <span data-ttu-id="48688-494">Adicionado suporte para o ASE e o tempo limite para `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="48688-494">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="48688-495">Adicionado suporte para o estabelecimento de CI CD em um pipeline do Azure DevOps de um repositório do Github para aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="48688-495">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="48688-496">Adicionado argumento `--github-pat` a `functionapp devops-build create` para aceitar o token de acesso pessoal do Github</span><span class="sxs-lookup"><span data-stu-id="48688-496">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="48688-497">Adicionado argumento `--github-repository` a `functionapp devops-build create` para aceitar o repositório Github que contém um código-fonte functionapp</span><span class="sxs-lookup"><span data-stu-id="48688-497">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="48688-498">Problema corrigido em que `az webapp up --logs` estava falhando com um erro e atualização da versão .NETCORE padrão para 2.1</span><span class="sxs-lookup"><span data-stu-id="48688-498">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="48688-499">Configurações de functionapp desnecessárias removidas durante a criação de um aplicativo de funções com plano de consumo</span><span class="sxs-lookup"><span data-stu-id="48688-499">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="48688-500">Alterado `webapp up` para que a cadeia de caracteres padrão asp agora acrescente o número no final para criar um novo ASP com base nas opções de SKU</span><span class="sxs-lookup"><span data-stu-id="48688-500">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="48688-501">Adicionado `-b` como uma opção a `webapp up` para iniciar o aplicativo no navegador</span><span class="sxs-lookup"><span data-stu-id="48688-501">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="48688-502">Alterado `webapp deployment source config zip` para lidar com a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="48688-502">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="48688-503">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="48688-503">Deployment Manager</span></span>
* <span data-ttu-id="48688-504">[VERSÃO PRÉVIA] Criar e gerenciar artefatos que dão suporte a distribuições</span><span class="sxs-lookup"><span data-stu-id="48688-504">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="48688-505">Laboratório</span><span class="sxs-lookup"><span data-stu-id="48688-505">Lab</span></span>
* <span data-ttu-id="48688-506">Corrigido o bug que causa uma saída inicial</span><span class="sxs-lookup"><span data-stu-id="48688-506">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="48688-507">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-507">Network</span></span>
* <span data-ttu-id="48688-508">Adicionada delegação de servidor de nome automática a `dns zone create` no pai durante a criação da zona filho</span><span class="sxs-lookup"><span data-stu-id="48688-508">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="48688-509">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-509">Resource</span></span>
* <span data-ttu-id="48688-510">[PRETERIDO] Argumentos `--link-id`, `--target-id` e `--filter-string` preteridos de `resource link`</span><span class="sxs-lookup"><span data-stu-id="48688-510">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="48688-511">Use os argumentos `--link`, `--target` e `--filter`</span><span class="sxs-lookup"><span data-stu-id="48688-511">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="48688-512">Corrigido o problema em que os comandos `resource link [create|update]` não funcionavam</span><span class="sxs-lookup"><span data-stu-id="48688-512">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="48688-513">Corrigido um problema em que a exclusão usando uma ID de recurso poderia causar falha no erro</span><span class="sxs-lookup"><span data-stu-id="48688-513">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="48688-514">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-514">SQL</span></span>
* <span data-ttu-id="48688-515">Adicionado suporte para fuso horário personalizado nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="48688-515">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="48688-516">Alterado para permitir que o nome do pool Elástico seja usado com `sql db update`</span><span class="sxs-lookup"><span data-stu-id="48688-516">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="48688-517">Adicionado o suporte `--no-wait` para `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-517">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="48688-518">Adicionado o comando `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="48688-518">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="48688-519">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-519">Storage</span></span>
* <span data-ttu-id="48688-520">Corrigido o problema com tokens SAS com codificação dupla em `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="48688-520">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="48688-521">VM</span><span class="sxs-lookup"><span data-stu-id="48688-521">VM</span></span>
* <span data-ttu-id="48688-522">Adicionado sinalizador `--skip-shutdown` a `vm|vmss stop` para desligar as VMs sem o desligamento</span><span class="sxs-lookup"><span data-stu-id="48688-522">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="48688-523">Adicionado argumento `--storage-account-type` a `sig image-version create` para definir o tipo de conta do perfil de publicação</span><span class="sxs-lookup"><span data-stu-id="48688-523">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="48688-524">Adicionado argumento `--target-regions` a `sig image-version create` para permitir definir os tipos de conta de armazenamento específico da região</span><span class="sxs-lookup"><span data-stu-id="48688-524">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="48688-525">9 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="48688-525">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="48688-526">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-526">Core</span></span>
* <span data-ttu-id="48688-527">Correção do problema em que algumas extensões mostraram uma versão do `Unknown` e não podiam ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="48688-527">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="48688-528">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-528">ACR</span></span>
* <span data-ttu-id="48688-529">Adição de suporte para execução de uma imagem sem contexto</span><span class="sxs-lookup"><span data-stu-id="48688-529">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="48688-530">AMS</span><span class="sxs-lookup"><span data-stu-id="48688-530">AMS</span></span>
* [PRETERIDO]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [ALTERAÇÃO SIGNIFICATIVA]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="48688-533">Adição de suporte para novos parâmetros de criptografia em `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="48688-533">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="48688-534">Adição de novo parâmetro `--filters` a `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="48688-534">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-535">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-535">AppService</span></span>
* <span data-ttu-id="48688-536">Adicionado o suporte `--logs` para `webapp up`</span><span class="sxs-lookup"><span data-stu-id="48688-536">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="48688-537">Correção de problemas do comando `functionapp devops-build create` de geração de `azure-pipelines.yml`</span><span class="sxs-lookup"><span data-stu-id="48688-537">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="48688-538">Melhoria do tratamento de erros e indicadores `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="48688-538">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="48688-539">[ALTERAÇÃO SIGNIFICATIVA] Remoção do sinalizador `--local-git` para o comando `devops-build`; a detecção de git local e a manipulação são obrigatórias para a criação de pipelines do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="48688-539">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="48688-540">Adição de suporte para a criação de planos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="48688-540">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="48688-541">Adição da capacidade de trocar um plano sob um aplicativo de funções usando `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="48688-541">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="48688-542">Adição de suporte para configurações de expansão de plano Premium do Azure Functions</span><span class="sxs-lookup"><span data-stu-id="48688-542">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="48688-543">CDN</span><span class="sxs-lookup"><span data-stu-id="48688-543">CDN</span></span>
* <span data-ttu-id="48688-544">Adição de suporte para `Microsoft_Standard` e `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="48688-544">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="48688-545">Comentários</span><span class="sxs-lookup"><span data-stu-id="48688-545">Feedback</span></span>
* <span data-ttu-id="48688-546">Alteração de `feedback` para mostrar metadados em comandos executados recentemente</span><span class="sxs-lookup"><span data-stu-id="48688-546">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="48688-547">Alteração de `feedback` para solicitar o auxílio do usuário no processo de criação de problema abrindo um navegador e usando um modelo de problema</span><span class="sxs-lookup"><span data-stu-id="48688-547">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="48688-548">Alteração do `feedback` para imprimir o corpo do problema ao executar com '--verbose'</span><span class="sxs-lookup"><span data-stu-id="48688-548">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="48688-549">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48688-549">Monitor</span></span>
* <span data-ttu-id="48688-550">Correção de um problema em que “count” não era um valor permitido com `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-550">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="48688-551">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-551">Network</span></span>
* <span data-ttu-id="48688-552">Correção do formato de tabela que não estava sendo exibido com `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="48688-552">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="48688-553">Adição dos comandos `list-request-headers` e `list-response-headers` para `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="48688-553">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="48688-554">Adição do comando `list-server-variables` para `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="48688-554">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="48688-555">Correção de um problema em que a atualização do estado do link em uma porta express-route geraria uma exceção de atributo desconhecido `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="48688-555">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="48688-556">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="48688-556">PrivateDNS</span></span>
* <span data-ttu-id="48688-557">Adição de `network private-dns` para zonas de DNS privado</span><span class="sxs-lookup"><span data-stu-id="48688-557">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="48688-558">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-558">Resource</span></span>
* <span data-ttu-id="48688-559">Correção do problema com `deployment create` e `group deployment create`, em que um arquivo de parâmetros com um conjunto vazio de parâmetros não funcionaria</span><span class="sxs-lookup"><span data-stu-id="48688-559">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="48688-560">Função</span><span class="sxs-lookup"><span data-stu-id="48688-560">Role</span></span>
* <span data-ttu-id="48688-561">Correção de `create-for-rbac` para lidar corretamente com `--years`</span><span class="sxs-lookup"><span data-stu-id="48688-561">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="48688-562">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `role assignment delete` para solicitar ao excluir todas as atribuições na assinatura incondicionalmente</span><span class="sxs-lookup"><span data-stu-id="48688-562">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="48688-563">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-563">SQL</span></span>
* <span data-ttu-id="48688-564">Atualização de `sql mi [create|update]` com as propriedades proxyOverride e publicDataEndpointEnabled</span><span class="sxs-lookup"><span data-stu-id="48688-564">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="48688-565">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-565">Storage</span></span>
* <span data-ttu-id="48688-566">[ALTERAÇÃO SIGNIFICATIVA] Remoção do resultado de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="48688-566">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="48688-567">Adição de `--full-uri` a `storage blob generate-sas` para criar o URI completo para o blob com SAS</span><span class="sxs-lookup"><span data-stu-id="48688-567">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="48688-568">Adição de `--file-snapshot` a `storage file copy start` para copiar arquivo do instantâneo</span><span class="sxs-lookup"><span data-stu-id="48688-568">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="48688-569">Alteração de `storage blob copy cancel` para mostrar apenas o erro em vez da exceção para NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="48688-569">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="48688-570">26 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="48688-570">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="48688-571">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-571">Core</span></span>
* <span data-ttu-id="48688-572">Correção de problemas com incompatibilidade da extensão de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="48688-572">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="48688-573">Agora o tratamento de erros encaminha os clientes para a página de problemas</span><span class="sxs-lookup"><span data-stu-id="48688-573">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="48688-574">Nuvem</span><span class="sxs-lookup"><span data-stu-id="48688-574">Cloud</span></span>
* <span data-ttu-id="48688-575">Erro de “assinatura não encontrada” corrigido em `cloud set`</span><span class="sxs-lookup"><span data-stu-id="48688-575">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="48688-576">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-576">ACR</span></span>
* <span data-ttu-id="48688-577">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="48688-577">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="48688-578">`--auth-mode` adicionado aos comandos `acr build`, `acr run`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="48688-578">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="48688-579">Grupo de comandos “acr task credential” adicionado para gerenciar as credenciais de uma Tarefa</span><span class="sxs-lookup"><span data-stu-id="48688-579">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="48688-580">“--no-wait” adicionado ao comando `acr build`</span><span class="sxs-lookup"><span data-stu-id="48688-580">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-581">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-581">AppService</span></span>
* <span data-ttu-id="48688-582">Bug corrigido onde `webapp up` não estava lidando corretamente com a execução do diretório vazio ou do cenário de código desconhecido</span><span class="sxs-lookup"><span data-stu-id="48688-582">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="48688-583">Bug corrigido onde os slots não funcionavam para `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="48688-583">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="48688-584">Serviço de BOT</span><span class="sxs-lookup"><span data-stu-id="48688-584">BOT Service</span></span>
* <span data-ttu-id="48688-585">`bot prepare-deploy` adicionado para se preparar para a implantação de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="48688-585">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="48688-586">`bot create --kind registration` alterado para mostrar a senha se ela não for fornecida</span><span class="sxs-lookup"><span data-stu-id="48688-586">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="48688-587">[ALTERAÇÃO SIGNIFICATIVA] `--endpoint` alterado em `bot create --kind registration` como padrão para uma cadeia de caracteres vazia, em vez de ser requerido</span><span class="sxs-lookup"><span data-stu-id="48688-587">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="48688-588">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="48688-588">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="48688-589">CDN</span><span class="sxs-lookup"><span data-stu-id="48688-589">CDN</span></span>
* <span data-ttu-id="48688-590">Adicionado o suporte ao `--no-wait` para `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="48688-590">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [ALTERAÇÃO SIGNIFICATIVA]: `cdn endpoint create` alterado para o comportamento de cache da cadeia de consulta padrão.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="48688-592">Não há mais padrão para "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="48688-592">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="48688-593">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="48688-593">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48688-594">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="48688-594">Cosmosdb</span></span>
* <span data-ttu-id="48688-595">Suporte adicionado para `--enable-multiple-write-locations` na atualização da conta</span><span class="sxs-lookup"><span data-stu-id="48688-595">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="48688-596">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="48688-596">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="48688-597">Interativo</span><span class="sxs-lookup"><span data-stu-id="48688-597">Interactive</span></span>
* <span data-ttu-id="48688-598">Incompatibilidade corrigida com a extensão Interativa instalada por meio do azdev</span><span class="sxs-lookup"><span data-stu-id="48688-598">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="48688-599">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48688-599">Monitor</span></span>
* <span data-ttu-id="48688-600">Alterado para permitir o valor de dimensão `*` para `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-600">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="48688-601">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-601">Network</span></span>
* <span data-ttu-id="48688-602">Grupo de comandos `rewrite-rule` adicionado em `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="48688-602">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="48688-603">Perfil</span><span class="sxs-lookup"><span data-stu-id="48688-603">Profile</span></span>
* <span data-ttu-id="48688-604">Suporte de conta no nível do locatário para a identidade de serviço gerenciado adicionado em `login`</span><span class="sxs-lookup"><span data-stu-id="48688-604">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="48688-605">Postgres</span><span class="sxs-lookup"><span data-stu-id="48688-605">Postgres</span></span> 
* <span data-ttu-id="48688-606">Adicionados os comandos postgresql `replica` e `restart server`</span><span class="sxs-lookup"><span data-stu-id="48688-606">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="48688-607">Alterado para obter o local padrão do grupo de recursos quando não fornecido para criar servidores e adicionar validação para os dias de retenção</span><span class="sxs-lookup"><span data-stu-id="48688-607">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="48688-608">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-608">Resource</span></span>
* <span data-ttu-id="48688-609">Saída da tabela aperfeiçoada para `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="48688-609">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="48688-610">Corrigido o problema com `deployment [create|validate]` onde o tipo secureObject não era reconhecido</span><span class="sxs-lookup"><span data-stu-id="48688-610">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="48688-611">Grafo</span><span class="sxs-lookup"><span data-stu-id="48688-611">Graph</span></span>
* <span data-ttu-id="48688-612">Adicionado o suporte ao `--end-date` para `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="48688-612">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="48688-613">Suporte adicionado para acrescentar permissões com `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="48688-613">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="48688-614">Bug corrigido com `ad app permission list` quando não havia nenhuma permissão</span><span class="sxs-lookup"><span data-stu-id="48688-614">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="48688-615">`ad sp delete` alterado para ignorar a exclusão da atribuição de função se a conta atual não tem nenhuma assinatura</span><span class="sxs-lookup"><span data-stu-id="48688-615">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="48688-616">`ad app create` alterado para `--identifier-uris` passar para lista vazia como padrão se não fornecido</span><span class="sxs-lookup"><span data-stu-id="48688-616">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="48688-617">storage</span><span class="sxs-lookup"><span data-stu-id="48688-617">storage</span></span>
* <span data-ttu-id="48688-618">`--snapshot` adicionado a `storage file download-batch` para baixar de um instantâneo de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="48688-618">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="48688-619">Barra de progresso `storage blob [download-batch|upload-batch]` alterada para ser menos detalhada e indicar o blob atual</span><span class="sxs-lookup"><span data-stu-id="48688-619">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="48688-620">Problema corrigido com `storage account update` ao atualizar os parâmetros de criptografia</span><span class="sxs-lookup"><span data-stu-id="48688-620">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="48688-621">Problema corrigido onde `storage blob show` falharia ao usar o oauth (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="48688-621">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="48688-622">VM</span><span class="sxs-lookup"><span data-stu-id="48688-622">VM</span></span>
* <span data-ttu-id="48688-623">Adicionado o comando `image update`</span><span class="sxs-lookup"><span data-stu-id="48688-623">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="48688-624">12 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="48688-624">March 12, 2019</span></span>

<span data-ttu-id="48688-625">Versão 2.0.60</span><span class="sxs-lookup"><span data-stu-id="48688-625">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="48688-626">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-626">Core</span></span>

* <span data-ttu-id="48688-627">Foi corrigido um erro incorreto no `cloud set` sobre assinatura não encontrada.</span><span class="sxs-lookup"><span data-stu-id="48688-627">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="48688-628">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-628">ACR</span></span>

* <span data-ttu-id="48688-629">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="48688-629">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="48688-630">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-630">ACS</span></span>

* <span data-ttu-id="48688-631">Alteração para ignorar o parâmetro `--listen-address` para `aks browse` se ele não for compatível com kubectl</span><span class="sxs-lookup"><span data-stu-id="48688-631">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="48688-632">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-632">AppService</span></span>

* <span data-ttu-id="48688-633">Adicionado `[webapp|functionapp] deployment list-publishing-credentials` para obter a URL de publicação do Kudu e suas credenciais.</span><span class="sxs-lookup"><span data-stu-id="48688-633">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="48688-634">Removida a instrução de impressão errônea de `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="48688-634">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="48688-635">Corrigido `functionapp` para definir a imagem correta do tempo de execução nos planos do Serviço de Aplicativo no Linux.</span><span class="sxs-lookup"><span data-stu-id="48688-635">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="48688-636">Removida a marca de versão prévia do `webapp up` e adicionadas melhorias ao comando.</span><span class="sxs-lookup"><span data-stu-id="48688-636">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="48688-637">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="48688-637">Botservice</span></span>

* <span data-ttu-id="48688-638">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="48688-638">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="48688-639">Adicionados `Microsoft-BotFramework-AppId` e `Microsoft-BotFramework-AppPassword` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="48688-639">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="48688-640">Removidas as aspas simples da saída de comando `bot publish`, no final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="48688-640">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="48688-641">Alterado `bot publish` para que seja assíncrono.</span><span class="sxs-lookup"><span data-stu-id="48688-641">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="48688-642">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-642">Container</span></span>

* <span data-ttu-id="48688-643">Adicionado o argumento `--no-wait` para `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="48688-643">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="48688-644">EventHub</span><span class="sxs-lookup"><span data-stu-id="48688-644">EventHub</span></span>

* <span data-ttu-id="48688-645">Adicionado o sinalizador `--skip-empty-archives` a `eventhub create|update` para dar suporte a arquivos vazios na captura.</span><span class="sxs-lookup"><span data-stu-id="48688-645">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="48688-646">Localizar</span><span class="sxs-lookup"><span data-stu-id="48688-646">Find</span></span>

* <span data-ttu-id="48688-647">Atualização de funcionalidade principal</span><span class="sxs-lookup"><span data-stu-id="48688-647">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="48688-648">HDInsight</span><span class="sxs-lookup"><span data-stu-id="48688-648">HDInsight</span></span>

* <span data-ttu-id="48688-649">Adicionado o parâmetro `--storage-account-managed-identity` a `hdinsight create` para oferecer suporte ao MSI do ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="48688-649">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="48688-650">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-650">Network</span></span>

* <span data-ttu-id="48688-651">Corrigido o problema com `vpn-connection update`, onde a atualização de uma conexão VPN entre gateways em assinaturas diferentes falharia.</span><span class="sxs-lookup"><span data-stu-id="48688-651">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="48688-652">Rdbms</span><span class="sxs-lookup"><span data-stu-id="48688-652">Rdbms</span></span>

* <span data-ttu-id="48688-653">Correções secundárias para obter a localização padrão do grupo de recursos, quando não fornecida, para criar servidores e adicionar validação nos dias de retenção.</span><span class="sxs-lookup"><span data-stu-id="48688-653">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="48688-654">Função</span><span class="sxs-lookup"><span data-stu-id="48688-654">Role</span></span>

* <span data-ttu-id="48688-655">Corrigido `role definition update` para usar ID a fim de resolver a definição corretamente.</span><span class="sxs-lookup"><span data-stu-id="48688-655">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="48688-656">Alterado `ad app credential reset` para remover a suposição de que a entidade de serviço do aplicativo já existe.</span><span class="sxs-lookup"><span data-stu-id="48688-656">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="48688-657">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="48688-657">Service Fabric</span></span>

* <span data-ttu-id="48688-658">Corrigido o problema com o fato de `sf cluster list` não ser iterável.</span><span class="sxs-lookup"><span data-stu-id="48688-658">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="48688-659">26 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="48688-659">February 26, 2019</span></span>

<span data-ttu-id="48688-660">Versão 2.0.59</span><span class="sxs-lookup"><span data-stu-id="48688-660">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="48688-661">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-661">Core</span></span>

* <span data-ttu-id="48688-662">Corrigido o problema onde algumas instâncias usando `--subscription NAME` produziriam uma exceção</span><span class="sxs-lookup"><span data-stu-id="48688-662">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="48688-663">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-663">ACR</span></span>

* <span data-ttu-id="48688-664">Parâmetro `--target` adicionado para os comandos `acr build`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="48688-664">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="48688-665">Melhor tratamento de erros para os comandos de execução quando não conectado ao Azure</span><span class="sxs-lookup"><span data-stu-id="48688-665">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="48688-666">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-666">ACS</span></span>

* <span data-ttu-id="48688-667">Opção `--listen-address` adicionada a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="48688-667">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-668">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-668">AppService</span></span>

* <span data-ttu-id="48688-669">Adicionado o comando `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="48688-669">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="48688-670">Lote</span><span class="sxs-lookup"><span data-stu-id="48688-670">Batch</span></span>
* <span data-ttu-id="48688-671">[ALTERAÇÃO SIGNIFICATIVA] Comando `batch pool upgrade os` removido</span><span class="sxs-lookup"><span data-stu-id="48688-671">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="48688-672">[ALTERAÇÃO SIGNIFICATIVA] Propriedade `Pacakges` removida das respostas `Application`</span><span class="sxs-lookup"><span data-stu-id="48688-672">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="48688-673">Comando `batch application package list` adicionado para listar os pacotes de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="48688-673">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="48688-674">[ALTERAÇÃO SIGNIFICATIVA] `--application-id` alterado para `--application-name` em todos os comandos `batch application`,</span><span class="sxs-lookup"><span data-stu-id="48688-674">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="48688-675">O argumento `--json-file` foi adicionado aos comandos para a solicitação de resposta da API bruta</span><span class="sxs-lookup"><span data-stu-id="48688-675">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="48688-676">Validação atualizada para incluir automaticamente `https://` em todos os pontos de extremidade, se ausente</span><span class="sxs-lookup"><span data-stu-id="48688-676">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48688-677">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48688-677">CosmosDB</span></span>

* <span data-ttu-id="48688-678">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="48688-678">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="48688-679">Kusto</span><span class="sxs-lookup"><span data-stu-id="48688-679">Kusto</span></span>

* <span data-ttu-id="48688-680">[ALTERAÇÃO SIGNIFICATIVA] Os tipos `hot_cache_period` e `soft_delete_period` foram alterados do banco de dados para o formato de duração ISO8601</span><span class="sxs-lookup"><span data-stu-id="48688-680">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="48688-681">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-681">Network</span></span>

* <span data-ttu-id="48688-682">Adicionado o argumento `--express-route-gateway-bypass` para `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-682">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="48688-683">Foram adicionados os grupos de comando a partir das extensões `express-route`</span><span class="sxs-lookup"><span data-stu-id="48688-683">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="48688-684">Os grupos de comando `express-route gateway` e `express-route port` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="48688-684">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="48688-685">Adicionado o argumento `--legacy-mode` para `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-685">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="48688-686">Os argumentos `--allow-classic-operations` e `--express-route-port` foram adicionados a `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-686">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="48688-687">Adicionado o argumento `--gateway-default-site` para `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-687">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="48688-688">Os comandos `ipsec-policy` foram adicionados a `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="48688-688">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="48688-689">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-689">Resource</span></span>

* <span data-ttu-id="48688-690">Foi corrigido o problema com `deployment create` em que o campo do tipo diferencia letras maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="48688-690">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="48688-691">Foi adicionado o suporte para arquivo de parâmetros de URI a `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="48688-691">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="48688-692">Foi adicionado o suporte para parâmetros de URI e definições a `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="48688-692">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="48688-693">Foi corrigido o tratamento de parâmetros e regras para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="48688-693">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="48688-694">Foi corrigido o problema com `resource show/update/delete/tag/invoke-action` em que as IDs de assinatura cruzada não respeitaram corretamente a ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="48688-694">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="48688-695">Função</span><span class="sxs-lookup"><span data-stu-id="48688-695">Role</span></span>

* <span data-ttu-id="48688-696">Foi adicionado o suporte para as funções do aplicativo a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-696">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="48688-697">VM</span><span class="sxs-lookup"><span data-stu-id="48688-697">VM</span></span>

* <span data-ttu-id="48688-698">Foi corrigido o problema com `vm create where ` – a rede acelerada não foi habilitada por padrão no Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="48688-698">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="48688-699">12 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="48688-699">February 12, 2019</span></span>

<span data-ttu-id="48688-700">Versão 2.0.58</span><span class="sxs-lookup"><span data-stu-id="48688-700">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="48688-701">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-701">Core</span></span>

* <span data-ttu-id="48688-702">`az --version` agora exibe uma notificação se você tiver pacotes para atualização</span><span class="sxs-lookup"><span data-stu-id="48688-702">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="48688-703">A regressão em que `--ids` não pode ser usado com a saída JSON foi corrigida</span><span class="sxs-lookup"><span data-stu-id="48688-703">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="48688-704">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-704">ACR</span></span>
* <span data-ttu-id="48688-705">[ALTERAÇÃO SIGNIFICATIVA] O grupo de comandos `acr build-task` foi removido</span><span class="sxs-lookup"><span data-stu-id="48688-705">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="48688-706">[ALTERAÇÃO SIGNIFICATIVA] As opções `--tag` e `--manifest` de `acr repository delete` foram removidas</span><span class="sxs-lookup"><span data-stu-id="48688-706">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="48688-707">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-707">ACS</span></span>
* <span data-ttu-id="48688-708">Suporte adicionado a `aks [enable-addons|disable-addons]` para nomes que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="48688-708">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="48688-709">Suporte adicionado para a operação de atualização do Azure Active Directory usando `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="48688-709">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="48688-710">Um esclarecimento informando que `--output` é ignorado para `aks get-credentials` foi adicionado</span><span class="sxs-lookup"><span data-stu-id="48688-710">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="48688-711">AMS</span><span class="sxs-lookup"><span data-stu-id="48688-711">AMS</span></span>
* <span data-ttu-id="48688-712">Adicionados os comandos `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="48688-712">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="48688-713">Adicionados os comandos `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="48688-713">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-714">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-714">Appservice</span></span>
* <span data-ttu-id="48688-715">Foi adicionada a capacidade de criar e configurar funções usando contêineres de ACR</span><span class="sxs-lookup"><span data-stu-id="48688-715">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="48688-716">Suporte adicionado para a atualização das configurações de aplicativos Web por meio de JSON</span><span class="sxs-lookup"><span data-stu-id="48688-716">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="48688-717">A ajuda foi aprimorada para `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="48688-717">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="48688-718">Suporte adicionado para o App Insights para auxiliar na criação de aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="48688-718">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="48688-719">Os problemas com o SSH do aplicativo Web foram corrigidos</span><span class="sxs-lookup"><span data-stu-id="48688-719">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="48688-720">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="48688-720">Botservice</span></span>
* <span data-ttu-id="48688-721">A experiência do usuário para `bot publish` foi aprimorada</span><span class="sxs-lookup"><span data-stu-id="48688-721">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="48688-722">Foram adicionados avisos de tempos limite ao executar `npm install` durante `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="48688-722">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="48688-723">O caractere inválido `.` de `--name` em `az bot create` foi removido</span><span class="sxs-lookup"><span data-stu-id="48688-723">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="48688-724">Alteração para interromper a geração aleatória de nomes de recursos durante a criação do Armazenamento do Azure, Plano do Serviço de Aplicativo, Aplicativo Web/de funções e Application Insights</span><span class="sxs-lookup"><span data-stu-id="48688-724">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="48688-725">[PRETERIDO] O argumento `--proj-name` foi preterido em favor de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="48688-725">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="48688-726">`az bot publish` foi alterado para remover arquivos de implantação do Node.js do IIS buscados, caso eles já não existissem</span><span class="sxs-lookup"><span data-stu-id="48688-726">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="48688-727">Foi adicionado o argumento `--keep-node-modules` para `az bot publish` para não excluir a pasta `node_modules` no Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48688-727">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="48688-728">O par chave-valor `"publishCommand"` foi adicionado à saída de `az bot create` durante a criação de uma função do Azure ou bot de aplicativo Web</span><span class="sxs-lookup"><span data-stu-id="48688-728">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="48688-729">O valor de `"publishCommand"` é um comando `az bot publish` que é automaticamente preenchido com os parâmetros necessários para publicar o bot recém-criado</span><span class="sxs-lookup"><span data-stu-id="48688-729">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="48688-730">O `"WEBSITE_NODE_DEFAULT_VERSION"` foi atualizado no modelo do ARM para que os bots de SDK v4 usem 10.14.1 em vez de 8.9.4</span><span class="sxs-lookup"><span data-stu-id="48688-730">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="48688-731">Key Vault</span><span class="sxs-lookup"><span data-stu-id="48688-731">Key Vault</span></span>
* <span data-ttu-id="48688-732">Foi corrigido o problema com `keyvault secret backup`, em que alguns usuários recebiam um erro `unexpected_keyword` ao usar `--id`</span><span class="sxs-lookup"><span data-stu-id="48688-732">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="48688-733">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48688-733">Monitor</span></span>
* <span data-ttu-id="48688-734">`monitor metrics alert [create|update]` foi alterado para permitir o valor dimensional `*`</span><span class="sxs-lookup"><span data-stu-id="48688-734">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="48688-735">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-735">Network</span></span>
* <span data-ttu-id="48688-736">`dns zone export` foi alterado para garantir que CNAMEs exportados fossem FQDNs</span><span class="sxs-lookup"><span data-stu-id="48688-736">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="48688-737">O parâmetro `--gateway-name` foi adicionado a `nic ip-config address-pool [add|remove]` para dar suporte a pools de endereços de back-end de gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="48688-737">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="48688-738">Os argumentos `--traffic-analytics` e `--workspace` foram adicionados a `network watcher flow-log configure` para dar suporte à análise de tráfego por meio de um espaço de trabalho do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="48688-738">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="48688-739">`--idle-timeout` e `--floating-ip` foram adicionados a `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-739">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="48688-740">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="48688-740">Policy Insights</span></span>
* <span data-ttu-id="48688-741">Os comandos `policy remediation` foram adicionados para dar suporte a recursos de correção de política de recursos</span><span class="sxs-lookup"><span data-stu-id="48688-741">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="48688-742">RDBMS</span><span class="sxs-lookup"><span data-stu-id="48688-742">RDBMS</span></span>
* <span data-ttu-id="48688-743">A mensagem e os parâmetros de comando de ajuda foram aprimorados</span><span class="sxs-lookup"><span data-stu-id="48688-743">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="48688-744">Redis</span><span class="sxs-lookup"><span data-stu-id="48688-744">Redis</span></span>
* <span data-ttu-id="48688-745">Foram adicionados comandos para gerenciar regras de firewall (criar, atualizar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="48688-745">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="48688-746">Foram adicionados comandos para gerenciar links do servidor (criar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="48688-746">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="48688-747">Foram adicionados comandos para gerenciar o agendamento de patches (criar, atualizar, excluir, mostrar)</span><span class="sxs-lookup"><span data-stu-id="48688-747">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="48688-748">Suporte adicionado para Zonas de Disponibilidade e versão mínima de TLS para criar Redis</span><span class="sxs-lookup"><span data-stu-id="48688-748">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="48688-749">[ALTERAÇÃO SIGNIFICATIVA] Os comandos `redis update-settings` e `redis list-all` foram removidos</span><span class="sxs-lookup"><span data-stu-id="48688-749">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="48688-750">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro para `redis create`: “configurações de locatário” não é aceito no formato chave[=valor]</span><span class="sxs-lookup"><span data-stu-id="48688-750">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="48688-751">[PRETERIDO] Uma mensagem de aviso foi adicionada para preterir o comando `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="48688-751">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="48688-752">Função</span><span class="sxs-lookup"><span data-stu-id="48688-752">Role</span></span>
* <span data-ttu-id="48688-753">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido dos comandos `vm` para esta localização</span><span class="sxs-lookup"><span data-stu-id="48688-753">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="48688-754">SQL VM</span><span class="sxs-lookup"><span data-stu-id="48688-754">SQL VM</span></span>
* <span data-ttu-id="48688-755">[PRETERIDO] O argumento `--boostrap-acc-pwd` foi preterido devido a um erro de digitação</span><span class="sxs-lookup"><span data-stu-id="48688-755">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="48688-756">VM</span><span class="sxs-lookup"><span data-stu-id="48688-756">VM</span></span>
* <span data-ttu-id="48688-757">`vm list-skus` foi alterado para permitir o uso de `--all` no lugar de `--all true`</span><span class="sxs-lookup"><span data-stu-id="48688-757">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="48688-758">Adicionado `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="48688-758">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="48688-759">Foi corrigido o bug em que `vmss encryption enable` falhava se fosse executado anteriormente</span><span class="sxs-lookup"><span data-stu-id="48688-759">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="48688-760">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido para os comandos `role`</span><span class="sxs-lookup"><span data-stu-id="48688-760">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="48688-761">31 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="48688-761">January 31, 2019</span></span>

<span data-ttu-id="48688-762">Versão 2.0.57</span><span class="sxs-lookup"><span data-stu-id="48688-762">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="48688-763">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-763">Core</span></span>

* <span data-ttu-id="48688-764">Hotfix para o [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="48688-764">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="48688-765">28 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="48688-765">January 28, 2019</span></span>

<span data-ttu-id="48688-766">Versão 2.0.56</span><span class="sxs-lookup"><span data-stu-id="48688-766">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="48688-767">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-767">ACR</span></span>
* <span data-ttu-id="48688-768">Suporte adicionado para regras de rede virtual/IP</span><span class="sxs-lookup"><span data-stu-id="48688-768">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="48688-769">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-769">ACS</span></span>
* <span data-ttu-id="48688-770">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="48688-770">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="48688-771">Comandos do OpenShift gerenciado foram adicionados</span><span class="sxs-lookup"><span data-stu-id="48688-771">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="48688-772">Suporte adicionado para operações de atualização da entidade de serviço com `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="48688-772">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="48688-773">AMS</span><span class="sxs-lookup"><span data-stu-id="48688-773">AMS</span></span>
* <span data-ttu-id="48688-774">[ALTERAÇÃO SIGNIFICATIVA] `ams asset get-streaming-locators` renomeado para `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="48688-774">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="48688-775">[ALTERAÇÃO SIGNIFICATIVA] `ams streaming-locator get-content-keys` renomeado para `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="48688-775">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-776">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-776">Appservice</span></span>
* <span data-ttu-id="48688-777">Suporte adicionado para o App Insights no `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="48688-777">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="48688-778">Suporte adicionado para a criação do plano de serviço de aplicativo (incluindo Elástico Premium) para Aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="48688-778">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="48688-779">Foram corrigidos os problemas com de configuração de aplicativo com os planos Elástico Premium</span><span class="sxs-lookup"><span data-stu-id="48688-779">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="48688-780">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-780">Container</span></span>
* <span data-ttu-id="48688-781">Adicionado o comando `container start`</span><span class="sxs-lookup"><span data-stu-id="48688-781">Added `container start` command</span></span>
* <span data-ttu-id="48688-782">Alteração para permitir o uso de valores decimais para CPU durante a criação do contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-782">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="48688-783">EventGrid</span><span class="sxs-lookup"><span data-stu-id="48688-783">EventGrid</span></span>
* <span data-ttu-id="48688-784">Parâmetro `--deadletter-endpoint` adicionado a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-784">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="48688-785">Storagequeue e hybridconnection foram adicionados como novos valores para 'event-subscription [create|update] --endpoint-type\`</span><span class="sxs-lookup"><span data-stu-id="48688-785">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="48688-786">Os parâmetros `--max-delivery-attempts` e `--event-ttl` foram adicionados a `event-subscription create` para especificar a política de repetição para eventos</span><span class="sxs-lookup"><span data-stu-id="48688-786">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="48688-787">Uma mensagem de aviso foi adicionada a `event-subscription [create|update]` quando o webhook como destino for usado para uma assinatura de evento</span><span class="sxs-lookup"><span data-stu-id="48688-787">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="48688-788">O parâmetro source-resource-id foi adicionado para todos os comandos relacionados a eventos e marcar todos os outros parâmetros relacionados ao recurso de origem como preteridos</span><span class="sxs-lookup"><span data-stu-id="48688-788">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="48688-789">HDInsight</span><span class="sxs-lookup"><span data-stu-id="48688-789">HDInsight</span></span>
* <span data-ttu-id="48688-790">[ALTERAÇÃO SIGNIFICATIVA] Os parâmetros `--virtual-network` e `--subnet-name` de `hdinsight [application] create` foram removidos</span><span class="sxs-lookup"><span data-stu-id="48688-790">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="48688-791">[ALTERAÇÃO SIGNIFICATIVA] `hdinsight create --storage-account` foi alterado para aceitar o nome ou ID da conta de armazenamento, em vez de pontos de extremidade de blob</span><span class="sxs-lookup"><span data-stu-id="48688-791">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="48688-792">Parâmetros `--vnet-name` e `--subnet-name` adicionados a `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="48688-792">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="48688-793">Suporte adicionado para a criptografia de disco e Enterprise Security Package ao `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="48688-793">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="48688-794">Adicionado o comando `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="48688-794">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="48688-795">Adicionado o comando `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="48688-795">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="48688-796">IoT</span><span class="sxs-lookup"><span data-stu-id="48688-796">IoT</span></span>
* <span data-ttu-id="48688-797">O formato de codificação foi adicionado ao comando routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="48688-797">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="48688-798">Kusto</span><span class="sxs-lookup"><span data-stu-id="48688-798">Kusto</span></span>
* <span data-ttu-id="48688-799">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="48688-799">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="48688-800">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48688-800">Monitor</span></span>
* <span data-ttu-id="48688-801">A comparação de ID foi alterada para diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="48688-801">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="48688-802">Perfil</span><span class="sxs-lookup"><span data-stu-id="48688-802">Profile</span></span>
* <span data-ttu-id="48688-803">A conta de nível de locatário foi habilitada para a identidade de serviço gerenciada de `login`</span><span class="sxs-lookup"><span data-stu-id="48688-803">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="48688-804">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-804">Network</span></span>
* <span data-ttu-id="48688-805">Foi corrigido o problema com `express-route update`: em que o argumento `--bandwidth` era ignorado</span><span class="sxs-lookup"><span data-stu-id="48688-805">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="48688-806">Foi corrigido o problema com `ddos-protection update` em que definir a compreensão levava ao rastreamento de pilha</span><span class="sxs-lookup"><span data-stu-id="48688-806">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="48688-807">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-807">Resource</span></span>
* <span data-ttu-id="48688-808">Suporte adicionado para o arquivo de parâmetros de URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="48688-808">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="48688-809">Suporte adicionado para a identidade gerenciada à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="48688-809">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="48688-810">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="48688-810">SQL Virtual Machine</span></span>
* <span data-ttu-id="48688-811">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="48688-811">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="48688-812">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-812">Storage</span></span>
* <span data-ttu-id="48688-813">Alteração na correção para atualizar apenas as propriedades que são alteradas no mesmo objeto</span><span class="sxs-lookup"><span data-stu-id="48688-813">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="48688-814">#8021 foi corrigido, dados binários são codificados em base 64 quando retornados</span><span class="sxs-lookup"><span data-stu-id="48688-814">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="48688-815">VM</span><span class="sxs-lookup"><span data-stu-id="48688-815">VM</span></span>
* <span data-ttu-id="48688-816">Alteração de `vm encryption enable` para validar o cofre de chaves de criptografia de disco e se esse cofre de chaves de criptografia de chave existe</span><span class="sxs-lookup"><span data-stu-id="48688-816">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="48688-817">O sinalizador `--force` foi adicionado a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="48688-817">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="48688-818">15 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="48688-818">January 15, 2019</span></span>

<span data-ttu-id="48688-819">Versão 2.0.55</span><span class="sxs-lookup"><span data-stu-id="48688-819">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="48688-820">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-820">ACR</span></span>
* <span data-ttu-id="48688-821">Alteração para permitir forçar o envio por push de um gráfico Helm que não existe</span><span class="sxs-lookup"><span data-stu-id="48688-821">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="48688-822">Alteração para permitir operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="48688-822">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="48688-823">[PRETERIDO] O parâmetro `--resource-group` foi preterido nos comandos:</span><span class="sxs-lookup"><span data-stu-id="48688-823">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="48688-824">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-824">ACS</span></span>
* <span data-ttu-id="48688-825">Suporte adicionado para novas regiões ACI</span><span class="sxs-lookup"><span data-stu-id="48688-825">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-826">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-826">Appservice</span></span>
* <span data-ttu-id="48688-827">Foi corrigido o problema com o carregamento de certificados para aplicativos que são hospedados em um ASE, em que o RG do ASE e o RG do aplicativo são diferentes</span><span class="sxs-lookup"><span data-stu-id="48688-827">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="48688-828">Alteração de `webapp up` para usar a SKU P1V1 como padrão para Linux</span><span class="sxs-lookup"><span data-stu-id="48688-828">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="48688-829">`[webapp|functionapp] deployment source config-zip` foi corrigido para mostrar a mensagem de erro adequada quando uma implantação falhar</span><span class="sxs-lookup"><span data-stu-id="48688-829">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="48688-830">Adicionado o comando `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="48688-830">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="48688-831">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="48688-831">Botservice</span></span>
* <span data-ttu-id="48688-832">Atualizações de status de implantação foram adicionadas a `bot create`</span><span class="sxs-lookup"><span data-stu-id="48688-832">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="48688-833">Configurar</span><span class="sxs-lookup"><span data-stu-id="48688-833">Configure</span></span>
* <span data-ttu-id="48688-834">`none` foi adicionado como um formato de saída configurável</span><span class="sxs-lookup"><span data-stu-id="48688-834">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48688-835">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48688-835">CosmosDB</span></span>
* <span data-ttu-id="48688-836">Suporte adicionado para criar o banco de dados com taxa de transferência compartilhada</span><span class="sxs-lookup"><span data-stu-id="48688-836">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="48688-837">HDInsight</span><span class="sxs-lookup"><span data-stu-id="48688-837">HDInsight</span></span>
* <span data-ttu-id="48688-838">Foram adicionados comandos para o gerenciamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="48688-838">Added commands for managing applications</span></span>
* <span data-ttu-id="48688-839">Foram adicionados comandos para o gerenciamento de ações de script</span><span class="sxs-lookup"><span data-stu-id="48688-839">Added commands for managing script actions</span></span>
* <span data-ttu-id="48688-840">Foram adicionados comandos para o gerenciamento do Operations Management Suite (OMS)</span><span class="sxs-lookup"><span data-stu-id="48688-840">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="48688-841">Suporte adicionado para listar a utilização regional ao `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="48688-841">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="48688-842">[ALTERAÇÃO SIGNIFICATIVA] O tipo de cluster padrão de `hdinsight create` foi removido</span><span class="sxs-lookup"><span data-stu-id="48688-842">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="48688-843">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-843">Network</span></span>
* <span data-ttu-id="48688-844">Adicionados os argumentos `--custom-headers` e `--status-code-ranges` para `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-844">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="48688-845">Novos tipos de roteamento foram adicionados: Subrede e múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="48688-845">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="48688-846">Adicionados os argumentos `--custom-headers` e `--subnets` para `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-846">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="48688-847">Foi corrigido o problema no qual fornecer `--vnets ""` a `ddos-protection update` causava um erro</span><span class="sxs-lookup"><span data-stu-id="48688-847">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="48688-848">Função</span><span class="sxs-lookup"><span data-stu-id="48688-848">Role</span></span>
* <span data-ttu-id="48688-849">[PRETERIDO] O argumento `--password` foi preterido para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="48688-849">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="48688-850">Como alternativa, use senhas seguras geradas pela CLI</span><span class="sxs-lookup"><span data-stu-id="48688-850">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="48688-851">Segurança</span><span class="sxs-lookup"><span data-stu-id="48688-851">Security</span></span>
* <span data-ttu-id="48688-852">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="48688-852">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="48688-853">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-853">Storage</span></span>
* <span data-ttu-id="48688-854">[ALTERAÇÃO SIGNIFICATIVA] O número padrão de resultados de `storage [blob|file|container|share] list` foi alterado para 5.000.</span><span class="sxs-lookup"><span data-stu-id="48688-854">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="48688-855">Use `--num-results *` para o comportamento original de retornar todos os resultados</span><span class="sxs-lookup"><span data-stu-id="48688-855">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="48688-856">Parâmetro `--marker` adicionado a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="48688-856">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="48688-857">Um marcador de log foi adicionado para a próxima página ao STDERR de `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="48688-857">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="48688-858">O comando `storage blob service-properties update` foi adicionado com suporte para sites estáticos</span><span class="sxs-lookup"><span data-stu-id="48688-858">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="48688-859">VM</span><span class="sxs-lookup"><span data-stu-id="48688-859">VM</span></span>
* <span data-ttu-id="48688-860">`vm [disk|unmanaged-disk]` e `vmss disk` foram alterados para que tenham parâmetros mais consistentes</span><span class="sxs-lookup"><span data-stu-id="48688-860">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="48688-861">Suporte adicionado para referência cruzada de imagem de locatário a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="48688-861">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="48688-862">O bug de configuração padrão foi corrigido em `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="48688-862">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="48688-863">O argumento `--provision-after-extensions` foi adicionado a `vmss extension set` para definir quais extensões deverão ser provisionadas antes da extensão ser definida</span><span class="sxs-lookup"><span data-stu-id="48688-863">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="48688-864">O argumento `--replica-count` foi adicionado a `sig image-version update` para definir a contagem de replicação padrão</span><span class="sxs-lookup"><span data-stu-id="48688-864">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="48688-865">Foi corrigido o bug com `image create --source` em que o disco do sistema operacional de origem era confundido com uma VM do mesmo nome, mesmo se a ID de recurso completa fosse fornecida</span><span class="sxs-lookup"><span data-stu-id="48688-865">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="48688-866">20 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-866">December 20, 2018</span></span>

<span data-ttu-id="48688-867">Versão 2.0.54</span><span class="sxs-lookup"><span data-stu-id="48688-867">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="48688-868">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-868">Appservice</span></span>
* <span data-ttu-id="48688-869">Corrigido o problema que causava falha na reimplantação do `webapp up`</span><span class="sxs-lookup"><span data-stu-id="48688-869">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="48688-870">Adicionado suporte para listar e restaurar instantâneos de aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="48688-870">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="48688-871">Adicionado suporte para o sinalizador `--runtime` para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="48688-871">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="48688-872">IoT Central</span><span class="sxs-lookup"><span data-stu-id="48688-872">IoTCentral</span></span>
* <span data-ttu-id="48688-873">Corrigida a chamada à API do comando de atualização</span><span class="sxs-lookup"><span data-stu-id="48688-873">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="48688-874">Função</span><span class="sxs-lookup"><span data-stu-id="48688-874">Role</span></span>
* <span data-ttu-id="48688-875">[ALTERAÇÃO SIGNIFICATIVA] `ad [app|sp] list` alterado para listar somente os 100 primeiros objetos por padrão</span><span class="sxs-lookup"><span data-stu-id="48688-875">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="48688-876">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-876">SQL</span></span>
* <span data-ttu-id="48688-877">Adicionado suporte para ordenação personalizada nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="48688-877">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="48688-878">VM</span><span class="sxs-lookup"><span data-stu-id="48688-878">VM</span></span>
* <span data-ttu-id="48688-879">Parâmetro `---os-type` adicionado a `disk create`</span><span class="sxs-lookup"><span data-stu-id="48688-879">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="48688-880">18 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-880">December 18, 2018</span></span>

<span data-ttu-id="48688-881">Versão 2.0.53</span><span class="sxs-lookup"><span data-stu-id="48688-881">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="48688-882">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-882">ACR</span></span>
* <span data-ttu-id="48688-883">Adicionado suporte para importação de imagem de Registros de Contêiner externos</span><span class="sxs-lookup"><span data-stu-id="48688-883">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="48688-884">Simplificado o layout da tabela para a lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="48688-884">Condensed the table layout for task list</span></span>
* <span data-ttu-id="48688-885">Adicionado suporte para URLs do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="48688-885">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="48688-886">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-886">ACS</span></span>
* <span data-ttu-id="48688-887">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="48688-887">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="48688-888">Removido “(VISUALIZAÇÃO)” de argumentos do AAD para `aks create`</span><span class="sxs-lookup"><span data-stu-id="48688-888">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="48688-889">[PRETERIDO] Comandos `az acs` preteridos.</span><span class="sxs-lookup"><span data-stu-id="48688-889">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="48688-890">O serviço ACS será desativado em 31 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="48688-890">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="48688-891">Adicionado suporte da Política de Rede durante a criação de novos clusters AKS</span><span class="sxs-lookup"><span data-stu-id="48688-891">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="48688-892">Removido o requisito do argumento `--nodepool-name` para `aks scale` se houver apenas um pool de nós</span><span class="sxs-lookup"><span data-stu-id="48688-892">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-893">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-893">Appservice</span></span>
* <span data-ttu-id="48688-894">Corrigido o problema em que `webapp config container` não honra o parâmetro `--slot`</span><span class="sxs-lookup"><span data-stu-id="48688-894">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="48688-895">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="48688-895">Botservice</span></span>
* <span data-ttu-id="48688-896">Suporte adicionado para análise do arquivo `.bot` ao chamar `bot show`</span><span class="sxs-lookup"><span data-stu-id="48688-896">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="48688-897">Corrigido o bug de provisionamento do AppInsights</span><span class="sxs-lookup"><span data-stu-id="48688-897">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="48688-898">Corrigido o bug de espaço em branco ao lidar com caminhos de arquivo</span><span class="sxs-lookup"><span data-stu-id="48688-898">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="48688-899">Reduzidas as chamadas de rede do Kudu</span><span class="sxs-lookup"><span data-stu-id="48688-899">Reduced Kudu network calls</span></span>
* <span data-ttu-id="48688-900">Melhorias de UX para comandos gerais</span><span class="sxs-lookup"><span data-stu-id="48688-900">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="48688-901">Consumo</span><span class="sxs-lookup"><span data-stu-id="48688-901">Consumption</span></span>
* <span data-ttu-id="48688-902">Corrigidos os bugs da API de orçamento ao mostrar notificações</span><span class="sxs-lookup"><span data-stu-id="48688-902">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48688-903">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48688-903">CosmosDB</span></span>
* <span data-ttu-id="48688-904">Suporte adicionado para atualizar a conta de vários mestres para mestre único</span><span class="sxs-lookup"><span data-stu-id="48688-904">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="48688-905">Mapas</span><span class="sxs-lookup"><span data-stu-id="48688-905">Maps</span></span>
* <span data-ttu-id="48688-906">Adicionado suporte ao SKU S1 para `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-906">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="48688-907">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-907">Network</span></span>
* <span data-ttu-id="48688-908">Adicionado suporte para `--format` e `--log-version` para `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="48688-908">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="48688-909">Corrigido o problema com `dns zone update` em que usar "" para limpar a resolução e o registro de redes virtuais não funcionava</span><span class="sxs-lookup"><span data-stu-id="48688-909">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="48688-910">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-910">Resource</span></span>
* <span data-ttu-id="48688-911">Corrigido o tratamento do parâmetro de escopo para grupos de gerenciamento do `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-911">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="48688-912">Adicionado o novo comando `resource wait`</span><span class="sxs-lookup"><span data-stu-id="48688-912">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="48688-913">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-913">Storage</span></span>
*  <span data-ttu-id="48688-914">Adicionada a capacidade de atualizar a versão do esquema de log para serviços de armazenamento no `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="48688-914">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="48688-915">VM</span><span class="sxs-lookup"><span data-stu-id="48688-915">VM</span></span>
* <span data-ttu-id="48688-916">Corrigida a falha em `vm identity remove` quando a VM especificada não tem nenhuma identidade de serviço gerenciado atribuída</span><span class="sxs-lookup"><span data-stu-id="48688-916">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="48688-917">4 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-917">December 4, 2018</span></span>

<span data-ttu-id="48688-918">Versão 2.0.52</span><span class="sxs-lookup"><span data-stu-id="48688-918">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="48688-919">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-919">Core</span></span>
* <span data-ttu-id="48688-920">Adicionado suporte para provisionamento de recursos de locatários cruzados para a entidade de serviço de multilocatários</span><span class="sxs-lookup"><span data-stu-id="48688-920">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="48688-921">Corrigido o bug onde as ids enviadas por pipe de um comando com a saída tsv eram analisados incorretamente</span><span class="sxs-lookup"><span data-stu-id="48688-921">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-922">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-922">Appservice</span></span>
* <span data-ttu-id="48688-923">[VERSÃO PRÉVIA] Adicionado o comando `webapp up` que ajuda a criar e implantar conteúdo em aplicativo</span><span class="sxs-lookup"><span data-stu-id="48688-923">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="48688-924">Corrigido um bug no aplicativo com base em contêiner do Windows devido à alteração de back-end</span><span class="sxs-lookup"><span data-stu-id="48688-924">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="48688-925">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-925">Network</span></span>
* <span data-ttu-id="48688-926">Adicionado o argumento `--exclusion` a `application-gateway waf-config set` para dar suporte a exclusões de WAF</span><span class="sxs-lookup"><span data-stu-id="48688-926">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="48688-927">Função</span><span class="sxs-lookup"><span data-stu-id="48688-927">Role</span></span>
* <span data-ttu-id="48688-928">Adicionado suporte para identificadores personalizados para a credencial de senha</span><span class="sxs-lookup"><span data-stu-id="48688-928">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="48688-929">VM</span><span class="sxs-lookup"><span data-stu-id="48688-929">VM</span></span>
* <span data-ttu-id="48688-930">[PRETERIDO] Parâmetro `vm extension [show|wait] --expand` preterido</span><span class="sxs-lookup"><span data-stu-id="48688-930">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="48688-931">Adicionado parâmetro `--force` a `vm restart` para reimplantar as VMs sem resposta</span><span class="sxs-lookup"><span data-stu-id="48688-931">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="48688-932">Alterado `[vm|vmss] create --authentication-type` para aceitar "todos" para criar uma VM com senha e autenticação SSH</span><span class="sxs-lookup"><span data-stu-id="48688-932">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="48688-933">Adicionado parâmetro `image create --os-disk-caching` para definir o cache de disco do sistema operacional para uma imagem</span><span class="sxs-lookup"><span data-stu-id="48688-933">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="48688-934">20 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-934">November 20, 2018</span></span>

<span data-ttu-id="48688-935">Versão 2.0.51</span><span class="sxs-lookup"><span data-stu-id="48688-935">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="48688-936">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-936">Core</span></span>
* <span data-ttu-id="48688-937">Logon do MSI alterado para não reutilizar o nome da assinatura na identidade</span><span class="sxs-lookup"><span data-stu-id="48688-937">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="48688-938">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-938">ACR</span></span>
* <span data-ttu-id="48688-939">Token de contexto adicionado à etapa da tarefa</span><span class="sxs-lookup"><span data-stu-id="48688-939">Added context token to task step</span></span>
* <span data-ttu-id="48688-940">Suporte adicionado para definir segredos na execução do acr para espelhar a tarefa do acr</span><span class="sxs-lookup"><span data-stu-id="48688-940">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="48688-941">Suporte aprimorado para `--top` e `--orderby` para os comandos `show-tags` e `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="48688-941">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-942">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-942">Appservice</span></span>
* <span data-ttu-id="48688-943">Tempo limite padrão para a implantação do zip alterado para sondar o status aumentado para 5 minutos, também adicionando uma propriedade de tempo limite para personalizar esse valor</span><span class="sxs-lookup"><span data-stu-id="48688-943">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="48688-944">Padrão `node_version` atualizado.</span><span class="sxs-lookup"><span data-stu-id="48688-944">Updated the default `node_version`.</span></span> <span data-ttu-id="48688-945">Redefinir a ação de troca de slots durante uma troca de duas fases preserva todas as configurações do aplicativo e cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="48688-945">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="48688-946">Verificação da SKU no lado do cliente removida para o Linux criar o plano do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="48688-946">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="48688-947">Erro corrigido ao tentar obter o status de implantação do zip</span><span class="sxs-lookup"><span data-stu-id="48688-947">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="48688-948">Iot Central</span><span class="sxs-lookup"><span data-stu-id="48688-948">IotCentral</span></span>
* <span data-ttu-id="48688-949">Verificação de disponibilidade do subdomínio adicionada ao criar um aplicativo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="48688-949">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="48688-950">KeyVault</span><span class="sxs-lookup"><span data-stu-id="48688-950">KeyVault</span></span>
* <span data-ttu-id="48688-951">Bug corrigido em que os erros podem ter sido ignorados</span><span class="sxs-lookup"><span data-stu-id="48688-951">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="48688-952">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-952">Network</span></span>
* <span data-ttu-id="48688-953">Subcomandos `root-cert` adicionados a `application-gateway` para lidar com os certificados de raiz confiável</span><span class="sxs-lookup"><span data-stu-id="48688-953">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="48688-954">Opções `--min-capacity` e `--custom-error-pages` adicionadas a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="48688-954">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="48688-955">`--zones` adicionado para suporte da zona de disponibilidade a `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="48688-955">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="48688-956">Argumentos `--file-upload-limit`, `--max-request-body-size` e `--request-body-check` a `application-gateway waf-config set` adicionados</span><span class="sxs-lookup"><span data-stu-id="48688-956">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="48688-957">Rdbms</span><span class="sxs-lookup"><span data-stu-id="48688-957">Rdbms</span></span>
* <span data-ttu-id="48688-958">Comandos vnet do mariadb adicionados</span><span class="sxs-lookup"><span data-stu-id="48688-958">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="48688-959">Rbac</span><span class="sxs-lookup"><span data-stu-id="48688-959">Rbac</span></span>
* <span data-ttu-id="48688-960">Um problema corrigido ao tentar atualizar credenciais inalteradas em `ad app update`</span><span class="sxs-lookup"><span data-stu-id="48688-960">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="48688-961">Avisos de saída adicionados para comunicar alterações de falha em um futuro próximo para `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="48688-961">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="48688-962">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-962">Storage</span></span>
* <span data-ttu-id="48688-963">Melhor manipulação de casos incomuns para os comandos da cópia de armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-963">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="48688-964">Corrigido o problema em que `storage blob copy start-batch` não usava credenciais de logon quando as contas de origem e destino eram iguais</span><span class="sxs-lookup"><span data-stu-id="48688-964">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="48688-965">Bug corrigido com `storage [blob|file] url` em que `sas_token` não foi incorporado na URL</span><span class="sxs-lookup"><span data-stu-id="48688-965">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="48688-966">Aviso de alteração da falha adicionado a `[blob|container] list`: produzirá apenas os primeiros 5.000 resultados por padrão</span><span class="sxs-lookup"><span data-stu-id="48688-966">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="48688-967">VM</span><span class="sxs-lookup"><span data-stu-id="48688-967">VM</span></span>
* <span data-ttu-id="48688-968">Suporte adicionado a `[vm|vmss] create --storage-sku` para especificar a SKU da conta de armazenamento para o SO gerenciado e os discos de dados separadamente</span><span class="sxs-lookup"><span data-stu-id="48688-968">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="48688-969">Parâmetros do nome da versão alterados de `sig image-version` para `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="48688-969">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="48688-970">Argumento `sig image-version` preterido `--image-version-name`, substituído por `--image-version`</span><span class="sxs-lookup"><span data-stu-id="48688-970">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="48688-971">Suporte adicionado para usar o disco local do SO a `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="48688-971">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="48688-972">Adicionado o suporte ao `--no-wait` para `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="48688-972">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="48688-973">Adicionado o comando `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="48688-973">Added `snapshot wait` command</span></span>
* <span data-ttu-id="48688-974">Suporte adicionado para usar o nome da instância com `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="48688-974">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="48688-975">6 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-975">November 6, 2018</span></span>

<span data-ttu-id="48688-976">Versão 2.0.50</span><span class="sxs-lookup"><span data-stu-id="48688-976">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="48688-977">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-977">Core</span></span>
* <span data-ttu-id="48688-978">Foi adicionado suporte para o serviço principal sn + autenticação do emissor</span><span class="sxs-lookup"><span data-stu-id="48688-978">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="48688-979">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-979">ACR</span></span>
* <span data-ttu-id="48688-980">Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa</span><span class="sxs-lookup"><span data-stu-id="48688-980">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="48688-981">Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação</span><span class="sxs-lookup"><span data-stu-id="48688-981">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="48688-982">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-982">ACS</span></span>
* <span data-ttu-id="48688-983">[ALTERAÇÃO SIGNIFICATIVA] `enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão</span><span class="sxs-lookup"><span data-stu-id="48688-983">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="48688-984">Supervisor</span><span class="sxs-lookup"><span data-stu-id="48688-984">Advisor</span></span>
* <span data-ttu-id="48688-985">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="48688-985">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="48688-986">AMS</span><span class="sxs-lookup"><span data-stu-id="48688-986">AMS</span></span>
* <span data-ttu-id="48688-987">Novos grupos de comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="48688-987">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="48688-988">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="48688-988">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="48688-989">Adicionados parâmetros de criptografia com suporte para `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="48688-989">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="48688-990">O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido</span><span class="sxs-lookup"><span data-stu-id="48688-990">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="48688-991">Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="48688-991">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="48688-992">Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="48688-992">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="48688-993">Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="48688-993">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="48688-994">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming locator` foi substituído por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="48688-994">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="48688-995">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--content-keys` de `ams streaming locator` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="48688-995">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="48688-996">[ALTERAÇÃO SIGNIFICATIVA] `--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="48688-996">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="48688-997">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming policy` foi substituído por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="48688-997">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="48688-998">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="48688-998">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="48688-999">Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="48688-999">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="48688-1000">Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado</span><span class="sxs-lookup"><span data-stu-id="48688-1000">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="48688-1001">[ALTERAÇÃO SIGNIFICATIVA] `--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="48688-1001">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="48688-1002">Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'.</span><span class="sxs-lookup"><span data-stu-id="48688-1002">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="48688-1003">Um ativo sem rótulo pode ser enviado assim: 'assetName='</span><span class="sxs-lookup"><span data-stu-id="48688-1003">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-1004">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-1004">AppService</span></span>
* <span data-ttu-id="48688-1005">Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido</span><span class="sxs-lookup"><span data-stu-id="48688-1005">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="48688-1006">Configurar</span><span class="sxs-lookup"><span data-stu-id="48688-1006">Configure</span></span>
* <span data-ttu-id="48688-1007">O YAML foi adicionado às opções de formato de saída</span><span class="sxs-lookup"><span data-stu-id="48688-1007">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="48688-1008">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-1008">Container</span></span>
* <span data-ttu-id="48688-1009">Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml</span><span class="sxs-lookup"><span data-stu-id="48688-1009">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="48688-1010">EventHub</span><span class="sxs-lookup"><span data-stu-id="48688-1010">EventHub</span></span>
* <span data-ttu-id="48688-1011">O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-1011">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="48688-1012">Interativo</span><span class="sxs-lookup"><span data-stu-id="48688-1012">Interactive</span></span>
* <span data-ttu-id="48688-1013">O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos</span><span class="sxs-lookup"><span data-stu-id="48688-1013">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="48688-1014">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48688-1014">Monitor</span></span>
* <span data-ttu-id="48688-1015">Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) para `--condition` em `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-1015">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="48688-1016">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-1016">Network</span></span>
* <span data-ttu-id="48688-1017">Os nomes de comandos `network interface-endpoint` foram preteridos em benefício de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="48688-1017">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="48688-1018">Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID</span><span class="sxs-lookup"><span data-stu-id="48688-1018">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="48688-1019">Foi corrigido um problema onde `--ip-tags` não funcionava corretamente com `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="48688-1019">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="48688-1020">Perfil</span><span class="sxs-lookup"><span data-stu-id="48688-1020">Profile</span></span>
* <span data-ttu-id="48688-1021">`--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado</span><span class="sxs-lookup"><span data-stu-id="48688-1021">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="48688-1022">RDBMS</span><span class="sxs-lookup"><span data-stu-id="48688-1022">RDBMS</span></span>
* <span data-ttu-id="48688-1023">Adicionados comandos da réplica mysql</span><span class="sxs-lookup"><span data-stu-id="48688-1023">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="48688-1024">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-1024">Resource</span></span>
* <span data-ttu-id="48688-1025">Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="48688-1025">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="48688-1026">Função</span><span class="sxs-lookup"><span data-stu-id="48688-1026">Role</span></span>
* <span data-ttu-id="48688-1027">Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais</span><span class="sxs-lookup"><span data-stu-id="48688-1027">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="48688-1028">`ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="48688-1028">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="48688-1029">Suporte adicionado para conceder permissões a aplicativos do AAD</span><span class="sxs-lookup"><span data-stu-id="48688-1029">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="48688-1030">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-1030">Storage</span></span>
* <span data-ttu-id="48688-1031">Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="48688-1031">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="48688-1032">VM</span><span class="sxs-lookup"><span data-stu-id="48688-1032">VM</span></span>
* <span data-ttu-id="48688-1033">O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem</span><span class="sxs-lookup"><span data-stu-id="48688-1033">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="48688-1034">O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido</span><span class="sxs-lookup"><span data-stu-id="48688-1034">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="48688-1035">O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado</span><span class="sxs-lookup"><span data-stu-id="48688-1035">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="48688-1036">`vm secret format` foi alterado para exigir a saída json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="48688-1036">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="48688-1037">Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido</span><span class="sxs-lookup"><span data-stu-id="48688-1037">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="48688-1038">Validação de argumento aprimorado para `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="48688-1038">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="48688-1039">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1039">October 23, 2018</span></span>

<span data-ttu-id="48688-1040">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="48688-1040">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="48688-1041">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-1041">Core</span></span>
* <span data-ttu-id="48688-1042">Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`</span><span class="sxs-lookup"><span data-stu-id="48688-1042">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="48688-1043">Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="48688-1043">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="48688-1044">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-1044">ACR</span></span>
* <span data-ttu-id="48688-1045">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="48688-1045">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="48688-1046">CDN</span><span class="sxs-lookup"><span data-stu-id="48688-1046">CDN</span></span>
* <span data-ttu-id="48688-1047">[ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="48688-1047">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="48688-1048">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="48688-1048">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="48688-1049">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-1049">Container</span></span>
* <span data-ttu-id="48688-1050">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="48688-1050">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="48688-1051">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="48688-1051">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="48688-1052">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="48688-1052">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="48688-1053">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="48688-1053">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="48688-1054">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="48688-1054">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="48688-1055">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="48688-1055">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="48688-1056">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="48688-1056">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48688-1057">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48688-1057">CosmosDB</span></span>
* <span data-ttu-id="48688-1058">Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="48688-1058">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="48688-1059">Interativo</span><span class="sxs-lookup"><span data-stu-id="48688-1059">Interactive</span></span>
* <span data-ttu-id="48688-1060">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="48688-1060">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="48688-1061">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="48688-1061">IoT Central</span></span>
* <span data-ttu-id="48688-1062">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="48688-1062">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="48688-1063">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="48688-1063">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="48688-1064">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48688-1064">Monitor</span></span>
* <span data-ttu-id="48688-1065">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="48688-1065">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="48688-1066">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="48688-1066">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="48688-1067">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="48688-1067">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="48688-1068">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="48688-1068">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="48688-1069">Adicionado `--namespace` como alias para a opção preterida `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="48688-1069">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="48688-1070">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="48688-1070">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="48688-1071">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="48688-1071">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="48688-1072">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="48688-1072">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="48688-1073">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="48688-1073">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="48688-1074">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="48688-1074">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="48688-1075">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-1075">Network</span></span>
* <span data-ttu-id="48688-1076">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="48688-1076">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="48688-1077">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="48688-1077">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="48688-1078">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="48688-1078">ServiceBus</span></span>
* <span data-ttu-id="48688-1079">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="48688-1079">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="48688-1080">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-1080">SQL</span></span>
* <span data-ttu-id="48688-1081">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="48688-1081">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="48688-1082">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-1082">Storage</span></span>
* <span data-ttu-id="48688-1083">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="48688-1083">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="48688-1084">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="48688-1084">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="48688-1085">VM</span><span class="sxs-lookup"><span data-stu-id="48688-1085">VM</span></span>
* <span data-ttu-id="48688-1086">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="48688-1086">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="48688-1087">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`</span><span class="sxs-lookup"><span data-stu-id="48688-1087">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="48688-1088">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`</span><span class="sxs-lookup"><span data-stu-id="48688-1088">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="48688-1089">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1089">October 16, 2018</span></span>

<span data-ttu-id="48688-1090">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="48688-1090">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="48688-1091">VM</span><span class="sxs-lookup"><span data-stu-id="48688-1091">VM</span></span>
* <span data-ttu-id="48688-1092">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="48688-1092">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="48688-1093">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1093">October 9, 2018</span></span>

<span data-ttu-id="48688-1094">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="48688-1094">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="48688-1095">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-1095">Core</span></span>
* <span data-ttu-id="48688-1096">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="48688-1096">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="48688-1097">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-1097">ACR</span></span>
* <span data-ttu-id="48688-1098">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="48688-1098">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="48688-1099">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-1099">ACS</span></span>
* <span data-ttu-id="48688-1100">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="48688-1100">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="48688-1101">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="48688-1101">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="48688-1102">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="48688-1102">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="48688-1103">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="48688-1103">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="48688-1104">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-1104">Container</span></span>
* <span data-ttu-id="48688-1105">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um tempo de execução específico</span><span class="sxs-lookup"><span data-stu-id="48688-1105">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="48688-1106">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="48688-1106">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="48688-1107">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="48688-1107">Event Hub</span></span>
* <span data-ttu-id="48688-1108">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="48688-1108">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="48688-1109">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="48688-1109">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="48688-1110">Extensões</span><span class="sxs-lookup"><span data-stu-id="48688-1110">Extensions</span></span>
* <span data-ttu-id="48688-1111">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="48688-1111">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="48688-1112">HDInsight</span><span class="sxs-lookup"><span data-stu-id="48688-1112">HDInsight</span></span>
* <span data-ttu-id="48688-1113">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="48688-1113">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="48688-1114">IoT</span><span class="sxs-lookup"><span data-stu-id="48688-1114">IoT</span></span>
* <span data-ttu-id="48688-1115">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="48688-1115">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="48688-1116">KeyVault</span><span class="sxs-lookup"><span data-stu-id="48688-1116">KeyVault</span></span>
* <span data-ttu-id="48688-1117">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="48688-1117">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="48688-1118">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-1118">Network</span></span>
* <span data-ttu-id="48688-1119">Corrigido `network dns zone create`: O comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="48688-1119">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="48688-1120">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="48688-1120">See #6052</span></span>
* <span data-ttu-id="48688-1121">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="48688-1121">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="48688-1122">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="48688-1122">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="48688-1123">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="48688-1123">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="48688-1124">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="48688-1124">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="48688-1125">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="48688-1125">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="48688-1126">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="48688-1126">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="48688-1127">Função</span><span class="sxs-lookup"><span data-stu-id="48688-1127">Role</span></span>
* <span data-ttu-id="48688-1128">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="48688-1128">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="48688-1129">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="48688-1129">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="48688-1130">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="48688-1130">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="48688-1131">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="48688-1131">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="48688-1132">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="48688-1132">Service Bus</span></span>
* <span data-ttu-id="48688-1133">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="48688-1133">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="48688-1134">VM</span><span class="sxs-lookup"><span data-stu-id="48688-1134">VM</span></span>
* <span data-ttu-id="48688-1135">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="48688-1135">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="48688-1136">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="48688-1136">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="48688-1137">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="48688-1137">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="48688-1138">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="48688-1138">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="48688-1139">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="48688-1139">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="48688-1140">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="48688-1140">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="48688-1141">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1141">September 21, 2018</span></span>

<span data-ttu-id="48688-1142">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="48688-1142">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="48688-1143">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-1143">ACR</span></span>
* <span data-ttu-id="48688-1144">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="48688-1144">Added ACR Task commands</span></span>
* <span data-ttu-id="48688-1145">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="48688-1145">Added quick run command</span></span>
* <span data-ttu-id="48688-1146">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="48688-1146">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="48688-1147">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="48688-1147">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="48688-1148">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="48688-1148">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="48688-1149">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="48688-1149">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="48688-1150">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-1150">ACS</span></span>
* <span data-ttu-id="48688-1151">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="48688-1151">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="48688-1152">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="48688-1152">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-1153">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-1153">AppService</span></span>

* <span data-ttu-id="48688-1154">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="48688-1154">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="48688-1155">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="48688-1155">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="48688-1156">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="48688-1156">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="48688-1157">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="48688-1157">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="48688-1158">Lote</span><span class="sxs-lookup"><span data-stu-id="48688-1158">Batch</span></span>
* <span data-ttu-id="48688-1159">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="48688-1159">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="48688-1160">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="48688-1160">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="48688-1161">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="48688-1161">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="48688-1162">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="48688-1162">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="48688-1163">Lote AI</span><span class="sxs-lookup"><span data-stu-id="48688-1163">Batch AI</span></span> 
* <span data-ttu-id="48688-1164">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="48688-1164">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="48688-1165">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="48688-1165">Cognitive Services</span></span>
* <span data-ttu-id="48688-1166">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="48688-1166">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="48688-1167">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="48688-1167">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="48688-1168">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="48688-1168">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="48688-1169">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="48688-1169">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="48688-1170">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="48688-1170">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="48688-1171">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="48688-1171">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="48688-1172">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-1172">Container</span></span>
* <span data-ttu-id="48688-1173">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="48688-1173">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="48688-1174">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="48688-1174">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="48688-1175">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="48688-1175">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="48688-1176">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="48688-1176">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="48688-1177">DataLake</span><span class="sxs-lookup"><span data-stu-id="48688-1177">Datalake</span></span>
* <span data-ttu-id="48688-1178">Comandos adicionados para regras da rede virtual</span><span class="sxs-lookup"><span data-stu-id="48688-1178">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="48688-1179">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="48688-1179">Interactive Shell</span></span>
* <span data-ttu-id="48688-1180">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="48688-1180">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="48688-1181">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="48688-1181">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="48688-1182">IoT</span><span class="sxs-lookup"><span data-stu-id="48688-1182">IoT</span></span>
* <span data-ttu-id="48688-1183">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="48688-1183">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="48688-1184">Key Vault</span><span class="sxs-lookup"><span data-stu-id="48688-1184">Key Vault</span></span>
* <span data-ttu-id="48688-1185">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="48688-1185">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="48688-1186">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-1186">Network</span></span>
* <span data-ttu-id="48688-1187">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="48688-1187">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="48688-1188">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="48688-1188">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="48688-1189">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="48688-1189">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="48688-1190">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="48688-1190">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="48688-1191">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="48688-1191">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="48688-1192">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="48688-1192">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="48688-1193">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="48688-1193">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="48688-1194">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="48688-1194">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="48688-1195">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="48688-1195">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="48688-1196">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="48688-1196">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="48688-1197">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="48688-1197">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="48688-1198">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="48688-1198">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="48688-1199">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="48688-1199">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="48688-1200">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="48688-1200">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="48688-1201">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="48688-1201">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="48688-1202">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="48688-1202">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="48688-1203">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="48688-1203">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="48688-1204">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="48688-1204">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="48688-1205">RDBMS</span><span class="sxs-lookup"><span data-stu-id="48688-1205">RDBMS</span></span>
* <span data-ttu-id="48688-1206">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="48688-1206">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="48688-1207">Reserva</span><span class="sxs-lookup"><span data-stu-id="48688-1207">Reservation</span></span>
* <span data-ttu-id="48688-1208">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="48688-1208">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="48688-1209">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="48688-1209">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="48688-1210">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="48688-1210">Manage App</span></span>
* <span data-ttu-id="48688-1211">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="48688-1211">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="48688-1212">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="48688-1212">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="48688-1213">Função</span><span class="sxs-lookup"><span data-stu-id="48688-1213">Role</span></span>
* <span data-ttu-id="48688-1214">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="48688-1214">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="48688-1215">SignalR</span><span class="sxs-lookup"><span data-stu-id="48688-1215">SignalR</span></span>
* <span data-ttu-id="48688-1216">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="48688-1216">First release</span></span>

### <a name="storage"></a><span data-ttu-id="48688-1217">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-1217">Storage</span></span>
* <span data-ttu-id="48688-1218">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="48688-1218">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="48688-1219">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="48688-1219">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="48688-1220">VM</span><span class="sxs-lookup"><span data-stu-id="48688-1220">VM</span></span>
* <span data-ttu-id="48688-1221">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="48688-1221">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="48688-1222">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="48688-1222">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="48688-1223">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1223">August 28, 2018</span></span>

<span data-ttu-id="48688-1224">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="48688-1224">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="48688-1225">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-1225">Core</span></span>

* <span data-ttu-id="48688-1226">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="48688-1226">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="48688-1227">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="48688-1227">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="48688-1228">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-1228">ACR</span></span>

* <span data-ttu-id="48688-1229">Adicionada uma solução alternativa para operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="48688-1229">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="48688-1230">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="48688-1230">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="48688-1231">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-1231">ACS</span></span>

* <span data-ttu-id="48688-1232">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="48688-1232">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="48688-1233">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="48688-1233">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-1234">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-1234">AppService</span></span>

* <span data-ttu-id="48688-1235">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="48688-1235">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="48688-1236">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="48688-1236">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="48688-1237">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="48688-1237">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="48688-1238">Backup</span><span class="sxs-lookup"><span data-stu-id="48688-1238">Backup</span></span>

* <span data-ttu-id="48688-1239">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="48688-1239">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="48688-1240">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="48688-1240">Bot Service</span></span>

* <span data-ttu-id="48688-1241">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="48688-1241">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="48688-1242">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="48688-1242">Cognitive Services</span></span>

* <span data-ttu-id="48688-1243">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="48688-1243">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="48688-1244">IoT</span><span class="sxs-lookup"><span data-stu-id="48688-1244">IoT</span></span>

* <span data-ttu-id="48688-1245">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="48688-1245">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="48688-1246">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48688-1246">Monitor</span></span>

* <span data-ttu-id="48688-1247">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="48688-1247">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="48688-1248">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="48688-1248">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="48688-1249">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-1249">Network</span></span>

* <span data-ttu-id="48688-1250">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="48688-1250">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="48688-1251">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-1251">Resource</span></span>

* <span data-ttu-id="48688-1252">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="48688-1252">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="48688-1253">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-1253">Storage</span></span>

* <span data-ttu-id="48688-1254">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="48688-1254">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="48688-1255">VM</span><span class="sxs-lookup"><span data-stu-id="48688-1255">VM</span></span>

* <span data-ttu-id="48688-1256">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="48688-1256">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="48688-1257">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="48688-1257">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="48688-1258">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1258">Auguest 14, 2018</span></span>

<span data-ttu-id="48688-1259">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="48688-1259">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="48688-1260">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-1260">Core</span></span>

* <span data-ttu-id="48688-1261">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="48688-1261">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="48688-1262">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="48688-1262">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="48688-1263">Telemetria</span><span class="sxs-lookup"><span data-stu-id="48688-1263">Telemetry</span></span>

* <span data-ttu-id="48688-1264">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="48688-1264">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="48688-1265">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-1265">ACR</span></span>

* <span data-ttu-id="48688-1266">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="48688-1266">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="48688-1267">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="48688-1267">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="48688-1268">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-1268">ACS</span></span>

* <span data-ttu-id="48688-1269">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="48688-1269">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="48688-1270">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="48688-1270">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="48688-1271">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="48688-1271">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="48688-1272">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="48688-1272">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="48688-1273">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="48688-1273">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="48688-1274">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-1274">AppService</span></span>

* <span data-ttu-id="48688-1275">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="48688-1275">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="48688-1276">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="48688-1276">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="48688-1277">BatchAI</span><span class="sxs-lookup"><span data-stu-id="48688-1277">BatchAI</span></span>

* <span data-ttu-id="48688-1278">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="48688-1278">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="48688-1279">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-1279">Container</span></span>

* <span data-ttu-id="48688-1280">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-1280">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="48688-1281">IoT</span><span class="sxs-lookup"><span data-stu-id="48688-1281">IoT</span></span>

* <span data-ttu-id="48688-1282">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="48688-1282">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="48688-1283">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="48688-1283">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="48688-1284">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="48688-1284">Iot Central</span></span>

* <span data-ttu-id="48688-1285">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="48688-1285">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="48688-1286">KeyVault</span><span class="sxs-lookup"><span data-stu-id="48688-1286">KeyVault</span></span>


* <span data-ttu-id="48688-1287">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="48688-1287">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="48688-1288">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="48688-1288">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="48688-1289">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="48688-1289">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="48688-1290">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="48688-1290">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="48688-1291">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="48688-1291">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="48688-1292">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="48688-1292">Relay</span></span>

* <span data-ttu-id="48688-1293">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="48688-1293">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="48688-1294">Sql</span><span class="sxs-lookup"><span data-stu-id="48688-1294">Sql</span></span>

* <span data-ttu-id="48688-1295">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="48688-1295">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="48688-1296">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-1296">Storage</span></span>

* <span data-ttu-id="48688-1297">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="48688-1297">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="48688-1298">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="48688-1298">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="48688-1299">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="48688-1299">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="48688-1300">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="48688-1300">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="48688-1301">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-1301">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="48688-1302">VM</span><span class="sxs-lookup"><span data-stu-id="48688-1302">VM</span></span>

* <span data-ttu-id="48688-1303">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="48688-1303">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="48688-1304">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1304">July 31, 2018</span></span>

<span data-ttu-id="48688-1305">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="48688-1305">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="48688-1306">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-1306">ACR</span></span>

* <span data-ttu-id="48688-1307">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="48688-1307">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="48688-1308">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="48688-1308">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="48688-1309">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-1309">ACS</span></span>

* <span data-ttu-id="48688-1310">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="48688-1310">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="48688-1311">Lote</span><span class="sxs-lookup"><span data-stu-id="48688-1311">Batch</span></span>

* <span data-ttu-id="48688-1312">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="48688-1312">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="48688-1313">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-1313">Container</span></span>

* <span data-ttu-id="48688-1314">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="48688-1314">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="48688-1315">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-1315">Network</span></span>

* <span data-ttu-id="48688-1316">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="48688-1316">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="48688-1317">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-1317">Resource</span></span>

* <span data-ttu-id="48688-1318">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="48688-1318">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="48688-1319">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="48688-1319">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="48688-1320">Função</span><span class="sxs-lookup"><span data-stu-id="48688-1320">Role</span></span>

* <span data-ttu-id="48688-1321">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="48688-1321">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="48688-1322">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="48688-1322">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="48688-1323">Search</span><span class="sxs-lookup"><span data-stu-id="48688-1323">Search</span></span>

* <span data-ttu-id="48688-1324">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="48688-1324">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="48688-1325">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="48688-1325">Service Bus</span></span>

* <span data-ttu-id="48688-1326">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="48688-1326">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="48688-1327">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="48688-1327">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="48688-1328">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="48688-1328">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="48688-1329">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="48688-1329">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="48688-1330">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-1330">Storage</span></span>

* <span data-ttu-id="48688-1331">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="48688-1331">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="48688-1332">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="48688-1332">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="48688-1333">VM</span><span class="sxs-lookup"><span data-stu-id="48688-1333">VM</span></span>

* <span data-ttu-id="48688-1334">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="48688-1334">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="48688-1335">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="48688-1335">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="48688-1336">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="48688-1336">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="48688-1337">[ALTERAÇÃO SIGNIFICATIVA] `[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="48688-1337">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="48688-1338">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1338">July 18, 2018</span></span>

<span data-ttu-id="48688-1339">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="48688-1339">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="48688-1340">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-1340">Core</span></span>

* <span data-ttu-id="48688-1341">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="48688-1341">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="48688-1342">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="48688-1342">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="48688-1343">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="48688-1343">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="48688-1344">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-1344">ACR</span></span>

* <span data-ttu-id="48688-1345">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="48688-1345">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="48688-1346">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="48688-1346">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="48688-1347">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="48688-1347">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="48688-1348">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="48688-1348">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="48688-1349">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-1349">ACS</span></span>

* <span data-ttu-id="48688-1350">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="48688-1350">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-1351">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-1351">AppService</span></span>

* <span data-ttu-id="48688-1352">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="48688-1352">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="48688-1353">Lote</span><span class="sxs-lookup"><span data-stu-id="48688-1353">Batch</span></span>

* <span data-ttu-id="48688-1354">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="48688-1354">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="48688-1355">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="48688-1355">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="48688-1356">Lote AI</span><span class="sxs-lookup"><span data-stu-id="48688-1356">Batch AI</span></span>

* <span data-ttu-id="48688-1357">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="48688-1357">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="48688-1358">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-1358">Container</span></span>

* <span data-ttu-id="48688-1359">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="48688-1359">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="48688-1360">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="48688-1360">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="48688-1361">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-1361">Network</span></span>

* <span data-ttu-id="48688-1362">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="48688-1362">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="48688-1363">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="48688-1363">Added `network nic wait`</span></span>
* <span data-ttu-id="48688-1364">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="48688-1364">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="48688-1365">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="48688-1365">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="48688-1366">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-1366">Resource</span></span>

* <span data-ttu-id="48688-1367">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="48688-1367">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="48688-1368">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="48688-1368">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="48688-1369">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="48688-1369">Added `deployment wait` command</span></span>
* <span data-ttu-id="48688-1370">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="48688-1370">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="48688-1371">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-1371">SQL</span></span>

* <span data-ttu-id="48688-1372">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="48688-1372">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="48688-1373">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="48688-1373">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="48688-1374">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="48688-1374">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="48688-1375">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-1375">Storage</span></span>

* <span data-ttu-id="48688-1376">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="48688-1376">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="48688-1377">VM</span><span class="sxs-lookup"><span data-stu-id="48688-1377">VM</span></span>

* <span data-ttu-id="48688-1378">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="48688-1378">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="48688-1379">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="48688-1379">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="48688-1380">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="48688-1380">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="48688-1381">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1381">July 3, 2018</span></span>

<span data-ttu-id="48688-1382">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="48688-1382">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="48688-1383">AKS</span><span class="sxs-lookup"><span data-stu-id="48688-1383">AKS</span></span>

* <span data-ttu-id="48688-1384">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="48688-1384">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="48688-1385">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1385">July 3, 2018</span></span>

<span data-ttu-id="48688-1386">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="48688-1386">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="48688-1387">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-1387">Core</span></span>

* <span data-ttu-id="48688-1388">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="48688-1388">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="48688-1389">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-1389">ACR</span></span>

* <span data-ttu-id="48688-1390">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="48688-1390">Added polling build status</span></span>
* <span data-ttu-id="48688-1391">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="48688-1391">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="48688-1392">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="48688-1392">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="48688-1393">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-1393">ACS</span></span>

* <span data-ttu-id="48688-1394">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="48688-1394">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="48688-1395">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="48688-1395">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="48688-1396">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="48688-1396">Updated options for `aks browse` command.</span></span> <span data-ttu-id="48688-1397">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="48688-1397">Added `--listen-port` support</span></span>
* <span data-ttu-id="48688-1398">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="48688-1398">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="48688-1399">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="48688-1399">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="48688-1400">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="48688-1400">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-1401">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-1401">AppService</span></span>

* <span data-ttu-id="48688-1402">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="48688-1402">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="48688-1403">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="48688-1403">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="48688-1404">Backup</span><span class="sxs-lookup"><span data-stu-id="48688-1404">Backup</span></span>

* <span data-ttu-id="48688-1405">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="48688-1405">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="48688-1406">BatchAI</span><span class="sxs-lookup"><span data-stu-id="48688-1406">BatchAI</span></span>

* <span data-ttu-id="48688-1407">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="48688-1407">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="48688-1408">Nuvem</span><span class="sxs-lookup"><span data-stu-id="48688-1408">Cloud</span></span>

* <span data-ttu-id="48688-1409">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="48688-1409">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="48688-1410">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-1410">Container</span></span>

* <span data-ttu-id="48688-1411">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="48688-1411">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="48688-1412">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="48688-1412">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="48688-1413">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="48688-1413">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="48688-1414">Extensão</span><span class="sxs-lookup"><span data-stu-id="48688-1414">Extension</span></span>

* <span data-ttu-id="48688-1415">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="48688-1415">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="48688-1416">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-1416">Network</span></span>

* <span data-ttu-id="48688-1417">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="48688-1417">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="48688-1418">Rdbms</span><span class="sxs-lookup"><span data-stu-id="48688-1418">Rdbms</span></span>

* <span data-ttu-id="48688-1419">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="48688-1419">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="48688-1420">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-1420">Resource</span></span>

* <span data-ttu-id="48688-1421">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="48688-1421">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="48688-1422">VM</span><span class="sxs-lookup"><span data-stu-id="48688-1422">VM</span></span>

* <span data-ttu-id="48688-1423">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="48688-1423">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="48688-1424">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1424">June 25, 2018</span></span>

<span data-ttu-id="48688-1425">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="48688-1425">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="48688-1426">CLI</span><span class="sxs-lookup"><span data-stu-id="48688-1426">CLI</span></span>

* <span data-ttu-id="48688-1427">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="48688-1427">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="48688-1428">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1428">June 19, 2018</span></span>

<span data-ttu-id="48688-1429">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="48688-1429">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="48688-1430">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-1430">Core</span></span>

* <span data-ttu-id="48688-1431">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="48688-1431">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="48688-1432">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-1432">ACR</span></span>

* <span data-ttu-id="48688-1433">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="48688-1433">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="48688-1434">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="48688-1434">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="48688-1435">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-1435">ACS</span></span>

* <span data-ttu-id="48688-1436">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="48688-1436">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="48688-1437">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="48688-1437">Added `--update` support</span></span>
* <span data-ttu-id="48688-1438">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="48688-1438">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="48688-1439">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="48688-1439">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="48688-1440">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="48688-1440">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="48688-1441">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="48688-1441">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="48688-1442">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="48688-1442">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="48688-1443">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="48688-1443">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-1444">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-1444">AppService</span></span>

* <span data-ttu-id="48688-1445">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="48688-1445">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="48688-1446">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="48688-1446">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="48688-1447">Lote</span><span class="sxs-lookup"><span data-stu-id="48688-1447">Batch</span></span>

* <span data-ttu-id="48688-1448">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="48688-1448">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="48688-1449">Lote AI</span><span class="sxs-lookup"><span data-stu-id="48688-1449">Batch AI</span></span>

* <span data-ttu-id="48688-1450">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="48688-1450">Added support for workspaces.</span></span> <span data-ttu-id="48688-1451">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="48688-1451">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="48688-1452">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="48688-1452">Added support for experiments.</span></span> <span data-ttu-id="48688-1453">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="48688-1453">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="48688-1454">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="48688-1454">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="48688-1455">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="48688-1455">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="48688-1456">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="48688-1456">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="48688-1457">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="48688-1457">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="48688-1458">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="48688-1458">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="48688-1459">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="48688-1459">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="48688-1460">[ALTERAÇÃO SIGNIFICATIVA] `--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="48688-1460">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="48688-1461">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="48688-1461">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="48688-1462">[ALTERAÇÃO SIGNIFICATIVA] `--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="48688-1462">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="48688-1463">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="48688-1463">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="48688-1464">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="48688-1464">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="48688-1465">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="48688-1465">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="48688-1466">[ALTERAÇÃO SIGNIFICATIVA] `--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="48688-1466">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="48688-1467">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="48688-1467">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="48688-1468">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="48688-1468">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="48688-1469">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="48688-1469">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="48688-1470">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="48688-1470">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="48688-1471">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="48688-1471">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="48688-1472">Mapas</span><span class="sxs-lookup"><span data-stu-id="48688-1472">Maps</span></span>

* <span data-ttu-id="48688-1473">[ALTERAÇÃO SIGNIFICATIVA] `maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="48688-1473">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="48688-1474">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-1474">Network</span></span>

* <span data-ttu-id="48688-1475">Foi adicionado suporte a `https` para `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="48688-1475">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="48688-1476">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="48688-1476">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="48688-1477">#6502</span><span class="sxs-lookup"><span data-stu-id="48688-1477">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="48688-1478">Reservas</span><span class="sxs-lookup"><span data-stu-id="48688-1478">Reservations</span></span>

* <span data-ttu-id="48688-1479">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="48688-1479">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="48688-1480">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="48688-1480">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="48688-1481">[ALTERAÇÃO SIGNIFICATIVA] `kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="48688-1481">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="48688-1482">[ALTERAÇÃO SIGNIFICATIVA] `capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="48688-1482">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="48688-1483">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="48688-1483">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="48688-1484">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="48688-1484">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="48688-1485">Função</span><span class="sxs-lookup"><span data-stu-id="48688-1485">Role</span></span>

* <span data-ttu-id="48688-1486">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="48688-1486">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="48688-1487">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-1487">SQL</span></span>

* <span data-ttu-id="48688-1488">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="48688-1488">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="48688-1489">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-1489">Storage</span></span>

* <span data-ttu-id="48688-1490">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="48688-1490">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="48688-1491">VM</span><span class="sxs-lookup"><span data-stu-id="48688-1491">VM</span></span>

* <span data-ttu-id="48688-1492">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="48688-1492">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="48688-1493">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="48688-1493">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="48688-1494">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="48688-1494">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="48688-1495">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1495">June 13, 2018</span></span>

<span data-ttu-id="48688-1496">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="48688-1496">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="48688-1497">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-1497">Core</span></span>

* <span data-ttu-id="48688-1498">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="48688-1498">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="48688-1499">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1499">June 13, 2018</span></span>

<span data-ttu-id="48688-1500">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="48688-1500">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="48688-1501">AKS</span><span class="sxs-lookup"><span data-stu-id="48688-1501">AKS</span></span>

* <span data-ttu-id="48688-1502">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="48688-1502">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="48688-1503">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="48688-1503">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="48688-1504">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="48688-1504">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="48688-1505">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="48688-1505">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="48688-1506">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="48688-1506">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-1507">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-1507">AppService</span></span>

* <span data-ttu-id="48688-1508">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="48688-1508">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="48688-1509">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1509">June 5, 2018</span></span>

<span data-ttu-id="48688-1510">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="48688-1510">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="48688-1511">Interativo</span><span class="sxs-lookup"><span data-stu-id="48688-1511">Interactive</span></span>

* <span data-ttu-id="48688-1512">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="48688-1512">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="48688-1513">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1513">June 5, 2018</span></span>

<span data-ttu-id="48688-1514">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="48688-1514">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="48688-1515">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-1515">Core</span></span>

* <span data-ttu-id="48688-1516">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="48688-1516">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="48688-1517">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="48688-1517">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="48688-1518">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-1518">ACR</span></span>

* <span data-ttu-id="48688-1519">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="48688-1519">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="48688-1520">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="48688-1520">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="48688-1521">AKS</span><span class="sxs-lookup"><span data-stu-id="48688-1521">AKS</span></span>

* <span data-ttu-id="48688-1522">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="48688-1522">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="48688-1523">Lote</span><span class="sxs-lookup"><span data-stu-id="48688-1523">Batch</span></span>

* <span data-ttu-id="48688-1524">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="48688-1524">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="48688-1525">IOT</span><span class="sxs-lookup"><span data-stu-id="48688-1525">IOT</span></span>

* <span data-ttu-id="48688-1526">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="48688-1526">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="48688-1527">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-1527">Network</span></span>

* <span data-ttu-id="48688-1528">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="48688-1528">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="48688-1529">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="48688-1529">Policy Insights</span></span>

* <span data-ttu-id="48688-1530">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="48688-1530">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="48688-1531">ARM</span><span class="sxs-lookup"><span data-stu-id="48688-1531">ARM</span></span>

* <span data-ttu-id="48688-1532">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="48688-1532">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="48688-1533">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-1533">SQL</span></span>

* <span data-ttu-id="48688-1534">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="48688-1534">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="48688-1535">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="48688-1535">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="48688-1536">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-1536">Storage</span></span>

* <span data-ttu-id="48688-1537">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="48688-1537">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="48688-1538">VM</span><span class="sxs-lookup"><span data-stu-id="48688-1538">VM</span></span>

* <span data-ttu-id="48688-1539">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="48688-1539">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="48688-1540">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="48688-1540">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="48688-1541">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="48688-1541">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="48688-1542">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1542">May 22, 2018</span></span>

<span data-ttu-id="48688-1543">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="48688-1543">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="48688-1544">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-1544">Core</span></span>

* <span data-ttu-id="48688-1545">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="48688-1545">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="48688-1546">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-1546">ACS</span></span>

* <span data-ttu-id="48688-1547">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="48688-1547">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="48688-1548">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="48688-1548">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-1549">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-1549">AppService</span></span>

* <span data-ttu-id="48688-1550">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="48688-1550">Improved generic update commands</span></span>
* <span data-ttu-id="48688-1551">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="48688-1551">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="48688-1552">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-1552">Container</span></span>

* <span data-ttu-id="48688-1553">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="48688-1553">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="48688-1554">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-1554">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="48688-1555">Extensão</span><span class="sxs-lookup"><span data-stu-id="48688-1555">Extension</span></span>

* <span data-ttu-id="48688-1556">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="48688-1556">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="48688-1557">Interativo</span><span class="sxs-lookup"><span data-stu-id="48688-1557">Interactive</span></span>

* <span data-ttu-id="48688-1558">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="48688-1558">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="48688-1559">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="48688-1559">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="48688-1560">KeyVault</span><span class="sxs-lookup"><span data-stu-id="48688-1560">KeyVault</span></span>

* <span data-ttu-id="48688-1561">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="48688-1561">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="48688-1562">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-1562">Network</span></span>

* <span data-ttu-id="48688-1563">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="48688-1563">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="48688-1564">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="48688-1564">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="48688-1565">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-1565">SQL</span></span>

* <span data-ttu-id="48688-1566">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="48688-1566">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="48688-1567">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="48688-1567">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="48688-1568">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="48688-1568">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="48688-1569">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48688-1569">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="48688-1570">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="48688-1570">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="48688-1571">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="48688-1571">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="48688-1572">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="48688-1572">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="48688-1573">`edition`.</span><span class="sxs-lookup"><span data-stu-id="48688-1573">`edition`.</span></span> <span data-ttu-id="48688-1574">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="48688-1574">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="48688-1575">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="48688-1575">`elasticPoolName`.</span></span> <span data-ttu-id="48688-1576">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="48688-1576">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="48688-1577">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="48688-1577">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="48688-1578">`edition`.</span><span class="sxs-lookup"><span data-stu-id="48688-1578">`edition`.</span></span> <span data-ttu-id="48688-1579">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="48688-1579">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="48688-1580">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="48688-1580">`dtu`.</span></span> <span data-ttu-id="48688-1581">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="48688-1581">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="48688-1582">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="48688-1582">`databaseDtuMin`.</span></span> <span data-ttu-id="48688-1583">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="48688-1583">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="48688-1584">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="48688-1584">`databaseDtuMax`.</span></span> <span data-ttu-id="48688-1585">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="48688-1585">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="48688-1586">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="48688-1586">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="48688-1587">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="48688-1587">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="48688-1588">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-1588">Storage</span></span>

* <span data-ttu-id="48688-1589">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="48688-1589">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="48688-1590">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="48688-1590">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="48688-1591">VM</span><span class="sxs-lookup"><span data-stu-id="48688-1591">VM</span></span>

* <span data-ttu-id="48688-1592">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="48688-1592">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="48688-1593">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="48688-1593">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="48688-1594">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="48688-1594">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="48688-1595">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="48688-1595">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="48688-1596">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="48688-1596">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="48688-1597">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1597">May 7, 2018</span></span>

<span data-ttu-id="48688-1598">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="48688-1598">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="48688-1599">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-1599">Core</span></span>

* <span data-ttu-id="48688-1600">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="48688-1600">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="48688-1601">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="48688-1601">Added limited support for positional arguments</span></span>
* <span data-ttu-id="48688-1602">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="48688-1602">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="48688-1603">#5591</span><span class="sxs-lookup"><span data-stu-id="48688-1603">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="48688-1604">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="48688-1604">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="48688-1605">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="48688-1605">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="48688-1606">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="48688-1606">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="48688-1607">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="48688-1607">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="48688-1608">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="48688-1608">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="48688-1609">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-1609">ACR</span></span>

* <span data-ttu-id="48688-1610">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="48688-1610">Added ACR Build commands</span></span>
* <span data-ttu-id="48688-1611">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="48688-1611">Improved resource not found error messages</span></span>
* <span data-ttu-id="48688-1612">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="48688-1612">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="48688-1613">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="48688-1613">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="48688-1614">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="48688-1614">Improved repository commands error messages</span></span>
* <span data-ttu-id="48688-1615">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="48688-1615">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="48688-1616">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-1616">ACS</span></span>

* <span data-ttu-id="48688-1617">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="48688-1617">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="48688-1618">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="48688-1618">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="48688-1619">AMS</span><span class="sxs-lookup"><span data-stu-id="48688-1619">AMS</span></span>

* <span data-ttu-id="48688-1620">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="48688-1620">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-1621">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-1621">Appservice</span></span>

* <span data-ttu-id="48688-1622">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="48688-1622">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="48688-1623">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="48688-1623">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="48688-1624">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="48688-1624">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="48688-1625">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="48688-1625">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="48688-1626">Lote AI</span><span class="sxs-lookup"><span data-stu-id="48688-1626">Batch AI</span></span>

* <span data-ttu-id="48688-1627">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="48688-1627">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="48688-1628">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="48688-1628">Cognitive Services</span></span>

* <span data-ttu-id="48688-1629">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="48688-1629">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="48688-1630">Consumo</span><span class="sxs-lookup"><span data-stu-id="48688-1630">Consumption</span></span>

* <span data-ttu-id="48688-1631">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="48688-1631">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="48688-1632">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-1632">Container</span></span>

* <span data-ttu-id="48688-1633">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="48688-1633">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="48688-1634">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="48688-1634">Cosmos DB</span></span>

* <span data-ttu-id="48688-1635">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="48688-1635">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="48688-1636">DMS</span><span class="sxs-lookup"><span data-stu-id="48688-1636">DMS</span></span>

* <span data-ttu-id="48688-1637">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="48688-1637">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="48688-1638">Extensão</span><span class="sxs-lookup"><span data-stu-id="48688-1638">Extension</span></span>

* <span data-ttu-id="48688-1639">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="48688-1639">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="48688-1640">Interativo</span><span class="sxs-lookup"><span data-stu-id="48688-1640">Interactive</span></span>

* <span data-ttu-id="48688-1641">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="48688-1641">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="48688-1642">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="48688-1642">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="48688-1643">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="48688-1643">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="48688-1644">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="48688-1644">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="48688-1645">Laboratório</span><span class="sxs-lookup"><span data-stu-id="48688-1645">Lab</span></span>

* <span data-ttu-id="48688-1646">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="48688-1646">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="48688-1647">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-1647">Network</span></span>

* <span data-ttu-id="48688-1648">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="48688-1648">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="48688-1649">Perfil</span><span class="sxs-lookup"><span data-stu-id="48688-1649">Profile</span></span>

* <span data-ttu-id="48688-1650">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="48688-1650">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="48688-1651">[ALTERAÇÃO SIGNIFICATIVA] `--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="48688-1651">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="48688-1652">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="48688-1652">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="48688-1653">Redis</span><span class="sxs-lookup"><span data-stu-id="48688-1653">Redis</span></span>

* <span data-ttu-id="48688-1654">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="48688-1654">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="48688-1655">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="48688-1655">Deprecated `redis list-all`.</span></span> <span data-ttu-id="48688-1656">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="48688-1656">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="48688-1657">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="48688-1657">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="48688-1658">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="48688-1658">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="48688-1659">Função</span><span class="sxs-lookup"><span data-stu-id="48688-1659">Role</span></span>

* <span data-ttu-id="48688-1660">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="48688-1660">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="48688-1661">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-1661">Storage</span></span>

* <span data-ttu-id="48688-1662">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="48688-1662">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="48688-1663">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="48688-1663">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="48688-1664">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="48688-1664">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="48688-1665">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="48688-1665">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="48688-1666">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="48688-1666">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="48688-1667">VM</span><span class="sxs-lookup"><span data-stu-id="48688-1667">VM</span></span>

* <span data-ttu-id="48688-1668">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="48688-1668">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="48688-1669">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="48688-1669">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="48688-1670">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="48688-1670">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="48688-1671">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="48688-1671">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="48688-1672">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="48688-1672">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="48688-1673">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="48688-1673">Added write accelerator support</span></span>
* <span data-ttu-id="48688-1674">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="48688-1674">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="48688-1675">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="48688-1675">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="48688-1676">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="48688-1676">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="48688-1677">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1677">April 10, 2018</span></span>

<span data-ttu-id="48688-1678">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="48688-1678">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="48688-1679">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-1679">ACR</span></span>

* <span data-ttu-id="48688-1680">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="48688-1680">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="48688-1681">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-1681">ACS</span></span>

* <span data-ttu-id="48688-1682">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="48688-1682">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-1683">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-1683">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="48688-1685">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="48688-1685">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="48688-1686">BatchAI</span><span class="sxs-lookup"><span data-stu-id="48688-1686">BatchAI</span></span>

* <span data-ttu-id="48688-1687">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="48688-1687">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="48688-1688">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="48688-1688">Job level mounting</span></span>
  - <span data-ttu-id="48688-1689">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="48688-1689">Environment variables with secret values</span></span>
  - <span data-ttu-id="48688-1690">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="48688-1690">Performance counters settings</span></span>
  - <span data-ttu-id="48688-1691">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="48688-1691">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="48688-1692">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="48688-1692">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="48688-1693">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="48688-1693">Usage and limits reporting</span></span>
  - <span data-ttu-id="48688-1694">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="48688-1694">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="48688-1695">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="48688-1695">Support for custom images</span></span>
  - <span data-ttu-id="48688-1696">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="48688-1696">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="48688-1697">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="48688-1697">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="48688-1698">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="48688-1698">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="48688-1699">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="48688-1699">National clouds are supported</span></span>
* <span data-ttu-id="48688-1700">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="48688-1700">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="48688-1701">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="48688-1701">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="48688-1702">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="48688-1702">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="48688-1703">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="48688-1703">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="48688-1704">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="48688-1704">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="48688-1705">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="48688-1705">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="48688-1706">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="48688-1706">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="48688-1707">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="48688-1707">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="48688-1708">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="48688-1708">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="48688-1709">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="48688-1709">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="48688-1710">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="48688-1710">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="48688-1711">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="48688-1711">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="48688-1712">[ALTERAÇÃO SIGNIFICATIVA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="48688-1712">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="48688-1713">Cobrança</span><span class="sxs-lookup"><span data-stu-id="48688-1713">Billing</span></span>

* <span data-ttu-id="48688-1714">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="48688-1714">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="48688-1715">Consumo</span><span class="sxs-lookup"><span data-stu-id="48688-1715">Consumption</span></span>

* <span data-ttu-id="48688-1716">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="48688-1716">Added `marketplace` commands</span></span>
* <span data-ttu-id="48688-1717">[ALTERAÇÃO SIGNIFICATIVA] `reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="48688-1717">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="48688-1718">[ALTERAÇÃO SIGNIFICATIVA] `reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="48688-1718">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="48688-1719">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="48688-1719">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="48688-1720">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="48688-1720">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="48688-1721">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="48688-1721">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="48688-1722">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-1722">Container</span></span>

* <span data-ttu-id="48688-1723">Adição dos parâmetros de montagem de volume de repositório git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="48688-1723">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="48688-1724">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="48688-1724">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="48688-1725">Extensão</span><span class="sxs-lookup"><span data-stu-id="48688-1725">Extension</span></span>

* <span data-ttu-id="48688-1726">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="48688-1726">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="48688-1727">Interativo</span><span class="sxs-lookup"><span data-stu-id="48688-1727">Interactive</span></span>

* <span data-ttu-id="48688-1728">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="48688-1728">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="48688-1729">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="48688-1729">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="48688-1730">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="48688-1730">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="48688-1731">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-1731">Network</span></span>

* <span data-ttu-id="48688-1732">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="48688-1732">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="48688-1733">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="48688-1733">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="48688-1734">#4910</span><span class="sxs-lookup"><span data-stu-id="48688-1734">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="48688-1735">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="48688-1735">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="48688-1736">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="48688-1736">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="48688-1737">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-1737">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="48688-1738">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-1738">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="48688-1739">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="48688-1739">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="48688-1740">Perfil</span><span class="sxs-lookup"><span data-stu-id="48688-1740">Profile</span></span>

* <span data-ttu-id="48688-1741">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="48688-1741">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="48688-1742">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="48688-1742">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="48688-1743">RDBMS</span><span class="sxs-lookup"><span data-stu-id="48688-1743">RDBMS</span></span>

* <span data-ttu-id="48688-1744">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="48688-1744">Added `georestore` command</span></span>
* <span data-ttu-id="48688-1745">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="48688-1745">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="48688-1746">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-1746">Resource</span></span>

* <span data-ttu-id="48688-1747">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="48688-1747">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="48688-1748">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="48688-1748">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="48688-1749">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-1749">SQL</span></span>

* <span data-ttu-id="48688-1750">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="48688-1750">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="48688-1751">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-1751">Storage</span></span>

* <span data-ttu-id="48688-1752">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="48688-1752">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="48688-1753">VM</span><span class="sxs-lookup"><span data-stu-id="48688-1753">VM</span></span>

* <span data-ttu-id="48688-1754">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="48688-1754">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="48688-1755">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="48688-1755">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="48688-1757">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="48688-1757">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="48688-1758">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="48688-1758">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="48688-1759">#5718</span><span class="sxs-lookup"><span data-stu-id="48688-1759">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="48688-1760">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="48688-1760">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="48688-1761">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1761">March 27, 2018</span></span>

<span data-ttu-id="48688-1762">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="48688-1762">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="48688-1763">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-1763">Core</span></span>

* <span data-ttu-id="48688-1764">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="48688-1764">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="48688-1765">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-1765">ACS</span></span>

* <span data-ttu-id="48688-1766">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="48688-1766">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-1767">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-1767">Appservice</span></span>

* <span data-ttu-id="48688-1768">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="48688-1768">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="48688-1769">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="48688-1769">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="48688-1770">Backup</span><span class="sxs-lookup"><span data-stu-id="48688-1770">Backup</span></span>

* <span data-ttu-id="48688-1771">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="48688-1771">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="48688-1772">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="48688-1772">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="48688-1773">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="48688-1773">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="48688-1774">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="48688-1774">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="48688-1775">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-1775">Container</span></span>

* <span data-ttu-id="48688-1776">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="48688-1776">Added `container exec` command.</span></span> <span data-ttu-id="48688-1777">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="48688-1777">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="48688-1778">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-1778">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="48688-1779">Extensão</span><span class="sxs-lookup"><span data-stu-id="48688-1779">Extension</span></span>

* <span data-ttu-id="48688-1780">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="48688-1780">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="48688-1781">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="48688-1781">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="48688-1782">[ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="48688-1782">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="48688-1783">Interativo</span><span class="sxs-lookup"><span data-stu-id="48688-1783">Interactive</span></span>

* <span data-ttu-id="48688-1784">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="48688-1784">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="48688-1785">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="48688-1785">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="48688-1786">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="48688-1786">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="48688-1787">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="48688-1787">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="48688-1788">Laboratório</span><span class="sxs-lookup"><span data-stu-id="48688-1788">Lab</span></span>

* <span data-ttu-id="48688-1789">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="48688-1789">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="48688-1790">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48688-1790">Monitor</span></span>

* <span data-ttu-id="48688-1791">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="48688-1791">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="48688-1792">Corrigido [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="48688-1792">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="48688-1793">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="48688-1793">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="48688-1794">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-1794">Network</span></span>

* <span data-ttu-id="48688-1795">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="48688-1795">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="48688-1796">Perfil</span><span class="sxs-lookup"><span data-stu-id="48688-1796">Profile</span></span>

* <span data-ttu-id="48688-1797">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="48688-1797">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="48688-1798">RDBMS</span><span class="sxs-lookup"><span data-stu-id="48688-1798">RDBMS</span></span>

* <span data-ttu-id="48688-1799">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="48688-1799">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="48688-1800">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-1800">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="48688-1802">Função</span><span class="sxs-lookup"><span data-stu-id="48688-1802">Role</span></span>

* <span data-ttu-id="48688-1803">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="48688-1803">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="48688-1804">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="48688-1804">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="48688-1805">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="48688-1805">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="48688-1806">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="48688-1806">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="48688-1807">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="48688-1807">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="48688-1808">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-1808">Storage</span></span>

* <span data-ttu-id="48688-1809">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="48688-1809">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="48688-1810">Corrigido [#4049](https://github.com/Azure/azure-cli/issues/4049): problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="48688-1810">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="48688-1811">VM</span><span class="sxs-lookup"><span data-stu-id="48688-1811">VM</span></span>

* <span data-ttu-id="48688-1812">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="48688-1812">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="48688-1813">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="48688-1813">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="48688-1814">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="48688-1814">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="48688-1815">[ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="48688-1815">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="48688-1816">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1816">March 13, 2018</span></span>

<span data-ttu-id="48688-1817">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="48688-1817">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="48688-1818">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-1818">ACR</span></span>

* <span data-ttu-id="48688-1819">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="48688-1819">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="48688-1820">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="48688-1820">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="48688-1821">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="48688-1821">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="48688-1822">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-1822">ACS</span></span>

* <span data-ttu-id="48688-1823">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="48688-1823">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="48688-1824">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="48688-1824">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="48688-1825">Supervisor</span><span class="sxs-lookup"><span data-stu-id="48688-1825">Advisor</span></span>

* <span data-ttu-id="48688-1826">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="48688-1826">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="48688-1827">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="48688-1827">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="48688-1828">[ALTERAÇÃO SIGNIFICATIVA] `advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="48688-1828">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="48688-1829">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="48688-1829">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="48688-1830">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="48688-1830">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-1831">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-1831">Appservice</span></span>

* <span data-ttu-id="48688-1832">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="48688-1832">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="48688-1833">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="48688-1833">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="48688-1834">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="48688-1834">Eventhubs</span></span>

* <span data-ttu-id="48688-1835">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="48688-1835">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="48688-1836">Extensão</span><span class="sxs-lookup"><span data-stu-id="48688-1836">Extension</span></span>

* <span data-ttu-id="48688-1837">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="48688-1837">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="48688-1838">Interativo</span><span class="sxs-lookup"><span data-stu-id="48688-1838">Interactive</span></span>

* <span data-ttu-id="48688-1839">Corrigido [#5625](https://github.com/Azure/azure-cli/issues/5625): manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="48688-1839">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="48688-1840">Corrigido [#3016](https://github.com/Azure/azure-cli/issues/3016): histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="48688-1840">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="48688-1841">Corrigido [#5688](https://github.com/Azure/azure-cli/issues/5688): as conclusões não aparecerão se o carregamento da tabela de comando encontrar uma exceção</span><span class="sxs-lookup"><span data-stu-id="48688-1841">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="48688-1842">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="48688-1842">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="48688-1843">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48688-1843">Monitor</span></span>

* <span data-ttu-id="48688-1844">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="48688-1844">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="48688-1845">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="48688-1845">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="48688-1846">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="48688-1846">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="48688-1847">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="48688-1847">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="48688-1848">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-1848">Network</span></span>

* <span data-ttu-id="48688-1849">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="48688-1849">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="48688-1850">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="48688-1850">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="48688-1851">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="48688-1851">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="48688-1852">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="48688-1852">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="48688-1853">Perfil</span><span class="sxs-lookup"><span data-stu-id="48688-1853">Profile</span></span>

* <span data-ttu-id="48688-1854">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="48688-1854">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="48688-1855">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="48688-1855">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="48688-1856">RDBMS</span><span class="sxs-lookup"><span data-stu-id="48688-1856">RDBMS</span></span>

* <span data-ttu-id="48688-1857">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="48688-1857">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="48688-1858">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="48688-1858">Service Bus</span></span>

* <span data-ttu-id="48688-1859">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="48688-1859">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="48688-1860">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-1860">Storage</span></span>

* <span data-ttu-id="48688-1861">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="48688-1861">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="48688-1862">Corrigido [#5286](https://github.com/Azure/azure-cli/issues/5286): os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="48688-1862">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="48688-1863">VM</span><span class="sxs-lookup"><span data-stu-id="48688-1863">VM</span></span>

* <span data-ttu-id="48688-1864">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="48688-1864">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="48688-1865">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="48688-1865">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="48688-1866">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="48688-1866">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="48688-1867">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="48688-1867">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="48688-1868">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1868">February 27, 2018</span></span>

<span data-ttu-id="48688-1869">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="48688-1869">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="48688-1870">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-1870">Core</span></span>

* <span data-ttu-id="48688-1871">Corrigido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="48688-1871">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="48688-1872">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="48688-1872">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="48688-1873">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="48688-1873">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="48688-1874">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-1874">ACS</span></span>

* <span data-ttu-id="48688-1875">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="48688-1875">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="48688-1876">Problema corrigido: permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="48688-1876">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="48688-1877">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="48688-1877">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="48688-1878">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="48688-1878">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-1879">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-1879">Appservice</span></span>

* <span data-ttu-id="48688-1880">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="48688-1880">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="48688-1881">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="48688-1881">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="48688-1882">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="48688-1882">Cognitive Services</span></span>

* <span data-ttu-id="48688-1883">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="48688-1883">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="48688-1884">Consumo</span><span class="sxs-lookup"><span data-stu-id="48688-1884">Consumption</span></span>

* <span data-ttu-id="48688-1885">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="48688-1885">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="48688-1886">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="48688-1886">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="48688-1887">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-1887">Container</span></span>

* <span data-ttu-id="48688-1888">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="48688-1888">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="48688-1889">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-1889">Network</span></span>

* <span data-ttu-id="48688-1890">Corrigido [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="48688-1890">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="48688-1891">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-1891">Resource</span></span>

* <span data-ttu-id="48688-1892">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="48688-1892">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="48688-1893">Função</span><span class="sxs-lookup"><span data-stu-id="48688-1893">Role</span></span>

* <span data-ttu-id="48688-1894">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="48688-1894">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="48688-1895">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-1895">SQL</span></span>

* <span data-ttu-id="48688-1896">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="48688-1896">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="48688-1897">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-1897">Storage</span></span>

* <span data-ttu-id="48688-1898">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="48688-1898">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="48688-1899">VM</span><span class="sxs-lookup"><span data-stu-id="48688-1899">VM</span></span>

* <span data-ttu-id="48688-1900">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="48688-1900">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="48688-1901">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1901">February 13, 2018</span></span>

<span data-ttu-id="48688-1902">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="48688-1902">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="48688-1903">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-1903">Core</span></span>

* <span data-ttu-id="48688-1904">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="48688-1904">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="48688-1905">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-1905">ACS</span></span>

* <span data-ttu-id="48688-1906">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="48688-1906">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="48688-1907">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="48688-1907">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="48688-1908">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="48688-1908">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="48688-1909">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="48688-1909">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="48688-1910">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="48688-1910">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="48688-1911">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="48688-1911">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="48688-1912">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="48688-1912">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="48688-1913">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="48688-1913">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-1914">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-1914">Appservice</span></span>

* <span data-ttu-id="48688-1915">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="48688-1915">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="48688-1916">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="48688-1916">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="48688-1917">CDN</span><span class="sxs-lookup"><span data-stu-id="48688-1917">CDN</span></span>

* <span data-ttu-id="48688-1918">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="48688-1918">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="48688-1919">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-1919">Container</span></span>

* <span data-ttu-id="48688-1920">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="48688-1920">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="48688-1921">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-1921">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48688-1922">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48688-1922">CosmosDB</span></span>

* <span data-ttu-id="48688-1923">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="48688-1923">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="48688-1924">Extensão</span><span class="sxs-lookup"><span data-stu-id="48688-1924">Extension</span></span>

* <span data-ttu-id="48688-1925">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-1925">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="48688-1926">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-1926">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="48688-1927">Comentários</span><span class="sxs-lookup"><span data-stu-id="48688-1927">Feedback</span></span>

* <span data-ttu-id="48688-1928">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="48688-1928">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="48688-1929">Interativo</span><span class="sxs-lookup"><span data-stu-id="48688-1929">Interactive</span></span>

* <span data-ttu-id="48688-1930">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="48688-1930">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="48688-1931">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="48688-1931">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="48688-1932">IoT</span><span class="sxs-lookup"><span data-stu-id="48688-1932">IoT</span></span>

* <span data-ttu-id="48688-1933">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="48688-1933">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="48688-1934">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="48688-1934">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="48688-1935">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-1935">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="48688-1936">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="48688-1936">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="48688-1937">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48688-1937">Monitor</span></span>

* <span data-ttu-id="48688-1938">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="48688-1938">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="48688-1939">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-1939">Network</span></span>

* <span data-ttu-id="48688-1940">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="48688-1940">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="48688-1941">Perfil</span><span class="sxs-lookup"><span data-stu-id="48688-1941">Profile</span></span>

* <span data-ttu-id="48688-1942">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="48688-1942">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="48688-1943">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-1943">Resource</span></span>

* <span data-ttu-id="48688-1944">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="48688-1944">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="48688-1945">Função</span><span class="sxs-lookup"><span data-stu-id="48688-1945">Role</span></span>

* <span data-ttu-id="48688-1946">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="48688-1946">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="48688-1947">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-1947">SQL</span></span>

* <span data-ttu-id="48688-1948">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="48688-1948">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="48688-1949">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="48688-1949">Added `sql db rename`</span></span>
* <span data-ttu-id="48688-1950">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="48688-1950">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="48688-1951">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-1951">Storage</span></span>

* <span data-ttu-id="48688-1952">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="48688-1952">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="48688-1953">VM</span><span class="sxs-lookup"><span data-stu-id="48688-1953">VM</span></span>

* <span data-ttu-id="48688-1954">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="48688-1954">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="48688-1955">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="48688-1955">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="48688-1956">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="48688-1956">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="48688-1957">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-1957">January 31, 2018</span></span>

<span data-ttu-id="48688-1958">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="48688-1958">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="48688-1959">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-1959">Core</span></span>

* <span data-ttu-id="48688-1960">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="48688-1960">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="48688-1961">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="48688-1961">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="48688-1962">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="48688-1962">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="48688-1963">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="48688-1963">Use `--verbose` to see</span></span>
* <span data-ttu-id="48688-1964">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="48688-1964">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="48688-1965">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-1965">ACS</span></span>

* <span data-ttu-id="48688-1966">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="48688-1966">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="48688-1967">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="48688-1967">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-1968">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-1968">Appservice</span></span>

* <span data-ttu-id="48688-1969">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="48688-1969">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="48688-1970">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="48688-1970">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="48688-1971">CDN</span><span class="sxs-lookup"><span data-stu-id="48688-1971">CDN</span></span>

* <span data-ttu-id="48688-1972">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="48688-1972">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48688-1973">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48688-1973">CosmosDB</span></span>

* <span data-ttu-id="48688-1974">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="48688-1974">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="48688-1975">Interativo</span><span class="sxs-lookup"><span data-stu-id="48688-1975">Interactive</span></span>

* <span data-ttu-id="48688-1976">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="48688-1976">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="48688-1977">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-1977">Network</span></span>

* <span data-ttu-id="48688-1978">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="48688-1978">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="48688-1979">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="48688-1979">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="48688-1980">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="48688-1980">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="48688-1981">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="48688-1981">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="48688-1982">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="48688-1982">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="48688-1983">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="48688-1983">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="48688-1984">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="48688-1984">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="48688-1985">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="48688-1985">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="48688-1986">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="48688-1986">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="48688-1987">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="48688-1987">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="48688-1988">Perfil</span><span class="sxs-lookup"><span data-stu-id="48688-1988">Profile</span></span>

* <span data-ttu-id="48688-1989">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="48688-1989">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="48688-1990">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-1990">Resource</span></span>

* <span data-ttu-id="48688-1991">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="48688-1991">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="48688-1992">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-1992">Storage</span></span>

* <span data-ttu-id="48688-1993">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="48688-1993">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="48688-1994">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="48688-1994">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="48688-1995">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="48688-1995">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="48688-1996">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="48688-1996">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="48688-1997">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="48688-1997">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="48688-1998">VM</span><span class="sxs-lookup"><span data-stu-id="48688-1998">VM</span></span>

* <span data-ttu-id="48688-1999">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="48688-1999">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="48688-2000">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="48688-2000">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="48688-2001">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="48688-2001">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="48688-2002">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="48688-2002">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="48688-2003">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="48688-2003">January 17, 2018</span></span>

<span data-ttu-id="48688-2004">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="48688-2004">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="48688-2005">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-2005">ACR</span></span>

* <span data-ttu-id="48688-2006">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="48688-2006">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="48688-2007">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="48688-2007">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="48688-2008">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-2008">ACS</span></span>

* <span data-ttu-id="48688-2009">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="48688-2009">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="48688-2010">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="48688-2010">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-2011">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-2011">Appservice</span></span>

* <span data-ttu-id="48688-2012">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="48688-2012">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="48688-2013">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="48688-2013">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="48688-2014">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="48688-2014">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="48688-2015">Backup</span><span class="sxs-lookup"><span data-stu-id="48688-2015">Backup</span></span>

* <span data-ttu-id="48688-2016">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="48688-2016">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="48688-2017">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="48688-2017">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="48688-2018">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="48688-2018">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="48688-2019">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="48688-2019">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="48688-2020">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="48688-2020">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="48688-2021">Lote</span><span class="sxs-lookup"><span data-stu-id="48688-2021">Batch</span></span>

* <span data-ttu-id="48688-2022">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="48688-2022">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="48688-2023">Nuvem</span><span class="sxs-lookup"><span data-stu-id="48688-2023">Cloud</span></span>

* <span data-ttu-id="48688-2024">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="48688-2024">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="48688-2025">Consumo</span><span class="sxs-lookup"><span data-stu-id="48688-2025">Consumption</span></span>

* <span data-ttu-id="48688-2026">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="48688-2026">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="48688-2027">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="48688-2027">Event Grid</span></span>

* <span data-ttu-id="48688-2028">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="48688-2028">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="48688-2029">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="48688-2029">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="48688-2030">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="48688-2030">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="48688-2031">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="48688-2031">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="48688-2032">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="48688-2032">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="48688-2033">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="48688-2033">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="48688-2034">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="48688-2034">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="48688-2035">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="48688-2035">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="48688-2036">Interativo</span><span class="sxs-lookup"><span data-stu-id="48688-2036">Interactive</span></span>

* <span data-ttu-id="48688-2037">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="48688-2037">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="48688-2038">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="48688-2038">Fixed errors on startup</span></span>
* <span data-ttu-id="48688-2039">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="48688-2039">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="48688-2040">IoT</span><span class="sxs-lookup"><span data-stu-id="48688-2040">IoT</span></span>

* <span data-ttu-id="48688-2041">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="48688-2041">Added support for device provisioning service</span></span>
* <span data-ttu-id="48688-2042">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="48688-2042">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="48688-2043">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="48688-2043">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="48688-2044">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48688-2044">Monitor</span></span>

* <span data-ttu-id="48688-2045">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="48688-2045">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="48688-2046">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="48688-2046">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="48688-2047">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="48688-2047">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="48688-2048">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-2048">Network</span></span>

* <span data-ttu-id="48688-2049">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="48688-2049">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="48688-2050">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-2050">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="48688-2051">Perfil</span><span class="sxs-lookup"><span data-stu-id="48688-2051">Profile</span></span>

* <span data-ttu-id="48688-2052">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="48688-2052">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="48688-2053">Função</span><span class="sxs-lookup"><span data-stu-id="48688-2053">Role</span></span>

* <span data-ttu-id="48688-2054">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="48688-2054">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="48688-2055">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="48688-2055">Service Fabric</span></span>

* <span data-ttu-id="48688-2056">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="48688-2056">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="48688-2057">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="48688-2057">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="48688-2058">VM</span><span class="sxs-lookup"><span data-stu-id="48688-2058">VM</span></span>

* <span data-ttu-id="48688-2059">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="48688-2059">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="48688-2060">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="48688-2060">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="48688-2061">[ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="48688-2061">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="48688-2062">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="48688-2062">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="48688-2063">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="48688-2063">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="48688-2064">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="48688-2064">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="48688-2065">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="48688-2065">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="48688-2066">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="48688-2066">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="48688-2067">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="48688-2067">December 19, 2017</span></span>

<span data-ttu-id="48688-2068">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="48688-2068">Version 2.0.23</span></span>

* <span data-ttu-id="48688-2069">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="48688-2069">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="48688-2070">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-2070">Container</span></span>

* <span data-ttu-id="48688-2071">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-2071">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="48688-2072">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-2072">Network</span></span>

* <span data-ttu-id="48688-2073">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-2073">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="48688-2074">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-2074">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="48688-2075">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-2075">Storage</span></span>

* <span data-ttu-id="48688-2076">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="48688-2076">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="48688-2077">VM</span><span class="sxs-lookup"><span data-stu-id="48688-2077">VM</span></span>

* <span data-ttu-id="48688-2078">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="48688-2078">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="48688-2079">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="48688-2079">December 5, 2017</span></span>

<span data-ttu-id="48688-2080">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="48688-2080">Version 2.0.22</span></span>

* <span data-ttu-id="48688-2081">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="48688-2081">Removed `az component` commands.</span></span> <span data-ttu-id="48688-2082">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="48688-2082">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="48688-2083">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-2083">Core</span></span>
* <span data-ttu-id="48688-2084">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="48688-2084">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="48688-2085">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="48688-2085">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="48688-2086">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-2086">ACS</span></span>

* <span data-ttu-id="48688-2087">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="48688-2087">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="48688-2088">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="48688-2088">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="48688-2089">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="48688-2089">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="48688-2090">Supervisor</span><span class="sxs-lookup"><span data-stu-id="48688-2090">Advisor</span></span>

* <span data-ttu-id="48688-2091">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="48688-2091">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-2092">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-2092">Appservice</span></span>

* <span data-ttu-id="48688-2093">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="48688-2093">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="48688-2094">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="48688-2094">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="48688-2095">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="48688-2095">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="48688-2096">Consumo</span><span class="sxs-lookup"><span data-stu-id="48688-2096">Consumption</span></span>

* <span data-ttu-id="48688-2097">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="48688-2097">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="48688-2098">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-2098">Container</span></span>

* <span data-ttu-id="48688-2099">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="48688-2099">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="48688-2100">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48688-2100">Monitor</span></span>

* <span data-ttu-id="48688-2101">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="48688-2101">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="48688-2102">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-2102">Resource</span></span>

* <span data-ttu-id="48688-2103">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="48688-2103">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="48688-2104">Função</span><span class="sxs-lookup"><span data-stu-id="48688-2104">Role</span></span>

* <span data-ttu-id="48688-2105">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="48688-2105">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="48688-2106">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="48688-2106">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="48688-2107">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="48688-2107">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="48688-2108">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-2108">SQL</span></span>

* <span data-ttu-id="48688-2109">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="48688-2109">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="48688-2110">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="48688-2110">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="48688-2111">VM</span><span class="sxs-lookup"><span data-stu-id="48688-2111">VM</span></span>

* <span data-ttu-id="48688-2112">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="48688-2112">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="48688-2113">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="48688-2113">November 14, 2017</span></span>

<span data-ttu-id="48688-2114">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="48688-2114">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="48688-2115">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-2115">ACR</span></span>

* <span data-ttu-id="48688-2116">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="48688-2116">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="48688-2117">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-2117">ACS</span></span>

* <span data-ttu-id="48688-2118">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="48688-2118">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="48688-2119">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="48688-2119">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="48688-2120">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="48688-2120">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="48688-2121">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="48688-2121">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="48688-2122">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="48688-2122">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-2123">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-2123">Appservice</span></span>

* <span data-ttu-id="48688-2124">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="48688-2124">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="48688-2125">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="48688-2125">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="48688-2126">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="48688-2126">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="48688-2127">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="48688-2127">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="48688-2128">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="48688-2128">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="48688-2129">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="48688-2129">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="48688-2130">Lote</span><span class="sxs-lookup"><span data-stu-id="48688-2130">Batch</span></span>

* <span data-ttu-id="48688-2131">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="48688-2131">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="48688-2132">Batchai</span><span class="sxs-lookup"><span data-stu-id="48688-2132">Batchai</span></span>

* <span data-ttu-id="48688-2133">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="48688-2133">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="48688-2134">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="48688-2134">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="48688-2135">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="48688-2135">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="48688-2136">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="48688-2136">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="48688-2137">Nuvem</span><span class="sxs-lookup"><span data-stu-id="48688-2137">Cloud</span></span>

* <span data-ttu-id="48688-2138">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="48688-2138">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="48688-2139">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-2139">Container</span></span>

* <span data-ttu-id="48688-2140">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="48688-2140">Added support to open multiple ports</span></span>
* <span data-ttu-id="48688-2141">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="48688-2141">Added container group restart policy</span></span>
* <span data-ttu-id="48688-2142">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="48688-2142">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="48688-2143">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="48688-2143">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="48688-2144">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="48688-2144">Data Lake Analytics</span></span>

* <span data-ttu-id="48688-2145">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="48688-2145">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="48688-2146">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="48688-2146">Data Lake Store</span></span>

* <span data-ttu-id="48688-2147">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="48688-2147">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="48688-2148">Extensão</span><span class="sxs-lookup"><span data-stu-id="48688-2148">Extension</span></span>

* <span data-ttu-id="48688-2149">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="48688-2149">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="48688-2150">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="48688-2150">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="48688-2151">IoT</span><span class="sxs-lookup"><span data-stu-id="48688-2151">IoT</span></span>

* <span data-ttu-id="48688-2152">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="48688-2152">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="48688-2153">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48688-2153">Monitor</span></span>

* <span data-ttu-id="48688-2154">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="48688-2154">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="48688-2155">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-2155">Network</span></span>

* <span data-ttu-id="48688-2156">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="48688-2156">Added support for CAA DNS records</span></span>
* <span data-ttu-id="48688-2157">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="48688-2157">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="48688-2158">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="48688-2158">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="48688-2159">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="48688-2159">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="48688-2160">Reservas</span><span class="sxs-lookup"><span data-stu-id="48688-2160">Reservations</span></span>

* <span data-ttu-id="48688-2161">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="48688-2161">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="48688-2162">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-2162">Resource</span></span>

* <span data-ttu-id="48688-2163">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="48688-2163">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="48688-2164">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-2164">SQL</span></span>

* <span data-ttu-id="48688-2165">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-2165">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="48688-2166">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-2166">Storage</span></span>

* <span data-ttu-id="48688-2167">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="48688-2167">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="48688-2168">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="48688-2168">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="48688-2169">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="48688-2169">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="48688-2170">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="48688-2170">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="48688-2171">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="48688-2171">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="48688-2172">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="48688-2172">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="48688-2173">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-2173">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="48688-2174">VM</span><span class="sxs-lookup"><span data-stu-id="48688-2174">VM</span></span>

* <span data-ttu-id="48688-2175">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="48688-2175">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="48688-2176">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="48688-2176">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="48688-2177">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="48688-2177">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="48688-2178">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="48688-2178">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="48688-2179">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="48688-2179">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="48688-2180">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="48688-2180">October 24, 2017</span></span>

<span data-ttu-id="48688-2181">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="48688-2181">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="48688-2182">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-2182">Core</span></span>

* <span data-ttu-id="48688-2183">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="48688-2183">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="48688-2184">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-2184">ACR</span></span>

* <span data-ttu-id="48688-2185">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="48688-2185">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="48688-2186">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="48688-2186">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="48688-2187">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="48688-2187">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="48688-2188">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-2188">ACS</span></span>

* <span data-ttu-id="48688-2189">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="48688-2189">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="48688-2190">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="48688-2190">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-2191">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-2191">Appservice</span></span>

* <span data-ttu-id="48688-2192">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="48688-2192">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="48688-2193">Componente</span><span class="sxs-lookup"><span data-stu-id="48688-2193">Component</span></span>

* <span data-ttu-id="48688-2194">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="48688-2194">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="48688-2195">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48688-2195">Monitor</span></span>

* <span data-ttu-id="48688-2196">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="48688-2196">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="48688-2197">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-2197">Resource</span></span>

* <span data-ttu-id="48688-2198">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="48688-2198">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="48688-2199">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="48688-2199">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="48688-2200">VM</span><span class="sxs-lookup"><span data-stu-id="48688-2200">VM</span></span>

* <span data-ttu-id="48688-2201">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="48688-2201">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="48688-2202">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="48688-2202">October 9, 2017</span></span>

<span data-ttu-id="48688-2203">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="48688-2203">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="48688-2204">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-2204">Core</span></span>

* <span data-ttu-id="48688-2205">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="48688-2205">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-2206">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-2206">Appservice</span></span>

* <span data-ttu-id="48688-2207">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="48688-2207">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="48688-2208">Lote</span><span class="sxs-lookup"><span data-stu-id="48688-2208">Batch</span></span>

* <span data-ttu-id="48688-2209">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="48688-2209">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="48688-2210">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="48688-2210">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="48688-2211">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="48688-2211">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="48688-2212">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="48688-2212">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="48688-2213">Batchai</span><span class="sxs-lookup"><span data-stu-id="48688-2213">Batchai</span></span>

* <span data-ttu-id="48688-2214">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="48688-2214">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="48688-2215">Keyvault</span><span class="sxs-lookup"><span data-stu-id="48688-2215">Keyvault</span></span>

* <span data-ttu-id="48688-2216">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="48688-2216">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="48688-2217">(#4448)</span><span class="sxs-lookup"><span data-stu-id="48688-2217">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="48688-2218">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-2218">Network</span></span>

* <span data-ttu-id="48688-2219">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="48688-2219">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="48688-2220">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="48688-2220">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="48688-2221">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-2221">Resource</span></span>

* <span data-ttu-id="48688-2222">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="48688-2222">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="48688-2223">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="48688-2223">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="48688-2224">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="48688-2224">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="48688-2225">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="48688-2225">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="48688-2226">Sql</span><span class="sxs-lookup"><span data-stu-id="48688-2226">Sql</span></span>

* <span data-ttu-id="48688-2227">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="48688-2227">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="48688-2228">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="48688-2228">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="48688-2229">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="48688-2229">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="48688-2230">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-2230">Storage</span></span>

* <span data-ttu-id="48688-2231">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="48688-2231">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="48688-2232">VM</span><span class="sxs-lookup"><span data-stu-id="48688-2232">Vm</span></span>

* <span data-ttu-id="48688-2233">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="48688-2233">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="48688-2234">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="48688-2234">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="48688-2235">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="48688-2235">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="48688-2236">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="48688-2236">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="48688-2237">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="48688-2237">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="48688-2238">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="48688-2238">September 22, 2017</span></span>

<span data-ttu-id="48688-2239">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="48688-2239">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="48688-2240">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-2240">Resource</span></span>

* <span data-ttu-id="48688-2241">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="48688-2241">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="48688-2242">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="48688-2242">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="48688-2243">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="48688-2243">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="48688-2244">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="48688-2244">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="48688-2245">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-2245">Network</span></span>

* <span data-ttu-id="48688-2246">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="48688-2246">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="48688-2247">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="48688-2247">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="48688-2248">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="48688-2248">Added `asg` application security group commands</span></span>
* <span data-ttu-id="48688-2249">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="48688-2249">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="48688-2250">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-2250">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="48688-2251">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-2251">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="48688-2252">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="48688-2252">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="48688-2253">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-2253">Storage</span></span>

* <span data-ttu-id="48688-2254">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="48688-2254">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="48688-2255">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="48688-2255">Eventgrid</span></span>

* <span data-ttu-id="48688-2256">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="48688-2256">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="48688-2257">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-2257">SQL</span></span>

* <span data-ttu-id="48688-2258">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="48688-2258">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="48688-2259">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="48688-2259">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="48688-2260">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-2260">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="48688-2261">Keyvault</span><span class="sxs-lookup"><span data-stu-id="48688-2261">Keyvault</span></span>

* <span data-ttu-id="48688-2262">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="48688-2262">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="48688-2263">VM</span><span class="sxs-lookup"><span data-stu-id="48688-2263">VM</span></span>

* <span data-ttu-id="48688-2264">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="48688-2264">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="48688-2265">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="48688-2265">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="48688-2266">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="48688-2266">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="48688-2267">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="48688-2267">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="48688-2268">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="48688-2268">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="48688-2269">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="48688-2269">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="48688-2270">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-2270">ACS</span></span>

* <span data-ttu-id="48688-2271">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="48688-2271">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-2272">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-2272">Appservice</span></span>

* <span data-ttu-id="48688-2273">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="48688-2273">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="48688-2274">Backup</span><span class="sxs-lookup"><span data-stu-id="48688-2274">Backup</span></span>

* <span data-ttu-id="48688-2275">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="48688-2275">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="48688-2276">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="48688-2276">September 11, 2017</span></span>

<span data-ttu-id="48688-2277">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="48688-2277">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="48688-2278">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-2278">Core</span></span>

* <span data-ttu-id="48688-2279">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="48688-2279">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="48688-2280">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="48688-2280">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="48688-2281">Acs</span><span class="sxs-lookup"><span data-stu-id="48688-2281">Acs</span></span>

* <span data-ttu-id="48688-2282">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="48688-2282">Added `acs list-locations` command</span></span>
* <span data-ttu-id="48688-2283">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="48688-2283">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-2284">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-2284">Appservice</span></span>

* <span data-ttu-id="48688-2285">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="48688-2285">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="48688-2286">CDN</span><span class="sxs-lookup"><span data-stu-id="48688-2286">CDN</span></span>

* <span data-ttu-id="48688-2287">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="48688-2287">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="48688-2288">Extensão</span><span class="sxs-lookup"><span data-stu-id="48688-2288">Extension</span></span>

* <span data-ttu-id="48688-2289">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="48688-2289">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="48688-2290">Keyvault</span><span class="sxs-lookup"><span data-stu-id="48688-2290">Keyvault</span></span>

* <span data-ttu-id="48688-2291">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="48688-2291">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="48688-2292">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-2292">Network</span></span>

* <span data-ttu-id="48688-2293">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="48688-2293">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="48688-2294">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="48688-2294">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="48688-2295">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="48688-2295">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="48688-2296">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="48688-2296">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="48688-2297">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="48688-2297">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="48688-2298">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-2298">Resource</span></span>

* <span data-ttu-id="48688-2299">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="48688-2299">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="48688-2300">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="48688-2300">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="48688-2301">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="48688-2301">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="48688-2302">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="48688-2302">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="48688-2303">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-2303">SQL</span></span>

* <span data-ttu-id="48688-2304">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="48688-2304">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="48688-2305">VM</span><span class="sxs-lookup"><span data-stu-id="48688-2305">VM</span></span>

* <span data-ttu-id="48688-2306">Corrigido: não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="48688-2306">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="48688-2307">Corrigido: usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="48688-2307">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="48688-2308">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="48688-2308">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="48688-2309">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="48688-2309">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="48688-2310">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="48688-2310">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="48688-2311">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="48688-2311">August 31, 2017</span></span>

<span data-ttu-id="48688-2312">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="48688-2312">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="48688-2313">Keyvault</span><span class="sxs-lookup"><span data-stu-id="48688-2313">Keyvault</span></span>

* <span data-ttu-id="48688-2314">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="48688-2314">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="48688-2315">Sf</span><span class="sxs-lookup"><span data-stu-id="48688-2315">Sf</span></span>

* <span data-ttu-id="48688-2316">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="48688-2316">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="48688-2317">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-2317">Storage</span></span>

* <span data-ttu-id="48688-2318">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="48688-2318">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="48688-2319">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="48688-2319">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="48688-2320">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="48688-2320">August 28, 2017</span></span>

<span data-ttu-id="48688-2321">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="48688-2321">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="48688-2322">CLI</span><span class="sxs-lookup"><span data-stu-id="48688-2322">CLI</span></span>

* <span data-ttu-id="48688-2323">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="48688-2323">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="48688-2324">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-2324">ACS</span></span>

* <span data-ttu-id="48688-2325">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="48688-2325">Corrected preview regions</span></span>
* <span data-ttu-id="48688-2326">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="48688-2326">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="48688-2327">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="48688-2327">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-2328">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-2328">Appservice</span></span>

* <span data-ttu-id="48688-2329">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="48688-2329">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="48688-2330">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="48688-2330">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="48688-2331">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="48688-2331">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="48688-2332">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="48688-2332">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="48688-2333">Corrigido: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="48688-2333">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="48688-2334">IoT</span><span class="sxs-lookup"><span data-stu-id="48688-2334">IoT</span></span>

* <span data-ttu-id="48688-2335">Corrigido #3934: a criação de uma política não limpa mais as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="48688-2335">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="48688-2336">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-2336">Network</span></span>

* <span data-ttu-id="48688-2337">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="48688-2337">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="48688-2338">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-2338">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="48688-2339">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="48688-2339">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="48688-2340">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="48688-2340">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="48688-2341">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="48688-2341">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="48688-2342">Perfil</span><span class="sxs-lookup"><span data-stu-id="48688-2342">Profile</span></span>

* <span data-ttu-id="48688-2343">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="48688-2343">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="48688-2344">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="48688-2344">Service Fabric</span></span>

* <span data-ttu-id="48688-2345">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="48688-2345">Preview release</span></span>
* <span data-ttu-id="48688-2346">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="48688-2346">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="48688-2347">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="48688-2347">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="48688-2348">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="48688-2348">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="48688-2349">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-2349">Storage</span></span>

* <span data-ttu-id="48688-2350">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="48688-2350">Enabled setting blob tier</span></span>
* <span data-ttu-id="48688-2351">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="48688-2351">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="48688-2352">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="48688-2352">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="48688-2353">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="48688-2353">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="48688-2354">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="48688-2354">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="48688-2355">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="48688-2355">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="48688-2356">VM</span><span class="sxs-lookup"><span data-stu-id="48688-2356">VM</span></span>

* <span data-ttu-id="48688-2357">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="48688-2357">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="48688-2358">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="48688-2358">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="48688-2359">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="48688-2359">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="48688-2360">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="48688-2360">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="48688-2361">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="48688-2361">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="48688-2362">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="48688-2362">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="48688-2363">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="48688-2363">August 15, 2017</span></span>

<span data-ttu-id="48688-2364">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="48688-2364">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="48688-2365">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-2365">ACS</span></span>

* <span data-ttu-id="48688-2366">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="48688-2366">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-2367">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-2367">Appservice</span></span>

* <span data-ttu-id="48688-2368">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="48688-2368">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="48688-2369">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="48688-2369">Event Grid</span></span>

* <span data-ttu-id="48688-2370">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="48688-2370">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="48688-2371">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="48688-2371">August 11, 2017</span></span>

<span data-ttu-id="48688-2372">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="48688-2372">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="48688-2373">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-2373">ACS</span></span>

* <span data-ttu-id="48688-2374">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="48688-2374">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="48688-2375">Lote</span><span class="sxs-lookup"><span data-stu-id="48688-2375">Batch</span></span>

* <span data-ttu-id="48688-2376">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="48688-2376">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="48688-2377">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="48688-2377">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="48688-2378">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="48688-2378">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="48688-2379">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://”</span><span class="sxs-lookup"><span data-stu-id="48688-2379">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="48688-2380">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="48688-2380">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="48688-2381">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="48688-2381">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="48688-2382">Componente</span><span class="sxs-lookup"><span data-stu-id="48688-2382">Component</span></span>

* <span data-ttu-id="48688-2383">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="48688-2383">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="48688-2384">Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-2384">Container</span></span>

* <span data-ttu-id="48688-2385">`create`: corrigido o problema em que o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="48688-2385">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="48688-2386">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="48688-2386">Data Lake Store</span></span>

* <span data-ttu-id="48688-2387">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="48688-2387">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="48688-2388">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="48688-2388">Event Grid</span></span>

* <span data-ttu-id="48688-2389">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="48688-2389">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="48688-2390">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-2390">Network</span></span>

* <span data-ttu-id="48688-2391">`lb`: corrigido o problema em que os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="48688-2391">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="48688-2392">`application-gateway {subresource} delete`: corrigido o problema em que `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="48688-2392">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="48688-2393">`application-gateway http-settings update`: corrigido o problema em que `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="48688-2393">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="48688-2394">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="48688-2394">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="48688-2395">Perfil</span><span class="sxs-lookup"><span data-stu-id="48688-2395">Profile</span></span>

* <span data-ttu-id="48688-2396">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="48688-2396">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="48688-2397">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-2397">Storage</span></span>

* <span data-ttu-id="48688-2398">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="48688-2398">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="48688-2399">VM</span><span class="sxs-lookup"><span data-stu-id="48688-2399">VM</span></span>

* <span data-ttu-id="48688-2400">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="48688-2400">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="48688-2401">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="48688-2401">Exposed `list-skus` command</span></span>
* <span data-ttu-id="48688-2402">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="48688-2402">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="48688-2403">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="48688-2403">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="48688-2404">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="48688-2404">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="48688-2405">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="48688-2405">July 28, 2017</span></span>

<span data-ttu-id="48688-2406">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="48688-2406">Version 2.0.12</span></span>

* <span data-ttu-id="48688-2407">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-2407">Added container commands</span></span>
* <span data-ttu-id="48688-2408">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="48688-2408">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="48688-2409">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-2409">Core</span></span>

* <span data-ttu-id="48688-2410">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="48688-2410">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="48688-2411">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="48688-2411">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="48688-2412">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="48688-2412">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="48688-2413">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="48688-2413">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="48688-2414">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="48688-2414">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="48688-2415">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="48688-2415">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="48688-2416">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="48688-2416">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="48688-2417">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="48688-2417">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="48688-2418">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="48688-2418">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="48688-2419">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="48688-2419">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="48688-2420">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="48688-2420">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="48688-2421">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="48688-2421">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="48688-2422">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="48688-2422">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="48688-2423">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="48688-2423">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="48688-2424">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="48688-2424">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="48688-2425">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="48688-2425">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="48688-2426">ACR</span><span class="sxs-lookup"><span data-stu-id="48688-2426">ACR</span></span>

* <span data-ttu-id="48688-2427">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="48688-2427">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="48688-2428">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="48688-2428">Support SKU update for managed registries</span></span>
* <span data-ttu-id="48688-2429">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="48688-2429">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="48688-2430">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="48688-2430">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="48688-2431">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="48688-2431">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="48688-2432">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="48688-2432">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="48688-2433">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-2433">ACS</span></span>

* <span data-ttu-id="48688-2434">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="48688-2434">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-2435">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-2435">Appservice</span></span>

* <span data-ttu-id="48688-2436">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="48688-2436">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="48688-2437">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="48688-2437">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="48688-2438">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="48688-2438">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="48688-2439">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="48688-2439">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="48688-2440">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="48688-2440">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="48688-2441">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="48688-2441">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="48688-2442">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="48688-2442">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="48688-2443">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="48688-2443">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="48688-2444">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="48688-2444">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="48688-2445">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="48688-2445">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="48688-2446">Lote</span><span class="sxs-lookup"><span data-stu-id="48688-2446">Batch</span></span>

* <span data-ttu-id="48688-2447">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="48688-2447">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="48688-2448">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="48688-2448">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="48688-2449">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="48688-2449">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="48688-2450">CDN</span><span class="sxs-lookup"><span data-stu-id="48688-2450">CDN</span></span>

* <span data-ttu-id="48688-2451">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="48688-2451">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="48688-2452">Nuvem</span><span class="sxs-lookup"><span data-stu-id="48688-2452">Cloud</span></span>

* <span data-ttu-id="48688-2453">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="48688-2453">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="48688-2454">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="48688-2454">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="48688-2455">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="48688-2455">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="48688-2456">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="48688-2456">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="48688-2457">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="48688-2457">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48688-2458">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48688-2458">CosmosDB</span></span>

* <span data-ttu-id="48688-2459">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="48688-2459">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="48688-2460">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="48688-2460">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="48688-2461">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="48688-2461">Data Lake Analytics</span></span>

* <span data-ttu-id="48688-2462">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="48688-2462">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="48688-2463">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="48688-2463">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="48688-2464">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="48688-2464">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="48688-2465">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="48688-2465">Data Lake Store</span></span>

* <span data-ttu-id="48688-2466">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="48688-2466">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="48688-2467">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="48688-2467">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="48688-2468">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="48688-2468">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="48688-2469">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="48688-2469">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="48688-2470">Interativo</span><span class="sxs-lookup"><span data-stu-id="48688-2470">Interactive</span></span>

* <span data-ttu-id="48688-2471">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="48688-2471">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="48688-2472">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="48688-2472">Increased test coverage</span></span>
* <span data-ttu-id="48688-2473">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="48688-2473">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="48688-2474">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="48688-2474">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="48688-2475">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="48688-2475">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="48688-2476">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="48688-2476">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="48688-2477">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="48688-2477">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="48688-2478">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="48688-2478">Added `--progress` flag</span></span>
* <span data-ttu-id="48688-2479">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="48688-2479">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="48688-2480">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="48688-2480">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="48688-2481">IoT</span><span class="sxs-lookup"><span data-stu-id="48688-2481">IoT</span></span>

* <span data-ttu-id="48688-2482">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="48688-2482">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="48688-2483">(#3934)</span><span class="sxs-lookup"><span data-stu-id="48688-2483">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="48688-2484">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="48688-2484">Key vault</span></span>

* <span data-ttu-id="48688-2485">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="48688-2485">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="48688-2486">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="48688-2486">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="48688-2487">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="48688-2487">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="48688-2488">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="48688-2488">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="48688-2489">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="48688-2489">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="48688-2490">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="48688-2490">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="48688-2491">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="48688-2491">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="48688-2492">(#3307)</span><span class="sxs-lookup"><span data-stu-id="48688-2492">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="48688-2493">Laboratório</span><span class="sxs-lookup"><span data-stu-id="48688-2493">Lab</span></span>

* <span data-ttu-id="48688-2494">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="48688-2494">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="48688-2495">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="48688-2495">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="48688-2496">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48688-2496">Monitor</span></span>

* <span data-ttu-id="48688-2497">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="48688-2497">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="48688-2498">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="48688-2498">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="48688-2499">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="48688-2499">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="48688-2500">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="48688-2500">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="48688-2501">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="48688-2501">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="48688-2502">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="48688-2502">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="48688-2503">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="48688-2503">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="48688-2504">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="48688-2504">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="48688-2505">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="48688-2505">`location` no longer required</span></span>
  * <span data-ttu-id="48688-2506">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="48688-2506">Add name and ID support for target</span></span>
  * <span data-ttu-id="48688-2507">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="48688-2507">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="48688-2508">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="48688-2508">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="48688-2509">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="48688-2509">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="48688-2510">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="48688-2510">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="48688-2511">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="48688-2511">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="48688-2512">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="48688-2512">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="48688-2513">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-2513">Network</span></span>

* <span data-ttu-id="48688-2514">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="48688-2514">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="48688-2515">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="48688-2515">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="48688-2516">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="48688-2516">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="48688-2517">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="48688-2517">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="48688-2518">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="48688-2518">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="48688-2519">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="48688-2519">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="48688-2520">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="48688-2520">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="48688-2521">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="48688-2521">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="48688-2522">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="48688-2522">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="48688-2523">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="48688-2523">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="48688-2524">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="48688-2524">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="48688-2525">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="48688-2525">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="48688-2526">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="48688-2526">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="48688-2527">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="48688-2527">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="48688-2528">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="48688-2528">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="48688-2529">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="48688-2529">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="48688-2530">Adicionado o suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para --dns-servers</span><span class="sxs-lookup"><span data-stu-id="48688-2530">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="48688-2531">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="48688-2531">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="48688-2532">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="48688-2532">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="48688-2533">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="48688-2533">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="48688-2534">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="48688-2534">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="48688-2535">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="48688-2535">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="48688-2536">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="48688-2536">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="48688-2537">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="48688-2537">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="48688-2538">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="48688-2538">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="48688-2539">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="48688-2539">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="48688-2540">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="48688-2540">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="48688-2541">Perfil</span><span class="sxs-lookup"><span data-stu-id="48688-2541">Profile</span></span>

* <span data-ttu-id="48688-2542">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="48688-2542">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="48688-2543">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="48688-2543">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="48688-2544">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="48688-2544">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="48688-2545">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="48688-2545">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="48688-2546">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="48688-2546">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="48688-2547">RDBMS</span><span class="sxs-lookup"><span data-stu-id="48688-2547">RDBMS</span></span>

* <span data-ttu-id="48688-2548">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="48688-2548">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="48688-2549">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="48688-2549">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="48688-2550">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="48688-2550">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="48688-2551">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="48688-2551">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="48688-2552">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-2552">Resource</span></span>

* <span data-ttu-id="48688-2553">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="48688-2553">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="48688-2554">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="48688-2554">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="48688-2555">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="48688-2555">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="48688-2556">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="48688-2556">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="48688-2557">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="48688-2557">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="48688-2558">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="48688-2558">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="48688-2559">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="48688-2559">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="48688-2560">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="48688-2560">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="48688-2561">Função</span><span class="sxs-lookup"><span data-stu-id="48688-2561">Role</span></span>

* <span data-ttu-id="48688-2562">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="48688-2562">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="48688-2563">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="48688-2563">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="48688-2564">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="48688-2564">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="48688-2565">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="48688-2565">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="48688-2566">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="48688-2566">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="48688-2567">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="48688-2567">Service Fabric</span></span>
* <span data-ttu-id="48688-2568">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="48688-2568">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="48688-2569">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="48688-2569">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="48688-2570">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="48688-2570">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="48688-2571">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-2571">SQL</span></span>

* <span data-ttu-id="48688-2572">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="48688-2572">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="48688-2573">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="48688-2573">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="48688-2574">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="48688-2574">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="48688-2575">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-2575">Storage</span></span>

* <span data-ttu-id="48688-2576">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="48688-2576">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="48688-2577">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="48688-2577">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="48688-2578">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="48688-2578">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="48688-2579">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="48688-2579">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="48688-2580">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="48688-2580">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="48688-2581">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="48688-2581">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="48688-2582">VM</span><span class="sxs-lookup"><span data-stu-id="48688-2582">VM</span></span>

* <span data-ttu-id="48688-2583">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="48688-2583">Support configuring nsg</span></span>
* <span data-ttu-id="48688-2584">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="48688-2584">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="48688-2585">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="48688-2585">Support managed service identities</span></span>
* <span data-ttu-id="48688-2586">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="48688-2586">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="48688-2587">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="48688-2587">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="48688-2588">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="48688-2588">May 10, 2017</span></span>

<span data-ttu-id="48688-2589">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="48688-2589">Version 2.0.6</span></span>

* <span data-ttu-id="48688-2590">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48688-2590">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="48688-2591">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="48688-2591">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="48688-2592">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="48688-2592">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="48688-2593">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="48688-2593">Include Cognitive Services module</span></span>
* <span data-ttu-id="48688-2594">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="48688-2594">Include Service Fabric module</span></span>
* <span data-ttu-id="48688-2595">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="48688-2595">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="48688-2596">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="48688-2596">Add support for CDN commands</span></span>
* <span data-ttu-id="48688-2597">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="48688-2597">Remove Container module</span></span>
* <span data-ttu-id="48688-2598">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="48688-2598">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="48688-2599">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="48688-2599">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="48688-2600">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-2600">Core</span></span>

* <span data-ttu-id="48688-2601">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="48688-2601">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="48688-2602">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="48688-2602">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="48688-2603">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="48688-2603">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="48688-2604">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="48688-2604">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="48688-2605">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="48688-2605">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="48688-2606">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="48688-2606">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="48688-2607">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="48688-2607">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="48688-2608">núcleo: permitir que o caminho do arquivo accessTokens.json seja configurável por meio de uma variável de ambiente ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="48688-2608">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="48688-2609">núcleo: permitir que padrões configurados sejam aplicados em argumentos opcionais ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="48688-2609">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="48688-2610">núcleo: desempenho aprimorado</span><span class="sxs-lookup"><span data-stu-id="48688-2610">core: Improved performance</span></span>
* <span data-ttu-id="48688-2611">núcleo: certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="48688-2611">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="48688-2612">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="48688-2612">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="48688-2613">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-2613">ACS</span></span>

* <span data-ttu-id="48688-2614">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48688-2614">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="48688-2615">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="48688-2615">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="48688-2616">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="48688-2616">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="48688-2617">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="48688-2617">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-2618">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-2618">AppService</span></span>

* <span data-ttu-id="48688-2619">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="48688-2619">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="48688-2620">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="48688-2620">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="48688-2621">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="48688-2621">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="48688-2622">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="48688-2622">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="48688-2623">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="48688-2623">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="48688-2624">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="48688-2624">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="48688-2625">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="48688-2625">support slot swap with preview</span></span>
* <span data-ttu-id="48688-2626">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="48688-2626">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="48688-2627">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="48688-2627">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="48688-2628">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48688-2628">CosmosDB</span></span>

* <span data-ttu-id="48688-2629">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48688-2629">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="48688-2630">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="48688-2630">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="48688-2631">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="48688-2631">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="48688-2632">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="48688-2632">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="48688-2633">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="48688-2633">Data Lake Analytics</span></span>

* <span data-ttu-id="48688-2634">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="48688-2634">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="48688-2635">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="48688-2635">Add support for new catalog item type: package.</span></span> <span data-ttu-id="48688-2636">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="48688-2636">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="48688-2637">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="48688-2637">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="48688-2638">Tabela</span><span class="sxs-lookup"><span data-stu-id="48688-2638">Table</span></span>
  * <span data-ttu-id="48688-2639">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="48688-2639">Table valued function</span></span>
  * <span data-ttu-id="48688-2640">Visualizar</span><span class="sxs-lookup"><span data-stu-id="48688-2640">View</span></span>
  * <span data-ttu-id="48688-2641">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="48688-2641">Table Statistics.</span></span> <span data-ttu-id="48688-2642">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="48688-2642">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="48688-2643">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="48688-2643">Data Lake Store</span></span>

* <span data-ttu-id="48688-2644">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="48688-2644">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="48688-2645">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="48688-2645">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="48688-2646">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="48688-2646">missed help for access show.</span></span> <span data-ttu-id="48688-2647">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="48688-2647">adding it.</span></span> <span data-ttu-id="48688-2648">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="48688-2648">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="48688-2649">Localizar</span><span class="sxs-lookup"><span data-stu-id="48688-2649">Find</span></span>

* <span data-ttu-id="48688-2650">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="48688-2650">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="48688-2651">KeyVault</span><span class="sxs-lookup"><span data-stu-id="48688-2651">KeyVault</span></span>

* <span data-ttu-id="48688-2652">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="48688-2652">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="48688-2653">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois estes parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="48688-2653">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="48688-2654">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="48688-2654">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="48688-2655">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="48688-2655">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="48688-2656">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="48688-2656">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="48688-2657">Laboratório</span><span class="sxs-lookup"><span data-stu-id="48688-2657">Lab</span></span>

* <span data-ttu-id="48688-2658">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="48688-2658">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="48688-2659">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="48688-2659">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="48688-2660">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="48688-2660">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="48688-2661">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="48688-2661">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="48688-2662">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="48688-2662">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="48688-2663">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="48688-2663">Monitor</span></span>

* <span data-ttu-id="48688-2664">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="48688-2664">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="48688-2665">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="48688-2665">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="48688-2666">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-2666">Network</span></span>

* <span data-ttu-id="48688-2667">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="48688-2667">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="48688-2668">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="48688-2668">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="48688-2669">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48688-2669">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="48688-2670">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48688-2670">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="48688-2671">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="48688-2671">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="48688-2672">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="48688-2672">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="48688-2673">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="48688-2673">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="48688-2674">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="48688-2674">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="48688-2675">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="48688-2675">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="48688-2676">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="48688-2676">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="48688-2677">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="48688-2677">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="48688-2678">BC: corrigido um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="48688-2678">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="48688-2679">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="48688-2679">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="48688-2680">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="48688-2680">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="48688-2681">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="48688-2681">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="48688-2682">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="48688-2682">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="48688-2683">Perfil</span><span class="sxs-lookup"><span data-stu-id="48688-2683">Profile</span></span>

* <span data-ttu-id="48688-2684">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="48688-2684">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="48688-2685">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="48688-2685">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="48688-2686">Redis</span><span class="sxs-lookup"><span data-stu-id="48688-2686">Redis</span></span>

* <span data-ttu-id="48688-2687">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="48688-2687">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="48688-2688">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="48688-2688">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="48688-2689">Recurso</span><span class="sxs-lookup"><span data-stu-id="48688-2689">Resource</span></span>

* <span data-ttu-id="48688-2690">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="48688-2690">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="48688-2691">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="48688-2691">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="48688-2692">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="48688-2692">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="48688-2693">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="48688-2693">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="48688-2694">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="48688-2694">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="48688-2695">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="48688-2695">Add docs for az lock update.</span></span> <span data-ttu-id="48688-2696">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="48688-2696">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="48688-2697">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="48688-2697">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="48688-2698">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="48688-2698">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="48688-2699">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="48688-2699">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="48688-2700">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="48688-2700">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="48688-2701">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="48688-2701">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="48688-2702">Função</span><span class="sxs-lookup"><span data-stu-id="48688-2702">Role</span></span>

* <span data-ttu-id="48688-2703">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="48688-2703">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="48688-2704">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="48688-2704">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="48688-2705">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="48688-2705">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="48688-2706">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="48688-2706">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="48688-2707">SQL</span><span class="sxs-lookup"><span data-stu-id="48688-2707">SQL</span></span>

* <span data-ttu-id="48688-2708">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="48688-2708">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="48688-2709">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="48688-2709">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="48688-2710">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-2710">Storage</span></span>

* <span data-ttu-id="48688-2711">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="48688-2711">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="48688-2712">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="48688-2712">Add support for incremental blob copy</span></span>
* <span data-ttu-id="48688-2713">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="48688-2713">Add support for large block blob upload</span></span>
* <span data-ttu-id="48688-2714">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="48688-2714">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="48688-2715">VM</span><span class="sxs-lookup"><span data-stu-id="48688-2715">VM</span></span>

* <span data-ttu-id="48688-2716">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="48688-2716">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="48688-2717">observação: em comandos da VM em nuvens soberanas, evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="48688-2717">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="48688-2718">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="48688-2718">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="48688-2719">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="48688-2719">az vm/vmss disk</span></span>
  3. <span data-ttu-id="48688-2720">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="48688-2720">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="48688-2721">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="48688-2721">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="48688-2722">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="48688-2722">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="48688-2723">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="48688-2723">April 3, 2017</span></span>

<span data-ttu-id="48688-2724">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="48688-2724">Version 2.0.2</span></span>

<span data-ttu-id="48688-2725">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="48688-2725">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="48688-2726">Núcleo</span><span class="sxs-lookup"><span data-stu-id="48688-2726">Core</span></span>

* <span data-ttu-id="48688-2727">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="48688-2727">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="48688-2728">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="48688-2728">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="48688-2729">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="48688-2729">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="48688-2730">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="48688-2730">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="48688-2731">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="48688-2731">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="48688-2732">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="48688-2732">Add prompting for missing template parameters.</span></span> <span data-ttu-id="48688-2733">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="48688-2733">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="48688-2734">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="48688-2734">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="48688-2735">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="48688-2735">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="48688-2736">ACS</span><span class="sxs-lookup"><span data-stu-id="48688-2736">ACS</span></span>

* <span data-ttu-id="48688-2737">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="48688-2737">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="48688-2738">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="48688-2738">Add support for ssh key password prompting.</span></span> <span data-ttu-id="48688-2739">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="48688-2739">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="48688-2740">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="48688-2740">Add support for windows clusters.</span></span> <span data-ttu-id="48688-2741">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="48688-2741">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="48688-2742">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="48688-2742">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="48688-2743">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="48688-2743">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="48688-2744">AppService</span><span class="sxs-lookup"><span data-stu-id="48688-2744">AppService</span></span>

* <span data-ttu-id="48688-2745">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="48688-2745">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="48688-2746">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="48688-2746">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="48688-2747">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="48688-2747">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="48688-2748">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="48688-2748">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="48688-2749">DataLake</span><span class="sxs-lookup"><span data-stu-id="48688-2749">DataLake</span></span>

* <span data-ttu-id="48688-2750">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="48688-2750">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="48688-2751">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="48688-2751">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="48688-2752">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="48688-2752">DocuemntDB</span></span>

* <span data-ttu-id="48688-2753">DocumentDB: adicionado suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="48688-2753">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="48688-2754">VM</span><span class="sxs-lookup"><span data-stu-id="48688-2754">VM</span></span>

* <span data-ttu-id="48688-2755">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="48688-2755">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="48688-2756">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="48688-2756">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="48688-2757">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="48688-2757">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="48688-2758">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="48688-2758">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="48688-2759">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="48688-2759">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="48688-2760">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="48688-2760">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="48688-2761">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="48688-2761">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="48688-2762">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="48688-2762">February 27, 2017</span></span>

<span data-ttu-id="48688-2763">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="48688-2763">Version 2.0.0</span></span>

<span data-ttu-id="48688-2764">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="48688-2764">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="48688-2765">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="48688-2765">Container Service (acs)</span></span>
- <span data-ttu-id="48688-2766">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="48688-2766">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="48688-2767">Rede</span><span class="sxs-lookup"><span data-stu-id="48688-2767">Networking</span></span>
- <span data-ttu-id="48688-2768">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="48688-2768">Storage</span></span>

<span data-ttu-id="48688-2769">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="48688-2769">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="48688-2770">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="48688-2770">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="48688-2771">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="48688-2771">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="48688-2772">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="48688-2772">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="48688-2773">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="48688-2773">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="48688-2774">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="48688-2774">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="48688-2775">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="48688-2775">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="48688-2776">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="48688-2776">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="48688-2777">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="48688-2777">Provide feedback from the command line with the `az feedback` command</span></span>

