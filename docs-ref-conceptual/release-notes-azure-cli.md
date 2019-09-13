---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/05/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 03594fc6e7e24fd1b7d2f9c846161a40e8ea7678
ms.sourcegitcommit: f9bfb4b063151434b3a9bff936a73b251666e775
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/10/2019
ms.locfileid: "70878231"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="f0d01-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="f0d01-103">Azure CLI release notes</span></span>

## <a name="september-5-2019"></a><span data-ttu-id="f0d01-104">5 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="f0d01-104">September 5, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-105">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-105">ACR</span></span>

* <span data-ttu-id="f0d01-106">Adição do grupo de comandos `acr config retention` para configurar a política de retenção</span><span class="sxs-lookup"><span data-stu-id="f0d01-106">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="f0d01-107">AKS</span><span class="sxs-lookup"><span data-stu-id="f0d01-107">AKS</span></span>

* <span data-ttu-id="f0d01-108">Adição de suporte para integração do ACR com os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="f0d01-108">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="f0d01-109">Adição do parâmetro `--attach-acr` a `aks [create|update]` para anexar um ACR a um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="f0d01-109">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="f0d01-110">Adição do parâmetro `--detach-acr` a `aks update` para desanexar o ACR de um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="f0d01-110">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="f0d01-111">ARM</span><span class="sxs-lookup"><span data-stu-id="f0d01-111">ARM</span></span>

* <span data-ttu-id="f0d01-112">Atualização para uso da versão de API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="f0d01-112">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="f0d01-113">Lote</span><span class="sxs-lookup"><span data-stu-id="f0d01-113">Batch</span></span>

* <span data-ttu-id="f0d01-114">Adição de novas definições de configuração JSON de `--json-file` para `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="f0d01-114">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="f0d01-115">Adição de `MountConfigurations` para montagens do sistema de arquivos (confira https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="f0d01-115">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="f0d01-116">Adição da propriedade opcional `publicIPs` a `NetworkConfiguration` para IPs públicos em pools (confira https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="f0d01-116">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="f0d01-117">Adição de suporte para galerias de imagens compartilhadas a `--image`</span><span class="sxs-lookup"><span data-stu-id="f0d01-117">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="f0d01-118">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `--start-task-wait-for-success` em `batch pool create` para `true`</span><span class="sxs-lookup"><span data-stu-id="f0d01-118">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="f0d01-119">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `Scope` em `AutoUserSpecification` para sempre ser Pool (anteriormente, `Task` em nós do Windows e `Pool` em nós do Linux)</span><span class="sxs-lookup"><span data-stu-id="f0d01-119">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="f0d01-120">Esse argumento só pode ser definido em uma configuração JSON com `--json-file`</span><span class="sxs-lookup"><span data-stu-id="f0d01-120">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f0d01-121">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f0d01-121">HDInsight</span></span>

* <span data-ttu-id="f0d01-122">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="f0d01-122">GA release</span></span>
* <span data-ttu-id="f0d01-123">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--workernode-count/-c` de `az hdinsight resize` para ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0d01-123">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="f0d01-124">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f0d01-124">Key Vault</span></span>

* <span data-ttu-id="f0d01-125">Correção do problema em que as sub-redes não podiam ser excluídas das regras da rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-125">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="f0d01-126">Correção do problema em que sub-redes e endereços IP duplicados podiam ser adicionados às regras da rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-126">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-127">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-127">Network</span></span>

* <span data-ttu-id="f0d01-128">Adição do parâmetro `--interval` a `network watcher flow-log` para definir o valor do intervalo de análise de tráfego</span><span class="sxs-lookup"><span data-stu-id="f0d01-128">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="f0d01-129">Adição de `network application-gateway identity` para gerenciar a identidade do gateway</span><span class="sxs-lookup"><span data-stu-id="f0d01-129">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="f0d01-130">Adição de suporte para definir a ID do Key Vault como `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="f0d01-130">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="f0d01-131">Adicionado `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-131">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="f0d01-132">Política</span><span class="sxs-lookup"><span data-stu-id="f0d01-132">Policy</span></span>

* <span data-ttu-id="f0d01-133">Atualização para uso da versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="f0d01-133">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="f0d01-134">27 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="f0d01-134">August 27, 2019</span></span>

<span data-ttu-id="f0d01-135">Versão 2.0.72</span><span class="sxs-lookup"><span data-stu-id="f0d01-135">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-136">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-136">ACR</span></span>

