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
ms.openlocfilehash: 1f829ba3d9ecdb158e96512bde5bcf1565cc205c
ms.sourcegitcommit: 5b9b4446c08b94256ced7f63c145b493ba8b50df
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2019
ms.locfileid: "71217419"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="82786-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="82786-103">Azure CLI release notes</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="82786-104">24 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-104">September 24, 2019</span></span>

<span data-ttu-id="82786-105">Versão 2.0.74</span><span class="sxs-lookup"><span data-stu-id="82786-105">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="82786-106">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-106">ACR</span></span>

* <span data-ttu-id="82786-107">Inclusão de um parâmetro `--type` obrigatório em `acr config retention update`</span><span class="sxs-lookup"><span data-stu-id="82786-107">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="82786-108">[ALTERAÇÃO DE FALHA] O parâmetro renomeado `--name -n` foi alterado para `--registry -r ` para o grupo de comando `acr config`</span><span class="sxs-lookup"><span data-stu-id="82786-108">[BREAKING CHNAGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="82786-109">AKS</span><span class="sxs-lookup"><span data-stu-id="82786-109">AKS</span></span>

* <span data-ttu-id="82786-110">Inclusão do parâmetro `--load-balancer-sku` no comando `aks create`, o que permite criar um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="82786-110">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="82786-111">Inclusão dos parâmetros `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` e `--load-balancer-outbound-ip-prefixes` nos comandos `aks [create|update]`, o que permite atualizar o perfil do balanceador de carga de um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="82786-111">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="82786-112">Inclusão do parâmetro `--vm-set-type` no comando `aks create`, o que permite especificar os tipos de VM de um cluster do AKS (vmas ou vmss)</span><span class="sxs-lookup"><span data-stu-id="82786-112">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="82786-113">ARM</span><span class="sxs-lookup"><span data-stu-id="82786-113">ARM</span></span>

* <span data-ttu-id="82786-114">Inclusão do parâmetro `--handle-extended-json-format` no comando `group deployment create` para compatibilidade com várias linhas e comentários no modelo JSON</span><span class="sxs-lookup"><span data-stu-id="82786-114">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="82786-115">Computação</span><span class="sxs-lookup"><span data-stu-id="82786-115">Compute</span></span>

* <span data-ttu-id="82786-116">Inclusão do parâmetro `--terminate-notification-time` nos comandos `vmss [create|update]` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="82786-116">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="82786-117">Inclusão do parâmetro `--enable-terminate-notification` no comando `vmss update` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="82786-117">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="82786-118">Inclusão dos parâmetros `--priority,`, `--eviction-policy,` e `--max-billing` nos comandos `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="82786-118">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="82786-119">Alteração de `disk create` para permitir a especificação do tamanho exato do carregamento de disco</span><span class="sxs-lookup"><span data-stu-id="82786-119">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="82786-120">Inclusão de compatibilidade com instantâneos incrementais para discos gerenciados para `snapshot create`</span><span class="sxs-lookup"><span data-stu-id="82786-120">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="82786-121">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82786-121">Cosmos DB</span></span>

* <span data-ttu-id="82786-122">Inclusão do parâmetro `--type <key-type>` no comando `cosmosdb keys list` para mostrar a chave, as chaves somente leitura ou cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="82786-122">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="82786-123">Adicionado o comando `cosmosdb keys regenerate`</span><span class="sxs-lookup"><span data-stu-id="82786-123">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="82786-124">[PRETERIDO] Comandos `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` e `cosmosdb list-read-only-keys` preteridos</span><span class="sxs-lookup"><span data-stu-id="82786-124">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="82786-125">EventGrid</span><span class="sxs-lookup"><span data-stu-id="82786-125">EventGrid</span></span>

* <span data-ttu-id="82786-126">Correção do texto de ajuda do ponto de extremidade para fazer referência ao parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="82786-126">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="82786-127">Key Vault</span><span class="sxs-lookup"><span data-stu-id="82786-127">Key Vault</span></span>

* <span data-ttu-id="82786-128">Correção do problema em que fazer logon com um locatário (`login -t`) poderia causar uma falha no `keyvault create`</span><span class="sxs-lookup"><span data-stu-id="82786-128">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="82786-129">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="82786-129">Monitor</span></span>

* <span data-ttu-id="82786-130">Correção do problema em que o caractere `:` não era permitido no argumento `--condition` para `monitor metrics alert create`</span><span class="sxs-lookup"><span data-stu-id="82786-130">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="82786-131">Política</span><span class="sxs-lookup"><span data-stu-id="82786-131">Policy</span></span>

* <span data-ttu-id="82786-132">Inclusão de compatibilidade com a API de Política, versão de 01/06/2019</span><span class="sxs-lookup"><span data-stu-id="82786-132">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="82786-133">Inclusão do parâmetro `--enforcement-mode` no comando `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="82786-133">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="82786-134">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-134">Storage</span></span>

* <span data-ttu-id="82786-135">Inclusão do parâmetro `--blob-type` no comando `az storage copy`</span><span class="sxs-lookup"><span data-stu-id="82786-135">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="82786-136">10 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-136">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="82786-137">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-137">ACR</span></span>

* <span data-ttu-id="82786-138">Adição do grupo de comandos `acr config retention` para configurar a política de retenção</span><span class="sxs-lookup"><span data-stu-id="82786-138">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="82786-139">AKS</span><span class="sxs-lookup"><span data-stu-id="82786-139">AKS</span></span>

* <span data-ttu-id="82786-140">Adição de suporte para integração do ACR com os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="82786-140">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="82786-141">Adição do parâmetro `--attach-acr` a `aks [create|update]` para anexar um ACR a um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="82786-141">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="82786-142">Adição do parâmetro `--detach-acr` a `aks update` para desanexar o ACR de um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="82786-142">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="82786-143">ARM</span><span class="sxs-lookup"><span data-stu-id="82786-143">ARM</span></span>

* <span data-ttu-id="82786-144">Atualização para uso da versão de API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="82786-144">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="82786-145">Lote</span><span class="sxs-lookup"><span data-stu-id="82786-145">Batch</span></span>

* <span data-ttu-id="82786-146">Adição de novas definições de configuração JSON de `--json-file` para `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="82786-146">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="82786-147">Adição de `MountConfigurations` para montagens do sistema de arquivos (confira https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="82786-147">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="82786-148">Adição da propriedade opcional `publicIPs` a `NetworkConfiguration` para IPs públicos em pools (confira https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="82786-148">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="82786-149">Adição de suporte para galerias de imagens compartilhadas a `--image`</span><span class="sxs-lookup"><span data-stu-id="82786-149">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="82786-150">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `--start-task-wait-for-success` em `batch pool create` para `true`</span><span class="sxs-lookup"><span data-stu-id="82786-150">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="82786-151">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `Scope` em `AutoUserSpecification` para sempre ser Pool (anteriormente, `Task` em nós do Windows e `Pool` em nós do Linux)</span><span class="sxs-lookup"><span data-stu-id="82786-151">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="82786-152">Esse argumento só pode ser definido em uma configuração JSON com `--json-file`</span><span class="sxs-lookup"><span data-stu-id="82786-152">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="82786-153">HDInsight</span><span class="sxs-lookup"><span data-stu-id="82786-153">HDInsight</span></span>

* <span data-ttu-id="82786-154">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="82786-154">GA release</span></span>
* <span data-ttu-id="82786-155">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--workernode-count/-c` de `az hdinsight resize` para ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82786-155">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="82786-156">Key Vault</span><span class="sxs-lookup"><span data-stu-id="82786-156">Key Vault</span></span>

* <span data-ttu-id="82786-157">Correção do problema em que as sub-redes não podiam ser excluídas das regras da rede</span><span class="sxs-lookup"><span data-stu-id="82786-157">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="82786-158">Correção do problema em que sub-redes e endereços IP duplicados podiam ser adicionados às regras da rede</span><span class="sxs-lookup"><span data-stu-id="82786-158">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="82786-159">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-159">Network</span></span>

* <span data-ttu-id="82786-160">Adição do parâmetro `--interval` a `network watcher flow-log` para definir o valor do intervalo de análise de tráfego</span><span class="sxs-lookup"><span data-stu-id="82786-160">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="82786-161">Adição de `network application-gateway identity` para gerenciar a identidade do gateway</span><span class="sxs-lookup"><span data-stu-id="82786-161">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="82786-162">Adição de suporte para definir a ID do Key Vault como `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="82786-162">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="82786-163">Adicionado `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="82786-163">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="82786-164">Política</span><span class="sxs-lookup"><span data-stu-id="82786-164">Policy</span></span>

* <span data-ttu-id="82786-165">Atualização para uso da versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="82786-165">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="82786-166">27 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-166">August 27, 2019</span></span>

<span data-ttu-id="82786-167">Versão 2.0.72</span><span class="sxs-lookup"><span data-stu-id="82786-167">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="82786-168">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-168">ACR</span></span>

* <span data-ttu-id="82786-169">[ALTERAÇÃO SIGNIFICATIVA] Remoção da compatibilidade com o SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="82786-169">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="82786-170">Gerenciamento de API</span><span class="sxs-lookup"><span data-stu-id="82786-170">API Management</span></span>

* <span data-ttu-id="82786-171">[VERSÃO PRÉVIA] Adição do grupo de comandos `apim`</span><span class="sxs-lookup"><span data-stu-id="82786-171">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-172">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-172">AppService</span></span>

* <span data-ttu-id="82786-173">Correção do problema com o comando `webapp webjob continuous start` ao especificar um slot</span><span class="sxs-lookup"><span data-stu-id="82786-173">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="82786-174">Alteração de `webapp up` para detectar a pasta `env` e removê-la do arquivo usado para implantação</span><span class="sxs-lookup"><span data-stu-id="82786-174">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="82786-175">Keyvault</span><span class="sxs-lookup"><span data-stu-id="82786-175">Keyvault</span></span>

* <span data-ttu-id="82786-176">Correção de um bug no `keyvault secret set` que ignorava o argumento `--expires`</span><span class="sxs-lookup"><span data-stu-id="82786-176">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="82786-177">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-177">Network</span></span>

* <span data-ttu-id="82786-178">Adição de suporte para endereços IPv6 a argumentos `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="82786-178">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="82786-179">Adição de novos comandos `network private-endpoint [create|update|list-types]` para o gerenciamento de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="82786-179">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="82786-180">Adição do grupo de comandos `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="82786-180">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="82786-181">Adicionados os argumentos `--private-endpoint-network-policies` e `--private-link-service-network-policies` para `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="82786-181">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="82786-182">RBAC</span><span class="sxs-lookup"><span data-stu-id="82786-182">RBAC</span></span>

* <span data-ttu-id="82786-183">Correção de um problema com `ad app update --homepage` em que a página inicial não era atualizada</span><span class="sxs-lookup"><span data-stu-id="82786-183">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="82786-184">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="82786-184">ServiceFabric</span></span>

* <span data-ttu-id="82786-185">Adição de suporte para nomes de Key Vault grafados com maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="82786-185">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="82786-186">Correção de um problema ao usar certificados no Key Vault</span><span class="sxs-lookup"><span data-stu-id="82786-186">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="82786-187">Correção de um problema com o uso de arquivos de certificado PFX</span><span class="sxs-lookup"><span data-stu-id="82786-187">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="82786-188">Correção de um problema com `sf cluster certificate add` quando o grupo de recursos do Key Vault não era especificado</span><span class="sxs-lookup"><span data-stu-id="82786-188">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="82786-189">Correção de um problema em que `sf cluster set` não funcionava</span><span class="sxs-lookup"><span data-stu-id="82786-189">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="82786-190">SignalR</span><span class="sxs-lookup"><span data-stu-id="82786-190">SignalR</span></span>

* <span data-ttu-id="82786-191">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="82786-191">Added new commands:</span></span>
  * <span data-ttu-id="82786-192">`signalr cors`: gerenciar CORS do SignalR</span><span class="sxs-lookup"><span data-stu-id="82786-192">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="82786-193">`signalr restart`: reiniciar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="82786-193">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="82786-194">`signalr update`: atualizar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="82786-194">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="82786-195">Adicionado o argumento `--service-mode` para `signalr create`</span><span class="sxs-lookup"><span data-stu-id="82786-195">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="82786-196">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-196">Storage</span></span>

* <span data-ttu-id="82786-197">Adicionado o comando `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="82786-197">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="82786-198">13 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-198">August 13, 2019</span></span>

<span data-ttu-id="82786-199">Versão 2.0.71</span><span class="sxs-lookup"><span data-stu-id="82786-199">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-200">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-200">AppService</span></span>

* <span data-ttu-id="82786-201">Um problema de falha de slots com os comandos `webapp webjob continuous` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="82786-201">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="82786-202">BotService</span><span class="sxs-lookup"><span data-stu-id="82786-202">BotService</span></span>

* <span data-ttu-id="82786-203">[ALTERAÇÃO SIGNIFICATIVA] O suporte para a criação de bots SDK v3 foi removido</span><span class="sxs-lookup"><span data-stu-id="82786-203">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="82786-204">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="82786-204">CognitiveServices</span></span>

* <span data-ttu-id="82786-205">Adicionados os comandos `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="82786-205">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="82786-206">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82786-206">Cosmos DB</span></span>

* <span data-ttu-id="82786-207">Removido o aviso ao atualizar vários locais de gravação</span><span class="sxs-lookup"><span data-stu-id="82786-207">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="82786-208">Foram adicionados os comandos CRUD para o CosmosDB SQL, MongoDB, Cassandra, Gremlin e Recursos de tabela e taxa de transferência do recurso</span><span class="sxs-lookup"><span data-stu-id="82786-208">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="82786-209">HDInsight</span><span class="sxs-lookup"><span data-stu-id="82786-209">HDInsight</span></span>

<span data-ttu-id="82786-210">Esta versão contém um grande número de alterações da falha.</span><span class="sxs-lookup"><span data-stu-id="82786-210">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="82786-211">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="82786-211">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="82786-212">`--storage-default-container` renomeado para `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="82786-212">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="82786-213">`--storage-default-filesystem` renomeado para `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="82786-213">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="82786-214">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--name` de `application create` foi alterado para representar o nome do aplicativo em vez do nome do cluster</span><span class="sxs-lookup"><span data-stu-id="82786-214">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="82786-215">O argumento `--cluster-name` foi adicionado a `application create` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="82786-215">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="82786-216">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `application create`:</span><span class="sxs-lookup"><span data-stu-id="82786-216">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="82786-217">`--application-type` renomeado para `--type`</span><span class="sxs-lookup"><span data-stu-id="82786-217">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="82786-218">`--marketplace-identifier` renomeado para `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="82786-218">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="82786-219">`--https-endpoint-access-mode` renomeado para `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="82786-219">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="82786-220">Renomeado de `--https-endpoint-destination-port` para `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="82786-220">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="82786-221">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros removidos para `application create`:</span><span class="sxs-lookup"><span data-stu-id="82786-221">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="82786-222">[ALTERAÇÃO DA FALHA] Renomeado de `--target-instance-count` para `--workernode-count` para `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="82786-222">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="82786-223">[ALTERAÇÃO SIGNIFICATIVA] Todos os comandos no grupo `hdinsight script-action` foram alterados para usar o parâmetro `--name` como o nome da ação de script.</span><span class="sxs-lookup"><span data-stu-id="82786-223">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="82786-224">O argumento `--cluster-name` foi adicionado a todos os comandos `hdinsight script-action` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="82786-224">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="82786-225">[ALTERAÇÃO SIGNIFICATIVA] Renomeado de `--script-execution-id` para `--execution-id` para todos os comandos `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="82786-225">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="82786-226">[ALTERAÇÃO SIGNIFICATIVA] `hdinsight script-action show` renomeado para `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="82786-226">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="82786-227">[ALTERAÇÃO DA FALHA] Os parâmetros foram alterados para `hdinsight script-action execute --roles` para serem separados por espaços em vez de separados por vírgula</span><span class="sxs-lookup"><span data-stu-id="82786-227">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="82786-228">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro `--persisted` de `hdinsight script-action list` foi removido</span><span class="sxs-lookup"><span data-stu-id="82786-228">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="82786-229">O parâmetro `hdinsight create --cluster-configurations` foi alterado para aceitar um caminho para um arquivo JSON local ou uma cadeia de caracteres JSON</span><span class="sxs-lookup"><span data-stu-id="82786-229">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="82786-230">Adicionado o comando `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="82786-230">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="82786-231">Alterado `hdinsight monitor enable --workspace` para aceitar uma ID do workspace ou nome do workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="82786-231">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="82786-232">O argumento `hdinsight monitor enable --primary-key`, que será necessário caso uma ID do workspace seja fornecida como o parâmetro, foi adicionado</span><span class="sxs-lookup"><span data-stu-id="82786-232">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="82786-233">Foram adicionados mais exemplos e atualização das descrições das mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="82786-233">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="82786-234">Interativo</span><span class="sxs-lookup"><span data-stu-id="82786-234">Interactive</span></span>

* <span data-ttu-id="82786-235">Um erro no carregamento foi corrigido</span><span class="sxs-lookup"><span data-stu-id="82786-235">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="82786-236">kubernetes</span><span class="sxs-lookup"><span data-stu-id="82786-236">Kubernetes</span></span>

* <span data-ttu-id="82786-237">Alterado para usar `https` se a porta do contêiner do painel estiver usando `https`</span><span class="sxs-lookup"><span data-stu-id="82786-237">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="82786-238">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-238">Network</span></span>

* <span data-ttu-id="82786-239">O argumento `--yes` foi adicionado a `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="82786-239">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="82786-240">Perfil</span><span class="sxs-lookup"><span data-stu-id="82786-240">Profile</span></span>

* <span data-ttu-id="82786-241">O argumento `--resource-type` foi adicionado a `account get-access-token` para obter tokens de acesso de recurso</span><span class="sxs-lookup"><span data-stu-id="82786-241">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="82786-242">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="82786-242">ServiceFabric</span></span>

* <span data-ttu-id="82786-243">Todas as versões de sistema operacional com suporte para criação do cluster sf foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="82786-243">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="82786-244">Foi corrigido o bug de validação do certificado primário</span><span class="sxs-lookup"><span data-stu-id="82786-244">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="82786-245">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-245">Storage</span></span>

* <span data-ttu-id="82786-246">Adicionado o comando `storage copy`</span><span class="sxs-lookup"><span data-stu-id="82786-246">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="82786-247">30 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-247">July 30, 2019</span></span>

<span data-ttu-id="82786-248">Versão 2.0.70</span><span class="sxs-lookup"><span data-stu-id="82786-248">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="82786-249">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-249">ACR</span></span>

* <span data-ttu-id="82786-250">Corrigido o problema #9952 (uma regressão no comando `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="82786-250">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="82786-251">Removido o nome da imagem do construtor padrão em `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="82786-251">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-252">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-252">Appservice</span></span>

* <span data-ttu-id="82786-253">Alterado `webapp config ssl` para mostrar uma mensagem se um recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="82786-253">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="82786-254">Corrigido o problema em que `functionapp create` não aceita o tipo de conta de armazenamento `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="82786-254">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="82786-255">Corrigido um problema em que `webapp up` falharia se fosse executado usando versões mais antigas do Python</span><span class="sxs-lookup"><span data-stu-id="82786-255">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="82786-256">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-256">Network</span></span>

* <span data-ttu-id="82786-257">Removido parâmetro inválido `--ids` de `network nic ip-config add` (corrige o #9861)</span><span class="sxs-lookup"><span data-stu-id="82786-257">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="82786-258">Corrige o #9604.</span><span class="sxs-lookup"><span data-stu-id="82786-258">Fixes #9604.</span></span> <span data-ttu-id="82786-259">Adicionado o parâmetro `--root-certs` ao `network application-gateway http-settings [create|update]` para dar suporte a certificados raiz confiáveis associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="82786-259">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="82786-260">Fixado argumento `--subscription` para `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="82786-260">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="82786-261">RBAC</span><span class="sxs-lookup"><span data-stu-id="82786-261">RBAC</span></span>

* <span data-ttu-id="82786-262">Adicionado o comando `user update`</span><span class="sxs-lookup"><span data-stu-id="82786-262">Added `user update` command</span></span>
* <span data-ttu-id="82786-263">[PRETERIDO] Preterido `--upn-or-object-id` de comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="82786-263">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="82786-264">Usar argumento de substituição `--id`</span><span class="sxs-lookup"><span data-stu-id="82786-264">Use replacement argument `--id`</span></span>
* <span data-ttu-id="82786-265">Adicionado argumento `--id` para comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="82786-265">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="82786-266">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-266">SQL</span></span>

* <span data-ttu-id="82786-267">Adicionados comandos de gerenciamento para chaves de instância gerenciada e protetor de TDE</span><span class="sxs-lookup"><span data-stu-id="82786-267">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="82786-268">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-268">Storage</span></span>

* <span data-ttu-id="82786-269">Adicionado o comando `storage remove`</span><span class="sxs-lookup"><span data-stu-id="82786-269">Added `storage remove` command</span></span>
* <span data-ttu-id="82786-270">Corrigido um problema com `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="82786-270">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="82786-271">VM</span><span class="sxs-lookup"><span data-stu-id="82786-271">VM</span></span>

* <span data-ttu-id="82786-272">Alterado `list-skus` para usar versão de API mais recente a fim de externar detalhes de zona</span><span class="sxs-lookup"><span data-stu-id="82786-272">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="82786-273">Alterado o padrão de `--single-placement-group` para `false` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="82786-273">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="82786-274">Adicionada a capacidade de selecionar SKUs de armazenamento ZRS para `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="82786-274">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="82786-275">Adicionado novo grupo de comandos `vm host` para dar suporte a hosts dedicados</span><span class="sxs-lookup"><span data-stu-id="82786-275">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="82786-276">Adicionados parâmetros `--host` e `--host-group` em `vm create` para definir o host dedicado da VM</span><span class="sxs-lookup"><span data-stu-id="82786-276">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="82786-277">16 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-277">July 16, 2019</span></span>

<span data-ttu-id="82786-278">Versão 2.0.69</span><span class="sxs-lookup"><span data-stu-id="82786-278">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-279">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-279">Appservice</span></span>

* <span data-ttu-id="82786-280">Os comandos `webapp identity` foram alterados para retornar uma mensagem de erro apropriada se o nome do aplicativo ou ResourceGroupName for inválido</span><span class="sxs-lookup"><span data-stu-id="82786-280">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="82786-281">`webapp list` corrigido para retornar o valor correto para numberOfSites se nenhum ResourceGroup foi fornecido</span><span class="sxs-lookup"><span data-stu-id="82786-281">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="82786-282">Corrigidos os efeitos colaterais de `appservice plan create` e `webapp create`</span><span class="sxs-lookup"><span data-stu-id="82786-282">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="82786-283">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-283">Core</span></span>

* <span data-ttu-id="82786-284">Corrigido um problema em que `--subscription` aparecia apesar de não ser aplicável</span><span class="sxs-lookup"><span data-stu-id="82786-284">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="82786-285">Lote</span><span class="sxs-lookup"><span data-stu-id="82786-285">Batch</span></span>

* <span data-ttu-id="82786-286">[ALTERAÇÃO SIGNIFICATIVA] `batch pool node-agent-skus list` foi substituído por `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="82786-286">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="82786-287">Adicionado suporte para regras de segurança bloqueando o acesso de rede a um pool com base na porta de origem do tráfego ao usar a opção `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="82786-287">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="82786-288">Suporte adicionado para executar a tarefa no diretório de trabalho de contêiner ou no diretório de trabalho de tarefa em lotes ao usar a opção `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="82786-288">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="82786-289">Corrigido o erro na opção `--application-package-references` de `batch pool create` em que ela funcionaria apenas com padrões</span><span class="sxs-lookup"><span data-stu-id="82786-289">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="82786-290">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="82786-290">Eventhubs</span></span>

* <span data-ttu-id="82786-291">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="82786-291">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="82786-292">RDBMS</span><span class="sxs-lookup"><span data-stu-id="82786-292">RDBMS</span></span>

* <span data-ttu-id="82786-293">Adicionado um parâmetro opcional para especificar a réplica de SKU para criar o comando de réplica</span><span class="sxs-lookup"><span data-stu-id="82786-293">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="82786-294">Corrigido o problema com a falha no teste de CI com a criação de réplica de MySQL</span><span class="sxs-lookup"><span data-stu-id="82786-294">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="82786-295">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="82786-295">Relay</span></span>

* <span data-ttu-id="82786-296">Corrigido o problema com a conexão híbrida quando a autorização do cliente desabilitava [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="82786-296">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="82786-297">Parâmetro `--requires-transport-security` adicionado a `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="82786-297">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="82786-298">Barramento de serviço</span><span class="sxs-lookup"><span data-stu-id="82786-298">Servicebus</span></span>

* <span data-ttu-id="82786-299">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="82786-299">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="82786-300">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-300">Storage</span></span>

* <span data-ttu-id="82786-301">Habilitar AADDS de arquivos para atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-301">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="82786-302">Problema corrigido `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="82786-302">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="82786-303">2 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-303">July 2, 2019</span></span>

<span data-ttu-id="82786-304">Versão 2.0.68</span><span class="sxs-lookup"><span data-stu-id="82786-304">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="82786-305">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-305">Core</span></span>

* <span data-ttu-id="82786-306">Agora, os módulos de comando são consolidados em um único Python distribuível.</span><span class="sxs-lookup"><span data-stu-id="82786-306">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="82786-307">Isso substitui o uso direto de muitos pacotes `azure-cli-` no PyPI.</span><span class="sxs-lookup"><span data-stu-id="82786-307">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="82786-308">Assim, o tamanho da instalação será reduzido e apenas os usuários que tiverem instalado diretamente por meio do `pip` serão afetados.</span><span class="sxs-lookup"><span data-stu-id="82786-308">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="82786-309">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-309">ACR</span></span>

* <span data-ttu-id="82786-310">Foi adicionado o suporte para gatilhos de temporizador para tarefa</span><span class="sxs-lookup"><span data-stu-id="82786-310">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-311">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-311">Appservice</span></span>

* <span data-ttu-id="82786-312">O `functionapp create` foi alterado para habilitar o Application Insights por padrão</span><span class="sxs-lookup"><span data-stu-id="82786-312">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="82786-313">[ALTERAÇÃO SIGNIFICATIVA] Foi removido o comando `functionapp devops-build` preterido.</span><span class="sxs-lookup"><span data-stu-id="82786-313">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="82786-314">Agora, use o novo comando `az functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="82786-314">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="82786-315">Foi adicionado o suporte ao plano de aplicativo de funções Consumo em Linux ao `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="82786-315">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="82786-316">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82786-316">Cosmos DB</span></span>

* <span data-ttu-id="82786-317">Foi adicionado o suporte para desabilitar a TTL</span><span class="sxs-lookup"><span data-stu-id="82786-317">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="82786-318">DLS</span><span class="sxs-lookup"><span data-stu-id="82786-318">DLS</span></span>

* <span data-ttu-id="82786-319">Versão atualizada do ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="82786-319">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="82786-320">Comentários</span><span class="sxs-lookup"><span data-stu-id="82786-320">Feedback</span></span>

* <span data-ttu-id="82786-321">Ao relatar um comando de extensão com falha, agora, o `az feedback` tenta abrir o navegador na URL do projeto/repositório da extensão por meio do índice</span><span class="sxs-lookup"><span data-stu-id="82786-321">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="82786-322">HDInsight</span><span class="sxs-lookup"><span data-stu-id="82786-322">HDInsight</span></span>

* <span data-ttu-id="82786-323">[ALTERAÇÃO SIGNIFICATIVA] O nome do grupo de comandos `oms` foi alterado para `monitor`</span><span class="sxs-lookup"><span data-stu-id="82786-323">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="82786-324">[ALTERAÇÃO SIGNIFICATIVA] `--http-password/-p` tornou-se um parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="82786-324">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="82786-325">Foram adicionados preenchedores para o preenchedor dos parâmetros `--cluster-admin-account` e `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="82786-325">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="82786-326">O parâmetro `cluster-users-group-dns` foi alterado para ser obrigatório quando `—esp` estiver presente</span><span class="sxs-lookup"><span data-stu-id="82786-326">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="82786-327">Foi adicionado um tempo limite para todos os preenchedores automáticos de argumento existentes</span><span class="sxs-lookup"><span data-stu-id="82786-327">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="82786-328">Foi adicionado um tempo limite para transformar o nome do recurso na ID de recurso</span><span class="sxs-lookup"><span data-stu-id="82786-328">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="82786-329">Os preenchedores automáticos foram alterados para selecionar recursos de qualquer grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="82786-329">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="82786-330">Pode ser um grupo de recursos diferente daquele especificado com `-g`</span><span class="sxs-lookup"><span data-stu-id="82786-330">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="82786-331">Foi adicionado o suporte para os parâmetros `--sub-domain-suffix` e `--disable_gateway_auth` no comando `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="82786-331">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="82786-332">Serviços gerenciados</span><span class="sxs-lookup"><span data-stu-id="82786-332">Managed Services</span></span>

* <span data-ttu-id="82786-333">Introdução ao módulo de comando de serviço gerenciado em versão prévia</span><span class="sxs-lookup"><span data-stu-id="82786-333">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="82786-334">Perfil</span><span class="sxs-lookup"><span data-stu-id="82786-334">Profile</span></span>
* <span data-ttu-id="82786-335">Suprimir o argumento `--subscription` para o comando de logoff</span><span class="sxs-lookup"><span data-stu-id="82786-335">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="82786-336">RBAC</span><span class="sxs-lookup"><span data-stu-id="82786-336">RBAC</span></span>

* <span data-ttu-id="82786-337">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--password` foi removido de `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="82786-337">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="82786-338">Foi adicionado o parâmetro `--assignee-principal-type` ao comando `create` para evitar falhas intermitentes causadas pela latência de replicação do servidor do AAD Graph</span><span class="sxs-lookup"><span data-stu-id="82786-338">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="82786-339">Foi corrigida uma falha em `ad signed-in-user` ao listar objetos de propriedade</span><span class="sxs-lookup"><span data-stu-id="82786-339">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="82786-340">Foi corrigido um problema em que o `ad sp` não localizava o aplicativo certo de uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="82786-340">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="82786-341">RDBMS</span><span class="sxs-lookup"><span data-stu-id="82786-341">RDBMS</span></span>

* <span data-ttu-id="82786-342">Foi adicionado o suporte à replicação para o MariaDB</span><span class="sxs-lookup"><span data-stu-id="82786-342">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="82786-343">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-343">SQL</span></span>

* <span data-ttu-id="82786-344">Valores permitidos documentados para `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="82786-344">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="82786-345">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-345">Storage</span></span>

* <span data-ttu-id="82786-346">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="82786-346">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="82786-347">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="82786-347">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="82786-348">VM</span><span class="sxs-lookup"><span data-stu-id="82786-348">VM</span></span>

* <span data-ttu-id="82786-349">Foi corrigido o bug em que o `vmss create` retornava uma mensagem de erro quando era executado com `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="82786-349">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="82786-350">Foi removida a validação do lado do cliente de `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="82786-350">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="82786-351">Não falha quando `--single-placement-group` é definido como `true` e `--instance-count` é maior que 100 ou quando são especificadas zonas de disponibilidade, mas deixa essa validação para o serviço de computação</span><span class="sxs-lookup"><span data-stu-id="82786-351">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="82786-352">Foi corrigido o bug em que o `[vm|vmss] extension image list` falhava quando era usado com `--latest`</span><span class="sxs-lookup"><span data-stu-id="82786-352">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="82786-353">18 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-353">June 18, 2019</span></span>

<span data-ttu-id="82786-354">Versão 2.0.67</span><span class="sxs-lookup"><span data-stu-id="82786-354">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="82786-355">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-355">Core</span></span>

<span data-ttu-id="82786-356">Esta versão apresenta uma nova marca [Versão prévia] para comunicar com mais clareza aos clientes quando um comando, um grupo de comandos ou um argumento está no status de versão prévia.</span><span class="sxs-lookup"><span data-stu-id="82786-356">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="82786-357">Anteriormente, essa informação era transmitida no texto de ajuda ou, implicitamente, pelo número da versão do módulo de comando.</span><span class="sxs-lookup"><span data-stu-id="82786-357">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="82786-358">A CLI removerá os números de versão dos pacotes individuais no futuro.</span><span class="sxs-lookup"><span data-stu-id="82786-358">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="82786-359">Se um comando estiver em versão prévia, todos os seus argumentos também estarão.</span><span class="sxs-lookup"><span data-stu-id="82786-359">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="82786-360">Se um grupo de comandos for rotulado com o status de versão prévia, então todos os seus comandos e argumentos também serão considerados em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="82786-360">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="82786-361">Como resultado dessa alteração, diversos grupos de comandos podem parecer surgir "de repente" com o status de versão prévia com esta liberação.</span><span class="sxs-lookup"><span data-stu-id="82786-361">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="82786-362">O que realmente aconteceu é que a maioria dos pacotes já estava com status de versão prévia, mas estão sendo consideradas GA com esta liberação</span><span class="sxs-lookup"><span data-stu-id="82786-362">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="82786-363">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-363">ACR</span></span>
* <span data-ttu-id="82786-364">Adicionado o comando 'acr check-health'</span><span class="sxs-lookup"><span data-stu-id="82786-364">Added 'acr check-health' command</span></span>
* <span data-ttu-id="82786-365">Melhorado o tratamento de erro para tokens do AAD e para recuperar comandos externos</span><span class="sxs-lookup"><span data-stu-id="82786-365">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="82786-366">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-366">ACS</span></span>
* <span data-ttu-id="82786-367">Comandos preteridos do ACS agora ficam ocultos da exibição da ajuda</span><span class="sxs-lookup"><span data-stu-id="82786-367">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="82786-368">AMS</span><span class="sxs-lookup"><span data-stu-id="82786-368">AMS</span></span>
* <span data-ttu-id="82786-369">[ALTERAÇÃO SIGNIFICATIVA] Alterada para retornar cadeias de caracteres de tempo da ISO 8601 para archive-window-length e key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="82786-369">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-370">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-370">AppService</span></span>
* <span data-ttu-id="82786-371">Adicionado roteamento com base no local para `webapp deleted list` e `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="82786-371">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="82786-372">Corrigido problema em que a URL de destino registrada do webapp ("Não é possível iniciar o aplicativo em...") não era clicável no Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="82786-372">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="82786-373">Corrigido um problema em que a criação de aplicativos com algumas SKUs falhava com um erro de AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="82786-373">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="82786-374">Adicionada a pré-validação para o `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="82786-374">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="82786-375">Corrigido o `[webapp|functionapp] traffic-routing` para usar o actionHostName correto</span><span class="sxs-lookup"><span data-stu-id="82786-375">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="82786-376">Adicionado o suporte de slot para comandos `functionapp`</span><span class="sxs-lookup"><span data-stu-id="82786-376">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="82786-377">Lote</span><span class="sxs-lookup"><span data-stu-id="82786-377">Batch</span></span>
* <span data-ttu-id="82786-378">Corrigida a regressão de autenticação do AAD causada pela geração de relatórios de erros superagressiva para autenticação de chave compartilhada</span><span class="sxs-lookup"><span data-stu-id="82786-378">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="82786-379">BatchAI</span><span class="sxs-lookup"><span data-stu-id="82786-379">BatchAI</span></span>
* <span data-ttu-id="82786-380">Agora os comandos do BatchAI estão preteridos e ocultos</span><span class="sxs-lookup"><span data-stu-id="82786-380">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="82786-381">BotService</span><span class="sxs-lookup"><span data-stu-id="82786-381">BotService</span></span>
* <span data-ttu-id="82786-382">Adição das mensagens de aviso "suporte descontinuado"/"modo de manutenção" para os comandos compatíveis com a v3 do SDK</span><span class="sxs-lookup"><span data-stu-id="82786-382">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82786-383">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="82786-383">CosmosDB</span></span>
* <span data-ttu-id="82786-384">[PRETERIDO] Preterido o comando `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="82786-384">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="82786-385">Adicionado o comando `cosmosdb keys list` – substitui o `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="82786-385">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="82786-386">`cosmsodb create/update`: Adicionado novo formato para --location a fim de permitir a configuração da propriedade "isZoneRedundant".</span><span class="sxs-lookup"><span data-stu-id="82786-386">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="82786-387">Formato antigo preterido</span><span class="sxs-lookup"><span data-stu-id="82786-387">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="82786-388">EventGrid</span><span class="sxs-lookup"><span data-stu-id="82786-388">EventGrid</span></span>
* <span data-ttu-id="82786-389">Adicionados comandos do `eventgrid domain` para operações de CRUD no domínio</span><span class="sxs-lookup"><span data-stu-id="82786-389">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="82786-390">Adicionados comandos do `eventgrid domain topic` para operações de CRUD nos tópicos do domínio</span><span class="sxs-lookup"><span data-stu-id="82786-390">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="82786-391">Adicionado argumento do `--odata-query` ao `eventgrid [topic|event-subscription] list` para filtrar os resultados usando a sintaxe do OData</span><span class="sxs-lookup"><span data-stu-id="82786-391">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="82786-392">`event-subscription create/update`: Adicionado o servicebusqueue como novos valores para o parâmetro `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="82786-392">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="82786-393">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para `--included-event-types All` com `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-393">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="82786-394">HDInsight</span><span class="sxs-lookup"><span data-stu-id="82786-394">HDInsight</span></span>
* <span data-ttu-id="82786-395">Adicionado suporte para o parâmetro `--ssh-public-key` no comando `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="82786-395">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="82786-396">IoT</span><span class="sxs-lookup"><span data-stu-id="82786-396">IoT</span></span>
* <span data-ttu-id="82786-397">Adicionado suporte para regenerar as chaves da política de autorização</span><span class="sxs-lookup"><span data-stu-id="82786-397">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="82786-398">Adicionados SDK e suporte para o serviço de provisionamento de repositórios do DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="82786-398">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="82786-399">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-399">Network</span></span>
* <span data-ttu-id="82786-400">Adicionado suporte de zona para o Gateway da NAT</span><span class="sxs-lookup"><span data-stu-id="82786-400">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="82786-401">Adicionado o comando `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="82786-401">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="82786-402">Corrigido o problema com o `dns zone import` em que os usuários não conseguiam importar registros do curinga A</span><span class="sxs-lookup"><span data-stu-id="82786-402">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="82786-403">Corrigido o problema com o `watcher flow-log configure` em que o registro de fluxo não podia ser habilitado em determinadas regiões</span><span class="sxs-lookup"><span data-stu-id="82786-403">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="82786-404">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-404">Resource</span></span>
* <span data-ttu-id="82786-405">Adicionado o comando do `az rest` para fazer chamadas REST</span><span class="sxs-lookup"><span data-stu-id="82786-405">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="82786-406">Corrigido o erro ao usar o `policy assignment list` com um grupo de recursos ou o nível de assinatura `--scope`</span><span class="sxs-lookup"><span data-stu-id="82786-406">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="82786-407">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="82786-407">ServiceBus</span></span>
* <span data-ttu-id="82786-408">Corrigido o problema com o `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="82786-408">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="82786-409">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-409">SQL</span></span>
* <span data-ttu-id="82786-410">Alterado o `--location` para ser opcional para `sql [server|mi] create` – usa o local do grupo de recursos se não especificado</span><span class="sxs-lookup"><span data-stu-id="82786-410">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="82786-411">Corrigido o erro "objeto 'NoneType' não é iterável" para `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="82786-411">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="82786-412">SQLVm</span><span class="sxs-lookup"><span data-stu-id="82786-412">SQLVm</span></span>
* <span data-ttu-id="82786-413">[ALTERAÇÃO DA FALHA] Alterado `sql vm create` para exigir o parâmetro `--license-type`</span><span class="sxs-lookup"><span data-stu-id="82786-413">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="82786-414">Alterado para permitir a configuração da SKU da imagem do SQL ao criar ou atualizar uma VM do SQL</span><span class="sxs-lookup"><span data-stu-id="82786-414">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="82786-415">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-415">Storage</span></span>
* <span data-ttu-id="82786-416">Corrigido o problema com a chave de conta ignorada para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="82786-416">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="82786-417">Corrigido o problema com o `storage blob sync` no Linux</span><span class="sxs-lookup"><span data-stu-id="82786-417">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="82786-418">VM</span><span class="sxs-lookup"><span data-stu-id="82786-418">VM</span></span>
* <span data-ttu-id="82786-419">[VERSÃO PRÉVIA] Adicionados os comandos `vm image template` para criar imagens de VM</span><span class="sxs-lookup"><span data-stu-id="82786-419">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="82786-420">4 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-420">June 4, 2019</span></span>

<span data-ttu-id="82786-421">Versão 2.0.66</span><span class="sxs-lookup"><span data-stu-id="82786-421">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="82786-422">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-422">Core</span></span>
* <span data-ttu-id="82786-423">Foi corrigido o bug em que os comandos falhavam quando `--output yaml` era usado com `--query`</span><span class="sxs-lookup"><span data-stu-id="82786-423">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="82786-424">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-424">ACR</span></span>
* <span data-ttu-id="82786-425">Foi adicionado o grupo de comando 'pack acr' para a criação de Tarefas de build rápida usando Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="82786-425">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="82786-426">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-426">ACS</span></span>
* <span data-ttu-id="82786-427">Permitir a opção de habilitar/desabilitar o complemento kube-dashboard do AKS</span><span class="sxs-lookup"><span data-stu-id="82786-427">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="82786-428">Imprimir uma mensagem amigável quando a assinatura não estiver na lista de permissões para usar o Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="82786-428">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="82786-429">Lote</span><span class="sxs-lookup"><span data-stu-id="82786-429">Batch</span></span>
* <span data-ttu-id="82786-430">Melhoria no tratamento de erro quando você não está conectado a uma conta \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="82786-430">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="82786-431">IoT</span><span class="sxs-lookup"><span data-stu-id="82786-431">IoT</span></span>
* <span data-ttu-id="82786-432">Foi adicionado o suporte para failover manual</span><span class="sxs-lookup"><span data-stu-id="82786-432">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="82786-433">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-433">Network</span></span>
* <span data-ttu-id="82786-434">Foram adicionados os comandos `network application-gateway waf-policy` para oferecer suporte às regras de WAF personalizadas.</span><span class="sxs-lookup"><span data-stu-id="82786-434">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="82786-435">Adicionados os argumentos `--waf-policy` e `--max-capacity` para `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-435">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="82786-436">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-436">Resource</span></span>
* <span data-ttu-id="82786-437">Melhoria da mensagem de erro do `deployment create` quando não há nenhum TTY disponível</span><span class="sxs-lookup"><span data-stu-id="82786-437">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="82786-438">Função</span><span class="sxs-lookup"><span data-stu-id="82786-438">Role</span></span>
* <span data-ttu-id="82786-439">O texto da Ajuda foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="82786-439">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="82786-440">Computação</span><span class="sxs-lookup"><span data-stu-id="82786-440">Compute</span></span>
* <span data-ttu-id="82786-441">Foi adicionado o suporte para `vm create` para as VMs de uma imagem gerenciada com LUNs de disco de dados que não começam em 0 ou que ignoram números</span><span class="sxs-lookup"><span data-stu-id="82786-441">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="82786-442">21 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-442">May 21, 2019</span></span>

<span data-ttu-id="82786-443">Versão 2.0.65</span><span class="sxs-lookup"><span data-stu-id="82786-443">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="82786-444">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-444">Core</span></span>
* <span data-ttu-id="82786-445">Foram adicionados comentários melhores para erros de autenticação</span><span class="sxs-lookup"><span data-stu-id="82786-445">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="82786-446">Corrigido um problema em que a CLI carregava extensões que não eram compatíveis com a versão do núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-446">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="82786-447">Corrigido um problema com a inicialização quando `clouds.config` está corrompido</span><span class="sxs-lookup"><span data-stu-id="82786-447">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="82786-448">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-448">ACR</span></span>
* <span data-ttu-id="82786-449">Foi adicionado suporte das Identidades Gerenciadas para Tarefas</span><span class="sxs-lookup"><span data-stu-id="82786-449">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="82786-450">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-450">ACS</span></span>
* <span data-ttu-id="82786-451">Corrigido o comando `openshift create` quando usado com o cliente AAD do consumidor</span><span class="sxs-lookup"><span data-stu-id="82786-451">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-452">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-452">AppService</span></span>
* <span data-ttu-id="82786-453">[PRETERIDO] Preterido o comando `functionapp devops-build` – Será removido na próxima versão</span><span class="sxs-lookup"><span data-stu-id="82786-453">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="82786-454">`functionapp devops-pipeline` foi alterado para buscar o log de build do Azure DevOps no modo detalhado</span><span class="sxs-lookup"><span data-stu-id="82786-454">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="82786-455">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--use_local_settings` foi removido do comando `functionapp devops-pipeline` – não estava operacional</span><span class="sxs-lookup"><span data-stu-id="82786-455">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="82786-456">`webapp up` foi alterado para retornar uma saída JSON se `--logs` não for usado</span><span class="sxs-lookup"><span data-stu-id="82786-456">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="82786-457">Foi adicionado suporte para escrever recursos padrão para a configuração local de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="82786-457">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="82786-458">Foi adicionado suporte para `webapp up` reimplantar um aplicativo sem usar o argumento `--location`</span><span class="sxs-lookup"><span data-stu-id="82786-458">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="82786-459">Corrigido um problema em que o valor do SKU gratuito não funcionava na criação do ASP do SKU gratuito do Linux</span><span class="sxs-lookup"><span data-stu-id="82786-459">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="82786-460">BotService</span><span class="sxs-lookup"><span data-stu-id="82786-460">BotService</span></span>
* <span data-ttu-id="82786-461">Alterado para permitir todas as capitalizações para parâmetros `--lang` em todos os comandos</span><span class="sxs-lookup"><span data-stu-id="82786-461">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="82786-462">Descrição atualizada do módulo de comando</span><span class="sxs-lookup"><span data-stu-id="82786-462">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="82786-463">Consumo</span><span class="sxs-lookup"><span data-stu-id="82786-463">Consumption</span></span>
* <span data-ttu-id="82786-464">O parâmetro obrigatório ausente foi adicionado para executar `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="82786-464">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="82786-465">IoT</span><span class="sxs-lookup"><span data-stu-id="82786-465">IoT</span></span>
* <span data-ttu-id="82786-466">Suporte adicionado para listar todas as chaves</span><span class="sxs-lookup"><span data-stu-id="82786-466">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="82786-467">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-467">Network</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="82786-469">O argumento `--nat-gateway` foi adicionado a `network vnet subnet [create|update]` para anexar a um gateway NAT</span><span class="sxs-lookup"><span data-stu-id="82786-469">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="82786-470">Corrigido o problema de `dns zone import`, em que os nomes de registro não correspondiam ao tipo de registro</span><span class="sxs-lookup"><span data-stu-id="82786-470">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="82786-471">RDBMS</span><span class="sxs-lookup"><span data-stu-id="82786-471">RDBMS</span></span>
* <span data-ttu-id="82786-472">Suporte a postgres e mysql adicionado para replicação geográfica</span><span class="sxs-lookup"><span data-stu-id="82786-472">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="82786-473">RBAC</span><span class="sxs-lookup"><span data-stu-id="82786-473">RBAC</span></span>
* <span data-ttu-id="82786-474">Suporte ao escopo de grupo de gerenciamento adicionado a `role assignment`</span><span class="sxs-lookup"><span data-stu-id="82786-474">Added support for mangement group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="82786-475">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-475">Storage</span></span>
* <span data-ttu-id="82786-476">`storage blob sync`: adicionar um comando de sincronização ao armazenamento de blobs</span><span class="sxs-lookup"><span data-stu-id="82786-476">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="82786-477">Computação</span><span class="sxs-lookup"><span data-stu-id="82786-477">Compute</span></span>
* <span data-ttu-id="82786-478">`--computer-name` foi adicionado a `vm create` para configurar o nome do computador da VM</span><span class="sxs-lookup"><span data-stu-id="82786-478">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="82786-479">`--ssh-key-value` foi renomeado para `--ssh-key-values` para `[vm|vmss] create` – Agora, pode aceitar vários valores de chave pública ou caminhos ssh</span><span class="sxs-lookup"><span data-stu-id="82786-479">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="82786-480">__Observação__: Isso **não** é uma alteração da falha – `--ssh-key-value` será analisado corretamente, pois corresponde somente a `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="82786-480">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="82786-481">O argumento `--type` de `ppg create` foi alterado para ser opcional</span><span class="sxs-lookup"><span data-stu-id="82786-481">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="82786-482">6 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-482">May 6, 2019</span></span>

<span data-ttu-id="82786-483">Versão 2.0.64</span><span class="sxs-lookup"><span data-stu-id="82786-483">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="82786-484">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-484">ACS</span></span>
* <span data-ttu-id="82786-485">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--fqdn` foi removido dos comandos `openshift`</span><span class="sxs-lookup"><span data-stu-id="82786-485">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="82786-486">Alterado para usar a versão da API do Red Hat OpenShift no Azure em disponibilidade geral</span><span class="sxs-lookup"><span data-stu-id="82786-486">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="82786-487">O sinalizador `customer-admin-group-id` foi adicionado a `openshift create`</span><span class="sxs-lookup"><span data-stu-id="82786-487">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="82786-488">[GA] `(PREVIEW)` foi removido da opção `aks create` `--network-policy`</span><span class="sxs-lookup"><span data-stu-id="82786-488">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-489">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-489">Appservice</span></span>
* <span data-ttu-id="82786-490">[PRETERIDO] O comando `functionapp devops-build` foi preterido</span><span class="sxs-lookup"><span data-stu-id="82786-490">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="82786-491">Renomeado para `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="82786-491">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="82786-492">Corrigido ao obter o nome de usuário correto para cloudshell que estava causando a falha em `webapp up`</span><span class="sxs-lookup"><span data-stu-id="82786-492">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="82786-493">Documentação `appservice plan --sku` atualizada para refletir o appserviceplans com suporte</span><span class="sxs-lookup"><span data-stu-id="82786-493">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="82786-494">Adicionado argumentos opcionais para o grupo de recursos e plano a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="82786-494">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="82786-495">Adicionado suporte a `webapp ssh` para respeitar a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="82786-495">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="82786-496">Adicionado suporte `appserviceplan create` para a SKU gratuita do Linux</span><span class="sxs-lookup"><span data-stu-id="82786-496">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="82786-497">Alterado `webapp up` para ter uma suspensão de 30 segundos depois de definir appsetting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` para lidar com a inicialização a frio kudu</span><span class="sxs-lookup"><span data-stu-id="82786-497">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="82786-498">Adicionado suporte para tempo de execução `powershell` a `functionapp create` no Windows</span><span class="sxs-lookup"><span data-stu-id="82786-498">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="82786-499">Adicionado o comando `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="82786-499">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="82786-500">Lote</span><span class="sxs-lookup"><span data-stu-id="82786-500">Batch</span></span>
* <span data-ttu-id="82786-501">Corrigido o bug no validador para as opções `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="82786-501">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="82786-502">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="82786-502">Botservice</span></span>
* <span data-ttu-id="82786-503">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para criar um Bot de Aplicativo Web vazio por padrão (ou seja, nenhum bot será implantado no Serviço de Aplicativo)</span><span class="sxs-lookup"><span data-stu-id="82786-503">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="82786-504">O sinalizador `--echo` foi adicionado ao `bot create` para usar o comportamento antigo com `-v v4`</span><span class="sxs-lookup"><span data-stu-id="82786-504">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="82786-505">[ALTERAÇÃO SIGNIFICATIVA] O valor padrão de `--version` foi alterado para `v4`</span><span class="sxs-lookup"><span data-stu-id="82786-505">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="82786-506">__OBSERVAÇÃO:__ `bot prepare-publish` ainda usa o padrão antigo</span><span class="sxs-lookup"><span data-stu-id="82786-506">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="82786-507">[ALTERAÇÃO SIGNIFICATIVA] `--lang` foi alterado para não definir mais `Csharp` como padrão.</span><span class="sxs-lookup"><span data-stu-id="82786-507">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="82786-508">Se o comando exigir `--lang` e ele não for fornecido, o comando será um erro</span><span class="sxs-lookup"><span data-stu-id="82786-508">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="82786-509">[ALTERAÇÃO SIGNIFICATIVA] Os argumentos `--appid` e `--password` foram alterados para `bot create` ser obrigatório e agora podem ser criados por meio de `ad app create`</span><span class="sxs-lookup"><span data-stu-id="82786-509">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="82786-510">Foi adicionada validação a `--appid` e `--password`</span><span class="sxs-lookup"><span data-stu-id="82786-510">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="82786-511">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4` foi alterado para não criar ou usar uma Conta de Armazenamento ou o Application Insights</span><span class="sxs-lookup"><span data-stu-id="82786-511">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="82786-512">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v3` foi alterado para exigir uma região em que o Application Insights está disponível</span><span class="sxs-lookup"><span data-stu-id="82786-512">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="82786-513">[ALTERAÇÃO SIGNIFICATIVA] O `bot update` foi alterado para afetar somente as propriedades específicas de um bot</span><span class="sxs-lookup"><span data-stu-id="82786-513">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="82786-514">[ALTERAÇÃO SIGNIFICATIVA] Os sinalizadores `--lang` foram alterados para aceitar `Javascript` em vez de `Node`</span><span class="sxs-lookup"><span data-stu-id="82786-514">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="82786-515">[ALTERAÇÃO SIGNIFICATIVA] O `Node` foi removido como um valor `--lang` permitido</span><span class="sxs-lookup"><span data-stu-id="82786-515">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="82786-516">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para não definir mais `SCM_DO_BUILD_DURING_DEPLOYMENT` como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="82786-516">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="82786-517">Todas as implantações por meio do Kudu atuarão de acordo com o comportamento padrão</span><span class="sxs-lookup"><span data-stu-id="82786-517">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="82786-518">O `bot download` foi alterado para os bots sem arquivos `.bot` para criar o arquivo de configuração específico a um idioma com os valores das Configurações de Aplicativo do bot</span><span class="sxs-lookup"><span data-stu-id="82786-518">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="82786-519">Adicionado o suporte `Typescript` para `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="82786-519">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="82786-520">Uma mensagem de aviso foi adicionada a `bot prepare-deploy` para os bots `Javascript` e `Typescript` para quando `--code-dir` não contiver `package.json`</span><span class="sxs-lookup"><span data-stu-id="82786-520">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="82786-521">O `bot prepare-deploy` foi alterado para retornar `true`, se bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="82786-521">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="82786-522">O log detalhado foi adicionado a `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="82786-522">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="82786-523">Mais regiões disponíveis do Application Insights foram adicionadas ao `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="82786-523">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="82786-524">Configurar</span><span class="sxs-lookup"><span data-stu-id="82786-524">Configure</span></span>
* <span data-ttu-id="82786-525">Adicionado suporte para configurações de valor padrão do argumento baseado em pasta</span><span class="sxs-lookup"><span data-stu-id="82786-525">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="82786-526">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="82786-526">Eventhubs</span></span>
* <span data-ttu-id="82786-527">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="82786-527">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="82786-528">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-528">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="82786-529">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-529">Network</span></span>
* <span data-ttu-id="82786-530">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--cache` foi substituído por `--defer` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-530">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="82786-531">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="82786-531">Policy Insights</span></span>
* <span data-ttu-id="82786-532">Suporte adicionado a `--expand PolicyEvaluationDetails` para detalhes de avaliação de política de consulta no recurso</span><span class="sxs-lookup"><span data-stu-id="82786-532">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="82786-533">Função</span><span class="sxs-lookup"><span data-stu-id="82786-533">Role</span></span>
* <span data-ttu-id="82786-534">[PRETERIDO] Alterado argumento ocultar '--password' `create-for-rbac` - suporte será removido em maio de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-534">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="82786-535">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="82786-535">Service Bus</span></span>
* <span data-ttu-id="82786-536">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="82786-536">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="82786-537">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-537">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="82786-538">`topic [create|update]` foi fixado para permitir suporte a `--max-size` para valores de 10, 20, 40 e 80 GB com a SKU Premium</span><span class="sxs-lookup"><span data-stu-id="82786-538">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="82786-539">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-539">SQL</span></span>
* <span data-ttu-id="82786-540">Adicionados os comandos `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="82786-540">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="82786-541">VM</span><span class="sxs-lookup"><span data-stu-id="82786-541">VM</span></span>
* <span data-ttu-id="82786-542">O `--protect-from-scale-in` e o `--protect-from-scale-set-actions` foram adicionados a `vmss update` para habilitar atualizações à política de proteção das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="82786-542">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="82786-543">Adicionado a `--instance-id` e `vmss update` para habilitar atualização genérica das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="82786-543">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="82786-544">`--instance-id` foi adicionado a `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="82786-544">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="82786-545">Adicionado um novo grupo de comandos `ppg` para gerenciar grupos de posicionamento de proximidade</span><span class="sxs-lookup"><span data-stu-id="82786-545">Added new `ppg` command group for manging Proximity Placement Groups</span></span>
* <span data-ttu-id="82786-546">Adicionado a `--ppg`, `[vm|vmss] create` e `vm availability-set create` para gerenciar PPGs</span><span class="sxs-lookup"><span data-stu-id="82786-546">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="82786-547">Parâmetro `--hyper-v-generation` adicionado a `image create`</span><span class="sxs-lookup"><span data-stu-id="82786-547">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="82786-548">23 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-548">April 23, 2019</span></span>

<span data-ttu-id="82786-549">Versão 2.0.63</span><span class="sxs-lookup"><span data-stu-id="82786-549">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="82786-550">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-550">ACS</span></span>
* <span data-ttu-id="82786-551">Alterado `aks get-credentials` para solicitar substituição dos valores duplicados</span><span class="sxs-lookup"><span data-stu-id="82786-551">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="82786-552">Removido `(PREVIEW)` dos comandos de espaços de desenvolvimento "aks use-dev-espaces" e "aks remove-dev-espaces"</span><span class="sxs-lookup"><span data-stu-id="82786-552">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="82786-553">AMS</span><span class="sxs-lookup"><span data-stu-id="82786-553">AMS</span></span>
* <span data-ttu-id="82786-554">Corrigido o bug com a atualização de filtros de conta e de ativo</span><span class="sxs-lookup"><span data-stu-id="82786-554">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-555">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-555">AppService</span></span>
* <span data-ttu-id="82786-556">Adicionado suporte para o ASE e o tempo limite para `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="82786-556">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="82786-557">Adicionado suporte para o estabelecimento de CI CD em um pipeline do Azure DevOps de um repositório do Github para aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="82786-557">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="82786-558">Adicionado argumento `--github-pat` a `functionapp devops-build create` para aceitar o token de acesso pessoal do Github</span><span class="sxs-lookup"><span data-stu-id="82786-558">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="82786-559">Adicionado argumento `--github-repository` a `functionapp devops-build create` para aceitar o repositório Github que contém um código-fonte functionapp</span><span class="sxs-lookup"><span data-stu-id="82786-559">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="82786-560">Problema corrigido em que `az webapp up --logs` estava falhando com um erro e atualização da versão .NETCORE padrão para 2.1</span><span class="sxs-lookup"><span data-stu-id="82786-560">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="82786-561">Configurações de functionapp desnecessárias removidas durante a criação de um aplicativo de funções com plano de consumo</span><span class="sxs-lookup"><span data-stu-id="82786-561">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="82786-562">Alterado `webapp up` para que a cadeia de caracteres padrão asp agora acrescente o número no final para criar um novo ASP com base nas opções de SKU</span><span class="sxs-lookup"><span data-stu-id="82786-562">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="82786-563">Adicionado `-b` como uma opção a `webapp up` para iniciar o aplicativo no navegador</span><span class="sxs-lookup"><span data-stu-id="82786-563">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="82786-564">Alterado `webapp deployment source config zip` para lidar com a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="82786-564">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="82786-565">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="82786-565">Deployment Manager</span></span>
* <span data-ttu-id="82786-566">[VERSÃO PRÉVIA] Criar e gerenciar artefatos que dão suporte a distribuições</span><span class="sxs-lookup"><span data-stu-id="82786-566">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="82786-567">Laboratório</span><span class="sxs-lookup"><span data-stu-id="82786-567">Lab</span></span>
* <span data-ttu-id="82786-568">Corrigido o bug que causa uma saída inicial</span><span class="sxs-lookup"><span data-stu-id="82786-568">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="82786-569">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-569">Network</span></span>
* <span data-ttu-id="82786-570">Adicionada delegação de servidor de nome automática a `dns zone create` no pai durante a criação da zona filho</span><span class="sxs-lookup"><span data-stu-id="82786-570">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="82786-571">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-571">Resource</span></span>
* <span data-ttu-id="82786-572">[PRETERIDO] Argumentos `--link-id`, `--target-id` e `--filter-string` preteridos de `resource link`</span><span class="sxs-lookup"><span data-stu-id="82786-572">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="82786-573">Use os argumentos `--link`, `--target` e `--filter`</span><span class="sxs-lookup"><span data-stu-id="82786-573">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="82786-574">Corrigido o problema em que os comandos `resource link [create|update]` não funcionavam</span><span class="sxs-lookup"><span data-stu-id="82786-574">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="82786-575">Corrigido um problema em que a exclusão usando uma ID de recurso poderia causar falha no erro</span><span class="sxs-lookup"><span data-stu-id="82786-575">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="82786-576">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-576">SQL</span></span>
* <span data-ttu-id="82786-577">Adicionado suporte para fuso horário personalizado nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="82786-577">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="82786-578">Alterado para permitir que o nome do pool Elástico seja usado com `sql db update`</span><span class="sxs-lookup"><span data-stu-id="82786-578">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="82786-579">Adicionado o suporte `--no-wait` para `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-579">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="82786-580">Adicionado o comando `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="82786-580">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="82786-581">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-581">Storage</span></span>
* <span data-ttu-id="82786-582">Corrigido o problema com tokens SAS com codificação dupla em `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="82786-582">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="82786-583">VM</span><span class="sxs-lookup"><span data-stu-id="82786-583">VM</span></span>
* <span data-ttu-id="82786-584">Adicionado sinalizador `--skip-shutdown` a `vm|vmss stop` para desligar as VMs sem o desligamento</span><span class="sxs-lookup"><span data-stu-id="82786-584">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="82786-585">Adicionado argumento `--storage-account-type` a `sig image-version create` para definir o tipo de conta do perfil de publicação</span><span class="sxs-lookup"><span data-stu-id="82786-585">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="82786-586">Adicionado argumento `--target-regions` a `sig image-version create` para permitir definir os tipos de conta de armazenamento específico da região</span><span class="sxs-lookup"><span data-stu-id="82786-586">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="82786-587">9 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-587">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="82786-588">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-588">Core</span></span>
* <span data-ttu-id="82786-589">Correção do problema em que algumas extensões mostraram uma versão do `Unknown` e não podiam ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="82786-589">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="82786-590">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-590">ACR</span></span>
* <span data-ttu-id="82786-591">Adição de suporte para execução de uma imagem sem contexto</span><span class="sxs-lookup"><span data-stu-id="82786-591">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="82786-592">AMS</span><span class="sxs-lookup"><span data-stu-id="82786-592">AMS</span></span>
* [PRETERIDO]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [ALTERAÇÃO SIGNIFICATIVA]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="82786-595">Adição de suporte para novos parâmetros de criptografia em `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="82786-595">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="82786-596">Adição de novo parâmetro `--filters` a `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="82786-596">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-597">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-597">AppService</span></span>
* <span data-ttu-id="82786-598">Adicionado o suporte `--logs` para `webapp up`</span><span class="sxs-lookup"><span data-stu-id="82786-598">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="82786-599">Correção de problemas do comando `functionapp devops-build create` de geração de `azure-pipelines.yml`</span><span class="sxs-lookup"><span data-stu-id="82786-599">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="82786-600">Melhoria do tratamento de erros e indicadores `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="82786-600">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="82786-601">[ALTERAÇÃO SIGNIFICATIVA] Remoção do sinalizador `--local-git` para o comando `devops-build`; a detecção de git local e a manipulação são obrigatórias para a criação de pipelines do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="82786-601">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="82786-602">Adição de suporte para a criação de planos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="82786-602">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="82786-603">Adição da capacidade de trocar um plano sob um aplicativo de funções usando `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="82786-603">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="82786-604">Adição de suporte para configurações de expansão de plano Premium do Azure Functions</span><span class="sxs-lookup"><span data-stu-id="82786-604">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="82786-605">CDN</span><span class="sxs-lookup"><span data-stu-id="82786-605">CDN</span></span>
* <span data-ttu-id="82786-606">Adição de suporte para `Microsoft_Standard` e `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="82786-606">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="82786-607">Comentários</span><span class="sxs-lookup"><span data-stu-id="82786-607">Feedback</span></span>
* <span data-ttu-id="82786-608">Alteração de `feedback` para mostrar metadados em comandos executados recentemente</span><span class="sxs-lookup"><span data-stu-id="82786-608">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="82786-609">Alteração de `feedback` para solicitar o auxílio do usuário no processo de criação de problema abrindo um navegador e usando um modelo de problema</span><span class="sxs-lookup"><span data-stu-id="82786-609">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="82786-610">Alteração do `feedback` para imprimir o corpo do problema ao executar com '--verbose'</span><span class="sxs-lookup"><span data-stu-id="82786-610">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="82786-611">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="82786-611">Monitor</span></span>
* <span data-ttu-id="82786-612">Correção de um problema em que “count” não era um valor permitido com `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-612">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="82786-613">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-613">Network</span></span>
* <span data-ttu-id="82786-614">Correção do formato de tabela que não estava sendo exibido com `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="82786-614">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="82786-615">Adição dos comandos `list-request-headers` e `list-response-headers` para `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="82786-615">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="82786-616">Adição do comando `list-server-variables` para `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="82786-616">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="82786-617">Correção de um problema em que a atualização do estado do link em uma porta express-route geraria uma exceção de atributo desconhecido `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="82786-617">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="82786-618">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="82786-618">PrivateDNS</span></span>
* <span data-ttu-id="82786-619">Adição de `network private-dns` para zonas de DNS privado</span><span class="sxs-lookup"><span data-stu-id="82786-619">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="82786-620">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-620">Resource</span></span>
* <span data-ttu-id="82786-621">Correção do problema com `deployment create` e `group deployment create`, em que um arquivo de parâmetros com um conjunto vazio de parâmetros não funcionaria</span><span class="sxs-lookup"><span data-stu-id="82786-621">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="82786-622">Função</span><span class="sxs-lookup"><span data-stu-id="82786-622">Role</span></span>
* <span data-ttu-id="82786-623">Correção de `create-for-rbac` para lidar corretamente com `--years`</span><span class="sxs-lookup"><span data-stu-id="82786-623">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="82786-624">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `role assignment delete` para solicitar ao excluir todas as atribuições na assinatura incondicionalmente</span><span class="sxs-lookup"><span data-stu-id="82786-624">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="82786-625">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-625">SQL</span></span>
* <span data-ttu-id="82786-626">Atualização de `sql mi [create|update]` com as propriedades proxyOverride e publicDataEndpointEnabled</span><span class="sxs-lookup"><span data-stu-id="82786-626">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="82786-627">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-627">Storage</span></span>
* <span data-ttu-id="82786-628">[ALTERAÇÃO SIGNIFICATIVA] Remoção do resultado de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="82786-628">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="82786-629">Adição de `--full-uri` a `storage blob generate-sas` para criar o URI completo para o blob com SAS</span><span class="sxs-lookup"><span data-stu-id="82786-629">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="82786-630">Adição de `--file-snapshot` a `storage file copy start` para copiar arquivo do instantâneo</span><span class="sxs-lookup"><span data-stu-id="82786-630">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="82786-631">Alteração de `storage blob copy cancel` para mostrar apenas o erro em vez da exceção para NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="82786-631">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="82786-632">26 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-632">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="82786-633">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-633">Core</span></span>
* <span data-ttu-id="82786-634">Correção de problemas com incompatibilidade da extensão de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="82786-634">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="82786-635">Agora o tratamento de erros encaminha os clientes para a página de problemas</span><span class="sxs-lookup"><span data-stu-id="82786-635">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="82786-636">Nuvem</span><span class="sxs-lookup"><span data-stu-id="82786-636">Cloud</span></span>
* <span data-ttu-id="82786-637">Erro de “assinatura não encontrada” corrigido em `cloud set`</span><span class="sxs-lookup"><span data-stu-id="82786-637">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="82786-638">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-638">ACR</span></span>
* <span data-ttu-id="82786-639">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="82786-639">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="82786-640">`--auth-mode` adicionado aos comandos `acr build`, `acr run`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="82786-640">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="82786-641">Grupo de comandos “acr task credential” adicionado para gerenciar as credenciais de uma Tarefa</span><span class="sxs-lookup"><span data-stu-id="82786-641">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="82786-642">“--no-wait” adicionado ao comando `acr build`</span><span class="sxs-lookup"><span data-stu-id="82786-642">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-643">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-643">AppService</span></span>
* <span data-ttu-id="82786-644">Bug corrigido onde `webapp up` não estava lidando corretamente com a execução do diretório vazio ou do cenário de código desconhecido</span><span class="sxs-lookup"><span data-stu-id="82786-644">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="82786-645">Bug corrigido onde os slots não funcionavam para `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="82786-645">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="82786-646">Serviço de BOT</span><span class="sxs-lookup"><span data-stu-id="82786-646">BOT Service</span></span>
* <span data-ttu-id="82786-647">`bot prepare-deploy` adicionado para se preparar para a implantação de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="82786-647">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="82786-648">`bot create --kind registration` alterado para mostrar a senha se ela não for fornecida</span><span class="sxs-lookup"><span data-stu-id="82786-648">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="82786-649">[ALTERAÇÃO SIGNIFICATIVA] `--endpoint` alterado em `bot create --kind registration` como padrão para uma cadeia de caracteres vazia, em vez de ser requerido</span><span class="sxs-lookup"><span data-stu-id="82786-649">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="82786-650">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="82786-650">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="82786-651">CDN</span><span class="sxs-lookup"><span data-stu-id="82786-651">CDN</span></span>
* <span data-ttu-id="82786-652">Adicionado o suporte ao `--no-wait` para `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="82786-652">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [ALTERAÇÃO SIGNIFICATIVA]: `cdn endpoint create` alterado para o comportamento de cache da cadeia de consulta padrão.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="82786-654">Não há mais padrão para "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="82786-654">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="82786-655">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="82786-655">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82786-656">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="82786-656">Cosmosdb</span></span>
* <span data-ttu-id="82786-657">Suporte adicionado para `--enable-multiple-write-locations` na atualização da conta</span><span class="sxs-lookup"><span data-stu-id="82786-657">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="82786-658">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82786-658">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="82786-659">Interativo</span><span class="sxs-lookup"><span data-stu-id="82786-659">Interactive</span></span>
* <span data-ttu-id="82786-660">Incompatibilidade corrigida com a extensão Interativa instalada por meio do azdev</span><span class="sxs-lookup"><span data-stu-id="82786-660">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="82786-661">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="82786-661">Monitor</span></span>
* <span data-ttu-id="82786-662">Alterado para permitir o valor de dimensão `*` para `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-662">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="82786-663">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-663">Network</span></span>
* <span data-ttu-id="82786-664">Grupo de comandos `rewrite-rule` adicionado em `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="82786-664">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="82786-665">Perfil</span><span class="sxs-lookup"><span data-stu-id="82786-665">Profile</span></span>
* <span data-ttu-id="82786-666">Suporte de conta no nível do locatário para a identidade de serviço gerenciado adicionado em `login`</span><span class="sxs-lookup"><span data-stu-id="82786-666">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="82786-667">Postgres</span><span class="sxs-lookup"><span data-stu-id="82786-667">Postgres</span></span> 
* <span data-ttu-id="82786-668">Adicionados os comandos postgresql `replica` e `restart server`</span><span class="sxs-lookup"><span data-stu-id="82786-668">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="82786-669">Alterado para obter o local padrão do grupo de recursos quando não fornecido para criar servidores e adicionar validação para os dias de retenção</span><span class="sxs-lookup"><span data-stu-id="82786-669">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="82786-670">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-670">Resource</span></span>
* <span data-ttu-id="82786-671">Saída da tabela aperfeiçoada para `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="82786-671">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="82786-672">Corrigido o problema com `deployment [create|validate]` onde o tipo secureObject não era reconhecido</span><span class="sxs-lookup"><span data-stu-id="82786-672">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="82786-673">Grafo</span><span class="sxs-lookup"><span data-stu-id="82786-673">Graph</span></span>
* <span data-ttu-id="82786-674">Adicionado o suporte ao `--end-date` para `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="82786-674">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="82786-675">Suporte adicionado para acrescentar permissões com `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="82786-675">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="82786-676">Bug corrigido com `ad app permission list` quando não havia nenhuma permissão</span><span class="sxs-lookup"><span data-stu-id="82786-676">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="82786-677">`ad sp delete` alterado para ignorar a exclusão da atribuição de função se a conta atual não tem nenhuma assinatura</span><span class="sxs-lookup"><span data-stu-id="82786-677">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="82786-678">`ad app create` alterado para `--identifier-uris` passar para lista vazia como padrão se não fornecido</span><span class="sxs-lookup"><span data-stu-id="82786-678">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="82786-679">storage</span><span class="sxs-lookup"><span data-stu-id="82786-679">storage</span></span>
* <span data-ttu-id="82786-680">`--snapshot` adicionado a `storage file download-batch` para baixar de um instantâneo de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="82786-680">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="82786-681">Barra de progresso `storage blob [download-batch|upload-batch]` alterada para ser menos detalhada e indicar o blob atual</span><span class="sxs-lookup"><span data-stu-id="82786-681">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="82786-682">Problema corrigido com `storage account update` ao atualizar os parâmetros de criptografia</span><span class="sxs-lookup"><span data-stu-id="82786-682">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="82786-683">Problema corrigido onde `storage blob show` falharia ao usar o oauth (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="82786-683">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="82786-684">VM</span><span class="sxs-lookup"><span data-stu-id="82786-684">VM</span></span>
* <span data-ttu-id="82786-685">Adicionado o comando `image update`</span><span class="sxs-lookup"><span data-stu-id="82786-685">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="82786-686">12 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-686">March 12, 2019</span></span>

<span data-ttu-id="82786-687">Versão 2.0.60</span><span class="sxs-lookup"><span data-stu-id="82786-687">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="82786-688">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-688">Core</span></span>

* <span data-ttu-id="82786-689">Foi corrigido um erro incorreto no `cloud set` sobre assinatura não encontrada.</span><span class="sxs-lookup"><span data-stu-id="82786-689">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="82786-690">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-690">ACR</span></span>

* <span data-ttu-id="82786-691">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="82786-691">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="82786-692">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-692">ACS</span></span>

* <span data-ttu-id="82786-693">Alteração para ignorar o parâmetro `--listen-address` para `aks browse` se ele não for compatível com kubectl</span><span class="sxs-lookup"><span data-stu-id="82786-693">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="82786-694">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-694">AppService</span></span>

* <span data-ttu-id="82786-695">Adicionado `[webapp|functionapp] deployment list-publishing-credentials` para obter a URL de publicação do Kudu e suas credenciais.</span><span class="sxs-lookup"><span data-stu-id="82786-695">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="82786-696">Removida a instrução de impressão errônea de `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="82786-696">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="82786-697">Corrigido `functionapp` para definir a imagem correta do tempo de execução nos planos do Serviço de Aplicativo no Linux.</span><span class="sxs-lookup"><span data-stu-id="82786-697">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="82786-698">Removida a marca de versão prévia do `webapp up` e adicionadas melhorias ao comando.</span><span class="sxs-lookup"><span data-stu-id="82786-698">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="82786-699">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="82786-699">Botservice</span></span>

* <span data-ttu-id="82786-700">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="82786-700">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="82786-701">Adicionados `Microsoft-BotFramework-AppId` e `Microsoft-BotFramework-AppPassword` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="82786-701">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="82786-702">Removidas as aspas simples da saída de comando `bot publish`, no final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="82786-702">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="82786-703">Alterado `bot publish` para que seja assíncrono.</span><span class="sxs-lookup"><span data-stu-id="82786-703">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="82786-704">Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-704">Container</span></span>

* <span data-ttu-id="82786-705">Adicionado o argumento `--no-wait` para `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="82786-705">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="82786-706">EventHub</span><span class="sxs-lookup"><span data-stu-id="82786-706">EventHub</span></span>

* <span data-ttu-id="82786-707">Adicionado o sinalizador `--skip-empty-archives` a `eventhub create|update` para dar suporte a arquivos vazios na captura.</span><span class="sxs-lookup"><span data-stu-id="82786-707">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="82786-708">Localizar</span><span class="sxs-lookup"><span data-stu-id="82786-708">Find</span></span>

* <span data-ttu-id="82786-709">Atualização de funcionalidade principal</span><span class="sxs-lookup"><span data-stu-id="82786-709">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="82786-710">HDInsight</span><span class="sxs-lookup"><span data-stu-id="82786-710">HDInsight</span></span>

* <span data-ttu-id="82786-711">Adicionado o parâmetro `--storage-account-managed-identity` a `hdinsight create` para oferecer suporte ao MSI do ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="82786-711">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="82786-712">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-712">Network</span></span>

* <span data-ttu-id="82786-713">Corrigido o problema com `vpn-connection update`, onde a atualização de uma conexão VPN entre gateways em assinaturas diferentes falharia.</span><span class="sxs-lookup"><span data-stu-id="82786-713">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="82786-714">Rdbms</span><span class="sxs-lookup"><span data-stu-id="82786-714">Rdbms</span></span>

* <span data-ttu-id="82786-715">Correções secundárias para obter a localização padrão do grupo de recursos, quando não fornecida, para criar servidores e adicionar validação nos dias de retenção.</span><span class="sxs-lookup"><span data-stu-id="82786-715">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="82786-716">Função</span><span class="sxs-lookup"><span data-stu-id="82786-716">Role</span></span>

* <span data-ttu-id="82786-717">Corrigido `role definition update` para usar ID a fim de resolver a definição corretamente.</span><span class="sxs-lookup"><span data-stu-id="82786-717">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="82786-718">Alterado `ad app credential reset` para remover a suposição de que a entidade de serviço do aplicativo já existe.</span><span class="sxs-lookup"><span data-stu-id="82786-718">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="82786-719">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="82786-719">Service Fabric</span></span>

* <span data-ttu-id="82786-720">Corrigido o problema com o fato de `sf cluster list` não ser iterável.</span><span class="sxs-lookup"><span data-stu-id="82786-720">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="82786-721">26 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-721">February 26, 2019</span></span>

<span data-ttu-id="82786-722">Versão 2.0.59</span><span class="sxs-lookup"><span data-stu-id="82786-722">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="82786-723">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-723">Core</span></span>

* <span data-ttu-id="82786-724">Corrigido o problema onde algumas instâncias usando `--subscription NAME` produziriam uma exceção</span><span class="sxs-lookup"><span data-stu-id="82786-724">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="82786-725">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-725">ACR</span></span>

* <span data-ttu-id="82786-726">Parâmetro `--target` adicionado para os comandos `acr build`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="82786-726">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="82786-727">Melhor tratamento de erros para os comandos de execução quando não conectado ao Azure</span><span class="sxs-lookup"><span data-stu-id="82786-727">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="82786-728">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-728">ACS</span></span>

* <span data-ttu-id="82786-729">Opção `--listen-address` adicionada a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="82786-729">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-730">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-730">AppService</span></span>

* <span data-ttu-id="82786-731">Adicionado o comando `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="82786-731">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="82786-732">Lote</span><span class="sxs-lookup"><span data-stu-id="82786-732">Batch</span></span>
* <span data-ttu-id="82786-733">[ALTERAÇÃO SIGNIFICATIVA] Comando `batch pool upgrade os` removido</span><span class="sxs-lookup"><span data-stu-id="82786-733">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="82786-734">[ALTERAÇÃO SIGNIFICATIVA] Propriedade `Pacakges` removida das respostas `Application`</span><span class="sxs-lookup"><span data-stu-id="82786-734">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="82786-735">Comando `batch application package list` adicionado para listar os pacotes de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="82786-735">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="82786-736">[ALTERAÇÃO SIGNIFICATIVA] `--application-id` alterado para `--application-name` em todos os comandos `batch application`,</span><span class="sxs-lookup"><span data-stu-id="82786-736">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="82786-737">O argumento `--json-file` foi adicionado aos comandos para a solicitação de resposta da API bruta</span><span class="sxs-lookup"><span data-stu-id="82786-737">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="82786-738">Validação atualizada para incluir automaticamente `https://` em todos os pontos de extremidade, se ausente</span><span class="sxs-lookup"><span data-stu-id="82786-738">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82786-739">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="82786-739">CosmosDB</span></span>

* <span data-ttu-id="82786-740">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82786-740">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="82786-741">Kusto</span><span class="sxs-lookup"><span data-stu-id="82786-741">Kusto</span></span>

* <span data-ttu-id="82786-742">[ALTERAÇÃO SIGNIFICATIVA] Os tipos `hot_cache_period` e `soft_delete_period` foram alterados do banco de dados para o formato de duração ISO8601</span><span class="sxs-lookup"><span data-stu-id="82786-742">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="82786-743">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-743">Network</span></span>

* <span data-ttu-id="82786-744">Adicionado o argumento `--express-route-gateway-bypass` para `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-744">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="82786-745">Foram adicionados os grupos de comando a partir das extensões `express-route`</span><span class="sxs-lookup"><span data-stu-id="82786-745">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="82786-746">Os grupos de comando `express-route gateway` e `express-route port` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="82786-746">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="82786-747">Adicionado o argumento `--legacy-mode` para `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-747">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="82786-748">Os argumentos `--allow-classic-operations` e `--express-route-port` foram adicionados a `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-748">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="82786-749">Adicionado o argumento `--gateway-default-site` para `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-749">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="82786-750">Os comandos `ipsec-policy` foram adicionados a `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="82786-750">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="82786-751">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-751">Resource</span></span>

* <span data-ttu-id="82786-752">Foi corrigido o problema com `deployment create` em que o campo do tipo diferencia letras maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="82786-752">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="82786-753">Foi adicionado o suporte para arquivo de parâmetros de URI a `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="82786-753">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="82786-754">Foi adicionado o suporte para parâmetros de URI e definições a `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="82786-754">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="82786-755">Foi corrigido o tratamento de parâmetros e regras para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="82786-755">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="82786-756">Foi corrigido o problema com `resource show/update/delete/tag/invoke-action` em que as IDs de assinatura cruzada não respeitaram corretamente a ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="82786-756">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="82786-757">Função</span><span class="sxs-lookup"><span data-stu-id="82786-757">Role</span></span>

* <span data-ttu-id="82786-758">Foi adicionado o suporte para as funções do aplicativo a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-758">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="82786-759">VM</span><span class="sxs-lookup"><span data-stu-id="82786-759">VM</span></span>

* <span data-ttu-id="82786-760">Foi corrigido o problema com `vm create where ` – a rede acelerada não foi habilitada por padrão no Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="82786-760">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="82786-761">12 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-761">February 12, 2019</span></span>

<span data-ttu-id="82786-762">Versão 2.0.58</span><span class="sxs-lookup"><span data-stu-id="82786-762">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="82786-763">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-763">Core</span></span>

* <span data-ttu-id="82786-764">`az --version` agora exibe uma notificação se você tiver pacotes para atualização</span><span class="sxs-lookup"><span data-stu-id="82786-764">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="82786-765">A regressão em que `--ids` não pode ser usado com a saída JSON foi corrigida</span><span class="sxs-lookup"><span data-stu-id="82786-765">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="82786-766">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-766">ACR</span></span>
* <span data-ttu-id="82786-767">[ALTERAÇÃO SIGNIFICATIVA] O grupo de comandos `acr build-task` foi removido</span><span class="sxs-lookup"><span data-stu-id="82786-767">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="82786-768">[ALTERAÇÃO SIGNIFICATIVA] As opções `--tag` e `--manifest` de `acr repository delete` foram removidas</span><span class="sxs-lookup"><span data-stu-id="82786-768">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="82786-769">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-769">ACS</span></span>
* <span data-ttu-id="82786-770">Suporte adicionado a `aks [enable-addons|disable-addons]` para nomes que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="82786-770">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="82786-771">Suporte adicionado para a operação de atualização do Azure Active Directory usando `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="82786-771">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="82786-772">Um esclarecimento informando que `--output` é ignorado para `aks get-credentials` foi adicionado</span><span class="sxs-lookup"><span data-stu-id="82786-772">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="82786-773">AMS</span><span class="sxs-lookup"><span data-stu-id="82786-773">AMS</span></span>
* <span data-ttu-id="82786-774">Adicionados os comandos `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="82786-774">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="82786-775">Adicionados os comandos `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="82786-775">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-776">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-776">Appservice</span></span>
* <span data-ttu-id="82786-777">Foi adicionada a capacidade de criar e configurar funções usando contêineres de ACR</span><span class="sxs-lookup"><span data-stu-id="82786-777">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="82786-778">Suporte adicionado para a atualização das configurações de aplicativos Web por meio de JSON</span><span class="sxs-lookup"><span data-stu-id="82786-778">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="82786-779">A ajuda foi aprimorada para `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="82786-779">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="82786-780">Suporte adicionado para o App Insights para auxiliar na criação de aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="82786-780">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="82786-781">Os problemas com o SSH do aplicativo Web foram corrigidos</span><span class="sxs-lookup"><span data-stu-id="82786-781">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="82786-782">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="82786-782">Botservice</span></span>
* <span data-ttu-id="82786-783">A experiência do usuário para `bot publish` foi aprimorada</span><span class="sxs-lookup"><span data-stu-id="82786-783">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="82786-784">Foram adicionados avisos de tempos limite ao executar `npm install` durante `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="82786-784">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="82786-785">O caractere inválido `.` de `--name` em `az bot create` foi removido</span><span class="sxs-lookup"><span data-stu-id="82786-785">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="82786-786">Alteração para interromper a geração aleatória de nomes de recursos durante a criação do Armazenamento do Azure, Plano do Serviço de Aplicativo, Aplicativo Web/de funções e Application Insights</span><span class="sxs-lookup"><span data-stu-id="82786-786">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="82786-787">[PRETERIDO] O argumento `--proj-name` foi preterido em favor de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="82786-787">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="82786-788">`az bot publish` foi alterado para remover arquivos de implantação do Node.js do IIS buscados, caso eles já não existissem</span><span class="sxs-lookup"><span data-stu-id="82786-788">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="82786-789">Foi adicionado o argumento `--keep-node-modules` para `az bot publish` para não excluir a pasta `node_modules` no Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82786-789">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="82786-790">O par chave-valor `"publishCommand"` foi adicionado à saída de `az bot create` durante a criação de uma função do Azure ou bot de aplicativo Web</span><span class="sxs-lookup"><span data-stu-id="82786-790">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="82786-791">O valor de `"publishCommand"` é um comando `az bot publish` que é automaticamente preenchido com os parâmetros necessários para publicar o bot recém-criado</span><span class="sxs-lookup"><span data-stu-id="82786-791">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="82786-792">O `"WEBSITE_NODE_DEFAULT_VERSION"` foi atualizado no modelo do ARM para que os bots de SDK v4 usem 10.14.1 em vez de 8.9.4</span><span class="sxs-lookup"><span data-stu-id="82786-792">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="82786-793">Key Vault</span><span class="sxs-lookup"><span data-stu-id="82786-793">Key Vault</span></span>
* <span data-ttu-id="82786-794">Foi corrigido o problema com `keyvault secret backup`, em que alguns usuários recebiam um erro `unexpected_keyword` ao usar `--id`</span><span class="sxs-lookup"><span data-stu-id="82786-794">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="82786-795">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="82786-795">Monitor</span></span>
* <span data-ttu-id="82786-796">`monitor metrics alert [create|update]` foi alterado para permitir o valor dimensional `*`</span><span class="sxs-lookup"><span data-stu-id="82786-796">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="82786-797">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-797">Network</span></span>
* <span data-ttu-id="82786-798">`dns zone export` foi alterado para garantir que CNAMEs exportados fossem FQDNs</span><span class="sxs-lookup"><span data-stu-id="82786-798">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="82786-799">O parâmetro `--gateway-name` foi adicionado a `nic ip-config address-pool [add|remove]` para dar suporte a pools de endereços de back-end de gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="82786-799">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="82786-800">Os argumentos `--traffic-analytics` e `--workspace` foram adicionados a `network watcher flow-log configure` para dar suporte à análise de tráfego por meio de um espaço de trabalho do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="82786-800">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="82786-801">`--idle-timeout` e `--floating-ip` foram adicionados a `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-801">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="82786-802">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="82786-802">Policy Insights</span></span>
* <span data-ttu-id="82786-803">Os comandos `policy remediation` foram adicionados para dar suporte a recursos de correção de política de recursos</span><span class="sxs-lookup"><span data-stu-id="82786-803">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="82786-804">RDBMS</span><span class="sxs-lookup"><span data-stu-id="82786-804">RDBMS</span></span>
* <span data-ttu-id="82786-805">A mensagem e os parâmetros de comando de ajuda foram aprimorados</span><span class="sxs-lookup"><span data-stu-id="82786-805">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="82786-806">Redis</span><span class="sxs-lookup"><span data-stu-id="82786-806">Redis</span></span>
* <span data-ttu-id="82786-807">Foram adicionados comandos para gerenciar regras de firewall (criar, atualizar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="82786-807">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="82786-808">Foram adicionados comandos para gerenciar links do servidor (criar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="82786-808">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="82786-809">Foram adicionados comandos para gerenciar o agendamento de patches (criar, atualizar, excluir, mostrar)</span><span class="sxs-lookup"><span data-stu-id="82786-809">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="82786-810">Suporte adicionado para Zonas de Disponibilidade e versão mínima de TLS para criar Redis</span><span class="sxs-lookup"><span data-stu-id="82786-810">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="82786-811">[ALTERAÇÃO SIGNIFICATIVA] Os comandos `redis update-settings` e `redis list-all` foram removidos</span><span class="sxs-lookup"><span data-stu-id="82786-811">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="82786-812">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro para `redis create`: “configurações de locatário” não é aceito no formato chave[=valor]</span><span class="sxs-lookup"><span data-stu-id="82786-812">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="82786-813">[PRETERIDO] Uma mensagem de aviso foi adicionada para preterir o comando `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="82786-813">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="82786-814">Função</span><span class="sxs-lookup"><span data-stu-id="82786-814">Role</span></span>
* <span data-ttu-id="82786-815">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido dos comandos `vm` para esta localização</span><span class="sxs-lookup"><span data-stu-id="82786-815">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="82786-816">SQL VM</span><span class="sxs-lookup"><span data-stu-id="82786-816">SQL VM</span></span>
* <span data-ttu-id="82786-817">[PRETERIDO] O argumento `--boostrap-acc-pwd` foi preterido devido a um erro de digitação</span><span class="sxs-lookup"><span data-stu-id="82786-817">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="82786-818">VM</span><span class="sxs-lookup"><span data-stu-id="82786-818">VM</span></span>
* <span data-ttu-id="82786-819">`vm list-skus` foi alterado para permitir o uso de `--all` no lugar de `--all true`</span><span class="sxs-lookup"><span data-stu-id="82786-819">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="82786-820">Adicionado `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="82786-820">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="82786-821">Foi corrigido o bug em que `vmss encryption enable` falhava se fosse executado anteriormente</span><span class="sxs-lookup"><span data-stu-id="82786-821">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="82786-822">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido para os comandos `role`</span><span class="sxs-lookup"><span data-stu-id="82786-822">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="82786-823">31 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-823">January 31, 2019</span></span>

<span data-ttu-id="82786-824">Versão 2.0.57</span><span class="sxs-lookup"><span data-stu-id="82786-824">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="82786-825">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-825">Core</span></span>

* <span data-ttu-id="82786-826">Hotfix para o [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="82786-826">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="82786-827">28 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-827">January 28, 2019</span></span>

<span data-ttu-id="82786-828">Versão 2.0.56</span><span class="sxs-lookup"><span data-stu-id="82786-828">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="82786-829">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-829">ACR</span></span>
* <span data-ttu-id="82786-830">Suporte adicionado para regras de rede virtual/IP</span><span class="sxs-lookup"><span data-stu-id="82786-830">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="82786-831">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-831">ACS</span></span>
* <span data-ttu-id="82786-832">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="82786-832">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="82786-833">Comandos do OpenShift gerenciado foram adicionados</span><span class="sxs-lookup"><span data-stu-id="82786-833">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="82786-834">Suporte adicionado para operações de atualização da entidade de serviço com `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="82786-834">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="82786-835">AMS</span><span class="sxs-lookup"><span data-stu-id="82786-835">AMS</span></span>
* <span data-ttu-id="82786-836">[ALTERAÇÃO SIGNIFICATIVA] `ams asset get-streaming-locators` renomeado para `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="82786-836">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="82786-837">[ALTERAÇÃO SIGNIFICATIVA] `ams streaming-locator get-content-keys` renomeado para `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="82786-837">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-838">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-838">Appservice</span></span>
* <span data-ttu-id="82786-839">Suporte adicionado para o App Insights no `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="82786-839">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="82786-840">Suporte adicionado para a criação do plano de serviço de aplicativo (incluindo Elástico Premium) para Aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="82786-840">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="82786-841">Foram corrigidos os problemas com de configuração de aplicativo com os planos Elástico Premium</span><span class="sxs-lookup"><span data-stu-id="82786-841">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="82786-842">Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-842">Container</span></span>
* <span data-ttu-id="82786-843">Adicionado o comando `container start`</span><span class="sxs-lookup"><span data-stu-id="82786-843">Added `container start` command</span></span>
* <span data-ttu-id="82786-844">Alteração para permitir o uso de valores decimais para CPU durante a criação do contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-844">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="82786-845">EventGrid</span><span class="sxs-lookup"><span data-stu-id="82786-845">EventGrid</span></span>
* <span data-ttu-id="82786-846">Parâmetro `--deadletter-endpoint` adicionado a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-846">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="82786-847">Storagequeue e hybridconnection foram adicionados como novos valores para 'event-subscription [create|update] --endpoint-type\`</span><span class="sxs-lookup"><span data-stu-id="82786-847">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="82786-848">Os parâmetros `--max-delivery-attempts` e `--event-ttl` foram adicionados a `event-subscription create` para especificar a política de repetição para eventos</span><span class="sxs-lookup"><span data-stu-id="82786-848">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="82786-849">Uma mensagem de aviso foi adicionada a `event-subscription [create|update]` quando o webhook como destino for usado para uma assinatura de evento</span><span class="sxs-lookup"><span data-stu-id="82786-849">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="82786-850">O parâmetro source-resource-id foi adicionado para todos os comandos relacionados a eventos e marcar todos os outros parâmetros relacionados ao recurso de origem como preteridos</span><span class="sxs-lookup"><span data-stu-id="82786-850">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="82786-851">HDInsight</span><span class="sxs-lookup"><span data-stu-id="82786-851">HDInsight</span></span>
* <span data-ttu-id="82786-852">[ALTERAÇÃO SIGNIFICATIVA] Os parâmetros `--virtual-network` e `--subnet-name` de `hdinsight [application] create` foram removidos</span><span class="sxs-lookup"><span data-stu-id="82786-852">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="82786-853">[ALTERAÇÃO SIGNIFICATIVA] `hdinsight create --storage-account` foi alterado para aceitar o nome ou ID da conta de armazenamento, em vez de pontos de extremidade de blob</span><span class="sxs-lookup"><span data-stu-id="82786-853">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="82786-854">Parâmetros `--vnet-name` e `--subnet-name` adicionados a `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="82786-854">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="82786-855">Suporte adicionado para a criptografia de disco e Enterprise Security Package ao `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="82786-855">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="82786-856">Adicionado o comando `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="82786-856">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="82786-857">Adicionado o comando `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="82786-857">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="82786-858">IoT</span><span class="sxs-lookup"><span data-stu-id="82786-858">IoT</span></span>
* <span data-ttu-id="82786-859">O formato de codificação foi adicionado ao comando routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="82786-859">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="82786-860">Kusto</span><span class="sxs-lookup"><span data-stu-id="82786-860">Kusto</span></span>
* <span data-ttu-id="82786-861">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="82786-861">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="82786-862">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="82786-862">Monitor</span></span>
* <span data-ttu-id="82786-863">A comparação de ID foi alterada para diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="82786-863">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="82786-864">Perfil</span><span class="sxs-lookup"><span data-stu-id="82786-864">Profile</span></span>
* <span data-ttu-id="82786-865">A conta de nível de locatário foi habilitada para a identidade de serviço gerenciada de `login`</span><span class="sxs-lookup"><span data-stu-id="82786-865">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="82786-866">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-866">Network</span></span>
* <span data-ttu-id="82786-867">Foi corrigido o problema com `express-route update`: em que o argumento `--bandwidth` era ignorado</span><span class="sxs-lookup"><span data-stu-id="82786-867">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="82786-868">Foi corrigido o problema com `ddos-protection update` em que definir a compreensão levava ao rastreamento de pilha</span><span class="sxs-lookup"><span data-stu-id="82786-868">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="82786-869">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-869">Resource</span></span>
* <span data-ttu-id="82786-870">Suporte adicionado para o arquivo de parâmetros de URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="82786-870">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="82786-871">Suporte adicionado para a identidade gerenciada à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="82786-871">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="82786-872">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="82786-872">SQL Virtual Machine</span></span>
* <span data-ttu-id="82786-873">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="82786-873">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="82786-874">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-874">Storage</span></span>
* <span data-ttu-id="82786-875">Alteração na correção para atualizar apenas as propriedades que são alteradas no mesmo objeto</span><span class="sxs-lookup"><span data-stu-id="82786-875">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="82786-876">#8021 foi corrigido, dados binários são codificados em base 64 quando retornados</span><span class="sxs-lookup"><span data-stu-id="82786-876">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="82786-877">VM</span><span class="sxs-lookup"><span data-stu-id="82786-877">VM</span></span>
* <span data-ttu-id="82786-878">Alteração de `vm encryption enable` para validar o cofre de chaves de criptografia de disco e se esse cofre de chaves de criptografia de chave existe</span><span class="sxs-lookup"><span data-stu-id="82786-878">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="82786-879">O sinalizador `--force` foi adicionado a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="82786-879">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="82786-880">15 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="82786-880">January 15, 2019</span></span>

<span data-ttu-id="82786-881">Versão 2.0.55</span><span class="sxs-lookup"><span data-stu-id="82786-881">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="82786-882">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-882">ACR</span></span>
* <span data-ttu-id="82786-883">Alteração para permitir forçar o envio por push de um gráfico Helm que não existe</span><span class="sxs-lookup"><span data-stu-id="82786-883">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="82786-884">Alteração para permitir operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="82786-884">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="82786-885">[PRETERIDO] O parâmetro `--resource-group` foi preterido nos comandos:</span><span class="sxs-lookup"><span data-stu-id="82786-885">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="82786-886">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-886">ACS</span></span>
* <span data-ttu-id="82786-887">Suporte adicionado para novas regiões ACI</span><span class="sxs-lookup"><span data-stu-id="82786-887">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-888">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-888">Appservice</span></span>
* <span data-ttu-id="82786-889">Foi corrigido o problema com o carregamento de certificados para aplicativos que são hospedados em um ASE, em que o RG do ASE e o RG do aplicativo são diferentes</span><span class="sxs-lookup"><span data-stu-id="82786-889">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="82786-890">Alteração de `webapp up` para usar a SKU P1V1 como padrão para Linux</span><span class="sxs-lookup"><span data-stu-id="82786-890">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="82786-891">`[webapp|functionapp] deployment source config-zip` foi corrigido para mostrar a mensagem de erro adequada quando uma implantação falhar</span><span class="sxs-lookup"><span data-stu-id="82786-891">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="82786-892">Adicionado o comando `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="82786-892">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="82786-893">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="82786-893">Botservice</span></span>
* <span data-ttu-id="82786-894">Atualizações de status de implantação foram adicionadas a `bot create`</span><span class="sxs-lookup"><span data-stu-id="82786-894">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="82786-895">Configurar</span><span class="sxs-lookup"><span data-stu-id="82786-895">Configure</span></span>
* <span data-ttu-id="82786-896">`none` foi adicionado como um formato de saída configurável</span><span class="sxs-lookup"><span data-stu-id="82786-896">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82786-897">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="82786-897">CosmosDB</span></span>
* <span data-ttu-id="82786-898">Suporte adicionado para criar o banco de dados com taxa de transferência compartilhada</span><span class="sxs-lookup"><span data-stu-id="82786-898">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="82786-899">HDInsight</span><span class="sxs-lookup"><span data-stu-id="82786-899">HDInsight</span></span>
* <span data-ttu-id="82786-900">Foram adicionados comandos para o gerenciamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="82786-900">Added commands for managing applications</span></span>
* <span data-ttu-id="82786-901">Foram adicionados comandos para o gerenciamento de ações de script</span><span class="sxs-lookup"><span data-stu-id="82786-901">Added commands for managing script actions</span></span>
* <span data-ttu-id="82786-902">Foram adicionados comandos para o gerenciamento do Operations Management Suite (OMS)</span><span class="sxs-lookup"><span data-stu-id="82786-902">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="82786-903">Suporte adicionado para listar a utilização regional ao `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="82786-903">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="82786-904">[ALTERAÇÃO SIGNIFICATIVA] O tipo de cluster padrão de `hdinsight create` foi removido</span><span class="sxs-lookup"><span data-stu-id="82786-904">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="82786-905">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-905">Network</span></span>
* <span data-ttu-id="82786-906">Adicionados os argumentos `--custom-headers` e `--status-code-ranges` para `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-906">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="82786-907">Novos tipos de roteamento foram adicionados: Subrede e múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="82786-907">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="82786-908">Adicionados os argumentos `--custom-headers` e `--subnets` para `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-908">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="82786-909">Foi corrigido o problema no qual fornecer `--vnets ""` a `ddos-protection update` causava um erro</span><span class="sxs-lookup"><span data-stu-id="82786-909">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="82786-910">Função</span><span class="sxs-lookup"><span data-stu-id="82786-910">Role</span></span>
* <span data-ttu-id="82786-911">[PRETERIDO] O argumento `--password` foi preterido para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="82786-911">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="82786-912">Como alternativa, use senhas seguras geradas pela CLI</span><span class="sxs-lookup"><span data-stu-id="82786-912">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="82786-913">Segurança</span><span class="sxs-lookup"><span data-stu-id="82786-913">Security</span></span>
* <span data-ttu-id="82786-914">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="82786-914">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="82786-915">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-915">Storage</span></span>
* <span data-ttu-id="82786-916">[ALTERAÇÃO SIGNIFICATIVA] O número padrão de resultados de `storage [blob|file|container|share] list` foi alterado para 5.000.</span><span class="sxs-lookup"><span data-stu-id="82786-916">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="82786-917">Use `--num-results *` para o comportamento original de retornar todos os resultados</span><span class="sxs-lookup"><span data-stu-id="82786-917">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="82786-918">Parâmetro `--marker` adicionado a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="82786-918">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="82786-919">Um marcador de log foi adicionado para a próxima página ao STDERR de `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="82786-919">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="82786-920">O comando `storage blob service-properties update` foi adicionado com suporte para sites estáticos</span><span class="sxs-lookup"><span data-stu-id="82786-920">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="82786-921">VM</span><span class="sxs-lookup"><span data-stu-id="82786-921">VM</span></span>
* <span data-ttu-id="82786-922">`vm [disk|unmanaged-disk]` e `vmss disk` foram alterados para que tenham parâmetros mais consistentes</span><span class="sxs-lookup"><span data-stu-id="82786-922">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="82786-923">Suporte adicionado para referência cruzada de imagem de locatário a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="82786-923">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="82786-924">O bug de configuração padrão foi corrigido em `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="82786-924">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="82786-925">O argumento `--provision-after-extensions` foi adicionado a `vmss extension set` para definir quais extensões deverão ser provisionadas antes da extensão ser definida</span><span class="sxs-lookup"><span data-stu-id="82786-925">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="82786-926">O argumento `--replica-count` foi adicionado a `sig image-version update` para definir a contagem de replicação padrão</span><span class="sxs-lookup"><span data-stu-id="82786-926">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="82786-927">Foi corrigido o bug com `image create --source` em que o disco do sistema operacional de origem era confundido com uma VM do mesmo nome, mesmo se a ID de recurso completa fosse fornecida</span><span class="sxs-lookup"><span data-stu-id="82786-927">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="82786-928">20 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-928">December 20, 2018</span></span>

<span data-ttu-id="82786-929">Versão 2.0.54</span><span class="sxs-lookup"><span data-stu-id="82786-929">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="82786-930">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-930">Appservice</span></span>
* <span data-ttu-id="82786-931">Corrigido o problema que causava falha na reimplantação do `webapp up`</span><span class="sxs-lookup"><span data-stu-id="82786-931">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="82786-932">Adicionado suporte para listar e restaurar instantâneos de aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="82786-932">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="82786-933">Adicionado suporte para o sinalizador `--runtime` para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="82786-933">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="82786-934">IoT Central</span><span class="sxs-lookup"><span data-stu-id="82786-934">IoTCentral</span></span>
* <span data-ttu-id="82786-935">Corrigida a chamada à API do comando de atualização</span><span class="sxs-lookup"><span data-stu-id="82786-935">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="82786-936">Função</span><span class="sxs-lookup"><span data-stu-id="82786-936">Role</span></span>
* <span data-ttu-id="82786-937">[ALTERAÇÃO SIGNIFICATIVA] `ad [app|sp] list` alterado para listar somente os 100 primeiros objetos por padrão</span><span class="sxs-lookup"><span data-stu-id="82786-937">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="82786-938">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-938">SQL</span></span>
* <span data-ttu-id="82786-939">Adicionado suporte para ordenação personalizada nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="82786-939">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="82786-940">VM</span><span class="sxs-lookup"><span data-stu-id="82786-940">VM</span></span>
* <span data-ttu-id="82786-941">Parâmetro `---os-type` adicionado a `disk create`</span><span class="sxs-lookup"><span data-stu-id="82786-941">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="82786-942">18 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-942">December 18, 2018</span></span>

<span data-ttu-id="82786-943">Versão 2.0.53</span><span class="sxs-lookup"><span data-stu-id="82786-943">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="82786-944">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-944">ACR</span></span>
* <span data-ttu-id="82786-945">Adicionado suporte para importação de imagem de Registros de Contêiner externos</span><span class="sxs-lookup"><span data-stu-id="82786-945">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="82786-946">Simplificado o layout da tabela para a lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="82786-946">Condensed the table layout for task list</span></span>
* <span data-ttu-id="82786-947">Adicionado suporte para URLs do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="82786-947">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="82786-948">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-948">ACS</span></span>
* <span data-ttu-id="82786-949">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="82786-949">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="82786-950">Removido “(VISUALIZAÇÃO)” de argumentos do AAD para `aks create`</span><span class="sxs-lookup"><span data-stu-id="82786-950">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="82786-951">[PRETERIDO] Comandos `az acs` preteridos.</span><span class="sxs-lookup"><span data-stu-id="82786-951">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="82786-952">O serviço ACS será desativado em 31 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="82786-952">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="82786-953">Adicionado suporte da Política de Rede durante a criação de novos clusters AKS</span><span class="sxs-lookup"><span data-stu-id="82786-953">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="82786-954">Removido o requisito do argumento `--nodepool-name` para `aks scale` se houver apenas um pool de nós</span><span class="sxs-lookup"><span data-stu-id="82786-954">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-955">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-955">Appservice</span></span>
* <span data-ttu-id="82786-956">Corrigido o problema em que `webapp config container` não honra o parâmetro `--slot`</span><span class="sxs-lookup"><span data-stu-id="82786-956">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="82786-957">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="82786-957">Botservice</span></span>
* <span data-ttu-id="82786-958">Suporte adicionado para análise do arquivo `.bot` ao chamar `bot show`</span><span class="sxs-lookup"><span data-stu-id="82786-958">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="82786-959">Corrigido o bug de provisionamento do AppInsights</span><span class="sxs-lookup"><span data-stu-id="82786-959">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="82786-960">Corrigido o bug de espaço em branco ao lidar com caminhos de arquivo</span><span class="sxs-lookup"><span data-stu-id="82786-960">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="82786-961">Reduzidas as chamadas de rede do Kudu</span><span class="sxs-lookup"><span data-stu-id="82786-961">Reduced Kudu network calls</span></span>
* <span data-ttu-id="82786-962">Melhorias de UX para comandos gerais</span><span class="sxs-lookup"><span data-stu-id="82786-962">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="82786-963">Consumo</span><span class="sxs-lookup"><span data-stu-id="82786-963">Consumption</span></span>
* <span data-ttu-id="82786-964">Corrigidos os bugs da API de orçamento ao mostrar notificações</span><span class="sxs-lookup"><span data-stu-id="82786-964">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82786-965">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="82786-965">CosmosDB</span></span>
* <span data-ttu-id="82786-966">Suporte adicionado para atualizar a conta de vários mestres para mestre único</span><span class="sxs-lookup"><span data-stu-id="82786-966">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="82786-967">Mapas</span><span class="sxs-lookup"><span data-stu-id="82786-967">Maps</span></span>
* <span data-ttu-id="82786-968">Adicionado suporte ao SKU S1 para `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-968">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="82786-969">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-969">Network</span></span>
* <span data-ttu-id="82786-970">Adicionado suporte para `--format` e `--log-version` para `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="82786-970">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="82786-971">Corrigido o problema com `dns zone update` em que usar "" para limpar a resolução e o registro de redes virtuais não funcionava</span><span class="sxs-lookup"><span data-stu-id="82786-971">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="82786-972">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-972">Resource</span></span>
* <span data-ttu-id="82786-973">Corrigido o tratamento do parâmetro de escopo para grupos de gerenciamento do `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-973">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="82786-974">Adicionado o novo comando `resource wait`</span><span class="sxs-lookup"><span data-stu-id="82786-974">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="82786-975">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-975">Storage</span></span>
*  <span data-ttu-id="82786-976">Adicionada a capacidade de atualizar a versão do esquema de log para serviços de armazenamento no `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="82786-976">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="82786-977">VM</span><span class="sxs-lookup"><span data-stu-id="82786-977">VM</span></span>
* <span data-ttu-id="82786-978">Corrigida a falha em `vm identity remove` quando a VM especificada não tem nenhuma identidade de serviço gerenciado atribuída</span><span class="sxs-lookup"><span data-stu-id="82786-978">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="82786-979">4 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-979">December 4, 2018</span></span>

<span data-ttu-id="82786-980">Versão 2.0.52</span><span class="sxs-lookup"><span data-stu-id="82786-980">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="82786-981">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-981">Core</span></span>
* <span data-ttu-id="82786-982">Adicionado suporte para provisionamento de recursos de locatários cruzados para a entidade de serviço de multilocatários</span><span class="sxs-lookup"><span data-stu-id="82786-982">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="82786-983">Corrigido o bug onde as ids enviadas por pipe de um comando com a saída tsv eram analisados incorretamente</span><span class="sxs-lookup"><span data-stu-id="82786-983">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-984">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-984">Appservice</span></span>
* <span data-ttu-id="82786-985">[VERSÃO PRÉVIA] Adicionado o comando `webapp up` que ajuda a criar e implantar conteúdo em aplicativo</span><span class="sxs-lookup"><span data-stu-id="82786-985">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="82786-986">Corrigido um bug no aplicativo com base em contêiner do Windows devido à alteração de back-end</span><span class="sxs-lookup"><span data-stu-id="82786-986">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="82786-987">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-987">Network</span></span>
* <span data-ttu-id="82786-988">Adicionado o argumento `--exclusion` a `application-gateway waf-config set` para dar suporte a exclusões de WAF</span><span class="sxs-lookup"><span data-stu-id="82786-988">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="82786-989">Função</span><span class="sxs-lookup"><span data-stu-id="82786-989">Role</span></span>
* <span data-ttu-id="82786-990">Adicionado suporte para identificadores personalizados para a credencial de senha</span><span class="sxs-lookup"><span data-stu-id="82786-990">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="82786-991">VM</span><span class="sxs-lookup"><span data-stu-id="82786-991">VM</span></span>
* <span data-ttu-id="82786-992">[PRETERIDO] Parâmetro `vm extension [show|wait] --expand` preterido</span><span class="sxs-lookup"><span data-stu-id="82786-992">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="82786-993">Adicionado parâmetro `--force` a `vm restart` para reimplantar as VMs sem resposta</span><span class="sxs-lookup"><span data-stu-id="82786-993">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="82786-994">Alterado `[vm|vmss] create --authentication-type` para aceitar "todos" para criar uma VM com senha e autenticação SSH</span><span class="sxs-lookup"><span data-stu-id="82786-994">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="82786-995">Adicionado parâmetro `image create --os-disk-caching` para definir o cache de disco do sistema operacional para uma imagem</span><span class="sxs-lookup"><span data-stu-id="82786-995">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="82786-996">20 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-996">November 20, 2018</span></span>

<span data-ttu-id="82786-997">Versão 2.0.51</span><span class="sxs-lookup"><span data-stu-id="82786-997">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="82786-998">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-998">Core</span></span>
* <span data-ttu-id="82786-999">Logon do MSI alterado para não reutilizar o nome da assinatura na identidade</span><span class="sxs-lookup"><span data-stu-id="82786-999">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="82786-1000">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-1000">ACR</span></span>
* <span data-ttu-id="82786-1001">Token de contexto adicionado à etapa da tarefa</span><span class="sxs-lookup"><span data-stu-id="82786-1001">Added context token to task step</span></span>
* <span data-ttu-id="82786-1002">Suporte adicionado para definir segredos na execução do acr para espelhar a tarefa do acr</span><span class="sxs-lookup"><span data-stu-id="82786-1002">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="82786-1003">Suporte aprimorado para `--top` e `--orderby` para os comandos `show-tags` e `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="82786-1003">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-1004">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-1004">Appservice</span></span>
* <span data-ttu-id="82786-1005">Tempo limite padrão para a implantação do zip alterado para sondar o status aumentado para 5 minutos, também adicionando uma propriedade de tempo limite para personalizar esse valor</span><span class="sxs-lookup"><span data-stu-id="82786-1005">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="82786-1006">Padrão `node_version` atualizado.</span><span class="sxs-lookup"><span data-stu-id="82786-1006">Updated the default `node_version`.</span></span> <span data-ttu-id="82786-1007">Redefinir a ação de troca de slots durante uma troca de duas fases preserva todas as configurações do aplicativo e cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="82786-1007">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="82786-1008">Verificação da SKU no lado do cliente removida para o Linux criar o plano do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="82786-1008">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="82786-1009">Erro corrigido ao tentar obter o status de implantação do zip</span><span class="sxs-lookup"><span data-stu-id="82786-1009">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="82786-1010">Iot Central</span><span class="sxs-lookup"><span data-stu-id="82786-1010">IotCentral</span></span>
* <span data-ttu-id="82786-1011">Verificação de disponibilidade do subdomínio adicionada ao criar um aplicativo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="82786-1011">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="82786-1012">KeyVault</span><span class="sxs-lookup"><span data-stu-id="82786-1012">KeyVault</span></span>
* <span data-ttu-id="82786-1013">Bug corrigido em que os erros podem ter sido ignorados</span><span class="sxs-lookup"><span data-stu-id="82786-1013">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="82786-1014">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-1014">Network</span></span>
* <span data-ttu-id="82786-1015">Subcomandos `root-cert` adicionados a `application-gateway` para lidar com os certificados de raiz confiável</span><span class="sxs-lookup"><span data-stu-id="82786-1015">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="82786-1016">Opções `--min-capacity` e `--custom-error-pages` adicionadas a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="82786-1016">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="82786-1017">`--zones` adicionado para suporte da zona de disponibilidade a `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="82786-1017">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="82786-1018">Argumentos `--file-upload-limit`, `--max-request-body-size` e `--request-body-check` a `application-gateway waf-config set` adicionados</span><span class="sxs-lookup"><span data-stu-id="82786-1018">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="82786-1019">Rdbms</span><span class="sxs-lookup"><span data-stu-id="82786-1019">Rdbms</span></span>
* <span data-ttu-id="82786-1020">Comandos vnet do mariadb adicionados</span><span class="sxs-lookup"><span data-stu-id="82786-1020">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="82786-1021">Rbac</span><span class="sxs-lookup"><span data-stu-id="82786-1021">Rbac</span></span>
* <span data-ttu-id="82786-1022">Um problema corrigido ao tentar atualizar credenciais inalteradas em `ad app update`</span><span class="sxs-lookup"><span data-stu-id="82786-1022">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="82786-1023">Avisos de saída adicionados para comunicar alterações de falha em um futuro próximo para `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="82786-1023">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="82786-1024">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-1024">Storage</span></span>
* <span data-ttu-id="82786-1025">Melhor manipulação de casos incomuns para os comandos da cópia de armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-1025">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="82786-1026">Corrigido o problema em que `storage blob copy start-batch` não usava credenciais de logon quando as contas de origem e destino eram iguais</span><span class="sxs-lookup"><span data-stu-id="82786-1026">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="82786-1027">Bug corrigido com `storage [blob|file] url` em que `sas_token` não foi incorporado na URL</span><span class="sxs-lookup"><span data-stu-id="82786-1027">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="82786-1028">Aviso de alteração da falha adicionado a `[blob|container] list`: produzirá apenas os primeiros 5.000 resultados por padrão</span><span class="sxs-lookup"><span data-stu-id="82786-1028">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="82786-1029">VM</span><span class="sxs-lookup"><span data-stu-id="82786-1029">VM</span></span>
* <span data-ttu-id="82786-1030">Suporte adicionado a `[vm|vmss] create --storage-sku` para especificar a SKU da conta de armazenamento para o SO gerenciado e os discos de dados separadamente</span><span class="sxs-lookup"><span data-stu-id="82786-1030">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="82786-1031">Parâmetros do nome da versão alterados de `sig image-version` para `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="82786-1031">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="82786-1032">Argumento `sig image-version` preterido `--image-version-name`, substituído por `--image-version`</span><span class="sxs-lookup"><span data-stu-id="82786-1032">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="82786-1033">Suporte adicionado para usar o disco local do SO a `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="82786-1033">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="82786-1034">Adicionado o suporte ao `--no-wait` para `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="82786-1034">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="82786-1035">Adicionado o comando `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="82786-1035">Added `snapshot wait` command</span></span>
* <span data-ttu-id="82786-1036">Suporte adicionado para usar o nome da instância com `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="82786-1036">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="82786-1037">6 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1037">November 6, 2018</span></span>

<span data-ttu-id="82786-1038">Versão 2.0.50</span><span class="sxs-lookup"><span data-stu-id="82786-1038">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="82786-1039">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-1039">Core</span></span>
* <span data-ttu-id="82786-1040">Foi adicionado suporte para o serviço principal sn + autenticação do emissor</span><span class="sxs-lookup"><span data-stu-id="82786-1040">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="82786-1041">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-1041">ACR</span></span>
* <span data-ttu-id="82786-1042">Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa</span><span class="sxs-lookup"><span data-stu-id="82786-1042">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="82786-1043">Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação</span><span class="sxs-lookup"><span data-stu-id="82786-1043">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="82786-1044">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-1044">ACS</span></span>
* <span data-ttu-id="82786-1045">[ALTERAÇÃO SIGNIFICATIVA] `enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão</span><span class="sxs-lookup"><span data-stu-id="82786-1045">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="82786-1046">Supervisor</span><span class="sxs-lookup"><span data-stu-id="82786-1046">Advisor</span></span>
* <span data-ttu-id="82786-1047">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="82786-1047">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="82786-1048">AMS</span><span class="sxs-lookup"><span data-stu-id="82786-1048">AMS</span></span>
* <span data-ttu-id="82786-1049">Novos grupos de comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="82786-1049">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="82786-1050">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="82786-1050">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="82786-1051">Adicionados parâmetros de criptografia com suporte para `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="82786-1051">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="82786-1052">O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido</span><span class="sxs-lookup"><span data-stu-id="82786-1052">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="82786-1053">Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="82786-1053">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="82786-1054">Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="82786-1054">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="82786-1055">Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="82786-1055">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="82786-1056">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming locator` foi substituído por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="82786-1056">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="82786-1057">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--content-keys` de `ams streaming locator` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="82786-1057">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="82786-1058">[ALTERAÇÃO SIGNIFICATIVA] `--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="82786-1058">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="82786-1059">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming policy` foi substituído por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="82786-1059">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="82786-1060">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="82786-1060">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="82786-1061">Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="82786-1061">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="82786-1062">Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado</span><span class="sxs-lookup"><span data-stu-id="82786-1062">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="82786-1063">[ALTERAÇÃO SIGNIFICATIVA] `--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="82786-1063">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="82786-1064">Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'.</span><span class="sxs-lookup"><span data-stu-id="82786-1064">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="82786-1065">Um ativo sem rótulo pode ser enviado assim: 'assetName='</span><span class="sxs-lookup"><span data-stu-id="82786-1065">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-1066">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-1066">AppService</span></span>
* <span data-ttu-id="82786-1067">Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido</span><span class="sxs-lookup"><span data-stu-id="82786-1067">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="82786-1068">Configurar</span><span class="sxs-lookup"><span data-stu-id="82786-1068">Configure</span></span>
* <span data-ttu-id="82786-1069">O YAML foi adicionado às opções de formato de saída</span><span class="sxs-lookup"><span data-stu-id="82786-1069">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="82786-1070">Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-1070">Container</span></span>
* <span data-ttu-id="82786-1071">Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml</span><span class="sxs-lookup"><span data-stu-id="82786-1071">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="82786-1072">EventHub</span><span class="sxs-lookup"><span data-stu-id="82786-1072">EventHub</span></span>
* <span data-ttu-id="82786-1073">O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-1073">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="82786-1074">Interativo</span><span class="sxs-lookup"><span data-stu-id="82786-1074">Interactive</span></span>
* <span data-ttu-id="82786-1075">O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos</span><span class="sxs-lookup"><span data-stu-id="82786-1075">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="82786-1076">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="82786-1076">Monitor</span></span>
* <span data-ttu-id="82786-1077">Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) para `--condition` em `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-1077">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="82786-1078">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-1078">Network</span></span>
* <span data-ttu-id="82786-1079">Os nomes de comandos `network interface-endpoint` foram preteridos em benefício de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="82786-1079">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="82786-1080">Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID</span><span class="sxs-lookup"><span data-stu-id="82786-1080">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="82786-1081">Foi corrigido um problema onde `--ip-tags` não funcionava corretamente com `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="82786-1081">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="82786-1082">Perfil</span><span class="sxs-lookup"><span data-stu-id="82786-1082">Profile</span></span>
* <span data-ttu-id="82786-1083">`--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado</span><span class="sxs-lookup"><span data-stu-id="82786-1083">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="82786-1084">RDBMS</span><span class="sxs-lookup"><span data-stu-id="82786-1084">RDBMS</span></span>
* <span data-ttu-id="82786-1085">Adicionados comandos da réplica mysql</span><span class="sxs-lookup"><span data-stu-id="82786-1085">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="82786-1086">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-1086">Resource</span></span>
* <span data-ttu-id="82786-1087">Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="82786-1087">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="82786-1088">Função</span><span class="sxs-lookup"><span data-stu-id="82786-1088">Role</span></span>
* <span data-ttu-id="82786-1089">Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais</span><span class="sxs-lookup"><span data-stu-id="82786-1089">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="82786-1090">`ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="82786-1090">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="82786-1091">Suporte adicionado para conceder permissões a aplicativos do AAD</span><span class="sxs-lookup"><span data-stu-id="82786-1091">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="82786-1092">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-1092">Storage</span></span>
* <span data-ttu-id="82786-1093">Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="82786-1093">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="82786-1094">VM</span><span class="sxs-lookup"><span data-stu-id="82786-1094">VM</span></span>
* <span data-ttu-id="82786-1095">O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem</span><span class="sxs-lookup"><span data-stu-id="82786-1095">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="82786-1096">O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido</span><span class="sxs-lookup"><span data-stu-id="82786-1096">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="82786-1097">O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado</span><span class="sxs-lookup"><span data-stu-id="82786-1097">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="82786-1098">`vm secret format` foi alterado para exigir a saída json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="82786-1098">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="82786-1099">Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido</span><span class="sxs-lookup"><span data-stu-id="82786-1099">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="82786-1100">Validação de argumento aprimorado para `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="82786-1100">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="82786-1101">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1101">October 23, 2018</span></span>

<span data-ttu-id="82786-1102">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="82786-1102">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="82786-1103">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-1103">Core</span></span>
* <span data-ttu-id="82786-1104">Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`</span><span class="sxs-lookup"><span data-stu-id="82786-1104">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="82786-1105">Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="82786-1105">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="82786-1106">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-1106">ACR</span></span>
* <span data-ttu-id="82786-1107">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="82786-1107">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="82786-1108">CDN</span><span class="sxs-lookup"><span data-stu-id="82786-1108">CDN</span></span>
* <span data-ttu-id="82786-1109">[ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="82786-1109">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="82786-1110">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="82786-1110">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="82786-1111">Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-1111">Container</span></span>
* <span data-ttu-id="82786-1112">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="82786-1112">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="82786-1113">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="82786-1113">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="82786-1114">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="82786-1114">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="82786-1115">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="82786-1115">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="82786-1116">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="82786-1116">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="82786-1117">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="82786-1117">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="82786-1118">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="82786-1118">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82786-1119">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="82786-1119">CosmosDB</span></span>
* <span data-ttu-id="82786-1120">Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="82786-1120">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="82786-1121">Interativo</span><span class="sxs-lookup"><span data-stu-id="82786-1121">Interactive</span></span>
* <span data-ttu-id="82786-1122">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="82786-1122">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="82786-1123">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="82786-1123">IoT Central</span></span>
* <span data-ttu-id="82786-1124">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="82786-1124">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="82786-1125">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="82786-1125">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="82786-1126">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="82786-1126">Monitor</span></span>
* <span data-ttu-id="82786-1127">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="82786-1127">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="82786-1128">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="82786-1128">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="82786-1129">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="82786-1129">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="82786-1130">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="82786-1130">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="82786-1131">Adicionado `--namespace` como alias para a opção preterida `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="82786-1131">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="82786-1132">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="82786-1132">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="82786-1133">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="82786-1133">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="82786-1134">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="82786-1134">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="82786-1135">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="82786-1135">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="82786-1136">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="82786-1136">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="82786-1137">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-1137">Network</span></span>
* <span data-ttu-id="82786-1138">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="82786-1138">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="82786-1139">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="82786-1139">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="82786-1140">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="82786-1140">ServiceBus</span></span>
* <span data-ttu-id="82786-1141">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="82786-1141">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="82786-1142">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-1142">SQL</span></span>
* <span data-ttu-id="82786-1143">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="82786-1143">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="82786-1144">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-1144">Storage</span></span>
* <span data-ttu-id="82786-1145">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="82786-1145">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="82786-1146">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="82786-1146">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="82786-1147">VM</span><span class="sxs-lookup"><span data-stu-id="82786-1147">VM</span></span>
* <span data-ttu-id="82786-1148">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="82786-1148">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="82786-1149">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`</span><span class="sxs-lookup"><span data-stu-id="82786-1149">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="82786-1150">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`</span><span class="sxs-lookup"><span data-stu-id="82786-1150">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="82786-1151">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1151">October 16, 2018</span></span>

<span data-ttu-id="82786-1152">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="82786-1152">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="82786-1153">VM</span><span class="sxs-lookup"><span data-stu-id="82786-1153">VM</span></span>
* <span data-ttu-id="82786-1154">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="82786-1154">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="82786-1155">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1155">October 9, 2018</span></span>

<span data-ttu-id="82786-1156">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="82786-1156">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="82786-1157">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-1157">Core</span></span>
* <span data-ttu-id="82786-1158">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="82786-1158">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="82786-1159">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-1159">ACR</span></span>
* <span data-ttu-id="82786-1160">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="82786-1160">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="82786-1161">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-1161">ACS</span></span>
* <span data-ttu-id="82786-1162">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="82786-1162">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="82786-1163">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="82786-1163">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="82786-1164">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="82786-1164">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="82786-1165">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="82786-1165">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="82786-1166">Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-1166">Container</span></span>
* <span data-ttu-id="82786-1167">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um tempo de execução específico</span><span class="sxs-lookup"><span data-stu-id="82786-1167">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="82786-1168">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="82786-1168">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="82786-1169">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="82786-1169">Event Hub</span></span>
* <span data-ttu-id="82786-1170">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="82786-1170">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="82786-1171">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="82786-1171">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="82786-1172">Extensões</span><span class="sxs-lookup"><span data-stu-id="82786-1172">Extensions</span></span>
* <span data-ttu-id="82786-1173">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="82786-1173">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="82786-1174">HDInsight</span><span class="sxs-lookup"><span data-stu-id="82786-1174">HDInsight</span></span>
* <span data-ttu-id="82786-1175">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="82786-1175">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="82786-1176">IoT</span><span class="sxs-lookup"><span data-stu-id="82786-1176">IoT</span></span>
* <span data-ttu-id="82786-1177">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="82786-1177">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="82786-1178">KeyVault</span><span class="sxs-lookup"><span data-stu-id="82786-1178">KeyVault</span></span>
* <span data-ttu-id="82786-1179">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="82786-1179">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="82786-1180">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-1180">Network</span></span>
* <span data-ttu-id="82786-1181">Corrigido `network dns zone create`: O comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="82786-1181">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="82786-1182">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="82786-1182">See #6052</span></span>
* <span data-ttu-id="82786-1183">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="82786-1183">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="82786-1184">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="82786-1184">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="82786-1185">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="82786-1185">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="82786-1186">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="82786-1186">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="82786-1187">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="82786-1187">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="82786-1188">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="82786-1188">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="82786-1189">Função</span><span class="sxs-lookup"><span data-stu-id="82786-1189">Role</span></span>
* <span data-ttu-id="82786-1190">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="82786-1190">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="82786-1191">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="82786-1191">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="82786-1192">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="82786-1192">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="82786-1193">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="82786-1193">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="82786-1194">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="82786-1194">Service Bus</span></span>
* <span data-ttu-id="82786-1195">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="82786-1195">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="82786-1196">VM</span><span class="sxs-lookup"><span data-stu-id="82786-1196">VM</span></span>
* <span data-ttu-id="82786-1197">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="82786-1197">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="82786-1198">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="82786-1198">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="82786-1199">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="82786-1199">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="82786-1200">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="82786-1200">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="82786-1201">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="82786-1201">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="82786-1202">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="82786-1202">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="82786-1203">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1203">September 21, 2018</span></span>

<span data-ttu-id="82786-1204">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="82786-1204">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="82786-1205">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-1205">ACR</span></span>
* <span data-ttu-id="82786-1206">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="82786-1206">Added ACR Task commands</span></span>
* <span data-ttu-id="82786-1207">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="82786-1207">Added quick run command</span></span>
* <span data-ttu-id="82786-1208">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="82786-1208">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="82786-1209">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="82786-1209">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="82786-1210">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="82786-1210">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="82786-1211">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="82786-1211">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="82786-1212">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-1212">ACS</span></span>
* <span data-ttu-id="82786-1213">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="82786-1213">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="82786-1214">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="82786-1214">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-1215">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-1215">AppService</span></span>

* <span data-ttu-id="82786-1216">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="82786-1216">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="82786-1217">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="82786-1217">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="82786-1218">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="82786-1218">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="82786-1219">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="82786-1219">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="82786-1220">Lote</span><span class="sxs-lookup"><span data-stu-id="82786-1220">Batch</span></span>
* <span data-ttu-id="82786-1221">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="82786-1221">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="82786-1222">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="82786-1222">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="82786-1223">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="82786-1223">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="82786-1224">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="82786-1224">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="82786-1225">Lote AI</span><span class="sxs-lookup"><span data-stu-id="82786-1225">Batch AI</span></span> 
* <span data-ttu-id="82786-1226">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="82786-1226">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="82786-1227">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="82786-1227">Cognitive Services</span></span>
* <span data-ttu-id="82786-1228">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="82786-1228">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="82786-1229">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="82786-1229">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="82786-1230">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="82786-1230">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="82786-1231">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="82786-1231">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="82786-1232">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="82786-1232">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="82786-1233">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="82786-1233">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="82786-1234">Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-1234">Container</span></span>
* <span data-ttu-id="82786-1235">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="82786-1235">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="82786-1236">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="82786-1236">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="82786-1237">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="82786-1237">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="82786-1238">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="82786-1238">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="82786-1239">DataLake</span><span class="sxs-lookup"><span data-stu-id="82786-1239">Datalake</span></span>
* <span data-ttu-id="82786-1240">Comandos adicionados para regras da rede virtual</span><span class="sxs-lookup"><span data-stu-id="82786-1240">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="82786-1241">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="82786-1241">Interactive Shell</span></span>
* <span data-ttu-id="82786-1242">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="82786-1242">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="82786-1243">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="82786-1243">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="82786-1244">IoT</span><span class="sxs-lookup"><span data-stu-id="82786-1244">IoT</span></span>
* <span data-ttu-id="82786-1245">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="82786-1245">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="82786-1246">Key Vault</span><span class="sxs-lookup"><span data-stu-id="82786-1246">Key Vault</span></span>
* <span data-ttu-id="82786-1247">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="82786-1247">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="82786-1248">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-1248">Network</span></span>
* <span data-ttu-id="82786-1249">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="82786-1249">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="82786-1250">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="82786-1250">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="82786-1251">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="82786-1251">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="82786-1252">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="82786-1252">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="82786-1253">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="82786-1253">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="82786-1254">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="82786-1254">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="82786-1255">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="82786-1255">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="82786-1256">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="82786-1256">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="82786-1257">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="82786-1257">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="82786-1258">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="82786-1258">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="82786-1259">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="82786-1259">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="82786-1260">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="82786-1260">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="82786-1261">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="82786-1261">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="82786-1262">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="82786-1262">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="82786-1263">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="82786-1263">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="82786-1264">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="82786-1264">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="82786-1265">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="82786-1265">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="82786-1266">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="82786-1266">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="82786-1267">RDBMS</span><span class="sxs-lookup"><span data-stu-id="82786-1267">RDBMS</span></span>
* <span data-ttu-id="82786-1268">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="82786-1268">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="82786-1269">Reserva</span><span class="sxs-lookup"><span data-stu-id="82786-1269">Reservation</span></span>
* <span data-ttu-id="82786-1270">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="82786-1270">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="82786-1271">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="82786-1271">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="82786-1272">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="82786-1272">Manage App</span></span>
* <span data-ttu-id="82786-1273">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="82786-1273">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="82786-1274">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="82786-1274">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="82786-1275">Função</span><span class="sxs-lookup"><span data-stu-id="82786-1275">Role</span></span>
* <span data-ttu-id="82786-1276">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="82786-1276">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="82786-1277">SignalR</span><span class="sxs-lookup"><span data-stu-id="82786-1277">SignalR</span></span>
* <span data-ttu-id="82786-1278">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="82786-1278">First release</span></span>

### <a name="storage"></a><span data-ttu-id="82786-1279">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-1279">Storage</span></span>
* <span data-ttu-id="82786-1280">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="82786-1280">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="82786-1281">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="82786-1281">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="82786-1282">VM</span><span class="sxs-lookup"><span data-stu-id="82786-1282">VM</span></span>
* <span data-ttu-id="82786-1283">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="82786-1283">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="82786-1284">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="82786-1284">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="82786-1285">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1285">August 28, 2018</span></span>

<span data-ttu-id="82786-1286">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="82786-1286">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="82786-1287">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-1287">Core</span></span>

* <span data-ttu-id="82786-1288">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="82786-1288">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="82786-1289">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="82786-1289">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="82786-1290">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-1290">ACR</span></span>

* <span data-ttu-id="82786-1291">Adicionada uma solução alternativa para operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="82786-1291">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="82786-1292">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="82786-1292">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="82786-1293">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-1293">ACS</span></span>

* <span data-ttu-id="82786-1294">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="82786-1294">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="82786-1295">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="82786-1295">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-1296">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-1296">AppService</span></span>

* <span data-ttu-id="82786-1297">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="82786-1297">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="82786-1298">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="82786-1298">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="82786-1299">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="82786-1299">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="82786-1300">Backup</span><span class="sxs-lookup"><span data-stu-id="82786-1300">Backup</span></span>

* <span data-ttu-id="82786-1301">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="82786-1301">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="82786-1302">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="82786-1302">Bot Service</span></span>

* <span data-ttu-id="82786-1303">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="82786-1303">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="82786-1304">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="82786-1304">Cognitive Services</span></span>

* <span data-ttu-id="82786-1305">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="82786-1305">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="82786-1306">IoT</span><span class="sxs-lookup"><span data-stu-id="82786-1306">IoT</span></span>

* <span data-ttu-id="82786-1307">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="82786-1307">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="82786-1308">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="82786-1308">Monitor</span></span>

* <span data-ttu-id="82786-1309">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="82786-1309">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="82786-1310">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="82786-1310">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="82786-1311">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-1311">Network</span></span>

* <span data-ttu-id="82786-1312">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="82786-1312">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="82786-1313">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-1313">Resource</span></span>

* <span data-ttu-id="82786-1314">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="82786-1314">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="82786-1315">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-1315">Storage</span></span>

* <span data-ttu-id="82786-1316">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="82786-1316">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="82786-1317">VM</span><span class="sxs-lookup"><span data-stu-id="82786-1317">VM</span></span>

* <span data-ttu-id="82786-1318">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="82786-1318">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="82786-1319">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="82786-1319">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="82786-1320">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1320">Auguest 14, 2018</span></span>

<span data-ttu-id="82786-1321">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="82786-1321">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="82786-1322">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-1322">Core</span></span>

* <span data-ttu-id="82786-1323">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="82786-1323">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="82786-1324">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="82786-1324">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="82786-1325">Telemetria</span><span class="sxs-lookup"><span data-stu-id="82786-1325">Telemetry</span></span>

* <span data-ttu-id="82786-1326">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="82786-1326">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="82786-1327">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-1327">ACR</span></span>

* <span data-ttu-id="82786-1328">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="82786-1328">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="82786-1329">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="82786-1329">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="82786-1330">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-1330">ACS</span></span>

* <span data-ttu-id="82786-1331">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="82786-1331">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="82786-1332">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="82786-1332">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="82786-1333">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="82786-1333">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="82786-1334">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="82786-1334">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="82786-1335">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="82786-1335">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="82786-1336">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-1336">AppService</span></span>

* <span data-ttu-id="82786-1337">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="82786-1337">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="82786-1338">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="82786-1338">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="82786-1339">BatchAI</span><span class="sxs-lookup"><span data-stu-id="82786-1339">BatchAI</span></span>

* <span data-ttu-id="82786-1340">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="82786-1340">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="82786-1341">Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-1341">Container</span></span>

* <span data-ttu-id="82786-1342">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-1342">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="82786-1343">IoT</span><span class="sxs-lookup"><span data-stu-id="82786-1343">IoT</span></span>

* <span data-ttu-id="82786-1344">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="82786-1344">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="82786-1345">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="82786-1345">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="82786-1346">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="82786-1346">Iot Central</span></span>

* <span data-ttu-id="82786-1347">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="82786-1347">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="82786-1348">KeyVault</span><span class="sxs-lookup"><span data-stu-id="82786-1348">KeyVault</span></span>


* <span data-ttu-id="82786-1349">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="82786-1349">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="82786-1350">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="82786-1350">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="82786-1351">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="82786-1351">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="82786-1352">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="82786-1352">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="82786-1353">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="82786-1353">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="82786-1354">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="82786-1354">Relay</span></span>

* <span data-ttu-id="82786-1355">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="82786-1355">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="82786-1356">Sql</span><span class="sxs-lookup"><span data-stu-id="82786-1356">Sql</span></span>

* <span data-ttu-id="82786-1357">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="82786-1357">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="82786-1358">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-1358">Storage</span></span>

* <span data-ttu-id="82786-1359">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="82786-1359">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="82786-1360">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="82786-1360">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="82786-1361">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="82786-1361">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="82786-1362">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="82786-1362">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="82786-1363">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-1363">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="82786-1364">VM</span><span class="sxs-lookup"><span data-stu-id="82786-1364">VM</span></span>

* <span data-ttu-id="82786-1365">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="82786-1365">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="82786-1366">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1366">July 31, 2018</span></span>

<span data-ttu-id="82786-1367">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="82786-1367">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="82786-1368">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-1368">ACR</span></span>

* <span data-ttu-id="82786-1369">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="82786-1369">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="82786-1370">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="82786-1370">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="82786-1371">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-1371">ACS</span></span>

* <span data-ttu-id="82786-1372">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="82786-1372">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="82786-1373">Lote</span><span class="sxs-lookup"><span data-stu-id="82786-1373">Batch</span></span>

* <span data-ttu-id="82786-1374">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="82786-1374">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="82786-1375">Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-1375">Container</span></span>

* <span data-ttu-id="82786-1376">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="82786-1376">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="82786-1377">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-1377">Network</span></span>

* <span data-ttu-id="82786-1378">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="82786-1378">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="82786-1379">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-1379">Resource</span></span>

* <span data-ttu-id="82786-1380">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="82786-1380">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="82786-1381">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="82786-1381">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="82786-1382">Função</span><span class="sxs-lookup"><span data-stu-id="82786-1382">Role</span></span>

* <span data-ttu-id="82786-1383">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="82786-1383">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="82786-1384">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="82786-1384">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="82786-1385">Search</span><span class="sxs-lookup"><span data-stu-id="82786-1385">Search</span></span>

* <span data-ttu-id="82786-1386">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="82786-1386">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="82786-1387">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="82786-1387">Service Bus</span></span>

* <span data-ttu-id="82786-1388">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="82786-1388">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="82786-1389">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="82786-1389">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="82786-1390">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="82786-1390">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="82786-1391">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="82786-1391">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="82786-1392">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-1392">Storage</span></span>

* <span data-ttu-id="82786-1393">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="82786-1393">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="82786-1394">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="82786-1394">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="82786-1395">VM</span><span class="sxs-lookup"><span data-stu-id="82786-1395">VM</span></span>

* <span data-ttu-id="82786-1396">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="82786-1396">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="82786-1397">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="82786-1397">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="82786-1398">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="82786-1398">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="82786-1399">[ALTERAÇÃO SIGNIFICATIVA] `[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="82786-1399">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="82786-1400">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1400">July 18, 2018</span></span>

<span data-ttu-id="82786-1401">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="82786-1401">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="82786-1402">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-1402">Core</span></span>

* <span data-ttu-id="82786-1403">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="82786-1403">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="82786-1404">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="82786-1404">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="82786-1405">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="82786-1405">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="82786-1406">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-1406">ACR</span></span>

* <span data-ttu-id="82786-1407">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="82786-1407">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="82786-1408">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="82786-1408">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="82786-1409">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="82786-1409">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="82786-1410">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="82786-1410">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="82786-1411">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-1411">ACS</span></span>

* <span data-ttu-id="82786-1412">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="82786-1412">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-1413">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-1413">AppService</span></span>

* <span data-ttu-id="82786-1414">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="82786-1414">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="82786-1415">Lote</span><span class="sxs-lookup"><span data-stu-id="82786-1415">Batch</span></span>

* <span data-ttu-id="82786-1416">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="82786-1416">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="82786-1417">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="82786-1417">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="82786-1418">Lote AI</span><span class="sxs-lookup"><span data-stu-id="82786-1418">Batch AI</span></span>

* <span data-ttu-id="82786-1419">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="82786-1419">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="82786-1420">Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-1420">Container</span></span>

* <span data-ttu-id="82786-1421">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="82786-1421">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="82786-1422">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="82786-1422">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="82786-1423">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-1423">Network</span></span>

* <span data-ttu-id="82786-1424">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="82786-1424">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="82786-1425">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="82786-1425">Added `network nic wait`</span></span>
* <span data-ttu-id="82786-1426">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="82786-1426">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="82786-1427">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="82786-1427">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="82786-1428">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-1428">Resource</span></span>

* <span data-ttu-id="82786-1429">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="82786-1429">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="82786-1430">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="82786-1430">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="82786-1431">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="82786-1431">Added `deployment wait` command</span></span>
* <span data-ttu-id="82786-1432">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="82786-1432">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="82786-1433">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-1433">SQL</span></span>

* <span data-ttu-id="82786-1434">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="82786-1434">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="82786-1435">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="82786-1435">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="82786-1436">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="82786-1436">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="82786-1437">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-1437">Storage</span></span>

* <span data-ttu-id="82786-1438">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="82786-1438">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="82786-1439">VM</span><span class="sxs-lookup"><span data-stu-id="82786-1439">VM</span></span>

* <span data-ttu-id="82786-1440">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="82786-1440">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="82786-1441">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="82786-1441">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="82786-1442">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="82786-1442">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="82786-1443">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1443">July 3, 2018</span></span>

<span data-ttu-id="82786-1444">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="82786-1444">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="82786-1445">AKS</span><span class="sxs-lookup"><span data-stu-id="82786-1445">AKS</span></span>

* <span data-ttu-id="82786-1446">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="82786-1446">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="82786-1447">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1447">July 3, 2018</span></span>

<span data-ttu-id="82786-1448">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="82786-1448">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="82786-1449">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-1449">Core</span></span>

* <span data-ttu-id="82786-1450">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="82786-1450">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="82786-1451">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-1451">ACR</span></span>

* <span data-ttu-id="82786-1452">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="82786-1452">Added polling build status</span></span>
* <span data-ttu-id="82786-1453">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="82786-1453">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="82786-1454">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="82786-1454">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="82786-1455">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-1455">ACS</span></span>

* <span data-ttu-id="82786-1456">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="82786-1456">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="82786-1457">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="82786-1457">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="82786-1458">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="82786-1458">Updated options for `aks browse` command.</span></span> <span data-ttu-id="82786-1459">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="82786-1459">Added `--listen-port` support</span></span>
* <span data-ttu-id="82786-1460">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="82786-1460">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="82786-1461">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="82786-1461">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="82786-1462">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="82786-1462">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-1463">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-1463">AppService</span></span>

* <span data-ttu-id="82786-1464">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="82786-1464">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="82786-1465">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="82786-1465">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="82786-1466">Backup</span><span class="sxs-lookup"><span data-stu-id="82786-1466">Backup</span></span>

* <span data-ttu-id="82786-1467">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="82786-1467">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="82786-1468">BatchAI</span><span class="sxs-lookup"><span data-stu-id="82786-1468">BatchAI</span></span>

* <span data-ttu-id="82786-1469">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="82786-1469">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="82786-1470">Nuvem</span><span class="sxs-lookup"><span data-stu-id="82786-1470">Cloud</span></span>

* <span data-ttu-id="82786-1471">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="82786-1471">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="82786-1472">Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-1472">Container</span></span>

* <span data-ttu-id="82786-1473">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="82786-1473">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="82786-1474">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="82786-1474">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="82786-1475">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="82786-1475">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="82786-1476">Extensão</span><span class="sxs-lookup"><span data-stu-id="82786-1476">Extension</span></span>

* <span data-ttu-id="82786-1477">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="82786-1477">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="82786-1478">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-1478">Network</span></span>

* <span data-ttu-id="82786-1479">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="82786-1479">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="82786-1480">Rdbms</span><span class="sxs-lookup"><span data-stu-id="82786-1480">Rdbms</span></span>

* <span data-ttu-id="82786-1481">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="82786-1481">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="82786-1482">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-1482">Resource</span></span>

* <span data-ttu-id="82786-1483">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="82786-1483">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="82786-1484">VM</span><span class="sxs-lookup"><span data-stu-id="82786-1484">VM</span></span>

* <span data-ttu-id="82786-1485">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="82786-1485">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="82786-1486">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1486">June 25, 2018</span></span>

<span data-ttu-id="82786-1487">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="82786-1487">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="82786-1488">CLI</span><span class="sxs-lookup"><span data-stu-id="82786-1488">CLI</span></span>

* <span data-ttu-id="82786-1489">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="82786-1489">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="82786-1490">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1490">June 19, 2018</span></span>

<span data-ttu-id="82786-1491">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="82786-1491">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="82786-1492">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-1492">Core</span></span>

* <span data-ttu-id="82786-1493">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="82786-1493">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="82786-1494">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-1494">ACR</span></span>

* <span data-ttu-id="82786-1495">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="82786-1495">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="82786-1496">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="82786-1496">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="82786-1497">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-1497">ACS</span></span>

* <span data-ttu-id="82786-1498">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="82786-1498">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="82786-1499">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="82786-1499">Added `--update` support</span></span>
* <span data-ttu-id="82786-1500">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="82786-1500">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="82786-1501">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="82786-1501">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="82786-1502">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="82786-1502">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="82786-1503">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="82786-1503">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="82786-1504">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="82786-1504">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="82786-1505">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="82786-1505">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-1506">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-1506">AppService</span></span>

* <span data-ttu-id="82786-1507">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="82786-1507">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="82786-1508">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="82786-1508">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="82786-1509">Lote</span><span class="sxs-lookup"><span data-stu-id="82786-1509">Batch</span></span>

* <span data-ttu-id="82786-1510">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="82786-1510">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="82786-1511">Lote AI</span><span class="sxs-lookup"><span data-stu-id="82786-1511">Batch AI</span></span>

* <span data-ttu-id="82786-1512">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="82786-1512">Added support for workspaces.</span></span> <span data-ttu-id="82786-1513">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="82786-1513">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="82786-1514">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="82786-1514">Added support for experiments.</span></span> <span data-ttu-id="82786-1515">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="82786-1515">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="82786-1516">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="82786-1516">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="82786-1517">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="82786-1517">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="82786-1518">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="82786-1518">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="82786-1519">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="82786-1519">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="82786-1520">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="82786-1520">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="82786-1521">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="82786-1521">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="82786-1522">[ALTERAÇÃO SIGNIFICATIVA] `--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="82786-1522">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="82786-1523">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="82786-1523">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="82786-1524">[ALTERAÇÃO SIGNIFICATIVA] `--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="82786-1524">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="82786-1525">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="82786-1525">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="82786-1526">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="82786-1526">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="82786-1527">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="82786-1527">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="82786-1528">[ALTERAÇÃO SIGNIFICATIVA] `--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="82786-1528">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="82786-1529">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="82786-1529">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="82786-1530">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="82786-1530">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="82786-1531">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="82786-1531">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="82786-1532">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="82786-1532">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="82786-1533">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="82786-1533">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="82786-1534">Mapas</span><span class="sxs-lookup"><span data-stu-id="82786-1534">Maps</span></span>

* <span data-ttu-id="82786-1535">[ALTERAÇÃO SIGNIFICATIVA] `maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="82786-1535">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="82786-1536">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-1536">Network</span></span>

* <span data-ttu-id="82786-1537">Foi adicionado suporte a `https` para `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="82786-1537">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="82786-1538">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="82786-1538">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="82786-1539">#6502</span><span class="sxs-lookup"><span data-stu-id="82786-1539">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="82786-1540">Reservas</span><span class="sxs-lookup"><span data-stu-id="82786-1540">Reservations</span></span>

* <span data-ttu-id="82786-1541">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="82786-1541">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="82786-1542">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="82786-1542">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="82786-1543">[ALTERAÇÃO SIGNIFICATIVA] `kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="82786-1543">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="82786-1544">[ALTERAÇÃO SIGNIFICATIVA] `capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="82786-1544">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="82786-1545">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="82786-1545">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="82786-1546">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="82786-1546">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="82786-1547">Função</span><span class="sxs-lookup"><span data-stu-id="82786-1547">Role</span></span>

* <span data-ttu-id="82786-1548">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="82786-1548">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="82786-1549">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-1549">SQL</span></span>

* <span data-ttu-id="82786-1550">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="82786-1550">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="82786-1551">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-1551">Storage</span></span>

* <span data-ttu-id="82786-1552">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="82786-1552">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="82786-1553">VM</span><span class="sxs-lookup"><span data-stu-id="82786-1553">VM</span></span>

* <span data-ttu-id="82786-1554">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="82786-1554">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="82786-1555">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="82786-1555">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="82786-1556">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="82786-1556">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="82786-1557">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1557">June 13, 2018</span></span>

<span data-ttu-id="82786-1558">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="82786-1558">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="82786-1559">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-1559">Core</span></span>

* <span data-ttu-id="82786-1560">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="82786-1560">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="82786-1561">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1561">June 13, 2018</span></span>

<span data-ttu-id="82786-1562">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="82786-1562">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="82786-1563">AKS</span><span class="sxs-lookup"><span data-stu-id="82786-1563">AKS</span></span>

* <span data-ttu-id="82786-1564">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="82786-1564">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="82786-1565">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="82786-1565">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="82786-1566">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="82786-1566">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="82786-1567">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="82786-1567">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="82786-1568">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="82786-1568">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-1569">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-1569">AppService</span></span>

* <span data-ttu-id="82786-1570">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="82786-1570">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="82786-1571">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1571">June 5, 2018</span></span>

<span data-ttu-id="82786-1572">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="82786-1572">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="82786-1573">Interativo</span><span class="sxs-lookup"><span data-stu-id="82786-1573">Interactive</span></span>

* <span data-ttu-id="82786-1574">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="82786-1574">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="82786-1575">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1575">June 5, 2018</span></span>

<span data-ttu-id="82786-1576">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="82786-1576">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="82786-1577">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-1577">Core</span></span>

* <span data-ttu-id="82786-1578">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="82786-1578">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="82786-1579">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="82786-1579">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="82786-1580">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-1580">ACR</span></span>

* <span data-ttu-id="82786-1581">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="82786-1581">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="82786-1582">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="82786-1582">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="82786-1583">AKS</span><span class="sxs-lookup"><span data-stu-id="82786-1583">AKS</span></span>

* <span data-ttu-id="82786-1584">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="82786-1584">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="82786-1585">Lote</span><span class="sxs-lookup"><span data-stu-id="82786-1585">Batch</span></span>

* <span data-ttu-id="82786-1586">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="82786-1586">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="82786-1587">IOT</span><span class="sxs-lookup"><span data-stu-id="82786-1587">IOT</span></span>

* <span data-ttu-id="82786-1588">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="82786-1588">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="82786-1589">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-1589">Network</span></span>

* <span data-ttu-id="82786-1590">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="82786-1590">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="82786-1591">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="82786-1591">Policy Insights</span></span>

* <span data-ttu-id="82786-1592">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="82786-1592">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="82786-1593">ARM</span><span class="sxs-lookup"><span data-stu-id="82786-1593">ARM</span></span>

* <span data-ttu-id="82786-1594">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="82786-1594">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="82786-1595">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-1595">SQL</span></span>

* <span data-ttu-id="82786-1596">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="82786-1596">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="82786-1597">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="82786-1597">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="82786-1598">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-1598">Storage</span></span>

* <span data-ttu-id="82786-1599">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="82786-1599">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="82786-1600">VM</span><span class="sxs-lookup"><span data-stu-id="82786-1600">VM</span></span>

* <span data-ttu-id="82786-1601">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="82786-1601">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="82786-1602">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="82786-1602">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="82786-1603">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="82786-1603">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="82786-1604">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1604">May 22, 2018</span></span>

<span data-ttu-id="82786-1605">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="82786-1605">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="82786-1606">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-1606">Core</span></span>

* <span data-ttu-id="82786-1607">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="82786-1607">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="82786-1608">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-1608">ACS</span></span>

* <span data-ttu-id="82786-1609">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="82786-1609">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="82786-1610">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="82786-1610">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-1611">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-1611">AppService</span></span>

* <span data-ttu-id="82786-1612">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="82786-1612">Improved generic update commands</span></span>
* <span data-ttu-id="82786-1613">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="82786-1613">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="82786-1614">Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-1614">Container</span></span>

* <span data-ttu-id="82786-1615">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="82786-1615">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="82786-1616">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-1616">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="82786-1617">Extensão</span><span class="sxs-lookup"><span data-stu-id="82786-1617">Extension</span></span>

* <span data-ttu-id="82786-1618">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="82786-1618">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="82786-1619">Interativo</span><span class="sxs-lookup"><span data-stu-id="82786-1619">Interactive</span></span>

* <span data-ttu-id="82786-1620">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="82786-1620">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="82786-1621">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="82786-1621">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="82786-1622">KeyVault</span><span class="sxs-lookup"><span data-stu-id="82786-1622">KeyVault</span></span>

* <span data-ttu-id="82786-1623">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="82786-1623">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="82786-1624">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-1624">Network</span></span>

* <span data-ttu-id="82786-1625">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="82786-1625">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="82786-1626">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="82786-1626">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="82786-1627">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-1627">SQL</span></span>

* <span data-ttu-id="82786-1628">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="82786-1628">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="82786-1629">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="82786-1629">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="82786-1630">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="82786-1630">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="82786-1631">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82786-1631">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="82786-1632">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="82786-1632">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="82786-1633">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="82786-1633">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="82786-1634">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="82786-1634">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="82786-1635">`edition`.</span><span class="sxs-lookup"><span data-stu-id="82786-1635">`edition`.</span></span> <span data-ttu-id="82786-1636">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="82786-1636">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="82786-1637">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="82786-1637">`elasticPoolName`.</span></span> <span data-ttu-id="82786-1638">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="82786-1638">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="82786-1639">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="82786-1639">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="82786-1640">`edition`.</span><span class="sxs-lookup"><span data-stu-id="82786-1640">`edition`.</span></span> <span data-ttu-id="82786-1641">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="82786-1641">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="82786-1642">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="82786-1642">`dtu`.</span></span> <span data-ttu-id="82786-1643">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="82786-1643">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="82786-1644">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="82786-1644">`databaseDtuMin`.</span></span> <span data-ttu-id="82786-1645">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="82786-1645">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="82786-1646">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="82786-1646">`databaseDtuMax`.</span></span> <span data-ttu-id="82786-1647">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="82786-1647">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="82786-1648">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="82786-1648">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="82786-1649">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="82786-1649">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="82786-1650">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-1650">Storage</span></span>

* <span data-ttu-id="82786-1651">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="82786-1651">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="82786-1652">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="82786-1652">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="82786-1653">VM</span><span class="sxs-lookup"><span data-stu-id="82786-1653">VM</span></span>

* <span data-ttu-id="82786-1654">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="82786-1654">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="82786-1655">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="82786-1655">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="82786-1656">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="82786-1656">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="82786-1657">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="82786-1657">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="82786-1658">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="82786-1658">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="82786-1659">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1659">May 7, 2018</span></span>

<span data-ttu-id="82786-1660">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="82786-1660">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="82786-1661">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-1661">Core</span></span>

* <span data-ttu-id="82786-1662">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="82786-1662">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="82786-1663">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="82786-1663">Added limited support for positional arguments</span></span>
* <span data-ttu-id="82786-1664">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="82786-1664">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="82786-1665">#5591</span><span class="sxs-lookup"><span data-stu-id="82786-1665">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="82786-1666">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="82786-1666">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="82786-1667">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="82786-1667">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="82786-1668">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="82786-1668">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="82786-1669">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="82786-1669">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="82786-1670">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="82786-1670">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="82786-1671">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-1671">ACR</span></span>

* <span data-ttu-id="82786-1672">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="82786-1672">Added ACR Build commands</span></span>
* <span data-ttu-id="82786-1673">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="82786-1673">Improved resource not found error messages</span></span>
* <span data-ttu-id="82786-1674">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="82786-1674">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="82786-1675">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="82786-1675">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="82786-1676">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="82786-1676">Improved repository commands error messages</span></span>
* <span data-ttu-id="82786-1677">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="82786-1677">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="82786-1678">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-1678">ACS</span></span>

* <span data-ttu-id="82786-1679">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="82786-1679">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="82786-1680">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="82786-1680">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="82786-1681">AMS</span><span class="sxs-lookup"><span data-stu-id="82786-1681">AMS</span></span>

* <span data-ttu-id="82786-1682">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="82786-1682">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-1683">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-1683">Appservice</span></span>

* <span data-ttu-id="82786-1684">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="82786-1684">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="82786-1685">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="82786-1685">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="82786-1686">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="82786-1686">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="82786-1687">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="82786-1687">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="82786-1688">Lote AI</span><span class="sxs-lookup"><span data-stu-id="82786-1688">Batch AI</span></span>

* <span data-ttu-id="82786-1689">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="82786-1689">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="82786-1690">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="82786-1690">Cognitive Services</span></span>

* <span data-ttu-id="82786-1691">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="82786-1691">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="82786-1692">Consumo</span><span class="sxs-lookup"><span data-stu-id="82786-1692">Consumption</span></span>

* <span data-ttu-id="82786-1693">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="82786-1693">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="82786-1694">Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-1694">Container</span></span>

* <span data-ttu-id="82786-1695">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="82786-1695">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="82786-1696">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82786-1696">Cosmos DB</span></span>

* <span data-ttu-id="82786-1697">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82786-1697">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="82786-1698">DMS</span><span class="sxs-lookup"><span data-stu-id="82786-1698">DMS</span></span>

* <span data-ttu-id="82786-1699">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="82786-1699">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="82786-1700">Extensão</span><span class="sxs-lookup"><span data-stu-id="82786-1700">Extension</span></span>

* <span data-ttu-id="82786-1701">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="82786-1701">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="82786-1702">Interativo</span><span class="sxs-lookup"><span data-stu-id="82786-1702">Interactive</span></span>

* <span data-ttu-id="82786-1703">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="82786-1703">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="82786-1704">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="82786-1704">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="82786-1705">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="82786-1705">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="82786-1706">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="82786-1706">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="82786-1707">Laboratório</span><span class="sxs-lookup"><span data-stu-id="82786-1707">Lab</span></span>

* <span data-ttu-id="82786-1708">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="82786-1708">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="82786-1709">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-1709">Network</span></span>

* <span data-ttu-id="82786-1710">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="82786-1710">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="82786-1711">Perfil</span><span class="sxs-lookup"><span data-stu-id="82786-1711">Profile</span></span>

* <span data-ttu-id="82786-1712">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="82786-1712">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="82786-1713">[ALTERAÇÃO SIGNIFICATIVA] `--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="82786-1713">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="82786-1714">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="82786-1714">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="82786-1715">Redis</span><span class="sxs-lookup"><span data-stu-id="82786-1715">Redis</span></span>

* <span data-ttu-id="82786-1716">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="82786-1716">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="82786-1717">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="82786-1717">Deprecated `redis list-all`.</span></span> <span data-ttu-id="82786-1718">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="82786-1718">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="82786-1719">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="82786-1719">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="82786-1720">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="82786-1720">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="82786-1721">Função</span><span class="sxs-lookup"><span data-stu-id="82786-1721">Role</span></span>

* <span data-ttu-id="82786-1722">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="82786-1722">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="82786-1723">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-1723">Storage</span></span>

* <span data-ttu-id="82786-1724">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="82786-1724">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="82786-1725">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="82786-1725">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="82786-1726">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="82786-1726">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="82786-1727">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="82786-1727">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="82786-1728">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="82786-1728">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="82786-1729">VM</span><span class="sxs-lookup"><span data-stu-id="82786-1729">VM</span></span>

* <span data-ttu-id="82786-1730">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="82786-1730">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="82786-1731">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="82786-1731">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="82786-1732">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="82786-1732">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="82786-1733">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="82786-1733">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="82786-1734">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="82786-1734">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="82786-1735">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="82786-1735">Added write accelerator support</span></span>
* <span data-ttu-id="82786-1736">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="82786-1736">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="82786-1737">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="82786-1737">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="82786-1738">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="82786-1738">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="82786-1739">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1739">April 10, 2018</span></span>

<span data-ttu-id="82786-1740">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="82786-1740">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="82786-1741">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-1741">ACR</span></span>

* <span data-ttu-id="82786-1742">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="82786-1742">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="82786-1743">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-1743">ACS</span></span>

* <span data-ttu-id="82786-1744">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="82786-1744">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-1745">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-1745">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="82786-1747">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="82786-1747">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="82786-1748">BatchAI</span><span class="sxs-lookup"><span data-stu-id="82786-1748">BatchAI</span></span>

* <span data-ttu-id="82786-1749">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="82786-1749">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="82786-1750">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="82786-1750">Job level mounting</span></span>
  - <span data-ttu-id="82786-1751">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="82786-1751">Environment variables with secret values</span></span>
  - <span data-ttu-id="82786-1752">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="82786-1752">Performance counters settings</span></span>
  - <span data-ttu-id="82786-1753">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="82786-1753">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="82786-1754">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="82786-1754">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="82786-1755">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="82786-1755">Usage and limits reporting</span></span>
  - <span data-ttu-id="82786-1756">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="82786-1756">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="82786-1757">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="82786-1757">Support for custom images</span></span>
  - <span data-ttu-id="82786-1758">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="82786-1758">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="82786-1759">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="82786-1759">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="82786-1760">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="82786-1760">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="82786-1761">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="82786-1761">National clouds are supported</span></span>
* <span data-ttu-id="82786-1762">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="82786-1762">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="82786-1763">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="82786-1763">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="82786-1764">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="82786-1764">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="82786-1765">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="82786-1765">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="82786-1766">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="82786-1766">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="82786-1767">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="82786-1767">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="82786-1768">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="82786-1768">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="82786-1769">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="82786-1769">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="82786-1770">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="82786-1770">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="82786-1771">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="82786-1771">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="82786-1772">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="82786-1772">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="82786-1773">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="82786-1773">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="82786-1774">[ALTERAÇÃO SIGNIFICATIVA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="82786-1774">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="82786-1775">Cobrança</span><span class="sxs-lookup"><span data-stu-id="82786-1775">Billing</span></span>

* <span data-ttu-id="82786-1776">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="82786-1776">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="82786-1777">Consumo</span><span class="sxs-lookup"><span data-stu-id="82786-1777">Consumption</span></span>

* <span data-ttu-id="82786-1778">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="82786-1778">Added `marketplace` commands</span></span>
* <span data-ttu-id="82786-1779">[ALTERAÇÃO SIGNIFICATIVA] `reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="82786-1779">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="82786-1780">[ALTERAÇÃO SIGNIFICATIVA] `reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="82786-1780">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="82786-1781">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="82786-1781">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="82786-1782">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="82786-1782">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="82786-1783">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="82786-1783">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="82786-1784">Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-1784">Container</span></span>

* <span data-ttu-id="82786-1785">Adição dos parâmetros de montagem de volume de repositório git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="82786-1785">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="82786-1786">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="82786-1786">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="82786-1787">Extensão</span><span class="sxs-lookup"><span data-stu-id="82786-1787">Extension</span></span>

* <span data-ttu-id="82786-1788">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="82786-1788">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="82786-1789">Interativo</span><span class="sxs-lookup"><span data-stu-id="82786-1789">Interactive</span></span>

* <span data-ttu-id="82786-1790">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="82786-1790">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="82786-1791">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="82786-1791">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="82786-1792">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="82786-1792">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="82786-1793">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-1793">Network</span></span>

* <span data-ttu-id="82786-1794">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="82786-1794">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="82786-1795">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82786-1795">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="82786-1796">#4910</span><span class="sxs-lookup"><span data-stu-id="82786-1796">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="82786-1797">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="82786-1797">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="82786-1798">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="82786-1798">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="82786-1799">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-1799">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="82786-1800">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-1800">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="82786-1801">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="82786-1801">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="82786-1802">Perfil</span><span class="sxs-lookup"><span data-stu-id="82786-1802">Profile</span></span>

* <span data-ttu-id="82786-1803">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="82786-1803">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="82786-1804">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="82786-1804">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="82786-1805">RDBMS</span><span class="sxs-lookup"><span data-stu-id="82786-1805">RDBMS</span></span>

* <span data-ttu-id="82786-1806">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="82786-1806">Added `georestore` command</span></span>
* <span data-ttu-id="82786-1807">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="82786-1807">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="82786-1808">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-1808">Resource</span></span>

* <span data-ttu-id="82786-1809">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="82786-1809">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="82786-1810">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="82786-1810">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="82786-1811">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-1811">SQL</span></span>

* <span data-ttu-id="82786-1812">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="82786-1812">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="82786-1813">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-1813">Storage</span></span>

* <span data-ttu-id="82786-1814">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="82786-1814">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="82786-1815">VM</span><span class="sxs-lookup"><span data-stu-id="82786-1815">VM</span></span>

* <span data-ttu-id="82786-1816">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="82786-1816">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="82786-1817">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="82786-1817">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="82786-1819">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="82786-1819">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="82786-1820">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="82786-1820">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="82786-1821">#5718</span><span class="sxs-lookup"><span data-stu-id="82786-1821">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="82786-1822">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="82786-1822">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="82786-1823">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1823">March 27, 2018</span></span>

<span data-ttu-id="82786-1824">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="82786-1824">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="82786-1825">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-1825">Core</span></span>

* <span data-ttu-id="82786-1826">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="82786-1826">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="82786-1827">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-1827">ACS</span></span>

* <span data-ttu-id="82786-1828">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="82786-1828">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-1829">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-1829">Appservice</span></span>

* <span data-ttu-id="82786-1830">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="82786-1830">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="82786-1831">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="82786-1831">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="82786-1832">Backup</span><span class="sxs-lookup"><span data-stu-id="82786-1832">Backup</span></span>

* <span data-ttu-id="82786-1833">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="82786-1833">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="82786-1834">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="82786-1834">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="82786-1835">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="82786-1835">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="82786-1836">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="82786-1836">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="82786-1837">Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-1837">Container</span></span>

* <span data-ttu-id="82786-1838">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="82786-1838">Added `container exec` command.</span></span> <span data-ttu-id="82786-1839">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="82786-1839">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="82786-1840">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-1840">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="82786-1841">Extensão</span><span class="sxs-lookup"><span data-stu-id="82786-1841">Extension</span></span>

* <span data-ttu-id="82786-1842">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="82786-1842">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="82786-1843">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="82786-1843">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="82786-1844">[ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="82786-1844">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="82786-1845">Interativo</span><span class="sxs-lookup"><span data-stu-id="82786-1845">Interactive</span></span>

* <span data-ttu-id="82786-1846">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="82786-1846">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="82786-1847">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="82786-1847">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="82786-1848">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="82786-1848">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="82786-1849">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="82786-1849">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="82786-1850">Laboratório</span><span class="sxs-lookup"><span data-stu-id="82786-1850">Lab</span></span>

* <span data-ttu-id="82786-1851">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="82786-1851">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="82786-1852">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="82786-1852">Monitor</span></span>

* <span data-ttu-id="82786-1853">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="82786-1853">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="82786-1854">Corrigido [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="82786-1854">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="82786-1855">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="82786-1855">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="82786-1856">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-1856">Network</span></span>

* <span data-ttu-id="82786-1857">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="82786-1857">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="82786-1858">Perfil</span><span class="sxs-lookup"><span data-stu-id="82786-1858">Profile</span></span>

* <span data-ttu-id="82786-1859">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="82786-1859">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="82786-1860">RDBMS</span><span class="sxs-lookup"><span data-stu-id="82786-1860">RDBMS</span></span>

* <span data-ttu-id="82786-1861">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="82786-1861">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="82786-1862">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-1862">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="82786-1864">Função</span><span class="sxs-lookup"><span data-stu-id="82786-1864">Role</span></span>

* <span data-ttu-id="82786-1865">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="82786-1865">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="82786-1866">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="82786-1866">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="82786-1867">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="82786-1867">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="82786-1868">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="82786-1868">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="82786-1869">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="82786-1869">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="82786-1870">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-1870">Storage</span></span>

* <span data-ttu-id="82786-1871">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="82786-1871">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="82786-1872">Corrigido [#4049](https://github.com/Azure/azure-cli/issues/4049): problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="82786-1872">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="82786-1873">VM</span><span class="sxs-lookup"><span data-stu-id="82786-1873">VM</span></span>

* <span data-ttu-id="82786-1874">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="82786-1874">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="82786-1875">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="82786-1875">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="82786-1876">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="82786-1876">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="82786-1877">[ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="82786-1877">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="82786-1878">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1878">March 13, 2018</span></span>

<span data-ttu-id="82786-1879">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="82786-1879">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="82786-1880">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-1880">ACR</span></span>

* <span data-ttu-id="82786-1881">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="82786-1881">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="82786-1882">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="82786-1882">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="82786-1883">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="82786-1883">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="82786-1884">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-1884">ACS</span></span>

* <span data-ttu-id="82786-1885">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="82786-1885">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="82786-1886">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="82786-1886">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="82786-1887">Supervisor</span><span class="sxs-lookup"><span data-stu-id="82786-1887">Advisor</span></span>

* <span data-ttu-id="82786-1888">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="82786-1888">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="82786-1889">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="82786-1889">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="82786-1890">[ALTERAÇÃO SIGNIFICATIVA] `advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="82786-1890">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="82786-1891">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="82786-1891">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="82786-1892">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="82786-1892">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-1893">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-1893">Appservice</span></span>

* <span data-ttu-id="82786-1894">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="82786-1894">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="82786-1895">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="82786-1895">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="82786-1896">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="82786-1896">Eventhubs</span></span>

* <span data-ttu-id="82786-1897">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="82786-1897">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="82786-1898">Extensão</span><span class="sxs-lookup"><span data-stu-id="82786-1898">Extension</span></span>

* <span data-ttu-id="82786-1899">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="82786-1899">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="82786-1900">Interativo</span><span class="sxs-lookup"><span data-stu-id="82786-1900">Interactive</span></span>

* <span data-ttu-id="82786-1901">Corrigido [#5625](https://github.com/Azure/azure-cli/issues/5625): manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="82786-1901">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="82786-1902">Corrigido [#3016](https://github.com/Azure/azure-cli/issues/3016): histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="82786-1902">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="82786-1903">Corrigido [#5688](https://github.com/Azure/azure-cli/issues/5688): as conclusões não aparecerão se o carregamento da tabela de comando encontrar uma exceção</span><span class="sxs-lookup"><span data-stu-id="82786-1903">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="82786-1904">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="82786-1904">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="82786-1905">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="82786-1905">Monitor</span></span>

* <span data-ttu-id="82786-1906">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="82786-1906">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="82786-1907">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="82786-1907">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="82786-1908">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="82786-1908">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="82786-1909">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="82786-1909">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="82786-1910">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-1910">Network</span></span>

* <span data-ttu-id="82786-1911">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="82786-1911">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="82786-1912">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="82786-1912">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="82786-1913">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="82786-1913">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="82786-1914">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="82786-1914">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="82786-1915">Perfil</span><span class="sxs-lookup"><span data-stu-id="82786-1915">Profile</span></span>

* <span data-ttu-id="82786-1916">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="82786-1916">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="82786-1917">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="82786-1917">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="82786-1918">RDBMS</span><span class="sxs-lookup"><span data-stu-id="82786-1918">RDBMS</span></span>

* <span data-ttu-id="82786-1919">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="82786-1919">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="82786-1920">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="82786-1920">Service Bus</span></span>

* <span data-ttu-id="82786-1921">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="82786-1921">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="82786-1922">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-1922">Storage</span></span>

* <span data-ttu-id="82786-1923">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="82786-1923">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="82786-1924">Corrigido [#5286](https://github.com/Azure/azure-cli/issues/5286): os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="82786-1924">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="82786-1925">VM</span><span class="sxs-lookup"><span data-stu-id="82786-1925">VM</span></span>

* <span data-ttu-id="82786-1926">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="82786-1926">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="82786-1927">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="82786-1927">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="82786-1928">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="82786-1928">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="82786-1929">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="82786-1929">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="82786-1930">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1930">February 27, 2018</span></span>

<span data-ttu-id="82786-1931">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="82786-1931">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="82786-1932">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-1932">Core</span></span>

* <span data-ttu-id="82786-1933">Corrigido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="82786-1933">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="82786-1934">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="82786-1934">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="82786-1935">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="82786-1935">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="82786-1936">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-1936">ACS</span></span>

* <span data-ttu-id="82786-1937">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="82786-1937">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="82786-1938">Problema corrigido: permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="82786-1938">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="82786-1939">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="82786-1939">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="82786-1940">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="82786-1940">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-1941">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-1941">Appservice</span></span>

* <span data-ttu-id="82786-1942">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="82786-1942">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="82786-1943">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="82786-1943">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="82786-1944">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="82786-1944">Cognitive Services</span></span>

* <span data-ttu-id="82786-1945">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="82786-1945">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="82786-1946">Consumo</span><span class="sxs-lookup"><span data-stu-id="82786-1946">Consumption</span></span>

* <span data-ttu-id="82786-1947">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="82786-1947">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="82786-1948">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="82786-1948">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="82786-1949">Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-1949">Container</span></span>

* <span data-ttu-id="82786-1950">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="82786-1950">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="82786-1951">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-1951">Network</span></span>

* <span data-ttu-id="82786-1952">Corrigido [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="82786-1952">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="82786-1953">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-1953">Resource</span></span>

* <span data-ttu-id="82786-1954">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="82786-1954">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="82786-1955">Função</span><span class="sxs-lookup"><span data-stu-id="82786-1955">Role</span></span>

* <span data-ttu-id="82786-1956">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="82786-1956">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="82786-1957">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-1957">SQL</span></span>

* <span data-ttu-id="82786-1958">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="82786-1958">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="82786-1959">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-1959">Storage</span></span>

* <span data-ttu-id="82786-1960">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="82786-1960">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="82786-1961">VM</span><span class="sxs-lookup"><span data-stu-id="82786-1961">VM</span></span>

* <span data-ttu-id="82786-1962">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="82786-1962">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="82786-1963">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-1963">February 13, 2018</span></span>

<span data-ttu-id="82786-1964">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="82786-1964">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="82786-1965">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-1965">Core</span></span>

* <span data-ttu-id="82786-1966">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="82786-1966">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="82786-1967">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-1967">ACS</span></span>

* <span data-ttu-id="82786-1968">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="82786-1968">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="82786-1969">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="82786-1969">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="82786-1970">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="82786-1970">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="82786-1971">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="82786-1971">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="82786-1972">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="82786-1972">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="82786-1973">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="82786-1973">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="82786-1974">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="82786-1974">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="82786-1975">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="82786-1975">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-1976">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-1976">Appservice</span></span>

* <span data-ttu-id="82786-1977">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="82786-1977">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="82786-1978">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="82786-1978">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="82786-1979">CDN</span><span class="sxs-lookup"><span data-stu-id="82786-1979">CDN</span></span>

* <span data-ttu-id="82786-1980">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="82786-1980">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="82786-1981">Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-1981">Container</span></span>

* <span data-ttu-id="82786-1982">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="82786-1982">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="82786-1983">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-1983">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82786-1984">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="82786-1984">CosmosDB</span></span>

* <span data-ttu-id="82786-1985">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="82786-1985">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="82786-1986">Extensão</span><span class="sxs-lookup"><span data-stu-id="82786-1986">Extension</span></span>

* <span data-ttu-id="82786-1987">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-1987">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="82786-1988">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-1988">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="82786-1989">Comentários</span><span class="sxs-lookup"><span data-stu-id="82786-1989">Feedback</span></span>

* <span data-ttu-id="82786-1990">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="82786-1990">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="82786-1991">Interativo</span><span class="sxs-lookup"><span data-stu-id="82786-1991">Interactive</span></span>

* <span data-ttu-id="82786-1992">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="82786-1992">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="82786-1993">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="82786-1993">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="82786-1994">IoT</span><span class="sxs-lookup"><span data-stu-id="82786-1994">IoT</span></span>

* <span data-ttu-id="82786-1995">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="82786-1995">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="82786-1996">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="82786-1996">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="82786-1997">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-1997">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="82786-1998">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="82786-1998">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="82786-1999">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="82786-1999">Monitor</span></span>

* <span data-ttu-id="82786-2000">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="82786-2000">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="82786-2001">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-2001">Network</span></span>

* <span data-ttu-id="82786-2002">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="82786-2002">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="82786-2003">Perfil</span><span class="sxs-lookup"><span data-stu-id="82786-2003">Profile</span></span>

* <span data-ttu-id="82786-2004">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="82786-2004">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="82786-2005">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-2005">Resource</span></span>

* <span data-ttu-id="82786-2006">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="82786-2006">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="82786-2007">Função</span><span class="sxs-lookup"><span data-stu-id="82786-2007">Role</span></span>

* <span data-ttu-id="82786-2008">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="82786-2008">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="82786-2009">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-2009">SQL</span></span>

* <span data-ttu-id="82786-2010">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="82786-2010">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="82786-2011">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="82786-2011">Added `sql db rename`</span></span>
* <span data-ttu-id="82786-2012">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="82786-2012">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="82786-2013">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-2013">Storage</span></span>

* <span data-ttu-id="82786-2014">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="82786-2014">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="82786-2015">VM</span><span class="sxs-lookup"><span data-stu-id="82786-2015">VM</span></span>

* <span data-ttu-id="82786-2016">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="82786-2016">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="82786-2017">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="82786-2017">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="82786-2018">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="82786-2018">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="82786-2019">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-2019">January 31, 2018</span></span>

<span data-ttu-id="82786-2020">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="82786-2020">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="82786-2021">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-2021">Core</span></span>

* <span data-ttu-id="82786-2022">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="82786-2022">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="82786-2023">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="82786-2023">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="82786-2024">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="82786-2024">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="82786-2025">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="82786-2025">Use `--verbose` to see</span></span>
* <span data-ttu-id="82786-2026">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="82786-2026">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="82786-2027">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-2027">ACS</span></span>

* <span data-ttu-id="82786-2028">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="82786-2028">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="82786-2029">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="82786-2029">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-2030">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-2030">Appservice</span></span>

* <span data-ttu-id="82786-2031">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="82786-2031">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="82786-2032">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="82786-2032">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="82786-2033">CDN</span><span class="sxs-lookup"><span data-stu-id="82786-2033">CDN</span></span>

* <span data-ttu-id="82786-2034">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="82786-2034">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82786-2035">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="82786-2035">CosmosDB</span></span>

* <span data-ttu-id="82786-2036">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="82786-2036">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="82786-2037">Interativo</span><span class="sxs-lookup"><span data-stu-id="82786-2037">Interactive</span></span>

* <span data-ttu-id="82786-2038">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="82786-2038">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="82786-2039">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-2039">Network</span></span>

* <span data-ttu-id="82786-2040">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="82786-2040">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="82786-2041">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="82786-2041">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="82786-2042">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="82786-2042">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="82786-2043">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="82786-2043">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="82786-2044">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="82786-2044">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="82786-2045">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="82786-2045">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="82786-2046">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="82786-2046">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="82786-2047">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="82786-2047">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="82786-2048">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="82786-2048">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="82786-2049">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="82786-2049">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="82786-2050">Perfil</span><span class="sxs-lookup"><span data-stu-id="82786-2050">Profile</span></span>

* <span data-ttu-id="82786-2051">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="82786-2051">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="82786-2052">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-2052">Resource</span></span>

* <span data-ttu-id="82786-2053">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="82786-2053">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="82786-2054">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-2054">Storage</span></span>

* <span data-ttu-id="82786-2055">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="82786-2055">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="82786-2056">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="82786-2056">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="82786-2057">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="82786-2057">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="82786-2058">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="82786-2058">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="82786-2059">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="82786-2059">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="82786-2060">VM</span><span class="sxs-lookup"><span data-stu-id="82786-2060">VM</span></span>

* <span data-ttu-id="82786-2061">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="82786-2061">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="82786-2062">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="82786-2062">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="82786-2063">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="82786-2063">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="82786-2064">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="82786-2064">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="82786-2065">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="82786-2065">January 17, 2018</span></span>

<span data-ttu-id="82786-2066">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="82786-2066">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="82786-2067">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-2067">ACR</span></span>

* <span data-ttu-id="82786-2068">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="82786-2068">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="82786-2069">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="82786-2069">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="82786-2070">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-2070">ACS</span></span>

* <span data-ttu-id="82786-2071">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="82786-2071">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="82786-2072">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="82786-2072">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-2073">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-2073">Appservice</span></span>

* <span data-ttu-id="82786-2074">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="82786-2074">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="82786-2075">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="82786-2075">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="82786-2076">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="82786-2076">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="82786-2077">Backup</span><span class="sxs-lookup"><span data-stu-id="82786-2077">Backup</span></span>

* <span data-ttu-id="82786-2078">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="82786-2078">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="82786-2079">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="82786-2079">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="82786-2080">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="82786-2080">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="82786-2081">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="82786-2081">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="82786-2082">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="82786-2082">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="82786-2083">Lote</span><span class="sxs-lookup"><span data-stu-id="82786-2083">Batch</span></span>

* <span data-ttu-id="82786-2084">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="82786-2084">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="82786-2085">Nuvem</span><span class="sxs-lookup"><span data-stu-id="82786-2085">Cloud</span></span>

* <span data-ttu-id="82786-2086">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="82786-2086">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="82786-2087">Consumo</span><span class="sxs-lookup"><span data-stu-id="82786-2087">Consumption</span></span>

* <span data-ttu-id="82786-2088">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="82786-2088">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="82786-2089">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="82786-2089">Event Grid</span></span>

* <span data-ttu-id="82786-2090">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="82786-2090">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="82786-2091">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="82786-2091">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="82786-2092">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="82786-2092">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="82786-2093">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="82786-2093">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="82786-2094">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="82786-2094">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="82786-2095">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="82786-2095">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="82786-2096">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="82786-2096">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="82786-2097">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="82786-2097">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="82786-2098">Interativo</span><span class="sxs-lookup"><span data-stu-id="82786-2098">Interactive</span></span>

* <span data-ttu-id="82786-2099">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="82786-2099">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="82786-2100">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="82786-2100">Fixed errors on startup</span></span>
* <span data-ttu-id="82786-2101">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="82786-2101">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="82786-2102">IoT</span><span class="sxs-lookup"><span data-stu-id="82786-2102">IoT</span></span>

* <span data-ttu-id="82786-2103">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="82786-2103">Added support for device provisioning service</span></span>
* <span data-ttu-id="82786-2104">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="82786-2104">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="82786-2105">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="82786-2105">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="82786-2106">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="82786-2106">Monitor</span></span>

* <span data-ttu-id="82786-2107">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="82786-2107">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="82786-2108">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="82786-2108">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="82786-2109">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="82786-2109">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="82786-2110">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-2110">Network</span></span>

* <span data-ttu-id="82786-2111">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="82786-2111">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="82786-2112">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-2112">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="82786-2113">Perfil</span><span class="sxs-lookup"><span data-stu-id="82786-2113">Profile</span></span>

* <span data-ttu-id="82786-2114">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="82786-2114">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="82786-2115">Função</span><span class="sxs-lookup"><span data-stu-id="82786-2115">Role</span></span>

* <span data-ttu-id="82786-2116">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="82786-2116">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="82786-2117">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="82786-2117">Service Fabric</span></span>

* <span data-ttu-id="82786-2118">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="82786-2118">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="82786-2119">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="82786-2119">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="82786-2120">VM</span><span class="sxs-lookup"><span data-stu-id="82786-2120">VM</span></span>

* <span data-ttu-id="82786-2121">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="82786-2121">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="82786-2122">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="82786-2122">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="82786-2123">[ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="82786-2123">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="82786-2124">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="82786-2124">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="82786-2125">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="82786-2125">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="82786-2126">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="82786-2126">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="82786-2127">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="82786-2127">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="82786-2128">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="82786-2128">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="82786-2129">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="82786-2129">December 19, 2017</span></span>

<span data-ttu-id="82786-2130">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="82786-2130">Version 2.0.23</span></span>

* <span data-ttu-id="82786-2131">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="82786-2131">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="82786-2132">Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-2132">Container</span></span>

* <span data-ttu-id="82786-2133">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-2133">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="82786-2134">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-2134">Network</span></span>

* <span data-ttu-id="82786-2135">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-2135">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="82786-2136">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-2136">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="82786-2137">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-2137">Storage</span></span>

* <span data-ttu-id="82786-2138">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="82786-2138">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="82786-2139">VM</span><span class="sxs-lookup"><span data-stu-id="82786-2139">VM</span></span>

* <span data-ttu-id="82786-2140">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="82786-2140">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="82786-2141">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="82786-2141">December 5, 2017</span></span>

<span data-ttu-id="82786-2142">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="82786-2142">Version 2.0.22</span></span>

* <span data-ttu-id="82786-2143">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="82786-2143">Removed `az component` commands.</span></span> <span data-ttu-id="82786-2144">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="82786-2144">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="82786-2145">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-2145">Core</span></span>
* <span data-ttu-id="82786-2146">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="82786-2146">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="82786-2147">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="82786-2147">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="82786-2148">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-2148">ACS</span></span>

* <span data-ttu-id="82786-2149">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="82786-2149">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="82786-2150">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="82786-2150">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="82786-2151">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="82786-2151">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="82786-2152">Supervisor</span><span class="sxs-lookup"><span data-stu-id="82786-2152">Advisor</span></span>

* <span data-ttu-id="82786-2153">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="82786-2153">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-2154">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-2154">Appservice</span></span>

* <span data-ttu-id="82786-2155">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="82786-2155">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="82786-2156">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="82786-2156">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="82786-2157">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="82786-2157">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="82786-2158">Consumo</span><span class="sxs-lookup"><span data-stu-id="82786-2158">Consumption</span></span>

* <span data-ttu-id="82786-2159">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="82786-2159">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="82786-2160">Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-2160">Container</span></span>

* <span data-ttu-id="82786-2161">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="82786-2161">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="82786-2162">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="82786-2162">Monitor</span></span>

* <span data-ttu-id="82786-2163">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="82786-2163">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="82786-2164">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-2164">Resource</span></span>

* <span data-ttu-id="82786-2165">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="82786-2165">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="82786-2166">Função</span><span class="sxs-lookup"><span data-stu-id="82786-2166">Role</span></span>

* <span data-ttu-id="82786-2167">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="82786-2167">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="82786-2168">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="82786-2168">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="82786-2169">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="82786-2169">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="82786-2170">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-2170">SQL</span></span>

* <span data-ttu-id="82786-2171">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="82786-2171">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="82786-2172">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="82786-2172">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="82786-2173">VM</span><span class="sxs-lookup"><span data-stu-id="82786-2173">VM</span></span>

* <span data-ttu-id="82786-2174">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="82786-2174">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="82786-2175">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="82786-2175">November 14, 2017</span></span>

<span data-ttu-id="82786-2176">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="82786-2176">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="82786-2177">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-2177">ACR</span></span>

* <span data-ttu-id="82786-2178">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="82786-2178">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="82786-2179">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-2179">ACS</span></span>

* <span data-ttu-id="82786-2180">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="82786-2180">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="82786-2181">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="82786-2181">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="82786-2182">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="82786-2182">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="82786-2183">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="82786-2183">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="82786-2184">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="82786-2184">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-2185">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-2185">Appservice</span></span>

* <span data-ttu-id="82786-2186">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="82786-2186">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="82786-2187">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="82786-2187">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="82786-2188">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="82786-2188">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="82786-2189">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="82786-2189">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="82786-2190">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="82786-2190">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="82786-2191">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="82786-2191">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="82786-2192">Lote</span><span class="sxs-lookup"><span data-stu-id="82786-2192">Batch</span></span>

* <span data-ttu-id="82786-2193">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="82786-2193">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="82786-2194">Batchai</span><span class="sxs-lookup"><span data-stu-id="82786-2194">Batchai</span></span>

* <span data-ttu-id="82786-2195">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="82786-2195">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="82786-2196">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="82786-2196">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="82786-2197">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="82786-2197">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="82786-2198">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="82786-2198">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="82786-2199">Nuvem</span><span class="sxs-lookup"><span data-stu-id="82786-2199">Cloud</span></span>

* <span data-ttu-id="82786-2200">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="82786-2200">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="82786-2201">Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-2201">Container</span></span>

* <span data-ttu-id="82786-2202">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="82786-2202">Added support to open multiple ports</span></span>
* <span data-ttu-id="82786-2203">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="82786-2203">Added container group restart policy</span></span>
* <span data-ttu-id="82786-2204">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="82786-2204">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="82786-2205">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="82786-2205">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="82786-2206">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="82786-2206">Data Lake Analytics</span></span>

* <span data-ttu-id="82786-2207">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="82786-2207">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="82786-2208">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="82786-2208">Data Lake Store</span></span>

* <span data-ttu-id="82786-2209">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="82786-2209">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="82786-2210">Extensão</span><span class="sxs-lookup"><span data-stu-id="82786-2210">Extension</span></span>

* <span data-ttu-id="82786-2211">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="82786-2211">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="82786-2212">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="82786-2212">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="82786-2213">IoT</span><span class="sxs-lookup"><span data-stu-id="82786-2213">IoT</span></span>

* <span data-ttu-id="82786-2214">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="82786-2214">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="82786-2215">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="82786-2215">Monitor</span></span>

* <span data-ttu-id="82786-2216">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="82786-2216">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="82786-2217">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-2217">Network</span></span>

* <span data-ttu-id="82786-2218">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="82786-2218">Added support for CAA DNS records</span></span>
* <span data-ttu-id="82786-2219">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="82786-2219">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="82786-2220">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="82786-2220">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="82786-2221">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="82786-2221">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="82786-2222">Reservas</span><span class="sxs-lookup"><span data-stu-id="82786-2222">Reservations</span></span>

* <span data-ttu-id="82786-2223">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="82786-2223">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="82786-2224">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-2224">Resource</span></span>

* <span data-ttu-id="82786-2225">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="82786-2225">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="82786-2226">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-2226">SQL</span></span>

* <span data-ttu-id="82786-2227">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-2227">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="82786-2228">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-2228">Storage</span></span>

* <span data-ttu-id="82786-2229">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="82786-2229">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="82786-2230">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="82786-2230">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="82786-2231">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="82786-2231">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="82786-2232">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="82786-2232">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="82786-2233">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="82786-2233">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="82786-2234">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="82786-2234">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="82786-2235">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-2235">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="82786-2236">VM</span><span class="sxs-lookup"><span data-stu-id="82786-2236">VM</span></span>

* <span data-ttu-id="82786-2237">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="82786-2237">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="82786-2238">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="82786-2238">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="82786-2239">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="82786-2239">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="82786-2240">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="82786-2240">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="82786-2241">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="82786-2241">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="82786-2242">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="82786-2242">October 24, 2017</span></span>

<span data-ttu-id="82786-2243">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="82786-2243">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="82786-2244">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-2244">Core</span></span>

* <span data-ttu-id="82786-2245">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="82786-2245">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="82786-2246">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-2246">ACR</span></span>

* <span data-ttu-id="82786-2247">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="82786-2247">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="82786-2248">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="82786-2248">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="82786-2249">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="82786-2249">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="82786-2250">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-2250">ACS</span></span>

* <span data-ttu-id="82786-2251">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="82786-2251">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="82786-2252">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="82786-2252">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-2253">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-2253">Appservice</span></span>

* <span data-ttu-id="82786-2254">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="82786-2254">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="82786-2255">Componente</span><span class="sxs-lookup"><span data-stu-id="82786-2255">Component</span></span>

* <span data-ttu-id="82786-2256">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="82786-2256">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="82786-2257">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="82786-2257">Monitor</span></span>

* <span data-ttu-id="82786-2258">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="82786-2258">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="82786-2259">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-2259">Resource</span></span>

* <span data-ttu-id="82786-2260">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="82786-2260">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="82786-2261">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="82786-2261">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="82786-2262">VM</span><span class="sxs-lookup"><span data-stu-id="82786-2262">VM</span></span>

* <span data-ttu-id="82786-2263">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="82786-2263">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="82786-2264">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="82786-2264">October 9, 2017</span></span>

<span data-ttu-id="82786-2265">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="82786-2265">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="82786-2266">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-2266">Core</span></span>

* <span data-ttu-id="82786-2267">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="82786-2267">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-2268">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-2268">Appservice</span></span>

* <span data-ttu-id="82786-2269">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="82786-2269">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="82786-2270">Lote</span><span class="sxs-lookup"><span data-stu-id="82786-2270">Batch</span></span>

* <span data-ttu-id="82786-2271">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="82786-2271">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="82786-2272">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="82786-2272">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="82786-2273">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="82786-2273">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="82786-2274">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="82786-2274">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="82786-2275">Batchai</span><span class="sxs-lookup"><span data-stu-id="82786-2275">Batchai</span></span>

* <span data-ttu-id="82786-2276">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="82786-2276">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="82786-2277">Keyvault</span><span class="sxs-lookup"><span data-stu-id="82786-2277">Keyvault</span></span>

* <span data-ttu-id="82786-2278">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="82786-2278">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="82786-2279">(#4448)</span><span class="sxs-lookup"><span data-stu-id="82786-2279">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="82786-2280">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-2280">Network</span></span>

* <span data-ttu-id="82786-2281">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="82786-2281">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="82786-2282">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="82786-2282">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="82786-2283">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-2283">Resource</span></span>

* <span data-ttu-id="82786-2284">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="82786-2284">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="82786-2285">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="82786-2285">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="82786-2286">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="82786-2286">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="82786-2287">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="82786-2287">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="82786-2288">Sql</span><span class="sxs-lookup"><span data-stu-id="82786-2288">Sql</span></span>

* <span data-ttu-id="82786-2289">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="82786-2289">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="82786-2290">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="82786-2290">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="82786-2291">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="82786-2291">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="82786-2292">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-2292">Storage</span></span>

* <span data-ttu-id="82786-2293">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="82786-2293">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="82786-2294">VM</span><span class="sxs-lookup"><span data-stu-id="82786-2294">Vm</span></span>

* <span data-ttu-id="82786-2295">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="82786-2295">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="82786-2296">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="82786-2296">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="82786-2297">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="82786-2297">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="82786-2298">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="82786-2298">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="82786-2299">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="82786-2299">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="82786-2300">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="82786-2300">September 22, 2017</span></span>

<span data-ttu-id="82786-2301">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="82786-2301">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="82786-2302">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-2302">Resource</span></span>

* <span data-ttu-id="82786-2303">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="82786-2303">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="82786-2304">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="82786-2304">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="82786-2305">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="82786-2305">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="82786-2306">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="82786-2306">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="82786-2307">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-2307">Network</span></span>

* <span data-ttu-id="82786-2308">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="82786-2308">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="82786-2309">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="82786-2309">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="82786-2310">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="82786-2310">Added `asg` application security group commands</span></span>
* <span data-ttu-id="82786-2311">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="82786-2311">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="82786-2312">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-2312">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="82786-2313">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-2313">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="82786-2314">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="82786-2314">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="82786-2315">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-2315">Storage</span></span>

* <span data-ttu-id="82786-2316">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="82786-2316">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="82786-2317">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="82786-2317">Eventgrid</span></span>

* <span data-ttu-id="82786-2318">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="82786-2318">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="82786-2319">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-2319">SQL</span></span>

* <span data-ttu-id="82786-2320">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="82786-2320">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="82786-2321">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="82786-2321">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="82786-2322">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-2322">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="82786-2323">Keyvault</span><span class="sxs-lookup"><span data-stu-id="82786-2323">Keyvault</span></span>

* <span data-ttu-id="82786-2324">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="82786-2324">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="82786-2325">VM</span><span class="sxs-lookup"><span data-stu-id="82786-2325">VM</span></span>

* <span data-ttu-id="82786-2326">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="82786-2326">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="82786-2327">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="82786-2327">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="82786-2328">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="82786-2328">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="82786-2329">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="82786-2329">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="82786-2330">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="82786-2330">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="82786-2331">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="82786-2331">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="82786-2332">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-2332">ACS</span></span>

* <span data-ttu-id="82786-2333">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="82786-2333">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-2334">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-2334">Appservice</span></span>

* <span data-ttu-id="82786-2335">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="82786-2335">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="82786-2336">Backup</span><span class="sxs-lookup"><span data-stu-id="82786-2336">Backup</span></span>

* <span data-ttu-id="82786-2337">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="82786-2337">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="82786-2338">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="82786-2338">September 11, 2017</span></span>

<span data-ttu-id="82786-2339">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="82786-2339">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="82786-2340">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-2340">Core</span></span>

* <span data-ttu-id="82786-2341">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="82786-2341">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="82786-2342">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="82786-2342">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="82786-2343">Acs</span><span class="sxs-lookup"><span data-stu-id="82786-2343">Acs</span></span>

* <span data-ttu-id="82786-2344">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="82786-2344">Added `acs list-locations` command</span></span>
* <span data-ttu-id="82786-2345">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="82786-2345">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-2346">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-2346">Appservice</span></span>

* <span data-ttu-id="82786-2347">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="82786-2347">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="82786-2348">CDN</span><span class="sxs-lookup"><span data-stu-id="82786-2348">CDN</span></span>

* <span data-ttu-id="82786-2349">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="82786-2349">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="82786-2350">Extensão</span><span class="sxs-lookup"><span data-stu-id="82786-2350">Extension</span></span>

* <span data-ttu-id="82786-2351">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="82786-2351">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="82786-2352">Keyvault</span><span class="sxs-lookup"><span data-stu-id="82786-2352">Keyvault</span></span>

* <span data-ttu-id="82786-2353">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="82786-2353">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="82786-2354">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-2354">Network</span></span>

* <span data-ttu-id="82786-2355">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="82786-2355">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="82786-2356">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="82786-2356">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="82786-2357">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="82786-2357">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="82786-2358">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="82786-2358">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="82786-2359">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="82786-2359">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="82786-2360">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-2360">Resource</span></span>

* <span data-ttu-id="82786-2361">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="82786-2361">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="82786-2362">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="82786-2362">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="82786-2363">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="82786-2363">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="82786-2364">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="82786-2364">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="82786-2365">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-2365">SQL</span></span>

* <span data-ttu-id="82786-2366">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="82786-2366">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="82786-2367">VM</span><span class="sxs-lookup"><span data-stu-id="82786-2367">VM</span></span>

* <span data-ttu-id="82786-2368">Corrigido: não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="82786-2368">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="82786-2369">Corrigido: usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="82786-2369">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="82786-2370">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="82786-2370">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="82786-2371">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="82786-2371">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="82786-2372">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="82786-2372">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="82786-2373">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="82786-2373">August 31, 2017</span></span>

<span data-ttu-id="82786-2374">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="82786-2374">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="82786-2375">Keyvault</span><span class="sxs-lookup"><span data-stu-id="82786-2375">Keyvault</span></span>

* <span data-ttu-id="82786-2376">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="82786-2376">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="82786-2377">Sf</span><span class="sxs-lookup"><span data-stu-id="82786-2377">Sf</span></span>

* <span data-ttu-id="82786-2378">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="82786-2378">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="82786-2379">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-2379">Storage</span></span>

* <span data-ttu-id="82786-2380">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="82786-2380">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="82786-2381">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="82786-2381">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="82786-2382">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="82786-2382">August 28, 2017</span></span>

<span data-ttu-id="82786-2383">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="82786-2383">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="82786-2384">CLI</span><span class="sxs-lookup"><span data-stu-id="82786-2384">CLI</span></span>

* <span data-ttu-id="82786-2385">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="82786-2385">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="82786-2386">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-2386">ACS</span></span>

* <span data-ttu-id="82786-2387">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="82786-2387">Corrected preview regions</span></span>
* <span data-ttu-id="82786-2388">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="82786-2388">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="82786-2389">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="82786-2389">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-2390">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-2390">Appservice</span></span>

* <span data-ttu-id="82786-2391">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="82786-2391">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="82786-2392">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="82786-2392">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="82786-2393">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="82786-2393">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="82786-2394">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="82786-2394">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="82786-2395">Corrigido: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="82786-2395">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="82786-2396">IoT</span><span class="sxs-lookup"><span data-stu-id="82786-2396">IoT</span></span>

* <span data-ttu-id="82786-2397">Corrigido #3934: a criação de uma política não limpa mais as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="82786-2397">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="82786-2398">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-2398">Network</span></span>

* <span data-ttu-id="82786-2399">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="82786-2399">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="82786-2400">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-2400">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="82786-2401">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82786-2401">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="82786-2402">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="82786-2402">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="82786-2403">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="82786-2403">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="82786-2404">Perfil</span><span class="sxs-lookup"><span data-stu-id="82786-2404">Profile</span></span>

* <span data-ttu-id="82786-2405">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="82786-2405">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="82786-2406">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="82786-2406">Service Fabric</span></span>

* <span data-ttu-id="82786-2407">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="82786-2407">Preview release</span></span>
* <span data-ttu-id="82786-2408">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="82786-2408">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="82786-2409">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="82786-2409">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="82786-2410">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="82786-2410">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="82786-2411">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-2411">Storage</span></span>

* <span data-ttu-id="82786-2412">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="82786-2412">Enabled setting blob tier</span></span>
* <span data-ttu-id="82786-2413">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="82786-2413">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="82786-2414">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="82786-2414">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="82786-2415">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="82786-2415">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="82786-2416">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="82786-2416">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="82786-2417">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="82786-2417">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="82786-2418">VM</span><span class="sxs-lookup"><span data-stu-id="82786-2418">VM</span></span>

* <span data-ttu-id="82786-2419">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="82786-2419">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="82786-2420">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="82786-2420">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="82786-2421">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="82786-2421">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="82786-2422">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="82786-2422">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="82786-2423">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="82786-2423">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="82786-2424">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="82786-2424">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="82786-2425">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="82786-2425">August 15, 2017</span></span>

<span data-ttu-id="82786-2426">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="82786-2426">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="82786-2427">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-2427">ACS</span></span>

* <span data-ttu-id="82786-2428">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="82786-2428">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-2429">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-2429">Appservice</span></span>

* <span data-ttu-id="82786-2430">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="82786-2430">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="82786-2431">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="82786-2431">Event Grid</span></span>

* <span data-ttu-id="82786-2432">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="82786-2432">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="82786-2433">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="82786-2433">August 11, 2017</span></span>

<span data-ttu-id="82786-2434">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="82786-2434">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="82786-2435">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-2435">ACS</span></span>

* <span data-ttu-id="82786-2436">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="82786-2436">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="82786-2437">Lote</span><span class="sxs-lookup"><span data-stu-id="82786-2437">Batch</span></span>

* <span data-ttu-id="82786-2438">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="82786-2438">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="82786-2439">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="82786-2439">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="82786-2440">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="82786-2440">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="82786-2441">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://”</span><span class="sxs-lookup"><span data-stu-id="82786-2441">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="82786-2442">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="82786-2442">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="82786-2443">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="82786-2443">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="82786-2444">Componente</span><span class="sxs-lookup"><span data-stu-id="82786-2444">Component</span></span>

* <span data-ttu-id="82786-2445">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="82786-2445">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="82786-2446">Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-2446">Container</span></span>

* <span data-ttu-id="82786-2447">`create`: corrigido o problema em que o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="82786-2447">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="82786-2448">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="82786-2448">Data Lake Store</span></span>

* <span data-ttu-id="82786-2449">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="82786-2449">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="82786-2450">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="82786-2450">Event Grid</span></span>

* <span data-ttu-id="82786-2451">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="82786-2451">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="82786-2452">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-2452">Network</span></span>

* <span data-ttu-id="82786-2453">`lb`: corrigido o problema em que os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="82786-2453">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="82786-2454">`application-gateway {subresource} delete`: corrigido o problema em que `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="82786-2454">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="82786-2455">`application-gateway http-settings update`: corrigido o problema em que `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="82786-2455">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="82786-2456">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="82786-2456">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="82786-2457">Perfil</span><span class="sxs-lookup"><span data-stu-id="82786-2457">Profile</span></span>

* <span data-ttu-id="82786-2458">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="82786-2458">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="82786-2459">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-2459">Storage</span></span>

* <span data-ttu-id="82786-2460">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="82786-2460">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="82786-2461">VM</span><span class="sxs-lookup"><span data-stu-id="82786-2461">VM</span></span>

* <span data-ttu-id="82786-2462">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="82786-2462">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="82786-2463">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="82786-2463">Exposed `list-skus` command</span></span>
* <span data-ttu-id="82786-2464">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="82786-2464">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="82786-2465">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="82786-2465">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="82786-2466">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="82786-2466">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="82786-2467">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="82786-2467">July 28, 2017</span></span>

<span data-ttu-id="82786-2468">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="82786-2468">Version 2.0.12</span></span>

* <span data-ttu-id="82786-2469">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-2469">Added container commands</span></span>
* <span data-ttu-id="82786-2470">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="82786-2470">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="82786-2471">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-2471">Core</span></span>

* <span data-ttu-id="82786-2472">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="82786-2472">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="82786-2473">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="82786-2473">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="82786-2474">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="82786-2474">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="82786-2475">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="82786-2475">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="82786-2476">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="82786-2476">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="82786-2477">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="82786-2477">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="82786-2478">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="82786-2478">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="82786-2479">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="82786-2479">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="82786-2480">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="82786-2480">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="82786-2481">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="82786-2481">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="82786-2482">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="82786-2482">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="82786-2483">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="82786-2483">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="82786-2484">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="82786-2484">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="82786-2485">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="82786-2485">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="82786-2486">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="82786-2486">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="82786-2487">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="82786-2487">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="82786-2488">ACR</span><span class="sxs-lookup"><span data-stu-id="82786-2488">ACR</span></span>

* <span data-ttu-id="82786-2489">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="82786-2489">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="82786-2490">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="82786-2490">Support SKU update for managed registries</span></span>
* <span data-ttu-id="82786-2491">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="82786-2491">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="82786-2492">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="82786-2492">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="82786-2493">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="82786-2493">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="82786-2494">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="82786-2494">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="82786-2495">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-2495">ACS</span></span>

* <span data-ttu-id="82786-2496">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="82786-2496">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-2497">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-2497">Appservice</span></span>

* <span data-ttu-id="82786-2498">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="82786-2498">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="82786-2499">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="82786-2499">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="82786-2500">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="82786-2500">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="82786-2501">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="82786-2501">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="82786-2502">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="82786-2502">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="82786-2503">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="82786-2503">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="82786-2504">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="82786-2504">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="82786-2505">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="82786-2505">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="82786-2506">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="82786-2506">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="82786-2507">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="82786-2507">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="82786-2508">Lote</span><span class="sxs-lookup"><span data-stu-id="82786-2508">Batch</span></span>

* <span data-ttu-id="82786-2509">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="82786-2509">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="82786-2510">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="82786-2510">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="82786-2511">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="82786-2511">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="82786-2512">CDN</span><span class="sxs-lookup"><span data-stu-id="82786-2512">CDN</span></span>

* <span data-ttu-id="82786-2513">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="82786-2513">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="82786-2514">Nuvem</span><span class="sxs-lookup"><span data-stu-id="82786-2514">Cloud</span></span>

* <span data-ttu-id="82786-2515">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="82786-2515">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="82786-2516">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="82786-2516">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="82786-2517">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="82786-2517">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="82786-2518">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="82786-2518">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="82786-2519">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="82786-2519">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82786-2520">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="82786-2520">CosmosDB</span></span>

* <span data-ttu-id="82786-2521">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="82786-2521">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="82786-2522">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="82786-2522">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="82786-2523">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="82786-2523">Data Lake Analytics</span></span>

* <span data-ttu-id="82786-2524">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="82786-2524">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="82786-2525">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="82786-2525">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="82786-2526">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="82786-2526">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="82786-2527">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="82786-2527">Data Lake Store</span></span>

* <span data-ttu-id="82786-2528">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="82786-2528">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="82786-2529">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="82786-2529">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="82786-2530">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="82786-2530">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="82786-2531">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="82786-2531">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="82786-2532">Interativo</span><span class="sxs-lookup"><span data-stu-id="82786-2532">Interactive</span></span>

* <span data-ttu-id="82786-2533">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="82786-2533">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="82786-2534">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="82786-2534">Increased test coverage</span></span>
* <span data-ttu-id="82786-2535">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="82786-2535">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="82786-2536">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="82786-2536">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="82786-2537">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="82786-2537">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="82786-2538">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="82786-2538">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="82786-2539">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="82786-2539">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="82786-2540">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="82786-2540">Added `--progress` flag</span></span>
* <span data-ttu-id="82786-2541">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="82786-2541">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="82786-2542">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="82786-2542">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="82786-2543">IoT</span><span class="sxs-lookup"><span data-stu-id="82786-2543">IoT</span></span>

* <span data-ttu-id="82786-2544">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="82786-2544">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="82786-2545">(#3934)</span><span class="sxs-lookup"><span data-stu-id="82786-2545">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="82786-2546">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="82786-2546">Key vault</span></span>

* <span data-ttu-id="82786-2547">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="82786-2547">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="82786-2548">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="82786-2548">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="82786-2549">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="82786-2549">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="82786-2550">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="82786-2550">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="82786-2551">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="82786-2551">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="82786-2552">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="82786-2552">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="82786-2553">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="82786-2553">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="82786-2554">(#3307)</span><span class="sxs-lookup"><span data-stu-id="82786-2554">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="82786-2555">Laboratório</span><span class="sxs-lookup"><span data-stu-id="82786-2555">Lab</span></span>

* <span data-ttu-id="82786-2556">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="82786-2556">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="82786-2557">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="82786-2557">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="82786-2558">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="82786-2558">Monitor</span></span>

* <span data-ttu-id="82786-2559">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="82786-2559">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="82786-2560">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="82786-2560">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="82786-2561">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="82786-2561">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="82786-2562">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="82786-2562">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="82786-2563">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="82786-2563">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="82786-2564">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="82786-2564">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="82786-2565">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="82786-2565">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="82786-2566">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="82786-2566">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="82786-2567">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="82786-2567">`location` no longer required</span></span>
  * <span data-ttu-id="82786-2568">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="82786-2568">Add name and ID support for target</span></span>
  * <span data-ttu-id="82786-2569">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="82786-2569">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="82786-2570">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="82786-2570">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="82786-2571">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="82786-2571">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="82786-2572">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="82786-2572">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="82786-2573">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="82786-2573">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="82786-2574">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="82786-2574">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="82786-2575">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-2575">Network</span></span>

* <span data-ttu-id="82786-2576">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="82786-2576">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="82786-2577">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="82786-2577">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="82786-2578">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="82786-2578">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="82786-2579">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="82786-2579">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="82786-2580">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="82786-2580">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="82786-2581">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="82786-2581">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="82786-2582">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="82786-2582">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="82786-2583">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="82786-2583">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="82786-2584">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="82786-2584">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="82786-2585">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="82786-2585">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="82786-2586">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="82786-2586">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="82786-2587">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="82786-2587">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="82786-2588">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="82786-2588">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="82786-2589">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="82786-2589">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="82786-2590">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="82786-2590">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="82786-2591">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="82786-2591">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="82786-2592">Adicionado o suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para --dns-servers</span><span class="sxs-lookup"><span data-stu-id="82786-2592">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="82786-2593">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="82786-2593">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="82786-2594">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="82786-2594">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="82786-2595">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="82786-2595">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="82786-2596">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="82786-2596">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="82786-2597">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="82786-2597">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="82786-2598">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="82786-2598">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="82786-2599">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="82786-2599">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="82786-2600">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="82786-2600">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="82786-2601">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="82786-2601">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="82786-2602">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="82786-2602">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="82786-2603">Perfil</span><span class="sxs-lookup"><span data-stu-id="82786-2603">Profile</span></span>

* <span data-ttu-id="82786-2604">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="82786-2604">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="82786-2605">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="82786-2605">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="82786-2606">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="82786-2606">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="82786-2607">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="82786-2607">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="82786-2608">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="82786-2608">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="82786-2609">RDBMS</span><span class="sxs-lookup"><span data-stu-id="82786-2609">RDBMS</span></span>

* <span data-ttu-id="82786-2610">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="82786-2610">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="82786-2611">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="82786-2611">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="82786-2612">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="82786-2612">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="82786-2613">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="82786-2613">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="82786-2614">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-2614">Resource</span></span>

* <span data-ttu-id="82786-2615">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="82786-2615">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="82786-2616">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="82786-2616">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="82786-2617">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="82786-2617">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="82786-2618">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="82786-2618">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="82786-2619">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="82786-2619">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="82786-2620">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="82786-2620">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="82786-2621">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="82786-2621">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="82786-2622">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="82786-2622">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="82786-2623">Função</span><span class="sxs-lookup"><span data-stu-id="82786-2623">Role</span></span>

* <span data-ttu-id="82786-2624">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="82786-2624">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="82786-2625">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="82786-2625">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="82786-2626">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="82786-2626">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="82786-2627">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="82786-2627">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="82786-2628">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="82786-2628">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="82786-2629">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="82786-2629">Service Fabric</span></span>
* <span data-ttu-id="82786-2630">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="82786-2630">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="82786-2631">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="82786-2631">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="82786-2632">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="82786-2632">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="82786-2633">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-2633">SQL</span></span>

* <span data-ttu-id="82786-2634">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="82786-2634">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="82786-2635">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="82786-2635">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="82786-2636">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="82786-2636">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="82786-2637">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-2637">Storage</span></span>

* <span data-ttu-id="82786-2638">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="82786-2638">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="82786-2639">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="82786-2639">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="82786-2640">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="82786-2640">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="82786-2641">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="82786-2641">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="82786-2642">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="82786-2642">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="82786-2643">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="82786-2643">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="82786-2644">VM</span><span class="sxs-lookup"><span data-stu-id="82786-2644">VM</span></span>

* <span data-ttu-id="82786-2645">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="82786-2645">Support configuring nsg</span></span>
* <span data-ttu-id="82786-2646">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="82786-2646">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="82786-2647">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="82786-2647">Support managed service identities</span></span>
* <span data-ttu-id="82786-2648">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="82786-2648">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="82786-2649">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="82786-2649">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="82786-2650">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="82786-2650">May 10, 2017</span></span>

<span data-ttu-id="82786-2651">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="82786-2651">Version 2.0.6</span></span>

* <span data-ttu-id="82786-2652">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="82786-2652">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="82786-2653">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="82786-2653">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="82786-2654">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="82786-2654">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="82786-2655">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="82786-2655">Include Cognitive Services module</span></span>
* <span data-ttu-id="82786-2656">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="82786-2656">Include Service Fabric module</span></span>
* <span data-ttu-id="82786-2657">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="82786-2657">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="82786-2658">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="82786-2658">Add support for CDN commands</span></span>
* <span data-ttu-id="82786-2659">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="82786-2659">Remove Container module</span></span>
* <span data-ttu-id="82786-2660">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="82786-2660">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="82786-2661">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="82786-2661">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="82786-2662">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-2662">Core</span></span>

* <span data-ttu-id="82786-2663">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="82786-2663">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="82786-2664">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="82786-2664">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="82786-2665">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="82786-2665">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="82786-2666">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="82786-2666">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="82786-2667">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="82786-2667">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="82786-2668">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="82786-2668">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="82786-2669">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="82786-2669">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="82786-2670">núcleo: permitir que o caminho do arquivo accessTokens.json seja configurável por meio de uma variável de ambiente ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="82786-2670">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="82786-2671">núcleo: permitir que padrões configurados sejam aplicados em argumentos opcionais ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="82786-2671">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="82786-2672">núcleo: desempenho aprimorado</span><span class="sxs-lookup"><span data-stu-id="82786-2672">core: Improved performance</span></span>
* <span data-ttu-id="82786-2673">núcleo: certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="82786-2673">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="82786-2674">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="82786-2674">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="82786-2675">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-2675">ACS</span></span>

* <span data-ttu-id="82786-2676">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82786-2676">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="82786-2677">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="82786-2677">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="82786-2678">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="82786-2678">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="82786-2679">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="82786-2679">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-2680">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-2680">AppService</span></span>

* <span data-ttu-id="82786-2681">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="82786-2681">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="82786-2682">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="82786-2682">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="82786-2683">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="82786-2683">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="82786-2684">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="82786-2684">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="82786-2685">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="82786-2685">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="82786-2686">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="82786-2686">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="82786-2687">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="82786-2687">support slot swap with preview</span></span>
* <span data-ttu-id="82786-2688">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="82786-2688">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="82786-2689">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="82786-2689">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82786-2690">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="82786-2690">CosmosDB</span></span>

* <span data-ttu-id="82786-2691">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="82786-2691">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="82786-2692">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="82786-2692">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="82786-2693">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="82786-2693">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="82786-2694">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="82786-2694">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="82786-2695">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="82786-2695">Data Lake Analytics</span></span>

* <span data-ttu-id="82786-2696">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="82786-2696">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="82786-2697">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="82786-2697">Add support for new catalog item type: package.</span></span> <span data-ttu-id="82786-2698">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="82786-2698">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="82786-2699">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="82786-2699">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="82786-2700">Tabela</span><span class="sxs-lookup"><span data-stu-id="82786-2700">Table</span></span>
  * <span data-ttu-id="82786-2701">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="82786-2701">Table valued function</span></span>
  * <span data-ttu-id="82786-2702">Visualizar</span><span class="sxs-lookup"><span data-stu-id="82786-2702">View</span></span>
  * <span data-ttu-id="82786-2703">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="82786-2703">Table Statistics.</span></span> <span data-ttu-id="82786-2704">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="82786-2704">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="82786-2705">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="82786-2705">Data Lake Store</span></span>

* <span data-ttu-id="82786-2706">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="82786-2706">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="82786-2707">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="82786-2707">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="82786-2708">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="82786-2708">missed help for access show.</span></span> <span data-ttu-id="82786-2709">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="82786-2709">adding it.</span></span> <span data-ttu-id="82786-2710">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="82786-2710">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="82786-2711">Localizar</span><span class="sxs-lookup"><span data-stu-id="82786-2711">Find</span></span>

* <span data-ttu-id="82786-2712">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="82786-2712">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="82786-2713">KeyVault</span><span class="sxs-lookup"><span data-stu-id="82786-2713">KeyVault</span></span>

* <span data-ttu-id="82786-2714">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="82786-2714">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="82786-2715">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois estes parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="82786-2715">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="82786-2716">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="82786-2716">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="82786-2717">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="82786-2717">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="82786-2718">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="82786-2718">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="82786-2719">Laboratório</span><span class="sxs-lookup"><span data-stu-id="82786-2719">Lab</span></span>

* <span data-ttu-id="82786-2720">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="82786-2720">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="82786-2721">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="82786-2721">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="82786-2722">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="82786-2722">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="82786-2723">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="82786-2723">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="82786-2724">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="82786-2724">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="82786-2725">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="82786-2725">Monitor</span></span>

* <span data-ttu-id="82786-2726">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="82786-2726">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="82786-2727">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="82786-2727">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="82786-2728">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-2728">Network</span></span>

* <span data-ttu-id="82786-2729">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="82786-2729">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="82786-2730">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="82786-2730">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="82786-2731">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82786-2731">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="82786-2732">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82786-2732">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="82786-2733">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="82786-2733">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="82786-2734">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="82786-2734">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="82786-2735">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="82786-2735">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="82786-2736">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="82786-2736">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="82786-2737">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="82786-2737">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="82786-2738">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="82786-2738">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="82786-2739">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="82786-2739">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="82786-2740">BC: corrigido um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="82786-2740">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="82786-2741">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="82786-2741">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="82786-2742">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="82786-2742">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="82786-2743">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="82786-2743">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="82786-2744">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="82786-2744">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="82786-2745">Perfil</span><span class="sxs-lookup"><span data-stu-id="82786-2745">Profile</span></span>

* <span data-ttu-id="82786-2746">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="82786-2746">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="82786-2747">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="82786-2747">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="82786-2748">Redis</span><span class="sxs-lookup"><span data-stu-id="82786-2748">Redis</span></span>

* <span data-ttu-id="82786-2749">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="82786-2749">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="82786-2750">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="82786-2750">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="82786-2751">Recurso</span><span class="sxs-lookup"><span data-stu-id="82786-2751">Resource</span></span>

* <span data-ttu-id="82786-2752">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="82786-2752">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="82786-2753">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="82786-2753">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="82786-2754">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="82786-2754">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="82786-2755">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="82786-2755">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="82786-2756">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="82786-2756">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="82786-2757">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="82786-2757">Add docs for az lock update.</span></span> <span data-ttu-id="82786-2758">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="82786-2758">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="82786-2759">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="82786-2759">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="82786-2760">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="82786-2760">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="82786-2761">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="82786-2761">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="82786-2762">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="82786-2762">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="82786-2763">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="82786-2763">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="82786-2764">Função</span><span class="sxs-lookup"><span data-stu-id="82786-2764">Role</span></span>

* <span data-ttu-id="82786-2765">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="82786-2765">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="82786-2766">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="82786-2766">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="82786-2767">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="82786-2767">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="82786-2768">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="82786-2768">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="82786-2769">SQL</span><span class="sxs-lookup"><span data-stu-id="82786-2769">SQL</span></span>

* <span data-ttu-id="82786-2770">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="82786-2770">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="82786-2771">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="82786-2771">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="82786-2772">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-2772">Storage</span></span>

* <span data-ttu-id="82786-2773">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="82786-2773">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="82786-2774">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="82786-2774">Add support for incremental blob copy</span></span>
* <span data-ttu-id="82786-2775">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="82786-2775">Add support for large block blob upload</span></span>
* <span data-ttu-id="82786-2776">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="82786-2776">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="82786-2777">VM</span><span class="sxs-lookup"><span data-stu-id="82786-2777">VM</span></span>

* <span data-ttu-id="82786-2778">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="82786-2778">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="82786-2779">observação: em comandos da VM em nuvens soberanas, evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="82786-2779">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="82786-2780">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="82786-2780">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="82786-2781">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="82786-2781">az vm/vmss disk</span></span>
  3. <span data-ttu-id="82786-2782">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="82786-2782">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="82786-2783">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="82786-2783">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="82786-2784">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="82786-2784">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="82786-2785">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="82786-2785">April 3, 2017</span></span>

<span data-ttu-id="82786-2786">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="82786-2786">Version 2.0.2</span></span>

<span data-ttu-id="82786-2787">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="82786-2787">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="82786-2788">Núcleo</span><span class="sxs-lookup"><span data-stu-id="82786-2788">Core</span></span>

* <span data-ttu-id="82786-2789">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="82786-2789">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="82786-2790">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="82786-2790">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="82786-2791">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="82786-2791">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="82786-2792">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="82786-2792">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="82786-2793">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="82786-2793">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="82786-2794">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="82786-2794">Add prompting for missing template parameters.</span></span> <span data-ttu-id="82786-2795">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="82786-2795">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="82786-2796">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="82786-2796">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="82786-2797">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="82786-2797">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="82786-2798">ACS</span><span class="sxs-lookup"><span data-stu-id="82786-2798">ACS</span></span>

* <span data-ttu-id="82786-2799">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="82786-2799">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="82786-2800">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="82786-2800">Add support for ssh key password prompting.</span></span> <span data-ttu-id="82786-2801">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="82786-2801">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="82786-2802">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="82786-2802">Add support for windows clusters.</span></span> <span data-ttu-id="82786-2803">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="82786-2803">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="82786-2804">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="82786-2804">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="82786-2805">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="82786-2805">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="82786-2806">AppService</span><span class="sxs-lookup"><span data-stu-id="82786-2806">AppService</span></span>

* <span data-ttu-id="82786-2807">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="82786-2807">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="82786-2808">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="82786-2808">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="82786-2809">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="82786-2809">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="82786-2810">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="82786-2810">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="82786-2811">DataLake</span><span class="sxs-lookup"><span data-stu-id="82786-2811">DataLake</span></span>

* <span data-ttu-id="82786-2812">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="82786-2812">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="82786-2813">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="82786-2813">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="82786-2814">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="82786-2814">DocuemntDB</span></span>

* <span data-ttu-id="82786-2815">DocumentDB: adicionado suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="82786-2815">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="82786-2816">VM</span><span class="sxs-lookup"><span data-stu-id="82786-2816">VM</span></span>

* <span data-ttu-id="82786-2817">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="82786-2817">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="82786-2818">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="82786-2818">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="82786-2819">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="82786-2819">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="82786-2820">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="82786-2820">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="82786-2821">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="82786-2821">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="82786-2822">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="82786-2822">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="82786-2823">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="82786-2823">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="82786-2824">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="82786-2824">February 27, 2017</span></span>

<span data-ttu-id="82786-2825">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="82786-2825">Version 2.0.0</span></span>

<span data-ttu-id="82786-2826">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="82786-2826">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="82786-2827">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="82786-2827">Container Service (acs)</span></span>
- <span data-ttu-id="82786-2828">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="82786-2828">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="82786-2829">Rede</span><span class="sxs-lookup"><span data-stu-id="82786-2829">Networking</span></span>
- <span data-ttu-id="82786-2830">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="82786-2830">Storage</span></span>

<span data-ttu-id="82786-2831">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="82786-2831">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="82786-2832">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="82786-2832">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="82786-2833">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="82786-2833">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="82786-2834">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="82786-2834">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="82786-2835">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="82786-2835">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="82786-2836">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="82786-2836">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="82786-2837">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="82786-2837">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="82786-2838">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="82786-2838">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="82786-2839">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="82786-2839">Provide feedback from the command line with the `az feedback` command</span></span>