* <span data-ttu-id="f0d01-137">[ALTERAÇÃO DA FALHA] Remoção do suporte para o SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="f0d01-137">[BREAKING CHNAGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="f0d01-138">Gerenciamento de API</span><span class="sxs-lookup"><span data-stu-id="f0d01-138">API Management</span></span>

* <span data-ttu-id="f0d01-139">[VERSÃO PRÉVIA] Adição do grupo de comandos `apim`</span><span class="sxs-lookup"><span data-stu-id="f0d01-139">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-140">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-140">AppService</span></span>

* <span data-ttu-id="f0d01-141">Correção do problema com o comando `webapp webjob continuous start` ao especificar um slot</span><span class="sxs-lookup"><span data-stu-id="f0d01-141">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="f0d01-142">Alteração de `webapp up` para detectar a pasta `env` e removê-la do arquivo usado para implantação</span><span class="sxs-lookup"><span data-stu-id="f0d01-142">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="f0d01-143">Keyvault</span><span class="sxs-lookup"><span data-stu-id="f0d01-143">Keyvault</span></span>

* <span data-ttu-id="f0d01-144">Correção de um bug no `keyvault secret set` que ignorava o argumento `--expires`</span><span class="sxs-lookup"><span data-stu-id="f0d01-144">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-145">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-145">Network</span></span>

* <span data-ttu-id="f0d01-146">Adição de suporte para endereços IPv6 a argumentos `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="f0d01-146">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="f0d01-147">Adição de novos comandos `network private-endpoint [create|update|list-types]` para o gerenciamento de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="f0d01-147">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="f0d01-148">Adição do grupo de comandos `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="f0d01-148">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="f0d01-149">Adicionados os argumentos `--private-endpoint-network-policies` e `--private-link-service-network-policies` para `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-149">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="f0d01-150">RBAC</span><span class="sxs-lookup"><span data-stu-id="f0d01-150">RBAC</span></span>

* <span data-ttu-id="f0d01-151">Correção de um problema com `ad app update --homepage` em que a página inicial não era atualizada</span><span class="sxs-lookup"><span data-stu-id="f0d01-151">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="f0d01-152">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f0d01-152">ServiceFabric</span></span>

* <span data-ttu-id="f0d01-153">Adição de suporte para nomes de Key Vault grafados com maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="f0d01-153">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="f0d01-154">Correção de um problema ao usar certificados no Key Vault</span><span class="sxs-lookup"><span data-stu-id="f0d01-154">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="f0d01-155">Correção de um problema com o uso de arquivos de certificado PFX</span><span class="sxs-lookup"><span data-stu-id="f0d01-155">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="f0d01-156">Correção de um problema com `sf cluster certificate add` quando o grupo de recursos do Key Vault não era especificado</span><span class="sxs-lookup"><span data-stu-id="f0d01-156">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="f0d01-157">Correção de um problema em que `sf cluster set` não funcionava</span><span class="sxs-lookup"><span data-stu-id="f0d01-157">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="f0d01-158">SignalR</span><span class="sxs-lookup"><span data-stu-id="f0d01-158">SignalR</span></span>

* <span data-ttu-id="f0d01-159">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="f0d01-159">Added new commands:</span></span>
  * <span data-ttu-id="f0d01-160">`signalr cors`: gerenciar CORS do SignalR</span><span class="sxs-lookup"><span data-stu-id="f0d01-160">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="f0d01-161">`signalr restart`: reiniciar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="f0d01-161">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="f0d01-162">`signalr update`: atualizar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="f0d01-162">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="f0d01-163">Adicionado o argumento `--service-mode` para `signalr create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-163">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-164">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-164">Storage</span></span>

* <span data-ttu-id="f0d01-165">Adicionado o comando `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="f0d01-165">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="f0d01-166">13 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="f0d01-166">August 13, 2019</span></span>

<span data-ttu-id="f0d01-167">Versão 2.0.71</span><span class="sxs-lookup"><span data-stu-id="f0d01-167">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-168">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-168">AppService</span></span>

* <span data-ttu-id="f0d01-169">Um problema de falha de slots com os comandos `webapp webjob continuous` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="f0d01-169">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="f0d01-170">BotService</span><span class="sxs-lookup"><span data-stu-id="f0d01-170">BotService</span></span>

* <span data-ttu-id="f0d01-171">[ALTERAÇÃO SIGNIFICATIVA] O suporte para a criação de bots SDK v3 foi removido</span><span class="sxs-lookup"><span data-stu-id="f0d01-171">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="f0d01-172">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="f0d01-172">CognitiveServices</span></span>

* <span data-ttu-id="f0d01-173">Adicionados os comandos `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="f0d01-173">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="f0d01-174">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f0d01-174">Cosmos DB</span></span>

* <span data-ttu-id="f0d01-175">Removido o aviso ao atualizar vários locais de gravação</span><span class="sxs-lookup"><span data-stu-id="f0d01-175">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="f0d01-176">Foram adicionados os comandos CRUD para o CosmosDB SQL, MongoDB, Cassandra, Gremlin e Recursos de tabela e taxa de transferência do recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-176">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f0d01-177">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f0d01-177">HDInsight</span></span>

<span data-ttu-id="f0d01-178">Esta versão contém um grande número de alterações da falha.</span><span class="sxs-lookup"><span data-stu-id="f0d01-178">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="f0d01-179">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="f0d01-179">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="f0d01-180">`--storage-default-container` renomeado para `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="f0d01-180">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="f0d01-181">`--storage-default-filesystem` renomeado para `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="f0d01-181">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="f0d01-182">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--name` de `application create` foi alterado para representar o nome do aplicativo em vez do nome do cluster</span><span class="sxs-lookup"><span data-stu-id="f0d01-182">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="f0d01-183">O argumento `--cluster-name` foi adicionado a `application create` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="f0d01-183">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="f0d01-184">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `application create`:</span><span class="sxs-lookup"><span data-stu-id="f0d01-184">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="f0d01-185">`--application-type` renomeado para `--type`</span><span class="sxs-lookup"><span data-stu-id="f0d01-185">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="f0d01-186">`--marketplace-identifier` renomeado para `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="f0d01-186">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="f0d01-187">`--https-endpoint-access-mode` renomeado para `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="f0d01-187">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="f0d01-188">Renomeado de `--https-endpoint-destination-port` para `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="f0d01-188">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="f0d01-189">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros removidos para `application create`:</span><span class="sxs-lookup"><span data-stu-id="f0d01-189">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="f0d01-190">[ALTERAÇÃO DA FALHA] Renomeado de `--target-instance-count` para `--workernode-count` para `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="f0d01-190">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="f0d01-191">[ALTERAÇÃO SIGNIFICATIVA] Todos os comandos no grupo `hdinsight script-action` foram alterados para usar o parâmetro `--name` como o nome da ação de script.</span><span class="sxs-lookup"><span data-stu-id="f0d01-191">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="f0d01-192">O argumento `--cluster-name` foi adicionado a todos os comandos `hdinsight script-action` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="f0d01-192">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="f0d01-193">[ALTERAÇÃO SIGNIFICATIVA] Renomeado de `--script-execution-id` para `--execution-id` para todos os comandos `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="f0d01-193">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="f0d01-194">[ALTERAÇÃO SIGNIFICATIVA] `hdinsight script-action show` renomeado para `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="f0d01-194">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="f0d01-195">[ALTERAÇÃO DA FALHA] Os parâmetros foram alterados para `hdinsight script-action execute --roles` para serem separados por espaços em vez de separados por vírgula</span><span class="sxs-lookup"><span data-stu-id="f0d01-195">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="f0d01-196">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro `--persisted` de `hdinsight script-action list` foi removido</span><span class="sxs-lookup"><span data-stu-id="f0d01-196">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="f0d01-197">O parâmetro `hdinsight create --cluster-configurations` foi alterado para aceitar um caminho para um arquivo JSON local ou uma cadeia de caracteres JSON</span><span class="sxs-lookup"><span data-stu-id="f0d01-197">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="f0d01-198">Adicionado o comando `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="f0d01-198">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="f0d01-199">Alterado `hdinsight monitor enable --workspace` para aceitar uma ID do workspace ou nome do workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="f0d01-199">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="f0d01-200">O argumento `hdinsight monitor enable --primary-key`, que será necessário caso uma ID do workspace seja fornecida como o parâmetro, foi adicionado</span><span class="sxs-lookup"><span data-stu-id="f0d01-200">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="f0d01-201">Foram adicionados mais exemplos e atualização das descrições das mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="f0d01-201">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="f0d01-202">Interativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-202">Interactive</span></span>

* <span data-ttu-id="f0d01-203">Um erro no carregamento foi corrigido</span><span class="sxs-lookup"><span data-stu-id="f0d01-203">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="f0d01-204">kubernetes</span><span class="sxs-lookup"><span data-stu-id="f0d01-204">Kubernetes</span></span>

* <span data-ttu-id="f0d01-205">Alterado para usar `https` se a porta do contêiner do painel estiver usando `https`</span><span class="sxs-lookup"><span data-stu-id="f0d01-205">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-206">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-206">Network</span></span>

* <span data-ttu-id="f0d01-207">O argumento `--yes` foi adicionado a `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="f0d01-207">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="f0d01-208">Perfil</span><span class="sxs-lookup"><span data-stu-id="f0d01-208">Profile</span></span>

* <span data-ttu-id="f0d01-209">O argumento `--resource-type` foi adicionado a `account get-access-token` para obter tokens de acesso de recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-209">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="f0d01-210">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f0d01-210">ServiceFabric</span></span>

* <span data-ttu-id="f0d01-211">Todas as versões de sistema operacional com suporte para criação do cluster sf foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="f0d01-211">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="f0d01-212">Foi corrigido o bug de validação do certificado primário</span><span class="sxs-lookup"><span data-stu-id="f0d01-212">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-213">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-213">Storage</span></span>

* <span data-ttu-id="f0d01-214">Adicionado o comando `storage copy`</span><span class="sxs-lookup"><span data-stu-id="f0d01-214">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="f0d01-215">30 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="f0d01-215">July 30, 2019</span></span>

<span data-ttu-id="f0d01-216">Versão 2.0.70</span><span class="sxs-lookup"><span data-stu-id="f0d01-216">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-217">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-217">ACR</span></span>

* <span data-ttu-id="f0d01-218">Corrigido o problema #9952 (uma regressão no comando `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="f0d01-218">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="f0d01-219">Removido o nome da imagem do construtor padrão em `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="f0d01-219">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-220">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-220">Appservice</span></span>

* <span data-ttu-id="f0d01-221">Alterado `webapp config ssl` para mostrar uma mensagem se um recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="f0d01-221">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="f0d01-222">Corrigido o problema em que `functionapp create` não aceita o tipo de conta de armazenamento `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="f0d01-222">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="f0d01-223">Corrigido um problema em que `webapp up` falharia se fosse executado usando versões mais antigas do Python</span><span class="sxs-lookup"><span data-stu-id="f0d01-223">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-224">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-224">Network</span></span>

* <span data-ttu-id="f0d01-225">Removido parâmetro inválido `--ids` de `network nic ip-config add` (corrige o #9861)</span><span class="sxs-lookup"><span data-stu-id="f0d01-225">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="f0d01-226">Corrige o #9604.</span><span class="sxs-lookup"><span data-stu-id="f0d01-226">Fixes #9604.</span></span> <span data-ttu-id="f0d01-227">Adicionado o parâmetro `--root-certs` ao `network application-gateway http-settings [create|update]` para dar suporte a certificados raiz confiáveis associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="f0d01-227">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="f0d01-228">Fixado argumento `--subscription` para `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="f0d01-228">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="f0d01-229">RBAC</span><span class="sxs-lookup"><span data-stu-id="f0d01-229">RBAC</span></span>

* <span data-ttu-id="f0d01-230">Adicionado o comando `user update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-230">Added `user update` command</span></span>
* <span data-ttu-id="f0d01-231">[PRETERIDO] Preterido `--upn-or-object-id` de comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="f0d01-231">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="f0d01-232">Usar argumento de substituição `--id`</span><span class="sxs-lookup"><span data-stu-id="f0d01-232">Use replacement argument `--id`</span></span>
* <span data-ttu-id="f0d01-233">Adicionado argumento `--id` para comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="f0d01-233">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-234">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-234">SQL</span></span>

* <span data-ttu-id="f0d01-235">Adicionados comandos de gerenciamento para chaves de instância gerenciada e protetor de TDE</span><span class="sxs-lookup"><span data-stu-id="f0d01-235">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-236">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-236">Storage</span></span>

* <span data-ttu-id="f0d01-237">Adicionado o comando `storage remove`</span><span class="sxs-lookup"><span data-stu-id="f0d01-237">Added `storage remove` command</span></span>
* <span data-ttu-id="f0d01-238">Corrigido um problema com `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-238">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-239">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-239">VM</span></span>

* <span data-ttu-id="f0d01-240">Alterado `list-skus` para usar versão de API mais recente a fim de externar detalhes de zona</span><span class="sxs-lookup"><span data-stu-id="f0d01-240">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="f0d01-241">Alterado o padrão de `--single-placement-group` para `false` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-241">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="f0d01-242">Adicionada a capacidade de selecionar SKUs de armazenamento ZRS para `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-242">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="f0d01-243">Adicionado novo grupo de comandos `vm host` para dar suporte a hosts dedicados</span><span class="sxs-lookup"><span data-stu-id="f0d01-243">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="f0d01-244">Adicionados parâmetros `--host` e `--host-group` em `vm create` para definir o host dedicado da VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-244">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="f0d01-245">16 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="f0d01-245">July 16, 2019</span></span>

<span data-ttu-id="f0d01-246">Versão 2.0.69</span><span class="sxs-lookup"><span data-stu-id="f0d01-246">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-247">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-247">Appservice</span></span>

* <span data-ttu-id="f0d01-248">Os comandos `webapp identity` foram alterados para retornar uma mensagem de erro apropriada se o nome do aplicativo ou ResourceGroupName for inválido</span><span class="sxs-lookup"><span data-stu-id="f0d01-248">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="f0d01-249">`webapp list` corrigido para retornar o valor correto para numberOfSites se nenhum ResourceGroup foi fornecido</span><span class="sxs-lookup"><span data-stu-id="f0d01-249">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="f0d01-250">Corrigidos os efeitos colaterais de `appservice plan create` e `webapp create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-250">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-251">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-251">Core</span></span>

* <span data-ttu-id="f0d01-252">Corrigido um problema em que `--subscription` aparecia apesar de não ser aplicável</span><span class="sxs-lookup"><span data-stu-id="f0d01-252">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="f0d01-253">Lote</span><span class="sxs-lookup"><span data-stu-id="f0d01-253">Batch</span></span>

* <span data-ttu-id="f0d01-254">[ALTERAÇÃO SIGNIFICATIVA] `batch pool node-agent-skus list` foi substituído por `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="f0d01-254">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="f0d01-255">Adicionado suporte para regras de segurança bloqueando o acesso de rede a um pool com base na porta de origem do tráfego ao usar a opção `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="f0d01-255">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="f0d01-256">Suporte adicionado para executar a tarefa no diretório de trabalho de contêiner ou no diretório de trabalho de tarefa em lotes ao usar a opção `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-256">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="f0d01-257">Corrigido o erro na opção `--application-package-references` de `batch pool create` em que ela funcionaria apenas com padrões</span><span class="sxs-lookup"><span data-stu-id="f0d01-257">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="f0d01-258">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="f0d01-258">Eventhubs</span></span>

* <span data-ttu-id="f0d01-259">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="f0d01-259">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="f0d01-260">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f0d01-260">RDBMS</span></span>

* <span data-ttu-id="f0d01-261">Adicionado um parâmetro opcional para especificar a réplica de SKU para criar o comando de réplica</span><span class="sxs-lookup"><span data-stu-id="f0d01-261">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="f0d01-262">Corrigido o problema com a falha no teste de CI com a criação de réplica de MySQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-262">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="f0d01-263">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="f0d01-263">Relay</span></span>

* <span data-ttu-id="f0d01-264">Corrigido o problema com a conexão híbrida quando a autorização do cliente desabilitava [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="f0d01-264">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="f0d01-265">Parâmetro `--requires-transport-security` adicionado a `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-265">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="f0d01-266">Barramento de serviço</span><span class="sxs-lookup"><span data-stu-id="f0d01-266">Servicebus</span></span>

* <span data-ttu-id="f0d01-267">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="f0d01-267">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-268">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-268">Storage</span></span>

* <span data-ttu-id="f0d01-269">Habilitar AADDS de arquivos para atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-269">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="f0d01-270">Problema corrigido `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="f0d01-270">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="f0d01-271">2 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="f0d01-271">July 2, 2019</span></span>

<span data-ttu-id="f0d01-272">Versão 2.0.68</span><span class="sxs-lookup"><span data-stu-id="f0d01-272">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-273">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-273">Core</span></span>

* <span data-ttu-id="f0d01-274">Agora, os módulos de comando são consolidados em um único Python distribuível.</span><span class="sxs-lookup"><span data-stu-id="f0d01-274">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="f0d01-275">Isso substitui o uso direto de muitos pacotes `azure-cli-` no PyPI.</span><span class="sxs-lookup"><span data-stu-id="f0d01-275">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="f0d01-276">Assim, o tamanho da instalação será reduzido e apenas os usuários que tiverem instalado diretamente por meio do `pip` serão afetados.</span><span class="sxs-lookup"><span data-stu-id="f0d01-276">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-277">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-277">ACR</span></span>

* <span data-ttu-id="f0d01-278">Foi adicionado o suporte para gatilhos de temporizador para tarefa</span><span class="sxs-lookup"><span data-stu-id="f0d01-278">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-279">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-279">Appservice</span></span>

* <span data-ttu-id="f0d01-280">O `functionapp create` foi alterado para habilitar o Application Insights por padrão</span><span class="sxs-lookup"><span data-stu-id="f0d01-280">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="f0d01-281">[ALTERAÇÃO SIGNIFICATIVA] Foi removido o comando `functionapp devops-build` preterido.</span><span class="sxs-lookup"><span data-stu-id="f0d01-281">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="f0d01-282">Agora, use o novo comando `az functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="f0d01-282">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="f0d01-283">Foi adicionado o suporte ao plano de aplicativo de funções Consumo em Linux ao `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="f0d01-283">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="f0d01-284">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f0d01-284">Cosmos DB</span></span>

* <span data-ttu-id="f0d01-285">Foi adicionado o suporte para desabilitar a TTL</span><span class="sxs-lookup"><span data-stu-id="f0d01-285">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="f0d01-286">DLS</span><span class="sxs-lookup"><span data-stu-id="f0d01-286">DLS</span></span>

* <span data-ttu-id="f0d01-287">Versão atualizada do ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="f0d01-287">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="f0d01-288">Comentários</span><span class="sxs-lookup"><span data-stu-id="f0d01-288">Feedback</span></span>

* <span data-ttu-id="f0d01-289">Ao relatar um comando de extensão com falha, agora, o `az feedback` tenta abrir o navegador na URL do projeto/repositório da extensão por meio do índice</span><span class="sxs-lookup"><span data-stu-id="f0d01-289">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f0d01-290">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f0d01-290">HDInsight</span></span>

* <span data-ttu-id="f0d01-291">[ALTERAÇÃO SIGNIFICATIVA] O nome do grupo de comandos `oms` foi alterado para `monitor`</span><span class="sxs-lookup"><span data-stu-id="f0d01-291">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="f0d01-292">[ALTERAÇÃO SIGNIFICATIVA] `--http-password/-p` tornou-se um parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="f0d01-292">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="f0d01-293">Foram adicionados preenchedores para o preenchedor dos parâmetros `--cluster-admin-account` e `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="f0d01-293">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="f0d01-294">O parâmetro `cluster-users-group-dns` foi alterado para ser obrigatório quando `—esp` estiver presente</span><span class="sxs-lookup"><span data-stu-id="f0d01-294">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="f0d01-295">Foi adicionado um tempo limite para todos os preenchedores automáticos de argumento existentes</span><span class="sxs-lookup"><span data-stu-id="f0d01-295">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="f0d01-296">Foi adicionado um tempo limite para transformar o nome do recurso na ID de recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-296">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="f0d01-297">Os preenchedores automáticos foram alterados para selecionar recursos de qualquer grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="f0d01-297">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="f0d01-298">Pode ser um grupo de recursos diferente daquele especificado com `-g`</span><span class="sxs-lookup"><span data-stu-id="f0d01-298">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="f0d01-299">Foi adicionado o suporte para os parâmetros `--sub-domain-suffix` e `--disable_gateway_auth` no comando `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-299">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="f0d01-300">Serviços gerenciados</span><span class="sxs-lookup"><span data-stu-id="f0d01-300">Managed Services</span></span>

* <span data-ttu-id="f0d01-301">Introdução ao módulo de comando de serviço gerenciado em versão prévia</span><span class="sxs-lookup"><span data-stu-id="f0d01-301">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="f0d01-302">Perfil</span><span class="sxs-lookup"><span data-stu-id="f0d01-302">Profile</span></span>
* <span data-ttu-id="f0d01-303">Suprimir o argumento `--subscription` para o comando de logoff</span><span class="sxs-lookup"><span data-stu-id="f0d01-303">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="f0d01-304">RBAC</span><span class="sxs-lookup"><span data-stu-id="f0d01-304">RBAC</span></span>

* <span data-ttu-id="f0d01-305">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--password` foi removido de `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="f0d01-305">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="f0d01-306">Foi adicionado o parâmetro `--assignee-principal-type` ao comando `create` para evitar falhas intermitentes causadas pela latência de replicação do servidor do AAD Graph</span><span class="sxs-lookup"><span data-stu-id="f0d01-306">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="f0d01-307">Foi corrigida uma falha em `ad signed-in-user` ao listar objetos de propriedade</span><span class="sxs-lookup"><span data-stu-id="f0d01-307">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="f0d01-308">Foi corrigido um problema em que o `ad sp` não localizava o aplicativo certo de uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="f0d01-308">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="f0d01-309">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f0d01-309">RDBMS</span></span>

* <span data-ttu-id="f0d01-310">Foi adicionado o suporte à replicação para o MariaDB</span><span class="sxs-lookup"><span data-stu-id="f0d01-310">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-311">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-311">SQL</span></span>

* <span data-ttu-id="f0d01-312">Valores permitidos documentados para `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="f0d01-312">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-313">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-313">Storage</span></span>

* <span data-ttu-id="f0d01-314">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="f0d01-314">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="f0d01-315">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="f0d01-315">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="f0d01-316">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-316">VM</span></span>

* <span data-ttu-id="f0d01-317">Foi corrigido o bug em que o `vmss create` retornava uma mensagem de erro quando era executado com `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="f0d01-317">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="f0d01-318">Foi removida a validação do lado do cliente de `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-318">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="f0d01-319">Não falha quando `--single-placement-group` é definido como `true` e `--instance-count` é maior que 100 ou quando são especificadas zonas de disponibilidade, mas deixa essa validação para o serviço de computação</span><span class="sxs-lookup"><span data-stu-id="f0d01-319">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="f0d01-320">Foi corrigido o bug em que o `[vm|vmss] extension image list` falhava quando era usado com `--latest`</span><span class="sxs-lookup"><span data-stu-id="f0d01-320">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="f0d01-321">18 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="f0d01-321">June 18, 2019</span></span>

<span data-ttu-id="f0d01-322">Versão 2.0.67</span><span class="sxs-lookup"><span data-stu-id="f0d01-322">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-323">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-323">Core</span></span>

<span data-ttu-id="f0d01-324">Esta versão apresenta uma nova marca [Versão prévia] para comunicar com mais clareza aos clientes quando um comando, um grupo de comandos ou um argumento está no status de versão prévia.</span><span class="sxs-lookup"><span data-stu-id="f0d01-324">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="f0d01-325">Anteriormente, essa informação era transmitida no texto de ajuda ou, implicitamente, pelo número da versão do módulo de comando.</span><span class="sxs-lookup"><span data-stu-id="f0d01-325">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="f0d01-326">A CLI removerá os números de versão dos pacotes individuais no futuro.</span><span class="sxs-lookup"><span data-stu-id="f0d01-326">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="f0d01-327">Se um comando estiver em versão prévia, todos os seus argumentos também estarão.</span><span class="sxs-lookup"><span data-stu-id="f0d01-327">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="f0d01-328">Se um grupo de comandos for rotulado com o status de versão prévia, então todos os seus comandos e argumentos também serão considerados em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="f0d01-328">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="f0d01-329">Como resultado dessa alteração, diversos grupos de comandos podem parecer surgir "de repente" com o status de versão prévia com esta liberação.</span><span class="sxs-lookup"><span data-stu-id="f0d01-329">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="f0d01-330">O que realmente aconteceu é que a maioria dos pacotes já estava com status de versão prévia, mas estão sendo consideradas GA com esta liberação</span><span class="sxs-lookup"><span data-stu-id="f0d01-330">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-331">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-331">ACR</span></span>
* <span data-ttu-id="f0d01-332">Adicionado o comando 'acr check-health'</span><span class="sxs-lookup"><span data-stu-id="f0d01-332">Added 'acr check-health' command</span></span>
* <span data-ttu-id="f0d01-333">Melhorado o tratamento de erro para tokens do AAD e para recuperar comandos externos</span><span class="sxs-lookup"><span data-stu-id="f0d01-333">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-334">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-334">ACS</span></span>
* <span data-ttu-id="f0d01-335">Comandos preteridos do ACS agora ficam ocultos da exibição da ajuda</span><span class="sxs-lookup"><span data-stu-id="f0d01-335">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="f0d01-336">AMS</span><span class="sxs-lookup"><span data-stu-id="f0d01-336">AMS</span></span>
* <span data-ttu-id="f0d01-337">[ALTERAÇÃO SIGNIFICATIVA] Alterada para retornar cadeias de caracteres de tempo da ISO 8601 para archive-window-length e key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="f0d01-337">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-338">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-338">AppService</span></span>
* <span data-ttu-id="f0d01-339">Adicionado roteamento com base no local para `webapp deleted list` e `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="f0d01-339">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="f0d01-340">Corrigido problema em que a URL de destino registrada do webapp ("Não é possível iniciar o aplicativo em...") não era clicável no Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="f0d01-340">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="f0d01-341">Corrigido um problema em que a criação de aplicativos com algumas SKUs falhava com um erro de AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="f0d01-341">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="f0d01-342">Adicionada a pré-validação para o `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-342">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="f0d01-343">Corrigido o `[webapp|functionapp] traffic-routing` para usar o actionHostName correto</span><span class="sxs-lookup"><span data-stu-id="f0d01-343">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="f0d01-344">Adicionado o suporte de slot para comandos `functionapp`</span><span class="sxs-lookup"><span data-stu-id="f0d01-344">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="f0d01-345">Lote</span><span class="sxs-lookup"><span data-stu-id="f0d01-345">Batch</span></span>
* <span data-ttu-id="f0d01-346">Corrigida a regressão de autenticação do AAD causada pela geração de relatórios de erros superagressiva para autenticação de chave compartilhada</span><span class="sxs-lookup"><span data-stu-id="f0d01-346">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="f0d01-347">BatchAI</span><span class="sxs-lookup"><span data-stu-id="f0d01-347">BatchAI</span></span>
* <span data-ttu-id="f0d01-348">Agora os comandos do BatchAI estão preteridos e ocultos</span><span class="sxs-lookup"><span data-stu-id="f0d01-348">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="f0d01-349">BotService</span><span class="sxs-lookup"><span data-stu-id="f0d01-349">BotService</span></span>
* <span data-ttu-id="f0d01-350">Adição das mensagens de aviso "suporte descontinuado"/"modo de manutenção" para os comandos compatíveis com a v3 do SDK</span><span class="sxs-lookup"><span data-stu-id="f0d01-350">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f0d01-351">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f0d01-351">CosmosDB</span></span>
* <span data-ttu-id="f0d01-352">[PRETERIDO] Preterido o comando `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="f0d01-352">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="f0d01-353">Adicionado o comando `cosmosdb keys list` – substitui o `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="f0d01-353">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="f0d01-354">`cosmsodb create/update`: Adicionado novo formato para --location a fim de permitir a configuração da propriedade "isZoneRedundant".</span><span class="sxs-lookup"><span data-stu-id="f0d01-354">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="f0d01-355">Formato antigo preterido</span><span class="sxs-lookup"><span data-stu-id="f0d01-355">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="f0d01-356">EventGrid</span><span class="sxs-lookup"><span data-stu-id="f0d01-356">EventGrid</span></span>
* <span data-ttu-id="f0d01-357">Adicionados comandos do `eventgrid domain` para operações de CRUD no domínio</span><span class="sxs-lookup"><span data-stu-id="f0d01-357">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="f0d01-358">Adicionados comandos do `eventgrid domain topic` para operações de CRUD nos tópicos do domínio</span><span class="sxs-lookup"><span data-stu-id="f0d01-358">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="f0d01-359">Adicionado argumento do `--odata-query` ao `eventgrid [topic|event-subscription] list` para filtrar os resultados usando a sintaxe do OData</span><span class="sxs-lookup"><span data-stu-id="f0d01-359">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="f0d01-360">`event-subscription create/update`: Adicionado o servicebusqueue como novos valores para o parâmetro `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="f0d01-360">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="f0d01-361">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para `--included-event-types All` com `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-361">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f0d01-362">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f0d01-362">HDInsight</span></span>
* <span data-ttu-id="f0d01-363">Adicionado suporte para o parâmetro `--ssh-public-key` no comando `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-363">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="f0d01-364">IoT</span><span class="sxs-lookup"><span data-stu-id="f0d01-364">IoT</span></span>
* <span data-ttu-id="f0d01-365">Adicionado suporte para regenerar as chaves da política de autorização</span><span class="sxs-lookup"><span data-stu-id="f0d01-365">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="f0d01-366">Adicionados SDK e suporte para o serviço de provisionamento de repositórios do DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="f0d01-366">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-367">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-367">Network</span></span>
* <span data-ttu-id="f0d01-368">Adicionado suporte de zona para o Gateway da NAT</span><span class="sxs-lookup"><span data-stu-id="f0d01-368">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="f0d01-369">Adicionado o comando `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="f0d01-369">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="f0d01-370">Corrigido o problema com o `dns zone import` em que os usuários não conseguiam importar registros do curinga A</span><span class="sxs-lookup"><span data-stu-id="f0d01-370">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="f0d01-371">Corrigido o problema com o `watcher flow-log configure` em que o registro de fluxo não podia ser habilitado em determinadas regiões</span><span class="sxs-lookup"><span data-stu-id="f0d01-371">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-372">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-372">Resource</span></span>
* <span data-ttu-id="f0d01-373">Adicionado o comando do `az rest` para fazer chamadas REST</span><span class="sxs-lookup"><span data-stu-id="f0d01-373">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="f0d01-374">Corrigido o erro ao usar o `policy assignment list` com um grupo de recursos ou o nível de assinatura `--scope`</span><span class="sxs-lookup"><span data-stu-id="f0d01-374">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="f0d01-375">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f0d01-375">ServiceBus</span></span>
* <span data-ttu-id="f0d01-376">Corrigido o problema com o `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="f0d01-376">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-377">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-377">SQL</span></span>
* <span data-ttu-id="f0d01-378">Alterado o `--location` para ser opcional para `sql [server|mi] create` – usa o local do grupo de recursos se não especificado</span><span class="sxs-lookup"><span data-stu-id="f0d01-378">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="f0d01-379">Corrigido o erro "objeto 'NoneType' não é iterável" para `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="f0d01-379">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="f0d01-380">SQLVm</span><span class="sxs-lookup"><span data-stu-id="f0d01-380">SQLVm</span></span>
* <span data-ttu-id="f0d01-381">[ALTERAÇÃO DA FALHA] Alterado `sql vm create` para exigir o parâmetro `--license-type`</span><span class="sxs-lookup"><span data-stu-id="f0d01-381">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="f0d01-382">Alterado para permitir a configuração da SKU da imagem do SQL ao criar ou atualizar uma VM do SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-382">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-383">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-383">Storage</span></span>
* <span data-ttu-id="f0d01-384">Corrigido o problema com a chave de conta ignorada para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="f0d01-384">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="f0d01-385">Corrigido o problema com o `storage blob sync` no Linux</span><span class="sxs-lookup"><span data-stu-id="f0d01-385">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-386">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-386">VM</span></span>
* <span data-ttu-id="f0d01-387">[VERSÃO PRÉVIA] Adicionados os comandos `vm image template` para criar imagens de VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-387">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="f0d01-388">4 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="f0d01-388">June 4, 2019</span></span>

<span data-ttu-id="f0d01-389">Versão 2.0.66</span><span class="sxs-lookup"><span data-stu-id="f0d01-389">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-390">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-390">Core</span></span>
* <span data-ttu-id="f0d01-391">Foi corrigido o bug em que os comandos falhavam quando `--output yaml` era usado com `--query`</span><span class="sxs-lookup"><span data-stu-id="f0d01-391">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-392">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-392">ACR</span></span>
* <span data-ttu-id="f0d01-393">Foi adicionado o grupo de comando 'pack acr' para a criação de Tarefas de build rápida usando Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="f0d01-393">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-394">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-394">ACS</span></span>
* <span data-ttu-id="f0d01-395">Permitir a opção de habilitar/desabilitar o complemento kube-dashboard do AKS</span><span class="sxs-lookup"><span data-stu-id="f0d01-395">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="f0d01-396">Imprimir uma mensagem amigável quando a assinatura não estiver na lista de permissões para usar o Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="f0d01-396">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="f0d01-397">Lote</span><span class="sxs-lookup"><span data-stu-id="f0d01-397">Batch</span></span>
* <span data-ttu-id="f0d01-398">Melhoria no tratamento de erro quando você não está conectado a uma conta \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="f0d01-398">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="f0d01-399">IoT</span><span class="sxs-lookup"><span data-stu-id="f0d01-399">IoT</span></span>
* <span data-ttu-id="f0d01-400">Foi adicionado o suporte para failover manual</span><span class="sxs-lookup"><span data-stu-id="f0d01-400">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-401">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-401">Network</span></span>
* <span data-ttu-id="f0d01-402">Foram adicionados os comandos `network application-gateway waf-policy` para oferecer suporte às regras de WAF personalizadas.</span><span class="sxs-lookup"><span data-stu-id="f0d01-402">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="f0d01-403">Adicionados os argumentos `--waf-policy` e `--max-capacity` para `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-403">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="f0d01-404">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-404">Resource</span></span>
* <span data-ttu-id="f0d01-405">Melhoria da mensagem de erro do `deployment create` quando não há nenhum TTY disponível</span><span class="sxs-lookup"><span data-stu-id="f0d01-405">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-406">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-406">Role</span></span>
* <span data-ttu-id="f0d01-407">O texto da Ajuda foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="f0d01-407">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="f0d01-408">Computação</span><span class="sxs-lookup"><span data-stu-id="f0d01-408">Compute</span></span>
* <span data-ttu-id="f0d01-409">Foi adicionado o suporte para `vm create` para as VMs de uma imagem gerenciada com LUNs de disco de dados que não começam em 0 ou que ignoram números</span><span class="sxs-lookup"><span data-stu-id="f0d01-409">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="f0d01-410">21 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="f0d01-410">May 21, 2019</span></span>

<span data-ttu-id="f0d01-411">Versão 2.0.65</span><span class="sxs-lookup"><span data-stu-id="f0d01-411">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-412">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-412">Core</span></span>
* <span data-ttu-id="f0d01-413">Foram adicionados comentários melhores para erros de autenticação</span><span class="sxs-lookup"><span data-stu-id="f0d01-413">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="f0d01-414">Corrigido um problema em que a CLI carregava extensões que não eram compatíveis com a versão do núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-414">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="f0d01-415">Corrigido um problema com a inicialização quando `clouds.config` está corrompido</span><span class="sxs-lookup"><span data-stu-id="f0d01-415">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-416">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-416">ACR</span></span>
* <span data-ttu-id="f0d01-417">Foi adicionado suporte das Identidades Gerenciadas para Tarefas</span><span class="sxs-lookup"><span data-stu-id="f0d01-417">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-418">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-418">ACS</span></span>
* <span data-ttu-id="f0d01-419">Corrigido o comando `openshift create` quando usado com o cliente AAD do consumidor</span><span class="sxs-lookup"><span data-stu-id="f0d01-419">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-420">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-420">AppService</span></span>
* <span data-ttu-id="f0d01-421">[PRETERIDO] Preterido o comando `functionapp devops-build` – Será removido na próxima versão</span><span class="sxs-lookup"><span data-stu-id="f0d01-421">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="f0d01-422">`functionapp devops-pipeline` foi alterado para buscar o log de build do Azure DevOps no modo detalhado</span><span class="sxs-lookup"><span data-stu-id="f0d01-422">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="f0d01-423">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--use_local_settings` foi removido do comando `functionapp devops-pipeline` – não estava operacional</span><span class="sxs-lookup"><span data-stu-id="f0d01-423">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="f0d01-424">`webapp up` foi alterado para retornar uma saída JSON se `--logs` não for usado</span><span class="sxs-lookup"><span data-stu-id="f0d01-424">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="f0d01-425">Foi adicionado suporte para escrever recursos padrão para a configuração local de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="f0d01-425">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="f0d01-426">Foi adicionado suporte para `webapp up` reimplantar um aplicativo sem usar o argumento `--location`</span><span class="sxs-lookup"><span data-stu-id="f0d01-426">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="f0d01-427">Corrigido um problema em que o valor do SKU gratuito não funcionava na criação do ASP do SKU gratuito do Linux</span><span class="sxs-lookup"><span data-stu-id="f0d01-427">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="f0d01-428">BotService</span><span class="sxs-lookup"><span data-stu-id="f0d01-428">BotService</span></span>
* <span data-ttu-id="f0d01-429">Alterado para permitir todas as capitalizações para parâmetros `--lang` em todos os comandos</span><span class="sxs-lookup"><span data-stu-id="f0d01-429">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="f0d01-430">Descrição atualizada do módulo de comando</span><span class="sxs-lookup"><span data-stu-id="f0d01-430">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="f0d01-431">Consumo</span><span class="sxs-lookup"><span data-stu-id="f0d01-431">Consumption</span></span>
* <span data-ttu-id="f0d01-432">O parâmetro obrigatório ausente foi adicionado para executar `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="f0d01-432">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="f0d01-433">IoT</span><span class="sxs-lookup"><span data-stu-id="f0d01-433">IoT</span></span>
* <span data-ttu-id="f0d01-434">Suporte adicionado para listar todas as chaves</span><span class="sxs-lookup"><span data-stu-id="f0d01-434">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-435">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-435">Network</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="f0d01-437">O argumento `--nat-gateway` foi adicionado a `network vnet subnet [create|update]` para anexar a um gateway NAT</span><span class="sxs-lookup"><span data-stu-id="f0d01-437">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="f0d01-438">Corrigido o problema de `dns zone import`, em que os nomes de registro não correspondiam ao tipo de registro</span><span class="sxs-lookup"><span data-stu-id="f0d01-438">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="f0d01-439">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f0d01-439">RDBMS</span></span>
* <span data-ttu-id="f0d01-440">Suporte a postgres e mysql adicionado para replicação geográfica</span><span class="sxs-lookup"><span data-stu-id="f0d01-440">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="f0d01-441">RBAC</span><span class="sxs-lookup"><span data-stu-id="f0d01-441">RBAC</span></span>
* <span data-ttu-id="f0d01-442">Suporte ao escopo de grupo de gerenciamento adicionado a `role assignment`</span><span class="sxs-lookup"><span data-stu-id="f0d01-442">Added support for mangement group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-443">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-443">Storage</span></span>
* <span data-ttu-id="f0d01-444">`storage blob sync`: adicionar um comando de sincronização ao armazenamento de blobs</span><span class="sxs-lookup"><span data-stu-id="f0d01-444">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="f0d01-445">Computação</span><span class="sxs-lookup"><span data-stu-id="f0d01-445">Compute</span></span>
* <span data-ttu-id="f0d01-446">`--computer-name` foi adicionado a `vm create` para configurar o nome do computador da VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-446">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="f0d01-447">`--ssh-key-value` foi renomeado para `--ssh-key-values` para `[vm|vmss] create` – Agora, pode aceitar vários valores de chave pública ou caminhos ssh</span><span class="sxs-lookup"><span data-stu-id="f0d01-447">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="f0d01-448">__Observação__: Isso **não** é uma alteração da falha – `--ssh-key-value` será analisado corretamente, pois corresponde somente a `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="f0d01-448">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="f0d01-449">O argumento `--type` de `ppg create` foi alterado para ser opcional</span><span class="sxs-lookup"><span data-stu-id="f0d01-449">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="f0d01-450">6 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="f0d01-450">May 6, 2019</span></span>

<span data-ttu-id="f0d01-451">Versão 2.0.64</span><span class="sxs-lookup"><span data-stu-id="f0d01-451">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-452">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-452">ACS</span></span>
* <span data-ttu-id="f0d01-453">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--fqdn` foi removido dos comandos `openshift`</span><span class="sxs-lookup"><span data-stu-id="f0d01-453">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="f0d01-454">Alterado para usar a versão da API do Red Hat OpenShift no Azure em disponibilidade geral</span><span class="sxs-lookup"><span data-stu-id="f0d01-454">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="f0d01-455">O sinalizador `customer-admin-group-id` foi adicionado a `openshift create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-455">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="f0d01-456">[GA] `(PREVIEW)` foi removido da opção `aks create` `--network-policy`</span><span class="sxs-lookup"><span data-stu-id="f0d01-456">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-457">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-457">Appservice</span></span>
* <span data-ttu-id="f0d01-458">[PRETERIDO] O comando `functionapp devops-build` foi preterido</span><span class="sxs-lookup"><span data-stu-id="f0d01-458">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="f0d01-459">Renomeado para `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="f0d01-459">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="f0d01-460">Corrigido ao obter o nome de usuário correto para cloudshell que estava causando a falha em `webapp up`</span><span class="sxs-lookup"><span data-stu-id="f0d01-460">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="f0d01-461">Documentação `appservice plan --sku` atualizada para refletir o appserviceplans com suporte</span><span class="sxs-lookup"><span data-stu-id="f0d01-461">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="f0d01-462">Adicionado argumentos opcionais para o grupo de recursos e plano a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="f0d01-462">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="f0d01-463">Adicionado suporte a `webapp ssh` para respeitar a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="f0d01-463">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="f0d01-464">Adicionado suporte `appserviceplan create` para a SKU gratuita do Linux</span><span class="sxs-lookup"><span data-stu-id="f0d01-464">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="f0d01-465">Alterado `webapp up` para ter uma suspensão de 30 segundos depois de definir appsetting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` para lidar com a inicialização a frio kudu</span><span class="sxs-lookup"><span data-stu-id="f0d01-465">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="f0d01-466">Adicionado suporte para tempo de execução `powershell` a `functionapp create` no Windows</span><span class="sxs-lookup"><span data-stu-id="f0d01-466">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="f0d01-467">Adicionado o comando `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="f0d01-467">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="f0d01-468">Lote</span><span class="sxs-lookup"><span data-stu-id="f0d01-468">Batch</span></span>
* <span data-ttu-id="f0d01-469">Corrigido o bug no validador para as opções `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="f0d01-469">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="f0d01-470">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="f0d01-470">Botservice</span></span>
* <span data-ttu-id="f0d01-471">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para criar um Bot de Aplicativo Web vazio por padrão (ou seja, nenhum bot será implantado no Serviço de Aplicativo)</span><span class="sxs-lookup"><span data-stu-id="f0d01-471">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="f0d01-472">O sinalizador `--echo` foi adicionado ao `bot create` para usar o comportamento antigo com `-v v4`</span><span class="sxs-lookup"><span data-stu-id="f0d01-472">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="f0d01-473">[ALTERAÇÃO SIGNIFICATIVA] O valor padrão de `--version` foi alterado para `v4`</span><span class="sxs-lookup"><span data-stu-id="f0d01-473">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="f0d01-474">__OBSERVAÇÃO:__ `bot prepare-publish` ainda usa o padrão antigo</span><span class="sxs-lookup"><span data-stu-id="f0d01-474">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="f0d01-475">[ALTERAÇÃO SIGNIFICATIVA] `--lang` foi alterado para não definir mais `Csharp` como padrão.</span><span class="sxs-lookup"><span data-stu-id="f0d01-475">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="f0d01-476">Se o comando exigir `--lang` e ele não for fornecido, o comando será um erro</span><span class="sxs-lookup"><span data-stu-id="f0d01-476">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="f0d01-477">[ALTERAÇÃO SIGNIFICATIVA] Os argumentos `--appid` e `--password` foram alterados para `bot create` ser obrigatório e agora podem ser criados por meio de `ad app create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-477">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="f0d01-478">Foi adicionada validação a `--appid` e `--password`</span><span class="sxs-lookup"><span data-stu-id="f0d01-478">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="f0d01-479">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4` foi alterado para não criar ou usar uma Conta de Armazenamento ou o Application Insights</span><span class="sxs-lookup"><span data-stu-id="f0d01-479">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="f0d01-480">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v3` foi alterado para exigir uma região em que o Application Insights está disponível</span><span class="sxs-lookup"><span data-stu-id="f0d01-480">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="f0d01-481">[ALTERAÇÃO SIGNIFICATIVA] O `bot update` foi alterado para afetar somente as propriedades específicas de um bot</span><span class="sxs-lookup"><span data-stu-id="f0d01-481">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="f0d01-482">[ALTERAÇÃO SIGNIFICATIVA] Os sinalizadores `--lang` foram alterados para aceitar `Javascript` em vez de `Node`</span><span class="sxs-lookup"><span data-stu-id="f0d01-482">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="f0d01-483">[ALTERAÇÃO SIGNIFICATIVA] O `Node` foi removido como um valor `--lang` permitido</span><span class="sxs-lookup"><span data-stu-id="f0d01-483">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="f0d01-484">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para não definir mais `SCM_DO_BUILD_DURING_DEPLOYMENT` como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="f0d01-484">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="f0d01-485">Todas as implantações por meio do Kudu atuarão de acordo com o comportamento padrão</span><span class="sxs-lookup"><span data-stu-id="f0d01-485">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="f0d01-486">O `bot download` foi alterado para os bots sem arquivos `.bot` para criar o arquivo de configuração específico a um idioma com os valores das Configurações de Aplicativo do bot</span><span class="sxs-lookup"><span data-stu-id="f0d01-486">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="f0d01-487">Adicionado o suporte `Typescript` para `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="f0d01-487">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="f0d01-488">Uma mensagem de aviso foi adicionada a `bot prepare-deploy` para os bots `Javascript` e `Typescript` para quando `--code-dir` não contiver `package.json`</span><span class="sxs-lookup"><span data-stu-id="f0d01-488">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="f0d01-489">O `bot prepare-deploy` foi alterado para retornar `true`, se bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="f0d01-489">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="f0d01-490">O log detalhado foi adicionado a `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="f0d01-490">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="f0d01-491">Mais regiões disponíveis do Application Insights foram adicionadas ao `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="f0d01-491">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="f0d01-492">Configurar</span><span class="sxs-lookup"><span data-stu-id="f0d01-492">Configure</span></span>
* <span data-ttu-id="f0d01-493">Adicionado suporte para configurações de valor padrão do argumento baseado em pasta</span><span class="sxs-lookup"><span data-stu-id="f0d01-493">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="f0d01-494">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="f0d01-494">Eventhubs</span></span>
* <span data-ttu-id="f0d01-495">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="f0d01-495">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="f0d01-496">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-496">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-497">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-497">Network</span></span>
* <span data-ttu-id="f0d01-498">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--cache` foi substituído por `--defer` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-498">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="f0d01-499">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="f0d01-499">Policy Insights</span></span>
* <span data-ttu-id="f0d01-500">Suporte adicionado a `--expand PolicyEvaluationDetails` para detalhes de avaliação de política de consulta no recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-500">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-501">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-501">Role</span></span>
* <span data-ttu-id="f0d01-502">[PRETERIDO] Alterado argumento ocultar '--password' `create-for-rbac` - suporte será removido em maio de 2019</span><span class="sxs-lookup"><span data-stu-id="f0d01-502">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="f0d01-503">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="f0d01-503">Service Bus</span></span>
* <span data-ttu-id="f0d01-504">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="f0d01-504">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="f0d01-505">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-505">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="f0d01-506">`topic [create|update]` foi fixado para permitir suporte a `--max-size` para valores de 10, 20, 40 e 80 GB com a SKU Premium</span><span class="sxs-lookup"><span data-stu-id="f0d01-506">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-507">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-507">SQL</span></span>
* <span data-ttu-id="f0d01-508">Adicionados os comandos `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-508">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-509">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-509">VM</span></span>
* <span data-ttu-id="f0d01-510">O `--protect-from-scale-in` e o `--protect-from-scale-set-actions` foram adicionados a `vmss update` para habilitar atualizações à política de proteção das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="f0d01-510">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="f0d01-511">Adicionado a `--instance-id` e `vmss update` para habilitar atualização genérica das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="f0d01-511">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="f0d01-512">`--instance-id` foi adicionado a `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="f0d01-512">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="f0d01-513">Adicionado um novo grupo de comandos `ppg` para gerenciar grupos de posicionamento de proximidade</span><span class="sxs-lookup"><span data-stu-id="f0d01-513">Added new `ppg` command group for manging Proximity Placement Groups</span></span>
* <span data-ttu-id="f0d01-514">Adicionado a `--ppg`, `[vm|vmss] create` e `vm availability-set create` para gerenciar PPGs</span><span class="sxs-lookup"><span data-stu-id="f0d01-514">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="f0d01-515">Parâmetro `--hyper-v-generation` adicionado a `image create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-515">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="f0d01-516">23 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="f0d01-516">April 23, 2019</span></span>

<span data-ttu-id="f0d01-517">Versão 2.0.63</span><span class="sxs-lookup"><span data-stu-id="f0d01-517">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-518">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-518">ACS</span></span>
* <span data-ttu-id="f0d01-519">Alterado `aks get-credentials` para solicitar substituição dos valores duplicados</span><span class="sxs-lookup"><span data-stu-id="f0d01-519">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="f0d01-520">Removido `(PREVIEW)` dos comandos de espaços de desenvolvimento "aks use-dev-espaces" e "aks remove-dev-espaces"</span><span class="sxs-lookup"><span data-stu-id="f0d01-520">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="f0d01-521">AMS</span><span class="sxs-lookup"><span data-stu-id="f0d01-521">AMS</span></span>
* <span data-ttu-id="f0d01-522">Corrigido o bug com a atualização de filtros de conta e de ativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-522">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-523">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-523">AppService</span></span>
* <span data-ttu-id="f0d01-524">Adicionado suporte para o ASE e o tempo limite para `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="f0d01-524">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="f0d01-525">Adicionado suporte para o estabelecimento de CI CD em um pipeline do Azure DevOps de um repositório do Github para aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="f0d01-525">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="f0d01-526">Adicionado argumento `--github-pat` a `functionapp devops-build create` para aceitar o token de acesso pessoal do Github</span><span class="sxs-lookup"><span data-stu-id="f0d01-526">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="f0d01-527">Adicionado argumento `--github-repository` a `functionapp devops-build create` para aceitar o repositório Github que contém um código-fonte functionapp</span><span class="sxs-lookup"><span data-stu-id="f0d01-527">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="f0d01-528">Problema corrigido em que `az webapp up --logs` estava falhando com um erro e atualização da versão .NETCORE padrão para 2.1</span><span class="sxs-lookup"><span data-stu-id="f0d01-528">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="f0d01-529">Configurações de functionapp desnecessárias removidas durante a criação de um aplicativo de funções com plano de consumo</span><span class="sxs-lookup"><span data-stu-id="f0d01-529">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="f0d01-530">Alterado `webapp up` para que a cadeia de caracteres padrão asp agora acrescente o número no final para criar um novo ASP com base nas opções de SKU</span><span class="sxs-lookup"><span data-stu-id="f0d01-530">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="f0d01-531">Adicionado `-b` como uma opção a `webapp up` para iniciar o aplicativo no navegador</span><span class="sxs-lookup"><span data-stu-id="f0d01-531">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="f0d01-532">Alterado `webapp deployment source config zip` para lidar com a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="f0d01-532">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="f0d01-533">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="f0d01-533">Deployment Manager</span></span>
* <span data-ttu-id="f0d01-534">[VERSÃO PRÉVIA] Criar e gerenciar artefatos que dão suporte a distribuições</span><span class="sxs-lookup"><span data-stu-id="f0d01-534">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="f0d01-535">Laboratório</span><span class="sxs-lookup"><span data-stu-id="f0d01-535">Lab</span></span>
* <span data-ttu-id="f0d01-536">Corrigido o bug que causa uma saída inicial</span><span class="sxs-lookup"><span data-stu-id="f0d01-536">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-537">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-537">Network</span></span>
* <span data-ttu-id="f0d01-538">Adicionada delegação de servidor de nome automática a `dns zone create` no pai durante a criação da zona filho</span><span class="sxs-lookup"><span data-stu-id="f0d01-538">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-539">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-539">Resource</span></span>
* <span data-ttu-id="f0d01-540">[PRETERIDO] Argumentos `--link-id`, `--target-id` e `--filter-string` preteridos de `resource link`</span><span class="sxs-lookup"><span data-stu-id="f0d01-540">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="f0d01-541">Use os argumentos `--link`, `--target` e `--filter`</span><span class="sxs-lookup"><span data-stu-id="f0d01-541">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="f0d01-542">Corrigido o problema em que os comandos `resource link [create|update]` não funcionavam</span><span class="sxs-lookup"><span data-stu-id="f0d01-542">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="f0d01-543">Corrigido um problema em que a exclusão usando uma ID de recurso poderia causar falha no erro</span><span class="sxs-lookup"><span data-stu-id="f0d01-543">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-544">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-544">SQL</span></span>
* <span data-ttu-id="f0d01-545">Adicionado suporte para fuso horário personalizado nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="f0d01-545">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="f0d01-546">Alterado para permitir que o nome do pool Elástico seja usado com `sql db update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-546">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="f0d01-547">Adicionado o suporte `--no-wait` para `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-547">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="f0d01-548">Adicionado o comando `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="f0d01-548">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-549">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-549">Storage</span></span>
* <span data-ttu-id="f0d01-550">Corrigido o problema com tokens SAS com codificação dupla em `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="f0d01-550">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-551">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-551">VM</span></span>
* <span data-ttu-id="f0d01-552">Adicionado sinalizador `--skip-shutdown` a `vm|vmss stop` para desligar as VMs sem o desligamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-552">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="f0d01-553">Adicionado argumento `--storage-account-type` a `sig image-version create` para definir o tipo de conta do perfil de publicação</span><span class="sxs-lookup"><span data-stu-id="f0d01-553">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="f0d01-554">Adicionado argumento `--target-regions` a `sig image-version create` para permitir definir os tipos de conta de armazenamento específico da região</span><span class="sxs-lookup"><span data-stu-id="f0d01-554">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="f0d01-555">9 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="f0d01-555">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-556">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-556">Core</span></span>
* <span data-ttu-id="f0d01-557">Correção do problema em que algumas extensões mostraram uma versão do `Unknown` e não podiam ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="f0d01-557">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-558">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-558">ACR</span></span>
* <span data-ttu-id="f0d01-559">Adição de suporte para execução de uma imagem sem contexto</span><span class="sxs-lookup"><span data-stu-id="f0d01-559">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="f0d01-560">AMS</span><span class="sxs-lookup"><span data-stu-id="f0d01-560">AMS</span></span>
* [PRETERIDO]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [ALTERAÇÃO SIGNIFICATIVA]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="f0d01-563">Adição de suporte para novos parâmetros de criptografia em `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-563">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="f0d01-564">Adição de novo parâmetro `--filters` a `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-564">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-565">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-565">AppService</span></span>
* <span data-ttu-id="f0d01-566">Adicionado o suporte `--logs` para `webapp up`</span><span class="sxs-lookup"><span data-stu-id="f0d01-566">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="f0d01-567">Correção de problemas do comando `functionapp devops-build create` de geração de `azure-pipelines.yml`</span><span class="sxs-lookup"><span data-stu-id="f0d01-567">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="f0d01-568">Melhoria do tratamento de erros e indicadores `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-568">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="f0d01-569">[ALTERAÇÃO SIGNIFICATIVA] Remoção do sinalizador `--local-git` para o comando `devops-build`; a detecção de git local e a manipulação são obrigatórias para a criação de pipelines do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="f0d01-569">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="f0d01-570">Adição de suporte para a criação de planos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="f0d01-570">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="f0d01-571">Adição da capacidade de trocar um plano sob um aplicativo de funções usando `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="f0d01-571">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="f0d01-572">Adição de suporte para configurações de expansão de plano Premium do Azure Functions</span><span class="sxs-lookup"><span data-stu-id="f0d01-572">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="f0d01-573">CDN</span><span class="sxs-lookup"><span data-stu-id="f0d01-573">CDN</span></span>
* <span data-ttu-id="f0d01-574">Adição de suporte para `Microsoft_Standard` e `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="f0d01-574">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="f0d01-575">Comentários</span><span class="sxs-lookup"><span data-stu-id="f0d01-575">Feedback</span></span>
* <span data-ttu-id="f0d01-576">Alteração de `feedback` para mostrar metadados em comandos executados recentemente</span><span class="sxs-lookup"><span data-stu-id="f0d01-576">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="f0d01-577">Alteração de `feedback` para solicitar o auxílio do usuário no processo de criação de problema abrindo um navegador e usando um modelo de problema</span><span class="sxs-lookup"><span data-stu-id="f0d01-577">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="f0d01-578">Alteração do `feedback` para imprimir o corpo do problema ao executar com '--verbose'</span><span class="sxs-lookup"><span data-stu-id="f0d01-578">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="f0d01-579">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f0d01-579">Monitor</span></span>
* <span data-ttu-id="f0d01-580">Correção de um problema em que “count” não era um valor permitido com `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-580">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="f0d01-581">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-581">Network</span></span>
* <span data-ttu-id="f0d01-582">Correção do formato de tabela que não estava sendo exibido com `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="f0d01-582">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="f0d01-583">Adição dos comandos `list-request-headers` e `list-response-headers` para `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="f0d01-583">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="f0d01-584">Adição do comando `list-server-variables` para `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="f0d01-584">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="f0d01-585">Correção de um problema em que a atualização do estado do link em uma porta express-route geraria uma exceção de atributo desconhecido `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-585">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="f0d01-586">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="f0d01-586">PrivateDNS</span></span>
* <span data-ttu-id="f0d01-587">Adição de `network private-dns` para zonas de DNS privado</span><span class="sxs-lookup"><span data-stu-id="f0d01-587">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-588">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-588">Resource</span></span>
* <span data-ttu-id="f0d01-589">Correção do problema com `deployment create` e `group deployment create`, em que um arquivo de parâmetros com um conjunto vazio de parâmetros não funcionaria</span><span class="sxs-lookup"><span data-stu-id="f0d01-589">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-590">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-590">Role</span></span>
* <span data-ttu-id="f0d01-591">Correção de `create-for-rbac` para lidar corretamente com `--years`</span><span class="sxs-lookup"><span data-stu-id="f0d01-591">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="f0d01-592">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `role assignment delete` para solicitar ao excluir todas as atribuições na assinatura incondicionalmente</span><span class="sxs-lookup"><span data-stu-id="f0d01-592">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-593">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-593">SQL</span></span>
* <span data-ttu-id="f0d01-594">Atualização de `sql mi [create|update]` com as propriedades proxyOverride e publicDataEndpointEnabled</span><span class="sxs-lookup"><span data-stu-id="f0d01-594">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-595">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-595">Storage</span></span>
* <span data-ttu-id="f0d01-596">[ALTERAÇÃO SIGNIFICATIVA] Remoção do resultado de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="f0d01-596">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="f0d01-597">Adição de `--full-uri` a `storage blob generate-sas` para criar o URI completo para o blob com SAS</span><span class="sxs-lookup"><span data-stu-id="f0d01-597">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="f0d01-598">Adição de `--file-snapshot` a `storage file copy start` para copiar arquivo do instantâneo</span><span class="sxs-lookup"><span data-stu-id="f0d01-598">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="f0d01-599">Alteração de `storage blob copy cancel` para mostrar apenas o erro em vez da exceção para NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="f0d01-599">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="f0d01-600">26 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="f0d01-600">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="f0d01-601">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-601">Core</span></span>
* <span data-ttu-id="f0d01-602">Correção de problemas com incompatibilidade da extensão de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="f0d01-602">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="f0d01-603">Agora o tratamento de erros encaminha os clientes para a página de problemas</span><span class="sxs-lookup"><span data-stu-id="f0d01-603">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="f0d01-604">Nuvem</span><span class="sxs-lookup"><span data-stu-id="f0d01-604">Cloud</span></span>
* <span data-ttu-id="f0d01-605">Erro de “assinatura não encontrada” corrigido em `cloud set`</span><span class="sxs-lookup"><span data-stu-id="f0d01-605">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-606">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-606">ACR</span></span>
* <span data-ttu-id="f0d01-607">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="f0d01-607">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="f0d01-608">`--auth-mode` adicionado aos comandos `acr build`, `acr run`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-608">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="f0d01-609">Grupo de comandos “acr task credential” adicionado para gerenciar as credenciais de uma Tarefa</span><span class="sxs-lookup"><span data-stu-id="f0d01-609">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="f0d01-610">“--no-wait” adicionado ao comando `acr build`</span><span class="sxs-lookup"><span data-stu-id="f0d01-610">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-611">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-611">AppService</span></span>
* <span data-ttu-id="f0d01-612">Bug corrigido onde `webapp up` não estava lidando corretamente com a execução do diretório vazio ou do cenário de código desconhecido</span><span class="sxs-lookup"><span data-stu-id="f0d01-612">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="f0d01-613">Bug corrigido onde os slots não funcionavam para `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="f0d01-613">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="f0d01-614">Serviço de BOT</span><span class="sxs-lookup"><span data-stu-id="f0d01-614">BOT Service</span></span>
* <span data-ttu-id="f0d01-615">`bot prepare-deploy` adicionado para se preparar para a implantação de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="f0d01-615">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="f0d01-616">`bot create --kind registration` alterado para mostrar a senha se ela não for fornecida</span><span class="sxs-lookup"><span data-stu-id="f0d01-616">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="f0d01-617">[ALTERAÇÃO SIGNIFICATIVA] `--endpoint` alterado em `bot create --kind registration` como padrão para uma cadeia de caracteres vazia, em vez de ser requerido</span><span class="sxs-lookup"><span data-stu-id="f0d01-617">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="f0d01-618">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="f0d01-618">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="f0d01-619">CDN</span><span class="sxs-lookup"><span data-stu-id="f0d01-619">CDN</span></span>
* <span data-ttu-id="f0d01-620">Adicionado o suporte ao `--no-wait` para `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-620">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [ALTERAÇÃO SIGNIFICATIVA]: `cdn endpoint create` alterado para o comportamento de cache da cadeia de consulta padrão.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="f0d01-622">Não há mais padrão para "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="f0d01-622">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="f0d01-623">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="f0d01-623">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f0d01-624">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="f0d01-624">Cosmosdb</span></span>
* <span data-ttu-id="f0d01-625">Suporte adicionado para `--enable-multiple-write-locations` na atualização da conta</span><span class="sxs-lookup"><span data-stu-id="f0d01-625">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="f0d01-626">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f0d01-626">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="f0d01-627">Interativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-627">Interactive</span></span>
* <span data-ttu-id="f0d01-628">Incompatibilidade corrigida com a extensão Interativa instalada por meio do azdev</span><span class="sxs-lookup"><span data-stu-id="f0d01-628">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="f0d01-629">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f0d01-629">Monitor</span></span>
* <span data-ttu-id="f0d01-630">Alterado para permitir o valor de dimensão `*` para `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-630">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-631">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-631">Network</span></span>
* <span data-ttu-id="f0d01-632">Grupo de comandos `rewrite-rule` adicionado em `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="f0d01-632">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="f0d01-633">Perfil</span><span class="sxs-lookup"><span data-stu-id="f0d01-633">Profile</span></span>
* <span data-ttu-id="f0d01-634">Suporte de conta no nível do locatário para a identidade de serviço gerenciado adicionado em `login`</span><span class="sxs-lookup"><span data-stu-id="f0d01-634">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="f0d01-635">Postgres</span><span class="sxs-lookup"><span data-stu-id="f0d01-635">Postgres</span></span> 
* <span data-ttu-id="f0d01-636">Adicionados os comandos postgresql `replica` e `restart server`</span><span class="sxs-lookup"><span data-stu-id="f0d01-636">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="f0d01-637">Alterado para obter o local padrão do grupo de recursos quando não fornecido para criar servidores e adicionar validação para os dias de retenção</span><span class="sxs-lookup"><span data-stu-id="f0d01-637">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-638">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-638">Resource</span></span>
* <span data-ttu-id="f0d01-639">Saída da tabela aperfeiçoada para `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-639">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="f0d01-640">Corrigido o problema com `deployment [create|validate]` onde o tipo secureObject não era reconhecido</span><span class="sxs-lookup"><span data-stu-id="f0d01-640">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="f0d01-641">Grafo</span><span class="sxs-lookup"><span data-stu-id="f0d01-641">Graph</span></span>
* <span data-ttu-id="f0d01-642">Adicionado o suporte ao `--end-date` para `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="f0d01-642">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="f0d01-643">Suporte adicionado para acrescentar permissões com `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="f0d01-643">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="f0d01-644">Bug corrigido com `ad app permission list` quando não havia nenhuma permissão</span><span class="sxs-lookup"><span data-stu-id="f0d01-644">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="f0d01-645">`ad sp delete` alterado para ignorar a exclusão da atribuição de função se a conta atual não tem nenhuma assinatura</span><span class="sxs-lookup"><span data-stu-id="f0d01-645">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="f0d01-646">`ad app create` alterado para `--identifier-uris` passar para lista vazia como padrão se não fornecido</span><span class="sxs-lookup"><span data-stu-id="f0d01-646">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-647">storage</span><span class="sxs-lookup"><span data-stu-id="f0d01-647">storage</span></span>
* <span data-ttu-id="f0d01-648">`--snapshot` adicionado a `storage file download-batch` para baixar de um instantâneo de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-648">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="f0d01-649">Barra de progresso `storage blob [download-batch|upload-batch]` alterada para ser menos detalhada e indicar o blob atual</span><span class="sxs-lookup"><span data-stu-id="f0d01-649">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="f0d01-650">Problema corrigido com `storage account update` ao atualizar os parâmetros de criptografia</span><span class="sxs-lookup"><span data-stu-id="f0d01-650">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="f0d01-651">Problema corrigido onde `storage blob show` falharia ao usar o oauth (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="f0d01-651">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-652">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-652">VM</span></span>
* <span data-ttu-id="f0d01-653">Adicionado o comando `image update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-653">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="f0d01-654">12 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="f0d01-654">March 12, 2019</span></span>

<span data-ttu-id="f0d01-655">Versão 2.0.60</span><span class="sxs-lookup"><span data-stu-id="f0d01-655">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-656">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-656">Core</span></span>

* <span data-ttu-id="f0d01-657">Foi corrigido um erro incorreto no `cloud set` sobre assinatura não encontrada.</span><span class="sxs-lookup"><span data-stu-id="f0d01-657">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-658">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-658">ACR</span></span>

* <span data-ttu-id="f0d01-659">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="f0d01-659">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-660">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-660">ACS</span></span>

* <span data-ttu-id="f0d01-661">Alteração para ignorar o parâmetro `--listen-address` para `aks browse` se ele não for compatível com kubectl</span><span class="sxs-lookup"><span data-stu-id="f0d01-661">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="f0d01-662">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-662">AppService</span></span>

* <span data-ttu-id="f0d01-663">Adicionado `[webapp|functionapp] deployment list-publishing-credentials` para obter a URL de publicação do Kudu e suas credenciais.</span><span class="sxs-lookup"><span data-stu-id="f0d01-663">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="f0d01-664">Removida a instrução de impressão errônea de `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-664">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="f0d01-665">Corrigido `functionapp` para definir a imagem correta do tempo de execução nos planos do Serviço de Aplicativo no Linux.</span><span class="sxs-lookup"><span data-stu-id="f0d01-665">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="f0d01-666">Removida a marca de versão prévia do `webapp up` e adicionadas melhorias ao comando.</span><span class="sxs-lookup"><span data-stu-id="f0d01-666">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="f0d01-667">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="f0d01-667">Botservice</span></span>

* <span data-ttu-id="f0d01-668">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="f0d01-668">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="f0d01-669">Adicionados `Microsoft-BotFramework-AppId` e `Microsoft-BotFramework-AppPassword` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="f0d01-669">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="f0d01-670">Removidas as aspas simples da saída de comando `bot publish`, no final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-670">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="f0d01-671">Alterado `bot publish` para que seja assíncrono.</span><span class="sxs-lookup"><span data-stu-id="f0d01-671">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="f0d01-672">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-672">Container</span></span>

* <span data-ttu-id="f0d01-673">Adicionado o argumento `--no-wait` para `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-673">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="f0d01-674">EventHub</span><span class="sxs-lookup"><span data-stu-id="f0d01-674">EventHub</span></span>

* <span data-ttu-id="f0d01-675">Adicionado o sinalizador `--skip-empty-archives` a `eventhub create|update` para dar suporte a arquivos vazios na captura.</span><span class="sxs-lookup"><span data-stu-id="f0d01-675">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="f0d01-676">Localizar</span><span class="sxs-lookup"><span data-stu-id="f0d01-676">Find</span></span>

* <span data-ttu-id="f0d01-677">Atualização de funcionalidade principal</span><span class="sxs-lookup"><span data-stu-id="f0d01-677">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f0d01-678">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f0d01-678">HDInsight</span></span>

* <span data-ttu-id="f0d01-679">Adicionado o parâmetro `--storage-account-managed-identity` a `hdinsight create` para oferecer suporte ao MSI do ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="f0d01-679">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-680">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-680">Network</span></span>

* <span data-ttu-id="f0d01-681">Corrigido o problema com `vpn-connection update`, onde a atualização de uma conexão VPN entre gateways em assinaturas diferentes falharia.</span><span class="sxs-lookup"><span data-stu-id="f0d01-681">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="f0d01-682">Rdbms</span><span class="sxs-lookup"><span data-stu-id="f0d01-682">Rdbms</span></span>

* <span data-ttu-id="f0d01-683">Correções secundárias para obter a localização padrão do grupo de recursos, quando não fornecida, para criar servidores e adicionar validação nos dias de retenção.</span><span class="sxs-lookup"><span data-stu-id="f0d01-683">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-684">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-684">Role</span></span>

* <span data-ttu-id="f0d01-685">Corrigido `role definition update` para usar ID a fim de resolver a definição corretamente.</span><span class="sxs-lookup"><span data-stu-id="f0d01-685">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="f0d01-686">Alterado `ad app credential reset` para remover a suposição de que a entidade de serviço do aplicativo já existe.</span><span class="sxs-lookup"><span data-stu-id="f0d01-686">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f0d01-687">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f0d01-687">Service Fabric</span></span>

* <span data-ttu-id="f0d01-688">Corrigido o problema com o fato de `sf cluster list` não ser iterável.</span><span class="sxs-lookup"><span data-stu-id="f0d01-688">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="f0d01-689">26 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="f0d01-689">February 26, 2019</span></span>

<span data-ttu-id="f0d01-690">Versão 2.0.59</span><span class="sxs-lookup"><span data-stu-id="f0d01-690">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-691">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-691">Core</span></span>

* <span data-ttu-id="f0d01-692">Corrigido o problema onde algumas instâncias usando `--subscription NAME` produziriam uma exceção</span><span class="sxs-lookup"><span data-stu-id="f0d01-692">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-693">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-693">ACR</span></span>

* <span data-ttu-id="f0d01-694">Parâmetro `--target` adicionado para os comandos `acr build`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-694">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="f0d01-695">Melhor tratamento de erros para os comandos de execução quando não conectado ao Azure</span><span class="sxs-lookup"><span data-stu-id="f0d01-695">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-696">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-696">ACS</span></span>

* <span data-ttu-id="f0d01-697">Opção `--listen-address` adicionada a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="f0d01-697">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-698">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-698">AppService</span></span>

* <span data-ttu-id="f0d01-699">Adicionado o comando `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="f0d01-699">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="f0d01-700">Lote</span><span class="sxs-lookup"><span data-stu-id="f0d01-700">Batch</span></span>
* <span data-ttu-id="f0d01-701">[ALTERAÇÃO SIGNIFICATIVA] Comando `batch pool upgrade os` removido</span><span class="sxs-lookup"><span data-stu-id="f0d01-701">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="f0d01-702">[ALTERAÇÃO SIGNIFICATIVA] Propriedade `Pacakges` removida das respostas `Application`</span><span class="sxs-lookup"><span data-stu-id="f0d01-702">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="f0d01-703">Comando `batch application package list` adicionado para listar os pacotes de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-703">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="f0d01-704">[ALTERAÇÃO SIGNIFICATIVA] `--application-id` alterado para `--application-name` em todos os comandos `batch application`,</span><span class="sxs-lookup"><span data-stu-id="f0d01-704">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="f0d01-705">O argumento `--json-file` foi adicionado aos comandos para a solicitação de resposta da API bruta</span><span class="sxs-lookup"><span data-stu-id="f0d01-705">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="f0d01-706">Validação atualizada para incluir automaticamente `https://` em todos os pontos de extremidade, se ausente</span><span class="sxs-lookup"><span data-stu-id="f0d01-706">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f0d01-707">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f0d01-707">CosmosDB</span></span>

* <span data-ttu-id="f0d01-708">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f0d01-708">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="f0d01-709">Kusto</span><span class="sxs-lookup"><span data-stu-id="f0d01-709">Kusto</span></span>

* <span data-ttu-id="f0d01-710">[ALTERAÇÃO SIGNIFICATIVA] Os tipos `hot_cache_period` e `soft_delete_period` foram alterados do banco de dados para o formato de duração ISO8601</span><span class="sxs-lookup"><span data-stu-id="f0d01-710">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-711">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-711">Network</span></span>

* <span data-ttu-id="f0d01-712">Adicionado o argumento `--express-route-gateway-bypass` para `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-712">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="f0d01-713">Foram adicionados os grupos de comando a partir das extensões `express-route`</span><span class="sxs-lookup"><span data-stu-id="f0d01-713">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="f0d01-714">Os grupos de comando `express-route gateway` e `express-route port` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="f0d01-714">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="f0d01-715">Adicionado o argumento `--legacy-mode` para `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-715">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="f0d01-716">Os argumentos `--allow-classic-operations` e `--express-route-port` foram adicionados a `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-716">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="f0d01-717">Adicionado o argumento `--gateway-default-site` para `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-717">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="f0d01-718">Os comandos `ipsec-policy` foram adicionados a `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="f0d01-718">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-719">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-719">Resource</span></span>

* <span data-ttu-id="f0d01-720">Foi corrigido o problema com `deployment create` em que o campo do tipo diferencia letras maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="f0d01-720">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="f0d01-721">Foi adicionado o suporte para arquivo de parâmetros de URI a `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-721">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="f0d01-722">Foi adicionado o suporte para parâmetros de URI e definições a `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-722">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="f0d01-723">Foi corrigido o tratamento de parâmetros e regras para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-723">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="f0d01-724">Foi corrigido o problema com `resource show/update/delete/tag/invoke-action` em que as IDs de assinatura cruzada não respeitaram corretamente a ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="f0d01-724">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-725">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-725">Role</span></span>

* <span data-ttu-id="f0d01-726">Foi adicionado o suporte para as funções do aplicativo a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-726">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-727">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-727">VM</span></span>

* <span data-ttu-id="f0d01-728">Foi corrigido o problema com `vm create where ` – a rede acelerada não foi habilitada por padrão no Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="f0d01-728">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="f0d01-729">12 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="f0d01-729">February 12, 2019</span></span>

<span data-ttu-id="f0d01-730">Versão 2.0.58</span><span class="sxs-lookup"><span data-stu-id="f0d01-730">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-731">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-731">Core</span></span>

* <span data-ttu-id="f0d01-732">`az --version` agora exibe uma notificação se você tiver pacotes para atualização</span><span class="sxs-lookup"><span data-stu-id="f0d01-732">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="f0d01-733">A regressão em que `--ids` não pode ser usado com a saída JSON foi corrigida</span><span class="sxs-lookup"><span data-stu-id="f0d01-733">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-734">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-734">ACR</span></span>
* <span data-ttu-id="f0d01-735">[ALTERAÇÃO SIGNIFICATIVA] O grupo de comandos `acr build-task` foi removido</span><span class="sxs-lookup"><span data-stu-id="f0d01-735">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="f0d01-736">[ALTERAÇÃO SIGNIFICATIVA] As opções `--tag` e `--manifest` de `acr repository delete` foram removidas</span><span class="sxs-lookup"><span data-stu-id="f0d01-736">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-737">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-737">ACS</span></span>
* <span data-ttu-id="f0d01-738">Suporte adicionado a `aks [enable-addons|disable-addons]` para nomes que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="f0d01-738">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="f0d01-739">Suporte adicionado para a operação de atualização do Azure Active Directory usando `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="f0d01-739">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="f0d01-740">Um esclarecimento informando que `--output` é ignorado para `aks get-credentials` foi adicionado</span><span class="sxs-lookup"><span data-stu-id="f0d01-740">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="f0d01-741">AMS</span><span class="sxs-lookup"><span data-stu-id="f0d01-741">AMS</span></span>
* <span data-ttu-id="f0d01-742">Adicionados os comandos `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="f0d01-742">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="f0d01-743">Adicionados os comandos `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="f0d01-743">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-744">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-744">Appservice</span></span>
* <span data-ttu-id="f0d01-745">Foi adicionada a capacidade de criar e configurar funções usando contêineres de ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-745">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="f0d01-746">Suporte adicionado para a atualização das configurações de aplicativos Web por meio de JSON</span><span class="sxs-lookup"><span data-stu-id="f0d01-746">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="f0d01-747">A ajuda foi aprimorada para `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-747">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="f0d01-748">Suporte adicionado para o App Insights para auxiliar na criação de aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="f0d01-748">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="f0d01-749">Os problemas com o SSH do aplicativo Web foram corrigidos</span><span class="sxs-lookup"><span data-stu-id="f0d01-749">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="f0d01-750">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="f0d01-750">Botservice</span></span>
* <span data-ttu-id="f0d01-751">A experiência do usuário para `bot publish` foi aprimorada</span><span class="sxs-lookup"><span data-stu-id="f0d01-751">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="f0d01-752">Foram adicionados avisos de tempos limite ao executar `npm install` durante `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="f0d01-752">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="f0d01-753">O caractere inválido `.` de `--name` em `az bot create` foi removido</span><span class="sxs-lookup"><span data-stu-id="f0d01-753">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="f0d01-754">Alteração para interromper a geração aleatória de nomes de recursos durante a criação do Armazenamento do Azure, Plano do Serviço de Aplicativo, Aplicativo Web/de funções e Application Insights</span><span class="sxs-lookup"><span data-stu-id="f0d01-754">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="f0d01-755">[PRETERIDO] O argumento `--proj-name` foi preterido em favor de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="f0d01-755">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="f0d01-756">`az bot publish` foi alterado para remover arquivos de implantação do Node.js do IIS buscados, caso eles já não existissem</span><span class="sxs-lookup"><span data-stu-id="f0d01-756">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="f0d01-757">Foi adicionado o argumento `--keep-node-modules` para `az bot publish` para não excluir a pasta `node_modules` no Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-757">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="f0d01-758">O par chave-valor `"publishCommand"` foi adicionado à saída de `az bot create` durante a criação de uma função do Azure ou bot de aplicativo Web</span><span class="sxs-lookup"><span data-stu-id="f0d01-758">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="f0d01-759">O valor de `"publishCommand"` é um comando `az bot publish` que é automaticamente preenchido com os parâmetros necessários para publicar o bot recém-criado</span><span class="sxs-lookup"><span data-stu-id="f0d01-759">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="f0d01-760">O `"WEBSITE_NODE_DEFAULT_VERSION"` foi atualizado no modelo do ARM para que os bots de SDK v4 usem 10.14.1 em vez de 8.9.4</span><span class="sxs-lookup"><span data-stu-id="f0d01-760">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="f0d01-761">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f0d01-761">Key Vault</span></span>
* <span data-ttu-id="f0d01-762">Foi corrigido o problema com `keyvault secret backup`, em que alguns usuários recebiam um erro `unexpected_keyword` ao usar `--id`</span><span class="sxs-lookup"><span data-stu-id="f0d01-762">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="f0d01-763">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f0d01-763">Monitor</span></span>
* <span data-ttu-id="f0d01-764">`monitor metrics alert [create|update]` foi alterado para permitir o valor dimensional `*`</span><span class="sxs-lookup"><span data-stu-id="f0d01-764">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-765">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-765">Network</span></span>
* <span data-ttu-id="f0d01-766">`dns zone export` foi alterado para garantir que CNAMEs exportados fossem FQDNs</span><span class="sxs-lookup"><span data-stu-id="f0d01-766">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="f0d01-767">O parâmetro `--gateway-name` foi adicionado a `nic ip-config address-pool [add|remove]` para dar suporte a pools de endereços de back-end de gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-767">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="f0d01-768">Os argumentos `--traffic-analytics` e `--workspace` foram adicionados a `network watcher flow-log configure` para dar suporte à análise de tráfego por meio de um espaço de trabalho do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="f0d01-768">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="f0d01-769">`--idle-timeout` e `--floating-ip` foram adicionados a `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-769">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="f0d01-770">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="f0d01-770">Policy Insights</span></span>
* <span data-ttu-id="f0d01-771">Os comandos `policy remediation` foram adicionados para dar suporte a recursos de correção de política de recursos</span><span class="sxs-lookup"><span data-stu-id="f0d01-771">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="f0d01-772">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f0d01-772">RDBMS</span></span>
* <span data-ttu-id="f0d01-773">A mensagem e os parâmetros de comando de ajuda foram aprimorados</span><span class="sxs-lookup"><span data-stu-id="f0d01-773">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="f0d01-774">Redis</span><span class="sxs-lookup"><span data-stu-id="f0d01-774">Redis</span></span>
* <span data-ttu-id="f0d01-775">Foram adicionados comandos para gerenciar regras de firewall (criar, atualizar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="f0d01-775">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="f0d01-776">Foram adicionados comandos para gerenciar links do servidor (criar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="f0d01-776">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="f0d01-777">Foram adicionados comandos para gerenciar o agendamento de patches (criar, atualizar, excluir, mostrar)</span><span class="sxs-lookup"><span data-stu-id="f0d01-777">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="f0d01-778">Suporte adicionado para Zonas de Disponibilidade e versão mínima de TLS para criar Redis</span><span class="sxs-lookup"><span data-stu-id="f0d01-778">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="f0d01-779">[ALTERAÇÃO SIGNIFICATIVA] Os comandos `redis update-settings` e `redis list-all` foram removidos</span><span class="sxs-lookup"><span data-stu-id="f0d01-779">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="f0d01-780">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro para `redis create`: “configurações de locatário” não é aceito no formato chave[=valor]</span><span class="sxs-lookup"><span data-stu-id="f0d01-780">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="f0d01-781">[PRETERIDO] Uma mensagem de aviso foi adicionada para preterir o comando `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="f0d01-781">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-782">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-782">Role</span></span>
* <span data-ttu-id="f0d01-783">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido dos comandos `vm` para esta localização</span><span class="sxs-lookup"><span data-stu-id="f0d01-783">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="f0d01-784">SQL VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-784">SQL VM</span></span>
* <span data-ttu-id="f0d01-785">[PRETERIDO] O argumento `--boostrap-acc-pwd` foi preterido devido a um erro de digitação</span><span class="sxs-lookup"><span data-stu-id="f0d01-785">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-786">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-786">VM</span></span>
* <span data-ttu-id="f0d01-787">`vm list-skus` foi alterado para permitir o uso de `--all` no lugar de `--all true`</span><span class="sxs-lookup"><span data-stu-id="f0d01-787">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="f0d01-788">Adicionado `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-788">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="f0d01-789">Foi corrigido o bug em que `vmss encryption enable` falhava se fosse executado anteriormente</span><span class="sxs-lookup"><span data-stu-id="f0d01-789">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="f0d01-790">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido para os comandos `role`</span><span class="sxs-lookup"><span data-stu-id="f0d01-790">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="f0d01-791">31 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="f0d01-791">January 31, 2019</span></span>

<span data-ttu-id="f0d01-792">Versão 2.0.57</span><span class="sxs-lookup"><span data-stu-id="f0d01-792">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-793">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-793">Core</span></span>

* <span data-ttu-id="f0d01-794">Hotfix para o [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="f0d01-794">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="f0d01-795">28 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="f0d01-795">January 28, 2019</span></span>

<span data-ttu-id="f0d01-796">Versão 2.0.56</span><span class="sxs-lookup"><span data-stu-id="f0d01-796">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-797">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-797">ACR</span></span>
* <span data-ttu-id="f0d01-798">Suporte adicionado para regras de rede virtual/IP</span><span class="sxs-lookup"><span data-stu-id="f0d01-798">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-799">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-799">ACS</span></span>
* <span data-ttu-id="f0d01-800">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="f0d01-800">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="f0d01-801">Comandos do OpenShift gerenciado foram adicionados</span><span class="sxs-lookup"><span data-stu-id="f0d01-801">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="f0d01-802">Suporte adicionado para operações de atualização da entidade de serviço com `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="f0d01-802">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="f0d01-803">AMS</span><span class="sxs-lookup"><span data-stu-id="f0d01-803">AMS</span></span>
* <span data-ttu-id="f0d01-804">[ALTERAÇÃO SIGNIFICATIVA] `ams asset get-streaming-locators` renomeado para `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="f0d01-804">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="f0d01-805">[ALTERAÇÃO SIGNIFICATIVA] `ams streaming-locator get-content-keys` renomeado para `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="f0d01-805">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-806">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-806">Appservice</span></span>
* <span data-ttu-id="f0d01-807">Suporte adicionado para o App Insights no `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-807">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="f0d01-808">Suporte adicionado para a criação do plano de serviço de aplicativo (incluindo Elástico Premium) para Aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="f0d01-808">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="f0d01-809">Foram corrigidos os problemas com de configuração de aplicativo com os planos Elástico Premium</span><span class="sxs-lookup"><span data-stu-id="f0d01-809">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="f0d01-810">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-810">Container</span></span>
* <span data-ttu-id="f0d01-811">Adicionado o comando `container start`</span><span class="sxs-lookup"><span data-stu-id="f0d01-811">Added `container start` command</span></span>
* <span data-ttu-id="f0d01-812">Alteração para permitir o uso de valores decimais para CPU durante a criação do contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-812">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="f0d01-813">EventGrid</span><span class="sxs-lookup"><span data-stu-id="f0d01-813">EventGrid</span></span>
* <span data-ttu-id="f0d01-814">Parâmetro `--deadletter-endpoint` adicionado a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-814">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="f0d01-815">Storagequeue e hybridconnection foram adicionados como novos valores para 'event-subscription [create|update] --endpoint-type\`</span><span class="sxs-lookup"><span data-stu-id="f0d01-815">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="f0d01-816">Os parâmetros `--max-delivery-attempts` e `--event-ttl` foram adicionados a `event-subscription create` para especificar a política de repetição para eventos</span><span class="sxs-lookup"><span data-stu-id="f0d01-816">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="f0d01-817">Uma mensagem de aviso foi adicionada a `event-subscription [create|update]` quando o webhook como destino for usado para uma assinatura de evento</span><span class="sxs-lookup"><span data-stu-id="f0d01-817">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="f0d01-818">O parâmetro source-resource-id foi adicionado para todos os comandos relacionados a eventos e marcar todos os outros parâmetros relacionados ao recurso de origem como preteridos</span><span class="sxs-lookup"><span data-stu-id="f0d01-818">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f0d01-819">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f0d01-819">HDInsight</span></span>
* <span data-ttu-id="f0d01-820">[ALTERAÇÃO SIGNIFICATIVA] Os parâmetros `--virtual-network` e `--subnet-name` de `hdinsight [application] create` foram removidos</span><span class="sxs-lookup"><span data-stu-id="f0d01-820">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="f0d01-821">[ALTERAÇÃO SIGNIFICATIVA] `hdinsight create --storage-account` foi alterado para aceitar o nome ou ID da conta de armazenamento, em vez de pontos de extremidade de blob</span><span class="sxs-lookup"><span data-stu-id="f0d01-821">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="f0d01-822">Parâmetros `--vnet-name` e `--subnet-name` adicionados a `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-822">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="f0d01-823">Suporte adicionado para a criptografia de disco e Enterprise Security Package ao `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-823">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="f0d01-824">Adicionado o comando `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="f0d01-824">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="f0d01-825">Adicionado o comando `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-825">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="f0d01-826">IoT</span><span class="sxs-lookup"><span data-stu-id="f0d01-826">IoT</span></span>
* <span data-ttu-id="f0d01-827">O formato de codificação foi adicionado ao comando routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="f0d01-827">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="f0d01-828">Kusto</span><span class="sxs-lookup"><span data-stu-id="f0d01-828">Kusto</span></span>
* <span data-ttu-id="f0d01-829">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="f0d01-829">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="f0d01-830">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f0d01-830">Monitor</span></span>
* <span data-ttu-id="f0d01-831">A comparação de ID foi alterada para diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="f0d01-831">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="f0d01-832">Perfil</span><span class="sxs-lookup"><span data-stu-id="f0d01-832">Profile</span></span>
* <span data-ttu-id="f0d01-833">A conta de nível de locatário foi habilitada para a identidade de serviço gerenciada de `login`</span><span class="sxs-lookup"><span data-stu-id="f0d01-833">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-834">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-834">Network</span></span>
* <span data-ttu-id="f0d01-835">Foi corrigido o problema com `express-route update`: em que o argumento `--bandwidth` era ignorado</span><span class="sxs-lookup"><span data-stu-id="f0d01-835">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="f0d01-836">Foi corrigido o problema com `ddos-protection update` em que definir a compreensão levava ao rastreamento de pilha</span><span class="sxs-lookup"><span data-stu-id="f0d01-836">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-837">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-837">Resource</span></span>
* <span data-ttu-id="f0d01-838">Suporte adicionado para o arquivo de parâmetros de URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-838">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="f0d01-839">Suporte adicionado para a identidade gerenciada à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-839">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="f0d01-840">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-840">SQL Virtual Machine</span></span>
* <span data-ttu-id="f0d01-841">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="f0d01-841">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-842">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-842">Storage</span></span>
* <span data-ttu-id="f0d01-843">Alteração na correção para atualizar apenas as propriedades que são alteradas no mesmo objeto</span><span class="sxs-lookup"><span data-stu-id="f0d01-843">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="f0d01-844">#8021 foi corrigido, dados binários são codificados em base 64 quando retornados</span><span class="sxs-lookup"><span data-stu-id="f0d01-844">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-845">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-845">VM</span></span>
* <span data-ttu-id="f0d01-846">Alteração de `vm encryption enable` para validar o cofre de chaves de criptografia de disco e se esse cofre de chaves de criptografia de chave existe</span><span class="sxs-lookup"><span data-stu-id="f0d01-846">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="f0d01-847">O sinalizador `--force` foi adicionado a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="f0d01-847">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="f0d01-848">15 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="f0d01-848">January 15, 2019</span></span>

<span data-ttu-id="f0d01-849">Versão 2.0.55</span><span class="sxs-lookup"><span data-stu-id="f0d01-849">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-850">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-850">ACR</span></span>
* <span data-ttu-id="f0d01-851">Alteração para permitir forçar o envio por push de um gráfico Helm que não existe</span><span class="sxs-lookup"><span data-stu-id="f0d01-851">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="f0d01-852">Alteração para permitir operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="f0d01-852">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="f0d01-853">[PRETERIDO] O parâmetro `--resource-group` foi preterido nos comandos:</span><span class="sxs-lookup"><span data-stu-id="f0d01-853">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="f0d01-854">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-854">ACS</span></span>
* <span data-ttu-id="f0d01-855">Suporte adicionado para novas regiões ACI</span><span class="sxs-lookup"><span data-stu-id="f0d01-855">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-856">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-856">Appservice</span></span>
* <span data-ttu-id="f0d01-857">Foi corrigido o problema com o carregamento de certificados para aplicativos que são hospedados em um ASE, em que o RG do ASE e o RG do aplicativo são diferentes</span><span class="sxs-lookup"><span data-stu-id="f0d01-857">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="f0d01-858">Alteração de `webapp up` para usar a SKU P1V1 como padrão para Linux</span><span class="sxs-lookup"><span data-stu-id="f0d01-858">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="f0d01-859">`[webapp|functionapp] deployment source config-zip` foi corrigido para mostrar a mensagem de erro adequada quando uma implantação falhar</span><span class="sxs-lookup"><span data-stu-id="f0d01-859">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="f0d01-860">Adicionado o comando `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="f0d01-860">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="f0d01-861">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="f0d01-861">Botservice</span></span>
* <span data-ttu-id="f0d01-862">Atualizações de status de implantação foram adicionadas a `bot create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-862">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="f0d01-863">Configurar</span><span class="sxs-lookup"><span data-stu-id="f0d01-863">Configure</span></span>
* <span data-ttu-id="f0d01-864">`none` foi adicionado como um formato de saída configurável</span><span class="sxs-lookup"><span data-stu-id="f0d01-864">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f0d01-865">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f0d01-865">CosmosDB</span></span>
* <span data-ttu-id="f0d01-866">Suporte adicionado para criar o banco de dados com taxa de transferência compartilhada</span><span class="sxs-lookup"><span data-stu-id="f0d01-866">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f0d01-867">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f0d01-867">HDInsight</span></span>
* <span data-ttu-id="f0d01-868">Foram adicionados comandos para o gerenciamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="f0d01-868">Added commands for managing applications</span></span>
* <span data-ttu-id="f0d01-869">Foram adicionados comandos para o gerenciamento de ações de script</span><span class="sxs-lookup"><span data-stu-id="f0d01-869">Added commands for managing script actions</span></span>
* <span data-ttu-id="f0d01-870">Foram adicionados comandos para o gerenciamento do Operations Management Suite (OMS)</span><span class="sxs-lookup"><span data-stu-id="f0d01-870">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="f0d01-871">Suporte adicionado para listar a utilização regional ao `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="f0d01-871">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="f0d01-872">[ALTERAÇÃO SIGNIFICATIVA] O tipo de cluster padrão de `hdinsight create` foi removido</span><span class="sxs-lookup"><span data-stu-id="f0d01-872">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-873">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-873">Network</span></span>
* <span data-ttu-id="f0d01-874">Adicionados os argumentos `--custom-headers` e `--status-code-ranges` para `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-874">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="f0d01-875">Novos tipos de roteamento foram adicionados: Subrede e múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="f0d01-875">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="f0d01-876">Adicionados os argumentos `--custom-headers` e `--subnets` para `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-876">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="f0d01-877">Foi corrigido o problema no qual fornecer `--vnets ""` a `ddos-protection update` causava um erro</span><span class="sxs-lookup"><span data-stu-id="f0d01-877">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-878">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-878">Role</span></span>
* <span data-ttu-id="f0d01-879">[PRETERIDO] O argumento `--password` foi preterido para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-879">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="f0d01-880">Como alternativa, use senhas seguras geradas pela CLI</span><span class="sxs-lookup"><span data-stu-id="f0d01-880">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="f0d01-881">Segurança</span><span class="sxs-lookup"><span data-stu-id="f0d01-881">Security</span></span>
* <span data-ttu-id="f0d01-882">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="f0d01-882">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-883">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-883">Storage</span></span>
* <span data-ttu-id="f0d01-884">[ALTERAÇÃO SIGNIFICATIVA] O número padrão de resultados de `storage [blob|file|container|share] list` foi alterado para 5.000.</span><span class="sxs-lookup"><span data-stu-id="f0d01-884">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="f0d01-885">Use `--num-results *` para o comportamento original de retornar todos os resultados</span><span class="sxs-lookup"><span data-stu-id="f0d01-885">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="f0d01-886">Parâmetro `--marker` adicionado a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="f0d01-886">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="f0d01-887">Um marcador de log foi adicionado para a próxima página ao STDERR de `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="f0d01-887">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="f0d01-888">O comando `storage blob service-properties update` foi adicionado com suporte para sites estáticos</span><span class="sxs-lookup"><span data-stu-id="f0d01-888">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-889">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-889">VM</span></span>
* <span data-ttu-id="f0d01-890">`vm [disk|unmanaged-disk]` e `vmss disk` foram alterados para que tenham parâmetros mais consistentes</span><span class="sxs-lookup"><span data-stu-id="f0d01-890">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="f0d01-891">Suporte adicionado para referência cruzada de imagem de locatário a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-891">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="f0d01-892">O bug de configuração padrão foi corrigido em `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="f0d01-892">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="f0d01-893">O argumento `--provision-after-extensions` foi adicionado a `vmss extension set` para definir quais extensões deverão ser provisionadas antes da extensão ser definida</span><span class="sxs-lookup"><span data-stu-id="f0d01-893">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="f0d01-894">O argumento `--replica-count` foi adicionado a `sig image-version update` para definir a contagem de replicação padrão</span><span class="sxs-lookup"><span data-stu-id="f0d01-894">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="f0d01-895">Foi corrigido o bug com `image create --source` em que o disco do sistema operacional de origem era confundido com uma VM do mesmo nome, mesmo se a ID de recurso completa fosse fornecida</span><span class="sxs-lookup"><span data-stu-id="f0d01-895">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="f0d01-896">20 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-896">December 20, 2018</span></span>

<span data-ttu-id="f0d01-897">Versão 2.0.54</span><span class="sxs-lookup"><span data-stu-id="f0d01-897">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="f0d01-898">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-898">Appservice</span></span>
* <span data-ttu-id="f0d01-899">Corrigido o problema que causava falha na reimplantação do `webapp up`</span><span class="sxs-lookup"><span data-stu-id="f0d01-899">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="f0d01-900">Adicionado suporte para listar e restaurar instantâneos de aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="f0d01-900">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="f0d01-901">Adicionado suporte para o sinalizador `--runtime` para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="f0d01-901">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="f0d01-902">IoT Central</span><span class="sxs-lookup"><span data-stu-id="f0d01-902">IoTCentral</span></span>
* <span data-ttu-id="f0d01-903">Corrigida a chamada à API do comando de atualização</span><span class="sxs-lookup"><span data-stu-id="f0d01-903">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-904">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-904">Role</span></span>
* <span data-ttu-id="f0d01-905">[ALTERAÇÃO SIGNIFICATIVA] `ad [app|sp] list` alterado para listar somente os 100 primeiros objetos por padrão</span><span class="sxs-lookup"><span data-stu-id="f0d01-905">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-906">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-906">SQL</span></span>
* <span data-ttu-id="f0d01-907">Adicionado suporte para ordenação personalizada nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="f0d01-907">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-908">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-908">VM</span></span>
* <span data-ttu-id="f0d01-909">Parâmetro `---os-type` adicionado a `disk create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-909">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="f0d01-910">18 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-910">December 18, 2018</span></span>

<span data-ttu-id="f0d01-911">Versão 2.0.53</span><span class="sxs-lookup"><span data-stu-id="f0d01-911">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="f0d01-912">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-912">ACR</span></span>
* <span data-ttu-id="f0d01-913">Adicionado suporte para importação de imagem de Registros de Contêiner externos</span><span class="sxs-lookup"><span data-stu-id="f0d01-913">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="f0d01-914">Simplificado o layout da tabela para a lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="f0d01-914">Condensed the table layout for task list</span></span>
* <span data-ttu-id="f0d01-915">Adicionado suporte para URLs do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="f0d01-915">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-916">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-916">ACS</span></span>
* <span data-ttu-id="f0d01-917">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="f0d01-917">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="f0d01-918">Removido “(VISUALIZAÇÃO)” de argumentos do AAD para `aks create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-918">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="f0d01-919">[PRETERIDO] Comandos `az acs` preteridos.</span><span class="sxs-lookup"><span data-stu-id="f0d01-919">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="f0d01-920">O serviço ACS será desativado em 31 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="f0d01-920">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="f0d01-921">Adicionado suporte da Política de Rede durante a criação de novos clusters AKS</span><span class="sxs-lookup"><span data-stu-id="f0d01-921">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="f0d01-922">Removido o requisito do argumento `--nodepool-name` para `aks scale` se houver apenas um pool de nós</span><span class="sxs-lookup"><span data-stu-id="f0d01-922">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-923">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-923">Appservice</span></span>
* <span data-ttu-id="f0d01-924">Corrigido o problema em que `webapp config container` não honra o parâmetro `--slot`</span><span class="sxs-lookup"><span data-stu-id="f0d01-924">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="f0d01-925">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="f0d01-925">Botservice</span></span>
* <span data-ttu-id="f0d01-926">Suporte adicionado para análise do arquivo `.bot` ao chamar `bot show`</span><span class="sxs-lookup"><span data-stu-id="f0d01-926">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="f0d01-927">Corrigido o bug de provisionamento do AppInsights</span><span class="sxs-lookup"><span data-stu-id="f0d01-927">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="f0d01-928">Corrigido o bug de espaço em branco ao lidar com caminhos de arquivo</span><span class="sxs-lookup"><span data-stu-id="f0d01-928">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="f0d01-929">Reduzidas as chamadas de rede do Kudu</span><span class="sxs-lookup"><span data-stu-id="f0d01-929">Reduced Kudu network calls</span></span>
* <span data-ttu-id="f0d01-930">Melhorias de UX para comandos gerais</span><span class="sxs-lookup"><span data-stu-id="f0d01-930">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="f0d01-931">Consumo</span><span class="sxs-lookup"><span data-stu-id="f0d01-931">Consumption</span></span>
* <span data-ttu-id="f0d01-932">Corrigidos os bugs da API de orçamento ao mostrar notificações</span><span class="sxs-lookup"><span data-stu-id="f0d01-932">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f0d01-933">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f0d01-933">CosmosDB</span></span>
* <span data-ttu-id="f0d01-934">Suporte adicionado para atualizar a conta de vários mestres para mestre único</span><span class="sxs-lookup"><span data-stu-id="f0d01-934">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="f0d01-935">Mapas</span><span class="sxs-lookup"><span data-stu-id="f0d01-935">Maps</span></span>
* <span data-ttu-id="f0d01-936">Adicionado suporte ao SKU S1 para `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-936">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-937">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-937">Network</span></span>
* <span data-ttu-id="f0d01-938">Adicionado suporte para `--format` e `--log-version` para `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="f0d01-938">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="f0d01-939">Corrigido o problema com `dns zone update` em que usar "" para limpar a resolução e o registro de redes virtuais não funcionava</span><span class="sxs-lookup"><span data-stu-id="f0d01-939">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-940">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-940">Resource</span></span>
* <span data-ttu-id="f0d01-941">Corrigido o tratamento do parâmetro de escopo para grupos de gerenciamento do `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-941">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="f0d01-942">Adicionado o novo comando `resource wait`</span><span class="sxs-lookup"><span data-stu-id="f0d01-942">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-943">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-943">Storage</span></span>
*  <span data-ttu-id="f0d01-944">Adicionada a capacidade de atualizar a versão do esquema de log para serviços de armazenamento no `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-944">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-945">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-945">VM</span></span>
* <span data-ttu-id="f0d01-946">Corrigida a falha em `vm identity remove` quando a VM especificada não tem nenhuma identidade de serviço gerenciado atribuída</span><span class="sxs-lookup"><span data-stu-id="f0d01-946">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="f0d01-947">4 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-947">December 4, 2018</span></span>

<span data-ttu-id="f0d01-948">Versão 2.0.52</span><span class="sxs-lookup"><span data-stu-id="f0d01-948">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="f0d01-949">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-949">Core</span></span>
* <span data-ttu-id="f0d01-950">Adicionado suporte para provisionamento de recursos de locatários cruzados para a entidade de serviço de multilocatários</span><span class="sxs-lookup"><span data-stu-id="f0d01-950">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="f0d01-951">Corrigido o bug onde as ids enviadas por pipe de um comando com a saída tsv eram analisados incorretamente</span><span class="sxs-lookup"><span data-stu-id="f0d01-951">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-952">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-952">Appservice</span></span>
* <span data-ttu-id="f0d01-953">[VERSÃO PRÉVIA] Adicionado o comando `webapp up` que ajuda a criar e implantar conteúdo em aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-953">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="f0d01-954">Corrigido um bug no aplicativo com base em contêiner do Windows devido à alteração de back-end</span><span class="sxs-lookup"><span data-stu-id="f0d01-954">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-955">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-955">Network</span></span>
* <span data-ttu-id="f0d01-956">Adicionado o argumento `--exclusion` a `application-gateway waf-config set` para dar suporte a exclusões de WAF</span><span class="sxs-lookup"><span data-stu-id="f0d01-956">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-957">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-957">Role</span></span>
* <span data-ttu-id="f0d01-958">Adicionado suporte para identificadores personalizados para a credencial de senha</span><span class="sxs-lookup"><span data-stu-id="f0d01-958">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="f0d01-959">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-959">VM</span></span>
* <span data-ttu-id="f0d01-960">[PRETERIDO] Parâmetro `vm extension [show|wait] --expand` preterido</span><span class="sxs-lookup"><span data-stu-id="f0d01-960">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="f0d01-961">Adicionado parâmetro `--force` a `vm restart` para reimplantar as VMs sem resposta</span><span class="sxs-lookup"><span data-stu-id="f0d01-961">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="f0d01-962">Alterado `[vm|vmss] create --authentication-type` para aceitar "todos" para criar uma VM com senha e autenticação SSH</span><span class="sxs-lookup"><span data-stu-id="f0d01-962">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="f0d01-963">Adicionado parâmetro `image create --os-disk-caching` para definir o cache de disco do sistema operacional para uma imagem</span><span class="sxs-lookup"><span data-stu-id="f0d01-963">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="f0d01-964">20 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-964">November 20, 2018</span></span>

<span data-ttu-id="f0d01-965">Versão 2.0.51</span><span class="sxs-lookup"><span data-stu-id="f0d01-965">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="f0d01-966">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-966">Core</span></span>
* <span data-ttu-id="f0d01-967">Logon do MSI alterado para não reutilizar o nome da assinatura na identidade</span><span class="sxs-lookup"><span data-stu-id="f0d01-967">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-968">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-968">ACR</span></span>
* <span data-ttu-id="f0d01-969">Token de contexto adicionado à etapa da tarefa</span><span class="sxs-lookup"><span data-stu-id="f0d01-969">Added context token to task step</span></span>
* <span data-ttu-id="f0d01-970">Suporte adicionado para definir segredos na execução do acr para espelhar a tarefa do acr</span><span class="sxs-lookup"><span data-stu-id="f0d01-970">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="f0d01-971">Suporte aprimorado para `--top` e `--orderby` para os comandos `show-tags` e `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="f0d01-971">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-972">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-972">Appservice</span></span>
* <span data-ttu-id="f0d01-973">Tempo limite padrão para a implantação do zip alterado para sondar o status aumentado para 5 minutos, também adicionando uma propriedade de tempo limite para personalizar esse valor</span><span class="sxs-lookup"><span data-stu-id="f0d01-973">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="f0d01-974">Padrão `node_version` atualizado.</span><span class="sxs-lookup"><span data-stu-id="f0d01-974">Updated the default `node_version`.</span></span> <span data-ttu-id="f0d01-975">Redefinir a ação de troca de slots durante uma troca de duas fases preserva todas as configurações do aplicativo e cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="f0d01-975">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="f0d01-976">Verificação da SKU no lado do cliente removida para o Linux criar o plano do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-976">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="f0d01-977">Erro corrigido ao tentar obter o status de implantação do zip</span><span class="sxs-lookup"><span data-stu-id="f0d01-977">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="f0d01-978">Iot Central</span><span class="sxs-lookup"><span data-stu-id="f0d01-978">IotCentral</span></span>
* <span data-ttu-id="f0d01-979">Verificação de disponibilidade do subdomínio adicionada ao criar um aplicativo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="f0d01-979">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="f0d01-980">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f0d01-980">KeyVault</span></span>
* <span data-ttu-id="f0d01-981">Bug corrigido em que os erros podem ter sido ignorados</span><span class="sxs-lookup"><span data-stu-id="f0d01-981">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-982">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-982">Network</span></span>
* <span data-ttu-id="f0d01-983">Subcomandos `root-cert` adicionados a `application-gateway` para lidar com os certificados de raiz confiável</span><span class="sxs-lookup"><span data-stu-id="f0d01-983">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="f0d01-984">Opções `--min-capacity` e `--custom-error-pages` adicionadas a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="f0d01-984">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="f0d01-985">`--zones` adicionado para suporte da zona de disponibilidade a `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-985">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="f0d01-986">Argumentos `--file-upload-limit`, `--max-request-body-size` e `--request-body-check` a `application-gateway waf-config set` adicionados</span><span class="sxs-lookup"><span data-stu-id="f0d01-986">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f0d01-987">Rdbms</span><span class="sxs-lookup"><span data-stu-id="f0d01-987">Rdbms</span></span>
* <span data-ttu-id="f0d01-988">Comandos vnet do mariadb adicionados</span><span class="sxs-lookup"><span data-stu-id="f0d01-988">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="f0d01-989">Rbac</span><span class="sxs-lookup"><span data-stu-id="f0d01-989">Rbac</span></span>
* <span data-ttu-id="f0d01-990">Um problema corrigido ao tentar atualizar credenciais inalteradas em `ad app update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-990">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="f0d01-991">Avisos de saída adicionados para comunicar alterações de falha em um futuro próximo para `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="f0d01-991">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="f0d01-992">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-992">Storage</span></span>
* <span data-ttu-id="f0d01-993">Melhor manipulação de casos incomuns para os comandos da cópia de armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-993">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="f0d01-994">Corrigido o problema em que `storage blob copy start-batch` não usava credenciais de logon quando as contas de origem e destino eram iguais</span><span class="sxs-lookup"><span data-stu-id="f0d01-994">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="f0d01-995">Bug corrigido com `storage [blob|file] url` em que `sas_token` não foi incorporado na URL</span><span class="sxs-lookup"><span data-stu-id="f0d01-995">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="f0d01-996">Aviso de alteração da falha adicionado a `[blob|container] list`: produzirá apenas os primeiros 5.000 resultados por padrão</span><span class="sxs-lookup"><span data-stu-id="f0d01-996">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-997">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-997">VM</span></span>
* <span data-ttu-id="f0d01-998">Suporte adicionado a `[vm|vmss] create --storage-sku` para especificar a SKU da conta de armazenamento para o SO gerenciado e os discos de dados separadamente</span><span class="sxs-lookup"><span data-stu-id="f0d01-998">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="f0d01-999">Parâmetros do nome da versão alterados de `sig image-version` para `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="f0d01-999">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="f0d01-1000">Argumento `sig image-version` preterido `--image-version-name`, substituído por `--image-version`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1000">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="f0d01-1001">Suporte adicionado para usar o disco local do SO a `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1001">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="f0d01-1002">Adicionado o suporte ao `--no-wait` para `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1002">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="f0d01-1003">Adicionado o comando `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1003">Added `snapshot wait` command</span></span>
* <span data-ttu-id="f0d01-1004">Suporte adicionado para usar o nome da instância com `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1004">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="f0d01-1005">6 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1005">November 6, 2018</span></span>

<span data-ttu-id="f0d01-1006">Versão 2.0.50</span><span class="sxs-lookup"><span data-stu-id="f0d01-1006">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-1007">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1007">Core</span></span>
* <span data-ttu-id="f0d01-1008">Foi adicionado suporte para o serviço principal sn + autenticação do emissor</span><span class="sxs-lookup"><span data-stu-id="f0d01-1008">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-1009">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-1009">ACR</span></span>
* <span data-ttu-id="f0d01-1010">Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa</span><span class="sxs-lookup"><span data-stu-id="f0d01-1010">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="f0d01-1011">Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação</span><span class="sxs-lookup"><span data-stu-id="f0d01-1011">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-1012">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1012">ACS</span></span>
* <span data-ttu-id="f0d01-1013">[ALTERAÇÃO SIGNIFICATIVA] `enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão</span><span class="sxs-lookup"><span data-stu-id="f0d01-1013">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="f0d01-1014">Supervisor</span><span class="sxs-lookup"><span data-stu-id="f0d01-1014">Advisor</span></span>
* <span data-ttu-id="f0d01-1015">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="f0d01-1015">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="f0d01-1016">AMS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1016">AMS</span></span>
* <span data-ttu-id="f0d01-1017">Novos grupos de comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="f0d01-1017">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="f0d01-1018">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="f0d01-1018">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="f0d01-1019">Adicionados parâmetros de criptografia com suporte para `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1019">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="f0d01-1020">O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido</span><span class="sxs-lookup"><span data-stu-id="f0d01-1020">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="f0d01-1021">Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1021">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="f0d01-1022">Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1022">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="f0d01-1023">Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1023">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="f0d01-1024">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming locator` foi substituído por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1024">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="f0d01-1025">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--content-keys` de `ams streaming locator` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="f0d01-1025">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="f0d01-1026">[ALTERAÇÃO SIGNIFICATIVA] `--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1026">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="f0d01-1027">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming policy` foi substituído por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1027">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="f0d01-1028">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1028">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="f0d01-1029">Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="f0d01-1029">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="f0d01-1030">Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado</span><span class="sxs-lookup"><span data-stu-id="f0d01-1030">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="f0d01-1031">[ALTERAÇÃO SIGNIFICATIVA] `--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1031">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="f0d01-1032">Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1032">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="f0d01-1033">Um ativo sem rótulo pode ser enviado assim: 'assetName='</span><span class="sxs-lookup"><span data-stu-id="f0d01-1033">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-1034">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-1034">AppService</span></span>
* <span data-ttu-id="f0d01-1035">Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido</span><span class="sxs-lookup"><span data-stu-id="f0d01-1035">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="f0d01-1036">Configurar</span><span class="sxs-lookup"><span data-stu-id="f0d01-1036">Configure</span></span>
* <span data-ttu-id="f0d01-1037">O YAML foi adicionado às opções de formato de saída</span><span class="sxs-lookup"><span data-stu-id="f0d01-1037">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="f0d01-1038">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-1038">Container</span></span>
* <span data-ttu-id="f0d01-1039">Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml</span><span class="sxs-lookup"><span data-stu-id="f0d01-1039">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="f0d01-1040">EventHub</span><span class="sxs-lookup"><span data-stu-id="f0d01-1040">EventHub</span></span>
* <span data-ttu-id="f0d01-1041">O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1041">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="f0d01-1042">Interativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1042">Interactive</span></span>
* <span data-ttu-id="f0d01-1043">O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1043">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="f0d01-1044">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1044">Monitor</span></span>
* <span data-ttu-id="f0d01-1045">Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) para `--condition` em `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1045">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-1046">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-1046">Network</span></span>
* <span data-ttu-id="f0d01-1047">Os nomes de comandos `network interface-endpoint` foram preteridos em benefício de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1047">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="f0d01-1048">Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID</span><span class="sxs-lookup"><span data-stu-id="f0d01-1048">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="f0d01-1049">Foi corrigido um problema onde `--ip-tags` não funcionava corretamente com `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1049">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="f0d01-1050">Perfil</span><span class="sxs-lookup"><span data-stu-id="f0d01-1050">Profile</span></span>
* <span data-ttu-id="f0d01-1051">`--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado</span><span class="sxs-lookup"><span data-stu-id="f0d01-1051">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="f0d01-1052">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1052">RDBMS</span></span>
* <span data-ttu-id="f0d01-1053">Adicionados comandos da réplica mysql</span><span class="sxs-lookup"><span data-stu-id="f0d01-1053">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-1054">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-1054">Resource</span></span>
* <span data-ttu-id="f0d01-1055">Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1055">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-1056">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-1056">Role</span></span>
* <span data-ttu-id="f0d01-1057">Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais</span><span class="sxs-lookup"><span data-stu-id="f0d01-1057">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="f0d01-1058">`ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="f0d01-1058">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="f0d01-1059">Suporte adicionado para conceder permissões a aplicativos do AAD</span><span class="sxs-lookup"><span data-stu-id="f0d01-1059">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-1060">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1060">Storage</span></span>
* <span data-ttu-id="f0d01-1061">Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1061">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-1062">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1062">VM</span></span>
* <span data-ttu-id="f0d01-1063">O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem</span><span class="sxs-lookup"><span data-stu-id="f0d01-1063">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="f0d01-1064">O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido</span><span class="sxs-lookup"><span data-stu-id="f0d01-1064">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="f0d01-1065">O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado</span><span class="sxs-lookup"><span data-stu-id="f0d01-1065">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="f0d01-1066">`vm secret format` foi alterado para exigir a saída json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1066">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="f0d01-1067">Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido</span><span class="sxs-lookup"><span data-stu-id="f0d01-1067">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="f0d01-1068">Validação de argumento aprimorado para `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1068">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="f0d01-1069">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1069">October 23, 2018</span></span>

<span data-ttu-id="f0d01-1070">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="f0d01-1070">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-1071">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1071">Core</span></span>
* <span data-ttu-id="f0d01-1072">Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1072">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="f0d01-1073">Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1073">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-1074">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-1074">ACR</span></span>
* <span data-ttu-id="f0d01-1075">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="f0d01-1075">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="f0d01-1076">CDN</span><span class="sxs-lookup"><span data-stu-id="f0d01-1076">CDN</span></span>
* <span data-ttu-id="f0d01-1077">[ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="f0d01-1077">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="f0d01-1078">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="f0d01-1078">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="f0d01-1079">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-1079">Container</span></span>
* <span data-ttu-id="f0d01-1080">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="f0d01-1080">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="f0d01-1081">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="f0d01-1081">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="f0d01-1082">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1082">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="f0d01-1083">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="f0d01-1083">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="f0d01-1084">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="f0d01-1084">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="f0d01-1085">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="f0d01-1085">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="f0d01-1086">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1086">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f0d01-1087">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f0d01-1087">CosmosDB</span></span>
* <span data-ttu-id="f0d01-1088">Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1088">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="f0d01-1089">Interativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1089">Interactive</span></span>
* <span data-ttu-id="f0d01-1090">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="f0d01-1090">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="f0d01-1091">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="f0d01-1091">IoT Central</span></span>
* <span data-ttu-id="f0d01-1092">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="f0d01-1092">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="f0d01-1093">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="f0d01-1093">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="f0d01-1094">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1094">Monitor</span></span>
* <span data-ttu-id="f0d01-1095">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="f0d01-1095">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="f0d01-1096">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="f0d01-1096">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="f0d01-1097">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="f0d01-1097">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="f0d01-1098">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="f0d01-1098">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="f0d01-1099">Adicionado `--namespace` como alias para a opção preterida `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1099">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="f0d01-1100">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="f0d01-1100">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="f0d01-1101">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="f0d01-1101">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="f0d01-1102">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="f0d01-1102">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="f0d01-1103">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="f0d01-1103">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="f0d01-1104">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1104">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-1105">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-1105">Network</span></span>
* <span data-ttu-id="f0d01-1106">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="f0d01-1106">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="f0d01-1107">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="f0d01-1107">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="f0d01-1108">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f0d01-1108">ServiceBus</span></span>
* <span data-ttu-id="f0d01-1109">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="f0d01-1109">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-1110">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-1110">SQL</span></span>
* <span data-ttu-id="f0d01-1111">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="f0d01-1111">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-1112">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1112">Storage</span></span>
* <span data-ttu-id="f0d01-1113">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="f0d01-1113">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="f0d01-1114">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="f0d01-1114">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-1115">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1115">VM</span></span>
* <span data-ttu-id="f0d01-1116">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1116">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="f0d01-1117">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1117">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="f0d01-1118">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1118">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="f0d01-1119">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1119">October 16, 2018</span></span>

<span data-ttu-id="f0d01-1120">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="f0d01-1120">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-1121">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1121">VM</span></span>
* <span data-ttu-id="f0d01-1122">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="f0d01-1122">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="f0d01-1123">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1123">October 9, 2018</span></span>

<span data-ttu-id="f0d01-1124">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="f0d01-1124">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-1125">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1125">Core</span></span>
* <span data-ttu-id="f0d01-1126">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="f0d01-1126">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-1127">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-1127">ACR</span></span>
* <span data-ttu-id="f0d01-1128">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="f0d01-1128">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-1129">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1129">ACS</span></span>
* <span data-ttu-id="f0d01-1130">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="f0d01-1130">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="f0d01-1131">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="f0d01-1131">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="f0d01-1132">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1132">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="f0d01-1133">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="f0d01-1133">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="f0d01-1134">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-1134">Container</span></span>
* <span data-ttu-id="f0d01-1135">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um tempo de execução específico</span><span class="sxs-lookup"><span data-stu-id="f0d01-1135">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="f0d01-1136">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="f0d01-1136">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="f0d01-1137">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1137">Event Hub</span></span>
* <span data-ttu-id="f0d01-1138">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1138">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="f0d01-1139">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="f0d01-1139">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="f0d01-1140">Extensões</span><span class="sxs-lookup"><span data-stu-id="f0d01-1140">Extensions</span></span>
* <span data-ttu-id="f0d01-1141">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="f0d01-1141">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f0d01-1142">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f0d01-1142">HDInsight</span></span>
* <span data-ttu-id="f0d01-1143">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="f0d01-1143">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="f0d01-1144">IoT</span><span class="sxs-lookup"><span data-stu-id="f0d01-1144">IoT</span></span>
* <span data-ttu-id="f0d01-1145">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="f0d01-1145">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="f0d01-1146">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f0d01-1146">KeyVault</span></span>
* <span data-ttu-id="f0d01-1147">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="f0d01-1147">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-1148">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-1148">Network</span></span>
* <span data-ttu-id="f0d01-1149">Corrigido `network dns zone create`: O comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1149">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="f0d01-1150">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="f0d01-1150">See #6052</span></span>
* <span data-ttu-id="f0d01-1151">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1151">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="f0d01-1152">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="f0d01-1152">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="f0d01-1153">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1153">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="f0d01-1154">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1154">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="f0d01-1155">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1155">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="f0d01-1156">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1156">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-1157">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-1157">Role</span></span>
* <span data-ttu-id="f0d01-1158">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1158">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="f0d01-1159">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1159">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="f0d01-1160">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="f0d01-1160">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="f0d01-1161">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="f0d01-1161">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="f0d01-1162">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="f0d01-1162">Service Bus</span></span>
* <span data-ttu-id="f0d01-1163">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="f0d01-1163">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-1164">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1164">VM</span></span>
* <span data-ttu-id="f0d01-1165">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1165">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="f0d01-1166">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1166">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="f0d01-1167">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1167">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="f0d01-1168">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1168">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="f0d01-1169">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1169">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="f0d01-1170">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="f0d01-1170">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="f0d01-1171">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1171">September 21, 2018</span></span>

<span data-ttu-id="f0d01-1172">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="f0d01-1172">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-1173">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-1173">ACR</span></span>
* <span data-ttu-id="f0d01-1174">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-1174">Added ACR Task commands</span></span>
* <span data-ttu-id="f0d01-1175">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="f0d01-1175">Added quick run command</span></span>
* <span data-ttu-id="f0d01-1176">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1176">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="f0d01-1177">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-1177">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="f0d01-1178">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="f0d01-1178">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="f0d01-1179">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="f0d01-1179">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-1180">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1180">ACS</span></span>
* <span data-ttu-id="f0d01-1181">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1181">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="f0d01-1182">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="f0d01-1182">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-1183">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-1183">AppService</span></span>

* <span data-ttu-id="f0d01-1184">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="f0d01-1184">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="f0d01-1185">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="f0d01-1185">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="f0d01-1186">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="f0d01-1186">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="f0d01-1187">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1187">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="f0d01-1188">Lote</span><span class="sxs-lookup"><span data-stu-id="f0d01-1188">Batch</span></span>
* <span data-ttu-id="f0d01-1189">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="f0d01-1189">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="f0d01-1190">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1190">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="f0d01-1191">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1191">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="f0d01-1192">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="f0d01-1192">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f0d01-1193">Lote AI</span><span class="sxs-lookup"><span data-stu-id="f0d01-1193">Batch AI</span></span> 
* <span data-ttu-id="f0d01-1194">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1194">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f0d01-1195">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1195">Cognitive Services</span></span>
* <span data-ttu-id="f0d01-1196">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1196">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="f0d01-1197">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1197">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="f0d01-1198">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1198">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="f0d01-1199">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1199">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="f0d01-1200">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1200">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="f0d01-1201">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1201">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="f0d01-1202">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-1202">Container</span></span>
* <span data-ttu-id="f0d01-1203">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="f0d01-1203">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="f0d01-1204">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-1204">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="f0d01-1205">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="f0d01-1205">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="f0d01-1206">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="f0d01-1206">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="f0d01-1207">DataLake</span><span class="sxs-lookup"><span data-stu-id="f0d01-1207">Datalake</span></span>
* <span data-ttu-id="f0d01-1208">Comandos adicionados para regras da rede virtual</span><span class="sxs-lookup"><span data-stu-id="f0d01-1208">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="f0d01-1209">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1209">Interactive Shell</span></span>
* <span data-ttu-id="f0d01-1210">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="f0d01-1210">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="f0d01-1211">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1211">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="f0d01-1212">IoT</span><span class="sxs-lookup"><span data-stu-id="f0d01-1212">IoT</span></span>
* <span data-ttu-id="f0d01-1213">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="f0d01-1213">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="f0d01-1214">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f0d01-1214">Key Vault</span></span>
* <span data-ttu-id="f0d01-1215">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="f0d01-1215">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-1216">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-1216">Network</span></span>
* <span data-ttu-id="f0d01-1217">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="f0d01-1217">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="f0d01-1218">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="f0d01-1218">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="f0d01-1219">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="f0d01-1219">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="f0d01-1220">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="f0d01-1220">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="f0d01-1221">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1221">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="f0d01-1222">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1222">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="f0d01-1223">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1223">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="f0d01-1224">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1224">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="f0d01-1225">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1225">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="f0d01-1226">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1226">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="f0d01-1227">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1227">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="f0d01-1228">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1228">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="f0d01-1229">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1229">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="f0d01-1230">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1230">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="f0d01-1231">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1231">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="f0d01-1232">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="f0d01-1232">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="f0d01-1233">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-1233">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="f0d01-1234">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="f0d01-1234">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="f0d01-1235">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1235">RDBMS</span></span>
* <span data-ttu-id="f0d01-1236">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="f0d01-1236">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="f0d01-1237">Reserva</span><span class="sxs-lookup"><span data-stu-id="f0d01-1237">Reservation</span></span>
* <span data-ttu-id="f0d01-1238">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="f0d01-1238">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="f0d01-1239">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="f0d01-1239">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="f0d01-1240">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1240">Manage App</span></span>
* <span data-ttu-id="f0d01-1241">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="f0d01-1241">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="f0d01-1242">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="f0d01-1242">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-1243">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-1243">Role</span></span>
* <span data-ttu-id="f0d01-1244">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="f0d01-1244">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="f0d01-1245">SignalR</span><span class="sxs-lookup"><span data-stu-id="f0d01-1245">SignalR</span></span>
* <span data-ttu-id="f0d01-1246">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="f0d01-1246">First release</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-1247">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1247">Storage</span></span>
* <span data-ttu-id="f0d01-1248">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="f0d01-1248">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="f0d01-1249">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="f0d01-1249">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-1250">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1250">VM</span></span>
* <span data-ttu-id="f0d01-1251">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="f0d01-1251">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="f0d01-1252">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1252">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="f0d01-1253">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1253">August 28, 2018</span></span>

<span data-ttu-id="f0d01-1254">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="f0d01-1254">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-1255">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1255">Core</span></span>

* <span data-ttu-id="f0d01-1256">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="f0d01-1256">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="f0d01-1257">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="f0d01-1257">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-1258">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-1258">ACR</span></span>

* <span data-ttu-id="f0d01-1259">Adicionada uma solução alternativa para operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1259">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="f0d01-1260">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1260">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-1261">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1261">ACS</span></span>

* <span data-ttu-id="f0d01-1262">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1262">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="f0d01-1263">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="f0d01-1263">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-1264">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-1264">AppService</span></span>

* <span data-ttu-id="f0d01-1265">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="f0d01-1265">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="f0d01-1266">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1266">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="f0d01-1267">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="f0d01-1267">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="f0d01-1268">Backup</span><span class="sxs-lookup"><span data-stu-id="f0d01-1268">Backup</span></span>

* <span data-ttu-id="f0d01-1269">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="f0d01-1269">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="f0d01-1270">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="f0d01-1270">Bot Service</span></span>

* <span data-ttu-id="f0d01-1271">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="f0d01-1271">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f0d01-1272">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1272">Cognitive Services</span></span>

* <span data-ttu-id="f0d01-1273">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="f0d01-1273">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="f0d01-1274">IoT</span><span class="sxs-lookup"><span data-stu-id="f0d01-1274">IoT</span></span>

* <span data-ttu-id="f0d01-1275">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="f0d01-1275">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="f0d01-1276">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1276">Monitor</span></span>

* <span data-ttu-id="f0d01-1277">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="f0d01-1277">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="f0d01-1278">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1278">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-1279">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-1279">Network</span></span>

* <span data-ttu-id="f0d01-1280">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="f0d01-1280">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-1281">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-1281">Resource</span></span>

* <span data-ttu-id="f0d01-1282">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="f0d01-1282">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-1283">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1283">Storage</span></span>

* <span data-ttu-id="f0d01-1284">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="f0d01-1284">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-1285">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1285">VM</span></span>

* <span data-ttu-id="f0d01-1286">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="f0d01-1286">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="f0d01-1287">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1287">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="f0d01-1288">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1288">Auguest 14, 2018</span></span>

<span data-ttu-id="f0d01-1289">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="f0d01-1289">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-1290">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1290">Core</span></span>

* <span data-ttu-id="f0d01-1291">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1291">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="f0d01-1292">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="f0d01-1292">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="f0d01-1293">Telemetria</span><span class="sxs-lookup"><span data-stu-id="f0d01-1293">Telemetry</span></span>

* <span data-ttu-id="f0d01-1294">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="f0d01-1294">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-1295">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-1295">ACR</span></span>

* <span data-ttu-id="f0d01-1296">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1296">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="f0d01-1297">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="f0d01-1297">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-1298">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1298">ACS</span></span>

* <span data-ttu-id="f0d01-1299">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="f0d01-1299">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="f0d01-1300">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="f0d01-1300">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="f0d01-1301">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="f0d01-1301">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="f0d01-1302">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="f0d01-1302">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="f0d01-1303">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="f0d01-1303">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="f0d01-1304">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-1304">AppService</span></span>

* <span data-ttu-id="f0d01-1305">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1305">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="f0d01-1306">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="f0d01-1306">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="f0d01-1307">BatchAI</span><span class="sxs-lookup"><span data-stu-id="f0d01-1307">BatchAI</span></span>

* <span data-ttu-id="f0d01-1308">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1308">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="f0d01-1309">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-1309">Container</span></span>

* <span data-ttu-id="f0d01-1310">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-1310">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="f0d01-1311">IoT</span><span class="sxs-lookup"><span data-stu-id="f0d01-1311">IoT</span></span>

* <span data-ttu-id="f0d01-1312">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="f0d01-1312">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="f0d01-1313">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1313">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="f0d01-1314">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="f0d01-1314">Iot Central</span></span>

* <span data-ttu-id="f0d01-1315">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="f0d01-1315">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="f0d01-1316">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f0d01-1316">KeyVault</span></span>


* <span data-ttu-id="f0d01-1317">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="f0d01-1317">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="f0d01-1318">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-1318">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="f0d01-1319">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1319">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="f0d01-1320">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="f0d01-1320">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="f0d01-1321">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="f0d01-1321">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="f0d01-1322">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="f0d01-1322">Relay</span></span>

* <span data-ttu-id="f0d01-1323">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="f0d01-1323">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-1324">Sql</span><span class="sxs-lookup"><span data-stu-id="f0d01-1324">Sql</span></span>

* <span data-ttu-id="f0d01-1325">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1325">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-1326">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1326">Storage</span></span>

* <span data-ttu-id="f0d01-1327">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="f0d01-1327">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="f0d01-1328">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1328">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="f0d01-1329">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="f0d01-1329">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="f0d01-1330">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1330">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="f0d01-1331">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-1331">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-1332">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1332">VM</span></span>

* <span data-ttu-id="f0d01-1333">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="f0d01-1333">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="f0d01-1334">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1334">July 31, 2018</span></span>

<span data-ttu-id="f0d01-1335">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="f0d01-1335">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-1336">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-1336">ACR</span></span>

* <span data-ttu-id="f0d01-1337">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1337">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="f0d01-1338">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1338">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-1339">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1339">ACS</span></span>

* <span data-ttu-id="f0d01-1340">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="f0d01-1340">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="f0d01-1341">Lote</span><span class="sxs-lookup"><span data-stu-id="f0d01-1341">Batch</span></span>

* <span data-ttu-id="f0d01-1342">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="f0d01-1342">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="f0d01-1343">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-1343">Container</span></span>

* <span data-ttu-id="f0d01-1344">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="f0d01-1344">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-1345">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-1345">Network</span></span>

* <span data-ttu-id="f0d01-1346">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="f0d01-1346">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="f0d01-1347">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-1347">Resource</span></span>

* <span data-ttu-id="f0d01-1348">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="f0d01-1348">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="f0d01-1349">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="f0d01-1349">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-1350">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-1350">Role</span></span>

* <span data-ttu-id="f0d01-1351">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="f0d01-1351">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="f0d01-1352">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="f0d01-1352">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="f0d01-1353">Search</span><span class="sxs-lookup"><span data-stu-id="f0d01-1353">Search</span></span>

* <span data-ttu-id="f0d01-1354">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="f0d01-1354">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="f0d01-1355">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="f0d01-1355">Service Bus</span></span>

* <span data-ttu-id="f0d01-1356">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="f0d01-1356">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="f0d01-1357">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="f0d01-1357">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="f0d01-1358">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1358">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="f0d01-1359">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1359">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-1360">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1360">Storage</span></span>

* <span data-ttu-id="f0d01-1361">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="f0d01-1361">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="f0d01-1362">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="f0d01-1362">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-1363">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1363">VM</span></span>

* <span data-ttu-id="f0d01-1364">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="f0d01-1364">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="f0d01-1365">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1365">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="f0d01-1366">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1366">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="f0d01-1367">[ALTERAÇÃO SIGNIFICATIVA] `[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="f0d01-1367">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="f0d01-1368">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1368">July 18, 2018</span></span>

<span data-ttu-id="f0d01-1369">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="f0d01-1369">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-1370">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1370">Core</span></span>

* <span data-ttu-id="f0d01-1371">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="f0d01-1371">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="f0d01-1372">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="f0d01-1372">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="f0d01-1373">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="f0d01-1373">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-1374">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-1374">ACR</span></span>

* <span data-ttu-id="f0d01-1375">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="f0d01-1375">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="f0d01-1376">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1376">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="f0d01-1377">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="f0d01-1377">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="f0d01-1378">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="f0d01-1378">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-1379">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1379">ACS</span></span>

* <span data-ttu-id="f0d01-1380">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="f0d01-1380">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-1381">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-1381">AppService</span></span>

* <span data-ttu-id="f0d01-1382">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="f0d01-1382">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="f0d01-1383">Lote</span><span class="sxs-lookup"><span data-stu-id="f0d01-1383">Batch</span></span>

* <span data-ttu-id="f0d01-1384">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="f0d01-1384">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="f0d01-1385">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="f0d01-1385">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f0d01-1386">Lote AI</span><span class="sxs-lookup"><span data-stu-id="f0d01-1386">Batch AI</span></span>

* <span data-ttu-id="f0d01-1387">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1387">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="f0d01-1388">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-1388">Container</span></span>

* <span data-ttu-id="f0d01-1389">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="f0d01-1389">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="f0d01-1390">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="f0d01-1390">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-1391">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-1391">Network</span></span>

* <span data-ttu-id="f0d01-1392">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1392">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="f0d01-1393">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1393">Added `network nic wait`</span></span>
* <span data-ttu-id="f0d01-1394">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1394">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="f0d01-1395">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1395">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="f0d01-1396">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-1396">Resource</span></span>

* <span data-ttu-id="f0d01-1397">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1397">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="f0d01-1398">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1398">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="f0d01-1399">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1399">Added `deployment wait` command</span></span>
* <span data-ttu-id="f0d01-1400">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="f0d01-1400">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-1401">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-1401">SQL</span></span>

* <span data-ttu-id="f0d01-1402">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1402">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="f0d01-1403">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1403">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="f0d01-1404">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1404">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-1405">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1405">Storage</span></span>

* <span data-ttu-id="f0d01-1406">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="f0d01-1406">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-1407">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1407">VM</span></span>

* <span data-ttu-id="f0d01-1408">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="f0d01-1408">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="f0d01-1409">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1409">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="f0d01-1410">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1410">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="f0d01-1411">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1411">July 3, 2018</span></span>

<span data-ttu-id="f0d01-1412">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="f0d01-1412">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="f0d01-1413">AKS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1413">AKS</span></span>

* <span data-ttu-id="f0d01-1414">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="f0d01-1414">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="f0d01-1415">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1415">July 3, 2018</span></span>

<span data-ttu-id="f0d01-1416">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="f0d01-1416">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-1417">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1417">Core</span></span>

* <span data-ttu-id="f0d01-1418">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1418">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-1419">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-1419">ACR</span></span>

* <span data-ttu-id="f0d01-1420">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="f0d01-1420">Added polling build status</span></span>
* <span data-ttu-id="f0d01-1421">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="f0d01-1421">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="f0d01-1422">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1422">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-1423">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1423">ACS</span></span>

* <span data-ttu-id="f0d01-1424">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="f0d01-1424">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="f0d01-1425">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="f0d01-1425">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="f0d01-1426">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1426">Updated options for `aks browse` command.</span></span> <span data-ttu-id="f0d01-1427">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="f0d01-1427">Added `--listen-port` support</span></span>
* <span data-ttu-id="f0d01-1428">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1428">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="f0d01-1429">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="f0d01-1429">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="f0d01-1430">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="f0d01-1430">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-1431">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-1431">AppService</span></span>

* <span data-ttu-id="f0d01-1432">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1432">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="f0d01-1433">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="f0d01-1433">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="f0d01-1434">Backup</span><span class="sxs-lookup"><span data-stu-id="f0d01-1434">Backup</span></span>

* <span data-ttu-id="f0d01-1435">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="f0d01-1435">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="f0d01-1436">BatchAI</span><span class="sxs-lookup"><span data-stu-id="f0d01-1436">BatchAI</span></span>

* <span data-ttu-id="f0d01-1437">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1437">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="f0d01-1438">Nuvem</span><span class="sxs-lookup"><span data-stu-id="f0d01-1438">Cloud</span></span>

* <span data-ttu-id="f0d01-1439">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="f0d01-1439">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="f0d01-1440">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-1440">Container</span></span>

* <span data-ttu-id="f0d01-1441">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="f0d01-1441">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="f0d01-1442">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="f0d01-1442">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="f0d01-1443">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="f0d01-1443">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="f0d01-1444">Extensão</span><span class="sxs-lookup"><span data-stu-id="f0d01-1444">Extension</span></span>

* <span data-ttu-id="f0d01-1445">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="f0d01-1445">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-1446">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-1446">Network</span></span>

* <span data-ttu-id="f0d01-1447">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="f0d01-1447">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="f0d01-1448">Rdbms</span><span class="sxs-lookup"><span data-stu-id="f0d01-1448">Rdbms</span></span>

* <span data-ttu-id="f0d01-1449">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1449">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-1450">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-1450">Resource</span></span>

* <span data-ttu-id="f0d01-1451">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="f0d01-1451">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-1452">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1452">VM</span></span>

* <span data-ttu-id="f0d01-1453">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="f0d01-1453">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="f0d01-1454">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1454">June 25, 2018</span></span>

<span data-ttu-id="f0d01-1455">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="f0d01-1455">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="f0d01-1456">CLI</span><span class="sxs-lookup"><span data-stu-id="f0d01-1456">CLI</span></span>

* <span data-ttu-id="f0d01-1457">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="f0d01-1457">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="f0d01-1458">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1458">June 19, 2018</span></span>

<span data-ttu-id="f0d01-1459">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="f0d01-1459">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-1460">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1460">Core</span></span>

* <span data-ttu-id="f0d01-1461">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1461">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-1462">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-1462">ACR</span></span>

* <span data-ttu-id="f0d01-1463">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="f0d01-1463">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="f0d01-1464">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1464">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-1465">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1465">ACS</span></span>

* <span data-ttu-id="f0d01-1466">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1466">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="f0d01-1467">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="f0d01-1467">Added `--update` support</span></span>
* <span data-ttu-id="f0d01-1468">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1468">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="f0d01-1469">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="f0d01-1469">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="f0d01-1470">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="f0d01-1470">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="f0d01-1471">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1471">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="f0d01-1472">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1472">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="f0d01-1473">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1473">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-1474">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-1474">AppService</span></span>

* <span data-ttu-id="f0d01-1475">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="f0d01-1475">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="f0d01-1476">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1476">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="f0d01-1477">Lote</span><span class="sxs-lookup"><span data-stu-id="f0d01-1477">Batch</span></span>

* <span data-ttu-id="f0d01-1478">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="f0d01-1478">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f0d01-1479">Lote AI</span><span class="sxs-lookup"><span data-stu-id="f0d01-1479">Batch AI</span></span>

* <span data-ttu-id="f0d01-1480">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1480">Added support for workspaces.</span></span> <span data-ttu-id="f0d01-1481">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="f0d01-1481">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="f0d01-1482">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1482">Added support for experiments.</span></span> <span data-ttu-id="f0d01-1483">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="f0d01-1483">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="f0d01-1484">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="f0d01-1484">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="f0d01-1485">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1485">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="f0d01-1486">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1486">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="f0d01-1487">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1487">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="f0d01-1488">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="f0d01-1488">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="f0d01-1489">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="f0d01-1489">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="f0d01-1490">[ALTERAÇÃO SIGNIFICATIVA] `--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1490">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="f0d01-1491">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1491">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="f0d01-1492">[ALTERAÇÃO SIGNIFICATIVA] `--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1492">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="f0d01-1493">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1493">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="f0d01-1494">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1494">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="f0d01-1495">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1495">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="f0d01-1496">[ALTERAÇÃO SIGNIFICATIVA] `--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1496">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="f0d01-1497">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="f0d01-1497">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="f0d01-1498">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="f0d01-1498">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="f0d01-1499">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="f0d01-1499">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="f0d01-1500">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="f0d01-1500">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="f0d01-1501">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="f0d01-1501">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="f0d01-1502">Mapas</span><span class="sxs-lookup"><span data-stu-id="f0d01-1502">Maps</span></span>

* <span data-ttu-id="f0d01-1503">[ALTERAÇÃO SIGNIFICATIVA] `maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1503">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-1504">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-1504">Network</span></span>

* <span data-ttu-id="f0d01-1505">Foi adicionado suporte a `https` para `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="f0d01-1505">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="f0d01-1506">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1506">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="f0d01-1507">#6502</span><span class="sxs-lookup"><span data-stu-id="f0d01-1507">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="f0d01-1508">Reservas</span><span class="sxs-lookup"><span data-stu-id="f0d01-1508">Reservations</span></span>

* <span data-ttu-id="f0d01-1509">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1509">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="f0d01-1510">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1510">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="f0d01-1511">[ALTERAÇÃO SIGNIFICATIVA] `kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1511">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="f0d01-1512">[ALTERAÇÃO SIGNIFICATIVA] `capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1512">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="f0d01-1513">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1513">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="f0d01-1514">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1514">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-1515">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-1515">Role</span></span>

* <span data-ttu-id="f0d01-1516">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="f0d01-1516">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-1517">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-1517">SQL</span></span>

* <span data-ttu-id="f0d01-1518">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="f0d01-1518">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-1519">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1519">Storage</span></span>

* <span data-ttu-id="f0d01-1520">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="f0d01-1520">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-1521">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1521">VM</span></span>

* <span data-ttu-id="f0d01-1522">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1522">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="f0d01-1523">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1523">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="f0d01-1524">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="f0d01-1524">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="f0d01-1525">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1525">June 13, 2018</span></span>

<span data-ttu-id="f0d01-1526">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="f0d01-1526">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-1527">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1527">Core</span></span>

* <span data-ttu-id="f0d01-1528">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="f0d01-1528">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="f0d01-1529">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1529">June 13, 2018</span></span>

<span data-ttu-id="f0d01-1530">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="f0d01-1530">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="f0d01-1531">AKS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1531">AKS</span></span>

* <span data-ttu-id="f0d01-1532">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1532">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="f0d01-1533">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="f0d01-1533">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="f0d01-1534">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1534">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="f0d01-1535">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1535">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="f0d01-1536">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1536">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-1537">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-1537">AppService</span></span>

* <span data-ttu-id="f0d01-1538">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="f0d01-1538">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="f0d01-1539">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1539">June 5, 2018</span></span>

<span data-ttu-id="f0d01-1540">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="f0d01-1540">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="f0d01-1541">Interativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1541">Interactive</span></span>

* <span data-ttu-id="f0d01-1542">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1542">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="f0d01-1543">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1543">June 5, 2018</span></span>

<span data-ttu-id="f0d01-1544">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="f0d01-1544">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-1545">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1545">Core</span></span>

* <span data-ttu-id="f0d01-1546">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="f0d01-1546">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="f0d01-1547">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="f0d01-1547">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-1548">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-1548">ACR</span></span>

* <span data-ttu-id="f0d01-1549">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="f0d01-1549">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="f0d01-1550">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1550">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="f0d01-1551">AKS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1551">AKS</span></span>

* <span data-ttu-id="f0d01-1552">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="f0d01-1552">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="f0d01-1553">Lote</span><span class="sxs-lookup"><span data-stu-id="f0d01-1553">Batch</span></span>

* <span data-ttu-id="f0d01-1554">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="f0d01-1554">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="f0d01-1555">IOT</span><span class="sxs-lookup"><span data-stu-id="f0d01-1555">IOT</span></span>

* <span data-ttu-id="f0d01-1556">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="f0d01-1556">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-1557">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-1557">Network</span></span>

* <span data-ttu-id="f0d01-1558">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="f0d01-1558">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="f0d01-1559">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="f0d01-1559">Policy Insights</span></span>

* <span data-ttu-id="f0d01-1560">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="f0d01-1560">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="f0d01-1561">ARM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1561">ARM</span></span>

* <span data-ttu-id="f0d01-1562">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1562">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-1563">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-1563">SQL</span></span>

* <span data-ttu-id="f0d01-1564">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="f0d01-1564">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="f0d01-1565">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="f0d01-1565">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="f0d01-1566">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1566">Storage</span></span>

* <span data-ttu-id="f0d01-1567">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1567">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-1568">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1568">VM</span></span>

* <span data-ttu-id="f0d01-1569">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1569">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="f0d01-1570">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1570">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="f0d01-1571">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1571">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="f0d01-1572">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1572">May 22, 2018</span></span>

<span data-ttu-id="f0d01-1573">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="f0d01-1573">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-1574">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1574">Core</span></span>

* <span data-ttu-id="f0d01-1575">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1575">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-1576">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1576">ACS</span></span>

* <span data-ttu-id="f0d01-1577">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="f0d01-1577">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="f0d01-1578">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="f0d01-1578">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-1579">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-1579">AppService</span></span>

* <span data-ttu-id="f0d01-1580">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="f0d01-1580">Improved generic update commands</span></span>
* <span data-ttu-id="f0d01-1581">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1581">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="f0d01-1582">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-1582">Container</span></span>

* <span data-ttu-id="f0d01-1583">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="f0d01-1583">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="f0d01-1584">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-1584">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="f0d01-1585">Extensão</span><span class="sxs-lookup"><span data-stu-id="f0d01-1585">Extension</span></span>

* <span data-ttu-id="f0d01-1586">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="f0d01-1586">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="f0d01-1587">Interativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1587">Interactive</span></span>

* <span data-ttu-id="f0d01-1588">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="f0d01-1588">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="f0d01-1589">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="f0d01-1589">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="f0d01-1590">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f0d01-1590">KeyVault</span></span>

* <span data-ttu-id="f0d01-1591">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="f0d01-1591">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-1592">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-1592">Network</span></span>

* <span data-ttu-id="f0d01-1593">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="f0d01-1593">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="f0d01-1594">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="f0d01-1594">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-1595">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-1595">SQL</span></span>

* <span data-ttu-id="f0d01-1596">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="f0d01-1596">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="f0d01-1597">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1597">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="f0d01-1598">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="f0d01-1598">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="f0d01-1599">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0d01-1599">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="f0d01-1600">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="f0d01-1600">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="f0d01-1601">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1601">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="f0d01-1602">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1602">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="f0d01-1603">`edition`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1603">`edition`.</span></span> <span data-ttu-id="f0d01-1604">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1604">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="f0d01-1605">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1605">`elasticPoolName`.</span></span> <span data-ttu-id="f0d01-1606">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1606">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="f0d01-1607">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="f0d01-1607">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="f0d01-1608">`edition`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1608">`edition`.</span></span> <span data-ttu-id="f0d01-1609">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1609">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="f0d01-1610">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1610">`dtu`.</span></span> <span data-ttu-id="f0d01-1611">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1611">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="f0d01-1612">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1612">`databaseDtuMin`.</span></span> <span data-ttu-id="f0d01-1613">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1613">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="f0d01-1614">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1614">`databaseDtuMax`.</span></span> <span data-ttu-id="f0d01-1615">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1615">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="f0d01-1616">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1616">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="f0d01-1617">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1617">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-1618">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1618">Storage</span></span>

* <span data-ttu-id="f0d01-1619">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1619">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="f0d01-1620">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="f0d01-1620">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-1621">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1621">VM</span></span>

* <span data-ttu-id="f0d01-1622">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1622">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="f0d01-1623">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1623">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="f0d01-1624">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1624">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="f0d01-1625">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="f0d01-1625">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="f0d01-1626">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1626">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="f0d01-1627">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1627">May 7, 2018</span></span>

<span data-ttu-id="f0d01-1628">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="f0d01-1628">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-1629">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1629">Core</span></span>

* <span data-ttu-id="f0d01-1630">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="f0d01-1630">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="f0d01-1631">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="f0d01-1631">Added limited support for positional arguments</span></span>
* <span data-ttu-id="f0d01-1632">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1632">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="f0d01-1633">#5591</span><span class="sxs-lookup"><span data-stu-id="f0d01-1633">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="f0d01-1634">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1634">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="f0d01-1635">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="f0d01-1635">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="f0d01-1636">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1636">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="f0d01-1637">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1637">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="f0d01-1638">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="f0d01-1638">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-1639">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-1639">ACR</span></span>

* <span data-ttu-id="f0d01-1640">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-1640">Added ACR Build commands</span></span>
* <span data-ttu-id="f0d01-1641">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="f0d01-1641">Improved resource not found error messages</span></span>
* <span data-ttu-id="f0d01-1642">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="f0d01-1642">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="f0d01-1643">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="f0d01-1643">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="f0d01-1644">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="f0d01-1644">Improved repository commands error messages</span></span>
* <span data-ttu-id="f0d01-1645">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="f0d01-1645">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-1646">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1646">ACS</span></span>

* <span data-ttu-id="f0d01-1647">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="f0d01-1647">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="f0d01-1648">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="f0d01-1648">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="f0d01-1649">AMS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1649">AMS</span></span>

* <span data-ttu-id="f0d01-1650">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="f0d01-1650">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-1651">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-1651">Appservice</span></span>

* <span data-ttu-id="f0d01-1652">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="f0d01-1652">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="f0d01-1653">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1653">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="f0d01-1654">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="f0d01-1654">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="f0d01-1655">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="f0d01-1655">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f0d01-1656">Lote AI</span><span class="sxs-lookup"><span data-stu-id="f0d01-1656">Batch AI</span></span>

* <span data-ttu-id="f0d01-1657">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="f0d01-1657">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f0d01-1658">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1658">Cognitive Services</span></span>

* <span data-ttu-id="f0d01-1659">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="f0d01-1659">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="f0d01-1660">Consumo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1660">Consumption</span></span>

* <span data-ttu-id="f0d01-1661">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1661">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="f0d01-1662">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-1662">Container</span></span>

* <span data-ttu-id="f0d01-1663">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="f0d01-1663">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="f0d01-1664">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f0d01-1664">Cosmos DB</span></span>

* <span data-ttu-id="f0d01-1665">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f0d01-1665">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="f0d01-1666">DMS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1666">DMS</span></span>

* <span data-ttu-id="f0d01-1667">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="f0d01-1667">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="f0d01-1668">Extensão</span><span class="sxs-lookup"><span data-stu-id="f0d01-1668">Extension</span></span>

* <span data-ttu-id="f0d01-1669">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1669">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="f0d01-1670">Interativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1670">Interactive</span></span>

* <span data-ttu-id="f0d01-1671">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="f0d01-1671">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="f0d01-1672">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="f0d01-1672">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="f0d01-1673">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="f0d01-1673">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="f0d01-1674">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="f0d01-1674">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="f0d01-1675">Laboratório</span><span class="sxs-lookup"><span data-stu-id="f0d01-1675">Lab</span></span>

* <span data-ttu-id="f0d01-1676">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="f0d01-1676">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-1677">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-1677">Network</span></span>

* <span data-ttu-id="f0d01-1678">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="f0d01-1678">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="f0d01-1679">Perfil</span><span class="sxs-lookup"><span data-stu-id="f0d01-1679">Profile</span></span>

* <span data-ttu-id="f0d01-1680">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="f0d01-1680">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="f0d01-1681">[ALTERAÇÃO SIGNIFICATIVA] `--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="f0d01-1681">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="f0d01-1682">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1682">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="f0d01-1683">Redis</span><span class="sxs-lookup"><span data-stu-id="f0d01-1683">Redis</span></span>

* <span data-ttu-id="f0d01-1684">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1684">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="f0d01-1685">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1685">Deprecated `redis list-all`.</span></span> <span data-ttu-id="f0d01-1686">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1686">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="f0d01-1687">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1687">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="f0d01-1688">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1688">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-1689">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-1689">Role</span></span>

* <span data-ttu-id="f0d01-1690">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="f0d01-1690">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-1691">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1691">Storage</span></span>

* <span data-ttu-id="f0d01-1692">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="f0d01-1692">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="f0d01-1693">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="f0d01-1693">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="f0d01-1694">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1694">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="f0d01-1695">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="f0d01-1695">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="f0d01-1696">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="f0d01-1696">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-1697">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1697">VM</span></span>

* <span data-ttu-id="f0d01-1698">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="f0d01-1698">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="f0d01-1699">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="f0d01-1699">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="f0d01-1700">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="f0d01-1700">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="f0d01-1701">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1701">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="f0d01-1702">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="f0d01-1702">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="f0d01-1703">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="f0d01-1703">Added write accelerator support</span></span>
* <span data-ttu-id="f0d01-1704">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1704">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="f0d01-1705">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="f0d01-1705">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="f0d01-1706">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="f0d01-1706">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="f0d01-1707">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1707">April 10, 2018</span></span>

<span data-ttu-id="f0d01-1708">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="f0d01-1708">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-1709">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-1709">ACR</span></span>

* <span data-ttu-id="f0d01-1710">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="f0d01-1710">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-1711">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1711">ACS</span></span>

* <span data-ttu-id="f0d01-1712">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1712">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-1713">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-1713">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="f0d01-1715">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="f0d01-1715">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="f0d01-1716">BatchAI</span><span class="sxs-lookup"><span data-stu-id="f0d01-1716">BatchAI</span></span>

* <span data-ttu-id="f0d01-1717">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="f0d01-1717">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="f0d01-1718">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="f0d01-1718">Job level mounting</span></span>
  - <span data-ttu-id="f0d01-1719">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1719">Environment variables with secret values</span></span>
  - <span data-ttu-id="f0d01-1720">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="f0d01-1720">Performance counters settings</span></span>
  - <span data-ttu-id="f0d01-1721">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="f0d01-1721">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="f0d01-1722">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="f0d01-1722">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="f0d01-1723">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="f0d01-1723">Usage and limits reporting</span></span>
  - <span data-ttu-id="f0d01-1724">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1724">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="f0d01-1725">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="f0d01-1725">Support for custom images</span></span>
  - <span data-ttu-id="f0d01-1726">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="f0d01-1726">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="f0d01-1727">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="f0d01-1727">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="f0d01-1728">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="f0d01-1728">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="f0d01-1729">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="f0d01-1729">National clouds are supported</span></span>
* <span data-ttu-id="f0d01-1730">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="f0d01-1730">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="f0d01-1731">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="f0d01-1731">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="f0d01-1732">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="f0d01-1732">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="f0d01-1733">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1733">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="f0d01-1734">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="f0d01-1734">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="f0d01-1735">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="f0d01-1735">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="f0d01-1736">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1736">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="f0d01-1737">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1737">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="f0d01-1738">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="f0d01-1738">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="f0d01-1739">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1739">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="f0d01-1740">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="f0d01-1740">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="f0d01-1741">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1741">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="f0d01-1742">[ALTERAÇÃO SIGNIFICATIVA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1742">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="f0d01-1743">Cobrança</span><span class="sxs-lookup"><span data-stu-id="f0d01-1743">Billing</span></span>

* <span data-ttu-id="f0d01-1744">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="f0d01-1744">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="f0d01-1745">Consumo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1745">Consumption</span></span>

* <span data-ttu-id="f0d01-1746">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1746">Added `marketplace` commands</span></span>
* <span data-ttu-id="f0d01-1747">[ALTERAÇÃO SIGNIFICATIVA] `reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1747">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="f0d01-1748">[ALTERAÇÃO SIGNIFICATIVA] `reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1748">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="f0d01-1749">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1749">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="f0d01-1750">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1750">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="f0d01-1751">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1751">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="f0d01-1752">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-1752">Container</span></span>

* <span data-ttu-id="f0d01-1753">Adição dos parâmetros de montagem de volume de repositório git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1753">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="f0d01-1754">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="f0d01-1754">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="f0d01-1755">Extensão</span><span class="sxs-lookup"><span data-stu-id="f0d01-1755">Extension</span></span>

* <span data-ttu-id="f0d01-1756">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="f0d01-1756">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="f0d01-1757">Interativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1757">Interactive</span></span>

* <span data-ttu-id="f0d01-1758">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1758">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="f0d01-1759">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="f0d01-1759">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="f0d01-1760">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1760">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-1761">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-1761">Network</span></span>

* <span data-ttu-id="f0d01-1762">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="f0d01-1762">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="f0d01-1763">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1763">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="f0d01-1764">#4910</span><span class="sxs-lookup"><span data-stu-id="f0d01-1764">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="f0d01-1765">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1765">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="f0d01-1766">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1766">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="f0d01-1767">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1767">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="f0d01-1768">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1768">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="f0d01-1769">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1769">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="f0d01-1770">Perfil</span><span class="sxs-lookup"><span data-stu-id="f0d01-1770">Profile</span></span>

* <span data-ttu-id="f0d01-1771">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1771">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="f0d01-1772">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1772">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="f0d01-1773">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1773">RDBMS</span></span>

* <span data-ttu-id="f0d01-1774">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1774">Added `georestore` command</span></span>
* <span data-ttu-id="f0d01-1775">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1775">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-1776">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-1776">Resource</span></span>

* <span data-ttu-id="f0d01-1777">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1777">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="f0d01-1778">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1778">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-1779">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-1779">SQL</span></span>

* <span data-ttu-id="f0d01-1780">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1780">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-1781">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1781">Storage</span></span>

* <span data-ttu-id="f0d01-1782">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="f0d01-1782">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-1783">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1783">VM</span></span>

* <span data-ttu-id="f0d01-1784">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1784">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="f0d01-1785">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1785">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="f0d01-1787">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1787">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="f0d01-1788">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1788">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="f0d01-1789">#5718</span><span class="sxs-lookup"><span data-stu-id="f0d01-1789">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="f0d01-1790">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="f0d01-1790">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="f0d01-1791">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1791">March 27, 2018</span></span>

<span data-ttu-id="f0d01-1792">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="f0d01-1792">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-1793">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1793">Core</span></span>

* <span data-ttu-id="f0d01-1794">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="f0d01-1794">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-1795">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1795">ACS</span></span>

* <span data-ttu-id="f0d01-1796">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="f0d01-1796">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-1797">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-1797">Appservice</span></span>

* <span data-ttu-id="f0d01-1798">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1798">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="f0d01-1799">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1799">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="f0d01-1800">Backup</span><span class="sxs-lookup"><span data-stu-id="f0d01-1800">Backup</span></span>

* <span data-ttu-id="f0d01-1801">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1801">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="f0d01-1802">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="f0d01-1802">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="f0d01-1803">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="f0d01-1803">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="f0d01-1804">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1804">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="f0d01-1805">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-1805">Container</span></span>

* <span data-ttu-id="f0d01-1806">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1806">Added `container exec` command.</span></span> <span data-ttu-id="f0d01-1807">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="f0d01-1807">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="f0d01-1808">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-1808">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="f0d01-1809">Extensão</span><span class="sxs-lookup"><span data-stu-id="f0d01-1809">Extension</span></span>

* <span data-ttu-id="f0d01-1810">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="f0d01-1810">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="f0d01-1811">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1811">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="f0d01-1812">[ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="f0d01-1812">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="f0d01-1813">Interativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1813">Interactive</span></span>

* <span data-ttu-id="f0d01-1814">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1814">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="f0d01-1815">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1815">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="f0d01-1816">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1816">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="f0d01-1817">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="f0d01-1817">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="f0d01-1818">Laboratório</span><span class="sxs-lookup"><span data-stu-id="f0d01-1818">Lab</span></span>

* <span data-ttu-id="f0d01-1819">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1819">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="f0d01-1820">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1820">Monitor</span></span>

* <span data-ttu-id="f0d01-1821">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="f0d01-1821">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="f0d01-1822">Corrigido [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="f0d01-1822">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="f0d01-1823">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="f0d01-1823">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-1824">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-1824">Network</span></span>

* <span data-ttu-id="f0d01-1825">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="f0d01-1825">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="f0d01-1826">Perfil</span><span class="sxs-lookup"><span data-stu-id="f0d01-1826">Profile</span></span>

* <span data-ttu-id="f0d01-1827">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1827">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f0d01-1828">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1828">RDBMS</span></span>

* <span data-ttu-id="f0d01-1829">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="f0d01-1829">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-1830">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-1830">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="f0d01-1832">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-1832">Role</span></span>

* <span data-ttu-id="f0d01-1833">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1833">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="f0d01-1834">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="f0d01-1834">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="f0d01-1835">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1835">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="f0d01-1836">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1836">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="f0d01-1837">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1837">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-1838">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1838">Storage</span></span>

* <span data-ttu-id="f0d01-1839">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="f0d01-1839">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="f0d01-1840">Corrigido [#4049](https://github.com/Azure/azure-cli/issues/4049): problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="f0d01-1840">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-1841">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1841">VM</span></span>

* <span data-ttu-id="f0d01-1842">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="f0d01-1842">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="f0d01-1843">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1843">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="f0d01-1844">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="f0d01-1844">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="f0d01-1845">[ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="f0d01-1845">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="f0d01-1846">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1846">March 13, 2018</span></span>

<span data-ttu-id="f0d01-1847">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="f0d01-1847">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-1848">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-1848">ACR</span></span>

* <span data-ttu-id="f0d01-1849">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1849">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="f0d01-1850">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1850">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="f0d01-1851">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="f0d01-1851">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-1852">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1852">ACS</span></span>

* <span data-ttu-id="f0d01-1853">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="f0d01-1853">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="f0d01-1854">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="f0d01-1854">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="f0d01-1855">Supervisor</span><span class="sxs-lookup"><span data-stu-id="f0d01-1855">Advisor</span></span>

* <span data-ttu-id="f0d01-1856">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1856">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="f0d01-1857">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1857">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="f0d01-1858">[ALTERAÇÃO SIGNIFICATIVA] `advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="f0d01-1858">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="f0d01-1859">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1859">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="f0d01-1860">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1860">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-1861">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-1861">Appservice</span></span>

* <span data-ttu-id="f0d01-1862">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1862">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="f0d01-1863">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="f0d01-1863">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="f0d01-1864">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1864">Eventhubs</span></span>

* <span data-ttu-id="f0d01-1865">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="f0d01-1865">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="f0d01-1866">Extensão</span><span class="sxs-lookup"><span data-stu-id="f0d01-1866">Extension</span></span>

* <span data-ttu-id="f0d01-1867">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="f0d01-1867">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="f0d01-1868">Interativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1868">Interactive</span></span>

* <span data-ttu-id="f0d01-1869">Corrigido [#5625](https://github.com/Azure/azure-cli/issues/5625): manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="f0d01-1869">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="f0d01-1870">Corrigido [#3016](https://github.com/Azure/azure-cli/issues/3016): histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1870">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="f0d01-1871">Corrigido [#5688](https://github.com/Azure/azure-cli/issues/5688): as conclusões não aparecerão se o carregamento da tabela de comando encontrar uma exceção</span><span class="sxs-lookup"><span data-stu-id="f0d01-1871">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="f0d01-1872">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="f0d01-1872">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="f0d01-1873">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1873">Monitor</span></span>

* <span data-ttu-id="f0d01-1874">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1874">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="f0d01-1875">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1875">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="f0d01-1876">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1876">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="f0d01-1877">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1877">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-1878">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-1878">Network</span></span>

* <span data-ttu-id="f0d01-1879">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1879">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="f0d01-1880">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="f0d01-1880">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="f0d01-1881">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="f0d01-1881">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="f0d01-1882">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1882">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="f0d01-1883">Perfil</span><span class="sxs-lookup"><span data-stu-id="f0d01-1883">Profile</span></span>

* <span data-ttu-id="f0d01-1884">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1884">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="f0d01-1885">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1885">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f0d01-1886">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1886">RDBMS</span></span>

* <span data-ttu-id="f0d01-1887">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="f0d01-1887">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="f0d01-1888">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="f0d01-1888">Service Bus</span></span>

* <span data-ttu-id="f0d01-1889">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="f0d01-1889">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-1890">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1890">Storage</span></span>

* <span data-ttu-id="f0d01-1891">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="f0d01-1891">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="f0d01-1892">Corrigido [#5286](https://github.com/Azure/azure-cli/issues/5286): os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="f0d01-1892">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-1893">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1893">VM</span></span>

* <span data-ttu-id="f0d01-1894">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="f0d01-1894">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="f0d01-1895">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1895">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="f0d01-1896">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1896">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="f0d01-1897">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="f0d01-1897">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="f0d01-1898">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1898">February 27, 2018</span></span>

<span data-ttu-id="f0d01-1899">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="f0d01-1899">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-1900">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1900">Core</span></span>

* <span data-ttu-id="f0d01-1901">Corrigido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="f0d01-1901">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="f0d01-1902">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="f0d01-1902">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="f0d01-1903">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1903">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-1904">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1904">ACS</span></span>

* <span data-ttu-id="f0d01-1905">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="f0d01-1905">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="f0d01-1906">Problema corrigido: permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="f0d01-1906">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="f0d01-1907">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1907">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="f0d01-1908">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1908">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-1909">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-1909">Appservice</span></span>

* <span data-ttu-id="f0d01-1910">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="f0d01-1910">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="f0d01-1911">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="f0d01-1911">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f0d01-1912">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1912">Cognitive Services</span></span>

* <span data-ttu-id="f0d01-1913">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1913">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="f0d01-1914">Consumo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1914">Consumption</span></span>

* <span data-ttu-id="f0d01-1915">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="f0d01-1915">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="f0d01-1916">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="f0d01-1916">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="f0d01-1917">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-1917">Container</span></span>

* <span data-ttu-id="f0d01-1918">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="f0d01-1918">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-1919">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-1919">Network</span></span>

* <span data-ttu-id="f0d01-1920">Corrigido [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1920">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-1921">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-1921">Resource</span></span>

* <span data-ttu-id="f0d01-1922">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="f0d01-1922">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-1923">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-1923">Role</span></span>

* <span data-ttu-id="f0d01-1924">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="f0d01-1924">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-1925">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-1925">SQL</span></span>

* <span data-ttu-id="f0d01-1926">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="f0d01-1926">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-1927">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1927">Storage</span></span>

* <span data-ttu-id="f0d01-1928">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1928">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-1929">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1929">VM</span></span>

* <span data-ttu-id="f0d01-1930">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1930">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="f0d01-1931">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1931">February 13, 2018</span></span>

<span data-ttu-id="f0d01-1932">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="f0d01-1932">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-1933">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1933">Core</span></span>

* <span data-ttu-id="f0d01-1934">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="f0d01-1934">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-1935">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1935">ACS</span></span>

* <span data-ttu-id="f0d01-1936">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="f0d01-1936">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="f0d01-1937">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1937">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="f0d01-1938">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="f0d01-1938">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="f0d01-1939">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1939">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="f0d01-1940">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="f0d01-1940">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="f0d01-1941">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1941">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="f0d01-1942">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="f0d01-1942">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="f0d01-1943">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1943">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-1944">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-1944">Appservice</span></span>

* <span data-ttu-id="f0d01-1945">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="f0d01-1945">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="f0d01-1946">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1946">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="f0d01-1947">CDN</span><span class="sxs-lookup"><span data-stu-id="f0d01-1947">CDN</span></span>

* <span data-ttu-id="f0d01-1948">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1948">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="f0d01-1949">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-1949">Container</span></span>

* <span data-ttu-id="f0d01-1950">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="f0d01-1950">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="f0d01-1951">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-1951">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f0d01-1952">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f0d01-1952">CosmosDB</span></span>

* <span data-ttu-id="f0d01-1953">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="f0d01-1953">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="f0d01-1954">Extensão</span><span class="sxs-lookup"><span data-stu-id="f0d01-1954">Extension</span></span>

* <span data-ttu-id="f0d01-1955">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1955">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="f0d01-1956">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1956">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="f0d01-1957">Comentários</span><span class="sxs-lookup"><span data-stu-id="f0d01-1957">Feedback</span></span>

* <span data-ttu-id="f0d01-1958">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="f0d01-1958">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="f0d01-1959">Interativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1959">Interactive</span></span>

* <span data-ttu-id="f0d01-1960">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="f0d01-1960">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="f0d01-1961">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="f0d01-1961">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="f0d01-1962">IoT</span><span class="sxs-lookup"><span data-stu-id="f0d01-1962">IoT</span></span>

* <span data-ttu-id="f0d01-1963">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="f0d01-1963">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="f0d01-1964">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="f0d01-1964">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="f0d01-1965">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1965">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="f0d01-1966">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="f0d01-1966">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="f0d01-1967">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1967">Monitor</span></span>

* <span data-ttu-id="f0d01-1968">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1968">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-1969">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-1969">Network</span></span>

* <span data-ttu-id="f0d01-1970">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="f0d01-1970">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="f0d01-1971">Perfil</span><span class="sxs-lookup"><span data-stu-id="f0d01-1971">Profile</span></span>

* <span data-ttu-id="f0d01-1972">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1972">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-1973">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-1973">Resource</span></span>

* <span data-ttu-id="f0d01-1974">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="f0d01-1974">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-1975">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-1975">Role</span></span>

* <span data-ttu-id="f0d01-1976">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1976">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-1977">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-1977">SQL</span></span>

* <span data-ttu-id="f0d01-1978">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1978">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="f0d01-1979">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1979">Added `sql db rename`</span></span>
* <span data-ttu-id="f0d01-1980">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="f0d01-1980">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-1981">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-1981">Storage</span></span>

* <span data-ttu-id="f0d01-1982">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="f0d01-1982">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-1983">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-1983">VM</span></span>

* <span data-ttu-id="f0d01-1984">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="f0d01-1984">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="f0d01-1985">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="f0d01-1985">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="f0d01-1986">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1986">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="f0d01-1987">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-1987">January 31, 2018</span></span>

<span data-ttu-id="f0d01-1988">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="f0d01-1988">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-1989">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1989">Core</span></span>

* <span data-ttu-id="f0d01-1990">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="f0d01-1990">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="f0d01-1991">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="f0d01-1991">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="f0d01-1992">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="f0d01-1992">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="f0d01-1993">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="f0d01-1993">Use `--verbose` to see</span></span>
* <span data-ttu-id="f0d01-1994">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="f0d01-1994">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-1995">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-1995">ACS</span></span>

* <span data-ttu-id="f0d01-1996">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="f0d01-1996">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="f0d01-1997">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="f0d01-1997">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-1998">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-1998">Appservice</span></span>

* <span data-ttu-id="f0d01-1999">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="f0d01-1999">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="f0d01-2000">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="f0d01-2000">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="f0d01-2001">CDN</span><span class="sxs-lookup"><span data-stu-id="f0d01-2001">CDN</span></span>

* <span data-ttu-id="f0d01-2002">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2002">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f0d01-2003">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f0d01-2003">CosmosDB</span></span>

* <span data-ttu-id="f0d01-2004">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="f0d01-2004">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="f0d01-2005">Interativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2005">Interactive</span></span>

* <span data-ttu-id="f0d01-2006">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="f0d01-2006">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-2007">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-2007">Network</span></span>

* <span data-ttu-id="f0d01-2008">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2008">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="f0d01-2009">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="f0d01-2009">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="f0d01-2010">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2010">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="f0d01-2011">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2011">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="f0d01-2012">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2012">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="f0d01-2013">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="f0d01-2013">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="f0d01-2014">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="f0d01-2014">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="f0d01-2015">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="f0d01-2015">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="f0d01-2016">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2016">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="f0d01-2017">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2017">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="f0d01-2018">Perfil</span><span class="sxs-lookup"><span data-stu-id="f0d01-2018">Profile</span></span>

* <span data-ttu-id="f0d01-2019">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="f0d01-2019">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-2020">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-2020">Resource</span></span>

* <span data-ttu-id="f0d01-2021">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="f0d01-2021">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-2022">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-2022">Storage</span></span>

* <span data-ttu-id="f0d01-2023">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="f0d01-2023">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="f0d01-2024">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="f0d01-2024">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="f0d01-2025">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2025">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="f0d01-2026">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2026">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="f0d01-2027">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="f0d01-2027">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-2028">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-2028">VM</span></span>

* <span data-ttu-id="f0d01-2029">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="f0d01-2029">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="f0d01-2030">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="f0d01-2030">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="f0d01-2031">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="f0d01-2031">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="f0d01-2032">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2032">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="f0d01-2033">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="f0d01-2033">January 17, 2018</span></span>

<span data-ttu-id="f0d01-2034">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="f0d01-2034">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-2035">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-2035">ACR</span></span>

* <span data-ttu-id="f0d01-2036">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="f0d01-2036">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="f0d01-2037">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="f0d01-2037">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-2038">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-2038">ACS</span></span>

* <span data-ttu-id="f0d01-2039">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2039">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="f0d01-2040">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="f0d01-2040">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-2041">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-2041">Appservice</span></span>

* <span data-ttu-id="f0d01-2042">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2042">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="f0d01-2043">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2043">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="f0d01-2044">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2044">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="f0d01-2045">Backup</span><span class="sxs-lookup"><span data-stu-id="f0d01-2045">Backup</span></span>

* <span data-ttu-id="f0d01-2046">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="f0d01-2046">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="f0d01-2047">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2047">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="f0d01-2048">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="f0d01-2048">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="f0d01-2049">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="f0d01-2049">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="f0d01-2050">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="f0d01-2050">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="f0d01-2051">Lote</span><span class="sxs-lookup"><span data-stu-id="f0d01-2051">Batch</span></span>

* <span data-ttu-id="f0d01-2052">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="f0d01-2052">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="f0d01-2053">Nuvem</span><span class="sxs-lookup"><span data-stu-id="f0d01-2053">Cloud</span></span>

* <span data-ttu-id="f0d01-2054">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="f0d01-2054">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="f0d01-2055">Consumo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2055">Consumption</span></span>

* <span data-ttu-id="f0d01-2056">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2056">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="f0d01-2057">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="f0d01-2057">Event Grid</span></span>

* <span data-ttu-id="f0d01-2058">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2058">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="f0d01-2059">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2059">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="f0d01-2060">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2060">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="f0d01-2061">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2061">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="f0d01-2062">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2062">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="f0d01-2063">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2063">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="f0d01-2064">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2064">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="f0d01-2065">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="f0d01-2065">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="f0d01-2066">Interativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2066">Interactive</span></span>

* <span data-ttu-id="f0d01-2067">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="f0d01-2067">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="f0d01-2068">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="f0d01-2068">Fixed errors on startup</span></span>
* <span data-ttu-id="f0d01-2069">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2069">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="f0d01-2070">IoT</span><span class="sxs-lookup"><span data-stu-id="f0d01-2070">IoT</span></span>

* <span data-ttu-id="f0d01-2071">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="f0d01-2071">Added support for device provisioning service</span></span>
* <span data-ttu-id="f0d01-2072">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="f0d01-2072">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="f0d01-2073">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="f0d01-2073">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="f0d01-2074">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f0d01-2074">Monitor</span></span>

* <span data-ttu-id="f0d01-2075">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2075">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="f0d01-2076">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2076">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="f0d01-2077">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="f0d01-2077">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-2078">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-2078">Network</span></span>

* <span data-ttu-id="f0d01-2079">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2079">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="f0d01-2080">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2080">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="f0d01-2081">Perfil</span><span class="sxs-lookup"><span data-stu-id="f0d01-2081">Profile</span></span>

* <span data-ttu-id="f0d01-2082">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="f0d01-2082">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-2083">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-2083">Role</span></span>

* <span data-ttu-id="f0d01-2084">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="f0d01-2084">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f0d01-2085">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f0d01-2085">Service Fabric</span></span>

* <span data-ttu-id="f0d01-2086">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="f0d01-2086">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="f0d01-2087">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="f0d01-2087">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-2088">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-2088">VM</span></span>

* <span data-ttu-id="f0d01-2089">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2089">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="f0d01-2090">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="f0d01-2090">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="f0d01-2091">[ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="f0d01-2091">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="f0d01-2092">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="f0d01-2092">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="f0d01-2093">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="f0d01-2093">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="f0d01-2094">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2094">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="f0d01-2095">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2095">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="f0d01-2096">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2096">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="f0d01-2097">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="f0d01-2097">December 19, 2017</span></span>

<span data-ttu-id="f0d01-2098">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="f0d01-2098">Version 2.0.23</span></span>

* <span data-ttu-id="f0d01-2099">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="f0d01-2099">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="f0d01-2100">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-2100">Container</span></span>

* <span data-ttu-id="f0d01-2101">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-2101">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-2102">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-2102">Network</span></span>

* <span data-ttu-id="f0d01-2103">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2103">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="f0d01-2104">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2104">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-2105">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-2105">Storage</span></span>

* <span data-ttu-id="f0d01-2106">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="f0d01-2106">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-2107">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-2107">VM</span></span>

* <span data-ttu-id="f0d01-2108">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="f0d01-2108">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="f0d01-2109">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="f0d01-2109">December 5, 2017</span></span>

<span data-ttu-id="f0d01-2110">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="f0d01-2110">Version 2.0.22</span></span>

* <span data-ttu-id="f0d01-2111">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2111">Removed `az component` commands.</span></span> <span data-ttu-id="f0d01-2112">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2112">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-2113">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2113">Core</span></span>
* <span data-ttu-id="f0d01-2114">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="f0d01-2114">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="f0d01-2115">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="f0d01-2115">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-2116">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-2116">ACS</span></span>

* <span data-ttu-id="f0d01-2117">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="f0d01-2117">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="f0d01-2118">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2118">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="f0d01-2119">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="f0d01-2119">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="f0d01-2120">Supervisor</span><span class="sxs-lookup"><span data-stu-id="f0d01-2120">Advisor</span></span>

* <span data-ttu-id="f0d01-2121">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="f0d01-2121">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-2122">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-2122">Appservice</span></span>

* <span data-ttu-id="f0d01-2123">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2123">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="f0d01-2124">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="f0d01-2124">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="f0d01-2125">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2125">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="f0d01-2126">Consumo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2126">Consumption</span></span>

* <span data-ttu-id="f0d01-2127">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="f0d01-2127">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="f0d01-2128">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-2128">Container</span></span>

* <span data-ttu-id="f0d01-2129">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="f0d01-2129">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="f0d01-2130">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f0d01-2130">Monitor</span></span>

* <span data-ttu-id="f0d01-2131">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="f0d01-2131">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-2132">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-2132">Resource</span></span>

* <span data-ttu-id="f0d01-2133">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2133">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-2134">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-2134">Role</span></span>

* <span data-ttu-id="f0d01-2135">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2135">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="f0d01-2136">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="f0d01-2136">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="f0d01-2137">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2137">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-2138">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-2138">SQL</span></span>

* <span data-ttu-id="f0d01-2139">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="f0d01-2139">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="f0d01-2140">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="f0d01-2140">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-2141">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-2141">VM</span></span>

* <span data-ttu-id="f0d01-2142">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2142">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="f0d01-2143">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="f0d01-2143">November 14, 2017</span></span>

<span data-ttu-id="f0d01-2144">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="f0d01-2144">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-2145">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-2145">ACR</span></span>

* <span data-ttu-id="f0d01-2146">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="f0d01-2146">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="f0d01-2147">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-2147">ACS</span></span>

* <span data-ttu-id="f0d01-2148">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="f0d01-2148">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="f0d01-2149">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2149">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="f0d01-2150">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2150">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="f0d01-2151">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="f0d01-2151">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="f0d01-2152">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="f0d01-2152">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-2153">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-2153">Appservice</span></span>

* <span data-ttu-id="f0d01-2154">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="f0d01-2154">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="f0d01-2155">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2155">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="f0d01-2156">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2156">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="f0d01-2157">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2157">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="f0d01-2158">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="f0d01-2158">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="f0d01-2159">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2159">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="f0d01-2160">Lote</span><span class="sxs-lookup"><span data-stu-id="f0d01-2160">Batch</span></span>

* <span data-ttu-id="f0d01-2161">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2161">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="f0d01-2162">Batchai</span><span class="sxs-lookup"><span data-stu-id="f0d01-2162">Batchai</span></span>

* <span data-ttu-id="f0d01-2163">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2163">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="f0d01-2164">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2164">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="f0d01-2165">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2165">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="f0d01-2166">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2166">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="f0d01-2167">Nuvem</span><span class="sxs-lookup"><span data-stu-id="f0d01-2167">Cloud</span></span>

* <span data-ttu-id="f0d01-2168">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="f0d01-2168">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="f0d01-2169">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-2169">Container</span></span>

* <span data-ttu-id="f0d01-2170">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="f0d01-2170">Added support to open multiple ports</span></span>
* <span data-ttu-id="f0d01-2171">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="f0d01-2171">Added container group restart policy</span></span>
* <span data-ttu-id="f0d01-2172">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="f0d01-2172">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="f0d01-2173">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="f0d01-2173">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f0d01-2174">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f0d01-2174">Data Lake Analytics</span></span>

* <span data-ttu-id="f0d01-2175">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="f0d01-2175">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f0d01-2176">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f0d01-2176">Data Lake Store</span></span>

* <span data-ttu-id="f0d01-2177">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="f0d01-2177">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="f0d01-2178">Extensão</span><span class="sxs-lookup"><span data-stu-id="f0d01-2178">Extension</span></span>

* <span data-ttu-id="f0d01-2179">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="f0d01-2179">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="f0d01-2180">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="f0d01-2180">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="f0d01-2181">IoT</span><span class="sxs-lookup"><span data-stu-id="f0d01-2181">IoT</span></span>

* <span data-ttu-id="f0d01-2182">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="f0d01-2182">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="f0d01-2183">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f0d01-2183">Monitor</span></span>

* <span data-ttu-id="f0d01-2184">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2184">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-2185">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-2185">Network</span></span>

* <span data-ttu-id="f0d01-2186">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="f0d01-2186">Added support for CAA DNS records</span></span>
* <span data-ttu-id="f0d01-2187">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2187">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="f0d01-2188">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="f0d01-2188">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="f0d01-2189">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2189">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="f0d01-2190">Reservas</span><span class="sxs-lookup"><span data-stu-id="f0d01-2190">Reservations</span></span>

* <span data-ttu-id="f0d01-2191">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="f0d01-2191">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-2192">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-2192">Resource</span></span>

* <span data-ttu-id="f0d01-2193">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-2193">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-2194">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-2194">SQL</span></span>

* <span data-ttu-id="f0d01-2195">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2195">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-2196">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-2196">Storage</span></span>

* <span data-ttu-id="f0d01-2197">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="f0d01-2197">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="f0d01-2198">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="f0d01-2198">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="f0d01-2199">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2199">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="f0d01-2200">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2200">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="f0d01-2201">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2201">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="f0d01-2202">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2202">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="f0d01-2203">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2203">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-2204">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-2204">VM</span></span>

* <span data-ttu-id="f0d01-2205">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2205">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="f0d01-2206">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="f0d01-2206">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="f0d01-2207">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="f0d01-2207">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="f0d01-2208">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2208">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="f0d01-2209">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2209">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="f0d01-2210">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="f0d01-2210">October 24, 2017</span></span>

<span data-ttu-id="f0d01-2211">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="f0d01-2211">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-2212">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2212">Core</span></span>

* <span data-ttu-id="f0d01-2213">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2213">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-2214">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-2214">ACR</span></span>

* <span data-ttu-id="f0d01-2215">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2215">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="f0d01-2216">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="f0d01-2216">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="f0d01-2217">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="f0d01-2217">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-2218">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-2218">ACS</span></span>

* <span data-ttu-id="f0d01-2219">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="f0d01-2219">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="f0d01-2220">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="f0d01-2220">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-2221">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-2221">Appservice</span></span>

* <span data-ttu-id="f0d01-2222">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="f0d01-2222">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="f0d01-2223">Componente</span><span class="sxs-lookup"><span data-stu-id="f0d01-2223">Component</span></span>

* <span data-ttu-id="f0d01-2224">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="f0d01-2224">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="f0d01-2225">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f0d01-2225">Monitor</span></span>

* <span data-ttu-id="f0d01-2226">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2226">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-2227">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-2227">Resource</span></span>

* <span data-ttu-id="f0d01-2228">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2228">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="f0d01-2229">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="f0d01-2229">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-2230">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-2230">VM</span></span>

* <span data-ttu-id="f0d01-2231">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2231">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="f0d01-2232">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="f0d01-2232">October 9, 2017</span></span>

<span data-ttu-id="f0d01-2233">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="f0d01-2233">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-2234">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2234">Core</span></span>

* <span data-ttu-id="f0d01-2235">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="f0d01-2235">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-2236">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-2236">Appservice</span></span>

* <span data-ttu-id="f0d01-2237">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2237">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="f0d01-2238">Lote</span><span class="sxs-lookup"><span data-stu-id="f0d01-2238">Batch</span></span>

* <span data-ttu-id="f0d01-2239">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="f0d01-2239">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="f0d01-2240">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="f0d01-2240">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="f0d01-2241">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="f0d01-2241">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="f0d01-2242">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="f0d01-2242">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="f0d01-2243">Batchai</span><span class="sxs-lookup"><span data-stu-id="f0d01-2243">Batchai</span></span>

* <span data-ttu-id="f0d01-2244">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="f0d01-2244">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="f0d01-2245">Keyvault</span><span class="sxs-lookup"><span data-stu-id="f0d01-2245">Keyvault</span></span>

* <span data-ttu-id="f0d01-2246">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2246">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="f0d01-2247">(#4448)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2247">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="f0d01-2248">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-2248">Network</span></span>

* <span data-ttu-id="f0d01-2249">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="f0d01-2249">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="f0d01-2250">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="f0d01-2250">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-2251">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-2251">Resource</span></span>

* <span data-ttu-id="f0d01-2252">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2252">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="f0d01-2253">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="f0d01-2253">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="f0d01-2254">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2254">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="f0d01-2255">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-2255">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-2256">Sql</span><span class="sxs-lookup"><span data-stu-id="f0d01-2256">Sql</span></span>

* <span data-ttu-id="f0d01-2257">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="f0d01-2257">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="f0d01-2258">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="f0d01-2258">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="f0d01-2259">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="f0d01-2259">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-2260">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-2260">Storage</span></span>

* <span data-ttu-id="f0d01-2261">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="f0d01-2261">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-2262">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-2262">Vm</span></span>

* <span data-ttu-id="f0d01-2263">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="f0d01-2263">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="f0d01-2264">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2264">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="f0d01-2265">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2265">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="f0d01-2266">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2266">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="f0d01-2267">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2267">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="f0d01-2268">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="f0d01-2268">September 22, 2017</span></span>

<span data-ttu-id="f0d01-2269">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="f0d01-2269">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-2270">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-2270">Resource</span></span>

* <span data-ttu-id="f0d01-2271">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="f0d01-2271">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="f0d01-2272">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="f0d01-2272">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="f0d01-2273">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2273">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="f0d01-2274">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2274">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-2275">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-2275">Network</span></span>

* <span data-ttu-id="f0d01-2276">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2276">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="f0d01-2277">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2277">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="f0d01-2278">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2278">Added `asg` application security group commands</span></span>
* <span data-ttu-id="f0d01-2279">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2279">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="f0d01-2280">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2280">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="f0d01-2281">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2281">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="f0d01-2282">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2282">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-2283">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-2283">Storage</span></span>

* <span data-ttu-id="f0d01-2284">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="f0d01-2284">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="f0d01-2285">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="f0d01-2285">Eventgrid</span></span>

* <span data-ttu-id="f0d01-2286">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="f0d01-2286">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-2287">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-2287">SQL</span></span>

* <span data-ttu-id="f0d01-2288">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2288">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="f0d01-2289">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="f0d01-2289">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="f0d01-2290">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2290">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="f0d01-2291">Keyvault</span><span class="sxs-lookup"><span data-stu-id="f0d01-2291">Keyvault</span></span>

* <span data-ttu-id="f0d01-2292">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="f0d01-2292">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-2293">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-2293">VM</span></span>

* <span data-ttu-id="f0d01-2294">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2294">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="f0d01-2295">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="f0d01-2295">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="f0d01-2296">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2296">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="f0d01-2297">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2297">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="f0d01-2298">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2298">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="f0d01-2299">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2299">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-2300">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-2300">ACS</span></span>

* <span data-ttu-id="f0d01-2301">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-2301">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-2302">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-2302">Appservice</span></span>

* <span data-ttu-id="f0d01-2303">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2303">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="f0d01-2304">Backup</span><span class="sxs-lookup"><span data-stu-id="f0d01-2304">Backup</span></span>

* <span data-ttu-id="f0d01-2305">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="f0d01-2305">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="f0d01-2306">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="f0d01-2306">September 11, 2017</span></span>

<span data-ttu-id="f0d01-2307">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="f0d01-2307">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="f0d01-2308">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2308">Core</span></span>

* <span data-ttu-id="f0d01-2309">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="f0d01-2309">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="f0d01-2310">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="f0d01-2310">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-2311">Acs</span><span class="sxs-lookup"><span data-stu-id="f0d01-2311">Acs</span></span>

* <span data-ttu-id="f0d01-2312">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2312">Added `acs list-locations` command</span></span>
* <span data-ttu-id="f0d01-2313">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="f0d01-2313">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-2314">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-2314">Appservice</span></span>

* <span data-ttu-id="f0d01-2315">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2315">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="f0d01-2316">CDN</span><span class="sxs-lookup"><span data-stu-id="f0d01-2316">CDN</span></span>

* <span data-ttu-id="f0d01-2317">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2317">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="f0d01-2318">Extensão</span><span class="sxs-lookup"><span data-stu-id="f0d01-2318">Extension</span></span>

* <span data-ttu-id="f0d01-2319">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="f0d01-2319">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="f0d01-2320">Keyvault</span><span class="sxs-lookup"><span data-stu-id="f0d01-2320">Keyvault</span></span>

* <span data-ttu-id="f0d01-2321">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2321">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-2322">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-2322">Network</span></span>

* <span data-ttu-id="f0d01-2323">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2323">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="f0d01-2324">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2324">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="f0d01-2325">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2325">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="f0d01-2326">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2326">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="f0d01-2327">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2327">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-2328">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-2328">Resource</span></span>

* <span data-ttu-id="f0d01-2329">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2329">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="f0d01-2330">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2330">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="f0d01-2331">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="f0d01-2331">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="f0d01-2332">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="f0d01-2332">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-2333">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-2333">SQL</span></span>

* <span data-ttu-id="f0d01-2334">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2334">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-2335">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-2335">VM</span></span>

* <span data-ttu-id="f0d01-2336">Corrigido: não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="f0d01-2336">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="f0d01-2337">Corrigido: usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="f0d01-2337">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="f0d01-2338">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2338">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="f0d01-2339">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="f0d01-2339">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="f0d01-2340">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="f0d01-2340">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="f0d01-2341">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="f0d01-2341">August 31, 2017</span></span>

<span data-ttu-id="f0d01-2342">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="f0d01-2342">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="f0d01-2343">Keyvault</span><span class="sxs-lookup"><span data-stu-id="f0d01-2343">Keyvault</span></span>

* <span data-ttu-id="f0d01-2344">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2344">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="f0d01-2345">Sf</span><span class="sxs-lookup"><span data-stu-id="f0d01-2345">Sf</span></span>

* <span data-ttu-id="f0d01-2346">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2346">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-2347">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-2347">Storage</span></span>

* <span data-ttu-id="f0d01-2348">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="f0d01-2348">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="f0d01-2349">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="f0d01-2349">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="f0d01-2350">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="f0d01-2350">August 28, 2017</span></span>

<span data-ttu-id="f0d01-2351">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="f0d01-2351">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="f0d01-2352">CLI</span><span class="sxs-lookup"><span data-stu-id="f0d01-2352">CLI</span></span>

* <span data-ttu-id="f0d01-2353">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2353">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-2354">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-2354">ACS</span></span>

* <span data-ttu-id="f0d01-2355">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="f0d01-2355">Corrected preview regions</span></span>
* <span data-ttu-id="f0d01-2356">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2356">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="f0d01-2357">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="f0d01-2357">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-2358">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-2358">Appservice</span></span>

* <span data-ttu-id="f0d01-2359">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2359">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="f0d01-2360">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2360">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="f0d01-2361">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2361">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="f0d01-2362">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2362">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="f0d01-2363">Corrigido: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="f0d01-2363">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="f0d01-2364">IoT</span><span class="sxs-lookup"><span data-stu-id="f0d01-2364">IoT</span></span>

* <span data-ttu-id="f0d01-2365">Corrigido #3934: a criação de uma política não limpa mais as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="f0d01-2365">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-2366">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-2366">Network</span></span>

* <span data-ttu-id="f0d01-2367">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2367">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="f0d01-2368">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2368">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="f0d01-2369">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2369">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="f0d01-2370">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2370">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="f0d01-2371">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2371">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="f0d01-2372">Perfil</span><span class="sxs-lookup"><span data-stu-id="f0d01-2372">Profile</span></span>

* <span data-ttu-id="f0d01-2373">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="f0d01-2373">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f0d01-2374">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f0d01-2374">Service Fabric</span></span>

* <span data-ttu-id="f0d01-2375">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="f0d01-2375">Preview release</span></span>
* <span data-ttu-id="f0d01-2376">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="f0d01-2376">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="f0d01-2377">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="f0d01-2377">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="f0d01-2378">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="f0d01-2378">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-2379">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-2379">Storage</span></span>

* <span data-ttu-id="f0d01-2380">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="f0d01-2380">Enabled setting blob tier</span></span>
* <span data-ttu-id="f0d01-2381">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="f0d01-2381">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="f0d01-2382">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="f0d01-2382">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="f0d01-2383">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="f0d01-2383">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="f0d01-2384">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2384">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="f0d01-2385">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="f0d01-2385">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-2386">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-2386">VM</span></span>

* <span data-ttu-id="f0d01-2387">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2387">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="f0d01-2388">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="f0d01-2388">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="f0d01-2389">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2389">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="f0d01-2390">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="f0d01-2390">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="f0d01-2391">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="f0d01-2391">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="f0d01-2392">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2392">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="f0d01-2393">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="f0d01-2393">August 15, 2017</span></span>

<span data-ttu-id="f0d01-2394">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="f0d01-2394">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-2395">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-2395">ACS</span></span>

* <span data-ttu-id="f0d01-2396">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="f0d01-2396">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-2397">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-2397">Appservice</span></span>

* <span data-ttu-id="f0d01-2398">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="f0d01-2398">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="f0d01-2399">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="f0d01-2399">Event Grid</span></span>

* <span data-ttu-id="f0d01-2400">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="f0d01-2400">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="f0d01-2401">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="f0d01-2401">August 11, 2017</span></span>

<span data-ttu-id="f0d01-2402">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="f0d01-2402">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-2403">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-2403">ACS</span></span>

* <span data-ttu-id="f0d01-2404">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="f0d01-2404">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="f0d01-2405">Lote</span><span class="sxs-lookup"><span data-stu-id="f0d01-2405">Batch</span></span>

* <span data-ttu-id="f0d01-2406">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="f0d01-2406">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="f0d01-2407">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="f0d01-2407">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="f0d01-2408">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-2408">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="f0d01-2409">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://”</span><span class="sxs-lookup"><span data-stu-id="f0d01-2409">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="f0d01-2410">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="f0d01-2410">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="f0d01-2411">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="f0d01-2411">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="f0d01-2412">Componente</span><span class="sxs-lookup"><span data-stu-id="f0d01-2412">Component</span></span>

* <span data-ttu-id="f0d01-2413">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="f0d01-2413">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="f0d01-2414">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-2414">Container</span></span>

* <span data-ttu-id="f0d01-2415">`create`: corrigido o problema em que o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="f0d01-2415">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="f0d01-2416">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f0d01-2416">Data Lake Store</span></span>

* <span data-ttu-id="f0d01-2417">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-2417">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="f0d01-2418">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="f0d01-2418">Event Grid</span></span>

* <span data-ttu-id="f0d01-2419">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="f0d01-2419">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-2420">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-2420">Network</span></span>

* <span data-ttu-id="f0d01-2421">`lb`: corrigido o problema em que os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="f0d01-2421">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="f0d01-2422">`application-gateway {subresource} delete`: corrigido o problema em que `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="f0d01-2422">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="f0d01-2423">`application-gateway http-settings update`: corrigido o problema em que `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="f0d01-2423">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="f0d01-2424">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2424">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="f0d01-2425">Perfil</span><span class="sxs-lookup"><span data-stu-id="f0d01-2425">Profile</span></span>

* <span data-ttu-id="f0d01-2426">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="f0d01-2426">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-2427">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-2427">Storage</span></span>

* <span data-ttu-id="f0d01-2428">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="f0d01-2428">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-2429">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-2429">VM</span></span>

* <span data-ttu-id="f0d01-2430">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="f0d01-2430">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="f0d01-2431">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2431">Exposed `list-skus` command</span></span>
* <span data-ttu-id="f0d01-2432">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="f0d01-2432">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="f0d01-2433">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="f0d01-2433">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="f0d01-2434">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="f0d01-2434">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="f0d01-2435">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="f0d01-2435">July 28, 2017</span></span>

<span data-ttu-id="f0d01-2436">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="f0d01-2436">Version 2.0.12</span></span>

* <span data-ttu-id="f0d01-2437">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-2437">Added container commands</span></span>
* <span data-ttu-id="f0d01-2438">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2438">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="f0d01-2439">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2439">Core</span></span>

* <span data-ttu-id="f0d01-2440">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="f0d01-2440">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="f0d01-2441">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="f0d01-2441">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="f0d01-2442">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="f0d01-2442">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="f0d01-2443">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2443">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="f0d01-2444">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="f0d01-2444">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="f0d01-2445">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2445">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="f0d01-2446">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2446">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="f0d01-2447">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2447">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="f0d01-2448">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2448">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="f0d01-2449">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="f0d01-2449">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="f0d01-2450">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="f0d01-2450">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="f0d01-2451">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2451">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="f0d01-2452">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="f0d01-2452">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="f0d01-2453">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="f0d01-2453">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="f0d01-2454">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="f0d01-2454">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="f0d01-2455">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2455">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="f0d01-2456">ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-2456">ACR</span></span>

* <span data-ttu-id="f0d01-2457">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="f0d01-2457">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="f0d01-2458">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="f0d01-2458">Support SKU update for managed registries</span></span>
* <span data-ttu-id="f0d01-2459">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="f0d01-2459">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="f0d01-2460">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-2460">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="f0d01-2461">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-2461">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="f0d01-2462">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="f0d01-2462">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-2463">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-2463">ACS</span></span>

* <span data-ttu-id="f0d01-2464">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="f0d01-2464">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-2465">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-2465">Appservice</span></span>

* <span data-ttu-id="f0d01-2466">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="f0d01-2466">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="f0d01-2467">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="f0d01-2467">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="f0d01-2468">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2468">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="f0d01-2469">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2469">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="f0d01-2470">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2470">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="f0d01-2471">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2471">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="f0d01-2472">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2472">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="f0d01-2473">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2473">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="f0d01-2474">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2474">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="f0d01-2475">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2475">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="f0d01-2476">Lote</span><span class="sxs-lookup"><span data-stu-id="f0d01-2476">Batch</span></span>

* <span data-ttu-id="f0d01-2477">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="f0d01-2477">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="f0d01-2478">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2478">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="f0d01-2479">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2479">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="f0d01-2480">CDN</span><span class="sxs-lookup"><span data-stu-id="f0d01-2480">CDN</span></span>

* <span data-ttu-id="f0d01-2481">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="f0d01-2481">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="f0d01-2482">Nuvem</span><span class="sxs-lookup"><span data-stu-id="f0d01-2482">Cloud</span></span>

* <span data-ttu-id="f0d01-2483">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="f0d01-2483">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="f0d01-2484">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="f0d01-2484">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="f0d01-2485">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="f0d01-2485">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="f0d01-2486">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="f0d01-2486">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="f0d01-2487">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2487">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f0d01-2488">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f0d01-2488">CosmosDB</span></span>

* <span data-ttu-id="f0d01-2489">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="f0d01-2489">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="f0d01-2490">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="f0d01-2490">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f0d01-2491">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f0d01-2491">Data Lake Analytics</span></span>

* <span data-ttu-id="f0d01-2492">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2492">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="f0d01-2493">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2493">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="f0d01-2494">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2494">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f0d01-2495">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f0d01-2495">Data Lake Store</span></span>

* <span data-ttu-id="f0d01-2496">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2496">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="f0d01-2497">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="f0d01-2497">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="f0d01-2498">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2498">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="f0d01-2499">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f0d01-2499">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="f0d01-2500">Interativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2500">Interactive</span></span>

* <span data-ttu-id="f0d01-2501">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="f0d01-2501">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="f0d01-2502">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="f0d01-2502">Increased test coverage</span></span>
* <span data-ttu-id="f0d01-2503">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="f0d01-2503">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="f0d01-2504">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2504">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="f0d01-2505">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2505">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="f0d01-2506">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2506">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="f0d01-2507">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2507">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="f0d01-2508">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2508">Added `--progress` flag</span></span>
* <span data-ttu-id="f0d01-2509">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="f0d01-2509">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="f0d01-2510">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2510">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="f0d01-2511">IoT</span><span class="sxs-lookup"><span data-stu-id="f0d01-2511">IoT</span></span>

* <span data-ttu-id="f0d01-2512">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2512">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="f0d01-2513">(#3934)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2513">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="f0d01-2514">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="f0d01-2514">Key vault</span></span>

* <span data-ttu-id="f0d01-2515">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="f0d01-2515">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="f0d01-2516">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2516">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="f0d01-2517">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2517">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="f0d01-2518">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2518">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="f0d01-2519">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2519">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="f0d01-2520">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2520">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="f0d01-2521">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2521">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="f0d01-2522">(#3307)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2522">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="f0d01-2523">Laboratório</span><span class="sxs-lookup"><span data-stu-id="f0d01-2523">Lab</span></span>

* <span data-ttu-id="f0d01-2524">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2524">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="f0d01-2525">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2525">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="f0d01-2526">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f0d01-2526">Monitor</span></span>

* <span data-ttu-id="f0d01-2527">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2527">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="f0d01-2528">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2528">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="f0d01-2529">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2529">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="f0d01-2530">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2530">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="f0d01-2531">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2531">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="f0d01-2532">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="f0d01-2532">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="f0d01-2533">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="f0d01-2533">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="f0d01-2534">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="f0d01-2534">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="f0d01-2535">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="f0d01-2535">`location` no longer required</span></span>
  * <span data-ttu-id="f0d01-2536">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="f0d01-2536">Add name and ID support for target</span></span>
  * <span data-ttu-id="f0d01-2537">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2537">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="f0d01-2538">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="f0d01-2538">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="f0d01-2539">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="f0d01-2539">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="f0d01-2540">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="f0d01-2540">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="f0d01-2541">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2541">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="f0d01-2542">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2542">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-2543">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-2543">Network</span></span>

* <span data-ttu-id="f0d01-2544">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2544">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="f0d01-2545">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2545">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="f0d01-2546">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="f0d01-2546">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="f0d01-2547">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="f0d01-2547">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="f0d01-2548">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2548">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="f0d01-2549">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2549">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="f0d01-2550">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2550">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="f0d01-2551">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2551">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="f0d01-2552">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2552">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="f0d01-2553">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2553">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="f0d01-2554">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2554">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="f0d01-2555">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2555">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="f0d01-2556">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2556">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="f0d01-2557">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2557">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="f0d01-2558">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2558">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="f0d01-2559">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2559">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="f0d01-2560">Adicionado o suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para --dns-servers</span><span class="sxs-lookup"><span data-stu-id="f0d01-2560">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="f0d01-2561">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2561">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="f0d01-2562">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2562">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="f0d01-2563">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2563">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="f0d01-2564">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2564">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="f0d01-2565">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2565">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="f0d01-2566">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2566">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="f0d01-2567">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="f0d01-2567">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="f0d01-2568">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="f0d01-2568">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="f0d01-2569">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="f0d01-2569">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="f0d01-2570">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="f0d01-2570">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="f0d01-2571">Perfil</span><span class="sxs-lookup"><span data-stu-id="f0d01-2571">Profile</span></span>

* <span data-ttu-id="f0d01-2572">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="f0d01-2572">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="f0d01-2573">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="f0d01-2573">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="f0d01-2574">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="f0d01-2574">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="f0d01-2575">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="f0d01-2575">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="f0d01-2576">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="f0d01-2576">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="f0d01-2577">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f0d01-2577">RDBMS</span></span>

* <span data-ttu-id="f0d01-2578">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2578">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="f0d01-2579">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2579">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="f0d01-2580">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2580">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="f0d01-2581">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2581">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-2582">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-2582">Resource</span></span>

* <span data-ttu-id="f0d01-2583">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2583">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="f0d01-2584">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2584">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="f0d01-2585">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2585">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="f0d01-2586">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2586">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="f0d01-2587">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2587">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="f0d01-2588">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2588">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="f0d01-2589">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2589">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="f0d01-2590">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2590">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-2591">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-2591">Role</span></span>

* <span data-ttu-id="f0d01-2592">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2592">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="f0d01-2593">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2593">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="f0d01-2594">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2594">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="f0d01-2595">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2595">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="f0d01-2596">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2596">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f0d01-2597">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f0d01-2597">Service Fabric</span></span>
* <span data-ttu-id="f0d01-2598">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2598">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="f0d01-2599">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2599">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="f0d01-2600">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2600">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-2601">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-2601">SQL</span></span>

* <span data-ttu-id="f0d01-2602">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2602">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="f0d01-2603">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2603">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="f0d01-2604">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2604">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-2605">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-2605">Storage</span></span>

* <span data-ttu-id="f0d01-2606">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2606">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="f0d01-2607">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="f0d01-2607">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="f0d01-2608">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2608">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="f0d01-2609">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2609">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="f0d01-2610">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2610">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="f0d01-2611">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2611">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-2612">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-2612">VM</span></span>

* <span data-ttu-id="f0d01-2613">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="f0d01-2613">Support configuring nsg</span></span>
* <span data-ttu-id="f0d01-2614">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="f0d01-2614">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="f0d01-2615">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="f0d01-2615">Support managed service identities</span></span>
* <span data-ttu-id="f0d01-2616">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2616">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="f0d01-2617">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="f0d01-2617">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="f0d01-2618">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="f0d01-2618">May 10, 2017</span></span>

<span data-ttu-id="f0d01-2619">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="f0d01-2619">Version 2.0.6</span></span>

* <span data-ttu-id="f0d01-2620">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f0d01-2620">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="f0d01-2621">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2621">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="f0d01-2622">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f0d01-2622">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="f0d01-2623">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="f0d01-2623">Include Cognitive Services module</span></span>
* <span data-ttu-id="f0d01-2624">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f0d01-2624">Include Service Fabric module</span></span>
* <span data-ttu-id="f0d01-2625">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2625">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="f0d01-2626">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="f0d01-2626">Add support for CDN commands</span></span>
* <span data-ttu-id="f0d01-2627">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="f0d01-2627">Remove Container module</span></span>
* <span data-ttu-id="f0d01-2628">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2628">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="f0d01-2629">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2629">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="f0d01-2630">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2630">Core</span></span>

* <span data-ttu-id="f0d01-2631">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="f0d01-2631">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="f0d01-2632">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2632">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="f0d01-2633">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2633">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="f0d01-2634">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2634">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="f0d01-2635">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2635">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="f0d01-2636">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2636">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="f0d01-2637">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2637">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="f0d01-2638">núcleo: permitir que o caminho do arquivo accessTokens.json seja configurável por meio de uma variável de ambiente ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2638">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="f0d01-2639">núcleo: permitir que padrões configurados sejam aplicados em argumentos opcionais ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2639">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="f0d01-2640">núcleo: desempenho aprimorado</span><span class="sxs-lookup"><span data-stu-id="f0d01-2640">core: Improved performance</span></span>
* <span data-ttu-id="f0d01-2641">núcleo: certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="f0d01-2641">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="f0d01-2642">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="f0d01-2642">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-2643">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-2643">ACS</span></span>

* <span data-ttu-id="f0d01-2644">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0d01-2644">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="f0d01-2645">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="f0d01-2645">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="f0d01-2646">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="f0d01-2646">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="f0d01-2647">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2647">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-2648">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-2648">AppService</span></span>

* <span data-ttu-id="f0d01-2649">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2649">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="f0d01-2650">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="f0d01-2650">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="f0d01-2651">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2651">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="f0d01-2652">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="f0d01-2652">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="f0d01-2653">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="f0d01-2653">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="f0d01-2654">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2654">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="f0d01-2655">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="f0d01-2655">support slot swap with preview</span></span>
* <span data-ttu-id="f0d01-2656">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2656">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="f0d01-2657">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2657">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f0d01-2658">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f0d01-2658">CosmosDB</span></span>

* <span data-ttu-id="f0d01-2659">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f0d01-2659">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="f0d01-2660">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="f0d01-2660">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="f0d01-2661">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="f0d01-2661">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="f0d01-2662">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="f0d01-2662">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f0d01-2663">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f0d01-2663">Data Lake Analytics</span></span>

* <span data-ttu-id="f0d01-2664">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="f0d01-2664">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="f0d01-2665">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2665">Add support for new catalog item type: package.</span></span> <span data-ttu-id="f0d01-2666">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2666">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="f0d01-2667">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="f0d01-2667">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="f0d01-2668">Tabela</span><span class="sxs-lookup"><span data-stu-id="f0d01-2668">Table</span></span>
  * <span data-ttu-id="f0d01-2669">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="f0d01-2669">Table valued function</span></span>
  * <span data-ttu-id="f0d01-2670">Visualizar</span><span class="sxs-lookup"><span data-stu-id="f0d01-2670">View</span></span>
  * <span data-ttu-id="f0d01-2671">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2671">Table Statistics.</span></span> <span data-ttu-id="f0d01-2672">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="f0d01-2672">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f0d01-2673">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f0d01-2673">Data Lake Store</span></span>

* <span data-ttu-id="f0d01-2674">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="f0d01-2674">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="f0d01-2675">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2675">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="f0d01-2676">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2676">missed help for access show.</span></span> <span data-ttu-id="f0d01-2677">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2677">adding it.</span></span> <span data-ttu-id="f0d01-2678">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2678">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="f0d01-2679">Localizar</span><span class="sxs-lookup"><span data-stu-id="f0d01-2679">Find</span></span>

* <span data-ttu-id="f0d01-2680">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="f0d01-2680">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="f0d01-2681">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f0d01-2681">KeyVault</span></span>

* <span data-ttu-id="f0d01-2682">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="f0d01-2682">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="f0d01-2683">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois estes parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="f0d01-2683">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="f0d01-2684">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="f0d01-2684">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="f0d01-2685">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="f0d01-2685">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="f0d01-2686">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2686">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="f0d01-2687">Laboratório</span><span class="sxs-lookup"><span data-stu-id="f0d01-2687">Lab</span></span>

* <span data-ttu-id="f0d01-2688">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="f0d01-2688">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="f0d01-2689">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="f0d01-2689">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="f0d01-2690">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="f0d01-2690">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="f0d01-2691">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="f0d01-2691">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="f0d01-2692">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="f0d01-2692">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="f0d01-2693">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f0d01-2693">Monitor</span></span>

* <span data-ttu-id="f0d01-2694">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2694">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="f0d01-2695">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2695">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="f0d01-2696">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-2696">Network</span></span>

* <span data-ttu-id="f0d01-2697">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2697">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="f0d01-2698">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2698">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="f0d01-2699">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2699">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="f0d01-2700">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2700">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="f0d01-2701">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="f0d01-2701">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="f0d01-2702">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="f0d01-2702">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="f0d01-2703">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="f0d01-2703">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="f0d01-2704">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="f0d01-2704">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="f0d01-2705">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2705">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="f0d01-2706">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="f0d01-2706">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="f0d01-2707">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2707">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="f0d01-2708">BC: corrigido um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2708">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="f0d01-2709">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="f0d01-2709">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="f0d01-2710">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="f0d01-2710">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="f0d01-2711">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="f0d01-2711">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="f0d01-2712">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="f0d01-2712">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="f0d01-2713">Perfil</span><span class="sxs-lookup"><span data-stu-id="f0d01-2713">Profile</span></span>

* <span data-ttu-id="f0d01-2714">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2714">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="f0d01-2715">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2715">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="f0d01-2716">Redis</span><span class="sxs-lookup"><span data-stu-id="f0d01-2716">Redis</span></span>

* <span data-ttu-id="f0d01-2717">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="f0d01-2717">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="f0d01-2718">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="f0d01-2718">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="f0d01-2719">Recurso</span><span class="sxs-lookup"><span data-stu-id="f0d01-2719">Resource</span></span>

* <span data-ttu-id="f0d01-2720">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2720">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="f0d01-2721">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2721">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="f0d01-2722">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2722">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="f0d01-2723">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2723">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="f0d01-2724">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2724">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="f0d01-2725">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2725">Add docs for az lock update.</span></span> <span data-ttu-id="f0d01-2726">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2726">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="f0d01-2727">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2727">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="f0d01-2728">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2728">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="f0d01-2729">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2729">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="f0d01-2730">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2730">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="f0d01-2731">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2731">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="f0d01-2732">Função</span><span class="sxs-lookup"><span data-stu-id="f0d01-2732">Role</span></span>

* <span data-ttu-id="f0d01-2733">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2733">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="f0d01-2734">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2734">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="f0d01-2735">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2735">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="f0d01-2736">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="f0d01-2736">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="f0d01-2737">SQL</span><span class="sxs-lookup"><span data-stu-id="f0d01-2737">SQL</span></span>

* <span data-ttu-id="f0d01-2738">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="f0d01-2738">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="f0d01-2739">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2739">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="f0d01-2740">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-2740">Storage</span></span>

* <span data-ttu-id="f0d01-2741">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2741">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="f0d01-2742">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="f0d01-2742">Add support for incremental blob copy</span></span>
* <span data-ttu-id="f0d01-2743">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="f0d01-2743">Add support for large block blob upload</span></span>
* <span data-ttu-id="f0d01-2744">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="f0d01-2744">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-2745">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-2745">VM</span></span>

* <span data-ttu-id="f0d01-2746">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="f0d01-2746">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="f0d01-2747">observação: em comandos da VM em nuvens soberanas, evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="f0d01-2747">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="f0d01-2748">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="f0d01-2748">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="f0d01-2749">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="f0d01-2749">az vm/vmss disk</span></span>
  3. <span data-ttu-id="f0d01-2750">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="f0d01-2750">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="f0d01-2751">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="f0d01-2751">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="f0d01-2752">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2752">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="f0d01-2753">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="f0d01-2753">April 3, 2017</span></span>

<span data-ttu-id="f0d01-2754">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="f0d01-2754">Version 2.0.2</span></span>

<span data-ttu-id="f0d01-2755">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="f0d01-2755">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="f0d01-2756">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f0d01-2756">Core</span></span>

* <span data-ttu-id="f0d01-2757">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="f0d01-2757">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="f0d01-2758">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2758">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="f0d01-2759">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2759">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="f0d01-2760">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2760">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="f0d01-2761">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2761">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="f0d01-2762">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2762">Add prompting for missing template parameters.</span></span> <span data-ttu-id="f0d01-2763">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2763">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="f0d01-2764">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="f0d01-2764">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="f0d01-2765">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="f0d01-2765">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="f0d01-2766">ACS</span><span class="sxs-lookup"><span data-stu-id="f0d01-2766">ACS</span></span>

* <span data-ttu-id="f0d01-2767">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2767">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="f0d01-2768">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2768">Add support for ssh key password prompting.</span></span> <span data-ttu-id="f0d01-2769">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2769">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="f0d01-2770">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2770">Add support for windows clusters.</span></span> <span data-ttu-id="f0d01-2771">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2771">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="f0d01-2772">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="f0d01-2772">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="f0d01-2773">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2773">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="f0d01-2774">AppService</span><span class="sxs-lookup"><span data-stu-id="f0d01-2774">AppService</span></span>

* <span data-ttu-id="f0d01-2775">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2775">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="f0d01-2776">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2776">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="f0d01-2777">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2777">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="f0d01-2778">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2778">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="f0d01-2779">DataLake</span><span class="sxs-lookup"><span data-stu-id="f0d01-2779">DataLake</span></span>

* <span data-ttu-id="f0d01-2780">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f0d01-2780">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="f0d01-2781">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f0d01-2781">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="f0d01-2782">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="f0d01-2782">DocuemntDB</span></span>

* <span data-ttu-id="f0d01-2783">DocumentDB: adicionado suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2783">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="f0d01-2784">VM</span><span class="sxs-lookup"><span data-stu-id="f0d01-2784">VM</span></span>

* <span data-ttu-id="f0d01-2785">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2785">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="f0d01-2786">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2786">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="f0d01-2787">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2787">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="f0d01-2788">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2788">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="f0d01-2789">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2789">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="f0d01-2790">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2790">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="f0d01-2791">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="f0d01-2791">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="f0d01-2792">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="f0d01-2792">February 27, 2017</span></span>

<span data-ttu-id="f0d01-2793">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="f0d01-2793">Version 2.0.0</span></span>

<span data-ttu-id="f0d01-2794">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="f0d01-2794">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="f0d01-2795">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2795">Container Service (acs)</span></span>
- <span data-ttu-id="f0d01-2796">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2796">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="f0d01-2797">Rede</span><span class="sxs-lookup"><span data-stu-id="f0d01-2797">Networking</span></span>
- <span data-ttu-id="f0d01-2798">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f0d01-2798">Storage</span></span>

<span data-ttu-id="f0d01-2799">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2799">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="f0d01-2800">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="f0d01-2800">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="f0d01-2801">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="f0d01-2801">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="f0d01-2802">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="f0d01-2802">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="f0d01-2803">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2803">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="f0d01-2804">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="f0d01-2804">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="f0d01-2805">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2805">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="f0d01-2806">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="f0d01-2806">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="f0d01-2807">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="f0d01-2807">Provide feedback from the command line with the `az feedback` command</span></span>

