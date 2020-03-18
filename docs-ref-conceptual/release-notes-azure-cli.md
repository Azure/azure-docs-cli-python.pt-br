---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 03/10/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: ff3a1da2343b96bfd78b20742c2c15707932f3d7
ms.sourcegitcommit: 21bc2a7125b6c38bf1c4def0a0e66e6673de4805
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2020
ms.locfileid: "79037941"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="7d05a-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="7d05a-103">Azure CLI release notes</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="7d05a-104">10 de março de 2020</span><span class="sxs-lookup"><span data-stu-id="7d05a-104">March 10, 2020</span></span>

<span data-ttu-id="7d05a-105">Versão 2.2.0</span><span class="sxs-lookup"><span data-stu-id="7d05a-105">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-106">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-106">ACR</span></span>

* <span data-ttu-id="7d05a-107">Correção: `az acr login` gerava erro incorretamente</span><span class="sxs-lookup"><span data-stu-id="7d05a-107">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="7d05a-108">Adicionou o novo comando `az acr helm install-cli`</span><span class="sxs-lookup"><span data-stu-id="7d05a-108">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="7d05a-109">Adicionou link privado e suporte do CMK</span><span class="sxs-lookup"><span data-stu-id="7d05a-109">Add private link and CMK support</span></span>
* <span data-ttu-id="7d05a-110">Adicionou o comando 'private-link-resource list'</span><span class="sxs-lookup"><span data-stu-id="7d05a-110">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="7d05a-111">AKS</span><span class="sxs-lookup"><span data-stu-id="7d05a-111">AKS</span></span>

* <span data-ttu-id="7d05a-112">correção da busca do AKS no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="7d05a-112">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="7d05a-113">az aks: correção dos erros de complemento de monitoramento e de agentpool NoneType</span><span class="sxs-lookup"><span data-stu-id="7d05a-113">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="7d05a-114">Adicionou --nodepool-tags ao pool de nós ao criar o cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="7d05a-114">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="7d05a-115">Adicionou --tags ao adicionar ou atualizar um pool de nós para o cluster</span><span class="sxs-lookup"><span data-stu-id="7d05a-115">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="7d05a-116">AKS create: adicionou `--enable-private-cluster`</span><span class="sxs-lookup"><span data-stu-id="7d05a-116">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="7d05a-117">Adicionou --nodepool-labels ao criar o cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="7d05a-117">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="7d05a-118">Adicionou --labels ao adicionar um novo pool de nós ao cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="7d05a-118">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="7d05a-119">Adicionou / ausente na URL do painel</span><span class="sxs-lookup"><span data-stu-id="7d05a-119">add missing / in the dashboard url</span></span>
* <span data-ttu-id="7d05a-120">Suporte para criar clusters do AKS habilitando identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="7d05a-120">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="7d05a-121">az aks: validou o plug-in de rede como "Azure" ou "Kubenet"</span><span class="sxs-lookup"><span data-stu-id="7d05a-121">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="7d05a-122">az aks: adicionou suporte da chave da sessão do AAD</span><span class="sxs-lookup"><span data-stu-id="7d05a-122">az aks: Add aad session key support</span></span>
* <span data-ttu-id="7d05a-123">[ALTERAÇÃO SIGNIFICATIVA] AZ AKS: suporte para alterações de MSI para GF e BF para omsagent (Monitoramento de contêiner) (#1)</span><span class="sxs-lookup"><span data-stu-id="7d05a-123">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="7d05a-124">az aks use-dev-spaces: adicionou a opção de tipo de ponto de extremidade ao comando use-dev-spaces para personalizar o ponto de extremidade criado em um controlador Azure Dev Spaces</span><span class="sxs-lookup"><span data-stu-id="7d05a-124">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="7d05a-125">AppConfig</span><span class="sxs-lookup"><span data-stu-id="7d05a-125">AppConfig</span></span>

* <span data-ttu-id="7d05a-126">Desbloqueou usando "KV set" para adicionar o recurso e a referência do keyvault...</span><span class="sxs-lookup"><span data-stu-id="7d05a-126">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-127">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-127">AppService</span></span>

* <span data-ttu-id="7d05a-128">az webapp create: correção do problema ao executar o comando com --runtime</span><span class="sxs-lookup"><span data-stu-id="7d05a-128">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="7d05a-129">az functionapp deployment source config-zip: adicionou uma mensagem de erro se o grupo de recursos ou o nome da função forem inválidos/não existirem</span><span class="sxs-lookup"><span data-stu-id="7d05a-129">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="7d05a-130">functionapp create: correção da mensagem de aviso que aparece com `functionapp create` hoje, que cita um sinalizador de `--functions_version`, mas usa erroneamente `_` em vez de `-` no nome do sinalizador</span><span class="sxs-lookup"><span data-stu-id="7d05a-130">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="7d05a-131">az functionapp create: atualizou o modo como linuxFxVersion e o nome da imagem de contêiner eram definidos para aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="7d05a-131">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="7d05a-132">az functionapp deployment source config-zip: correção de um problema causado pelas configurações do aplicativo que alterava a condição de corrida durante a implantação do zip, provocando erros 5xx durante a implantação</span><span class="sxs-lookup"><span data-stu-id="7d05a-132">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="7d05a-133">Correção #5720946: AZ WebApp backup falha ao definir o nome</span><span class="sxs-lookup"><span data-stu-id="7d05a-133">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="7d05a-134">ARM</span><span class="sxs-lookup"><span data-stu-id="7d05a-134">ARM</span></span>

* <span data-ttu-id="7d05a-135">az resource: aprimorou os exemplos do módulo de recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-135">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="7d05a-136">az policy assignment list: suporte à listagem de atribuições de política no escopo do Grupo de Gerenciamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-136">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="7d05a-137">Adicionou `az deployment group` e `az deployment operation group` para a implantação de modelos nos grupos de recursos.</span><span class="sxs-lookup"><span data-stu-id="7d05a-137">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="7d05a-138">Esta é uma duplicata de `az group deployment` e `az group deployment operation`</span><span class="sxs-lookup"><span data-stu-id="7d05a-138">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="7d05a-139">Adicionou `az deployment sub` e `az deployment operation sub` para a implantação de modelos no escopo da assinatura.</span><span class="sxs-lookup"><span data-stu-id="7d05a-139">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="7d05a-140">Esta é uma duplicata de `az deployment` e `az deployment operation`</span><span class="sxs-lookup"><span data-stu-id="7d05a-140">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="7d05a-141">Adicionou `az deployment mg` e `az deployment operation mg` para implantação de modelos nos grupos de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="7d05a-141">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="7d05a-142">Adicionou `az deployment tenant` e `az deployment operation tenant` para implantação de modelos no escopo do locatário.</span><span class="sxs-lookup"><span data-stu-id="7d05a-142">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="7d05a-143">az policy assignment create: adicionou descrição ao parâmetro `--location`</span><span class="sxs-lookup"><span data-stu-id="7d05a-143">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="7d05a-144">az group deployment create: adicionou o parâmetro `--aux-tenants` para dar suporte a locatários cruzados</span><span class="sxs-lookup"><span data-stu-id="7d05a-144">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="7d05a-145">CDN</span><span class="sxs-lookup"><span data-stu-id="7d05a-145">CDN</span></span>

* <span data-ttu-id="7d05a-146">Adicionou comandos do WAF da CDN</span><span class="sxs-lookup"><span data-stu-id="7d05a-146">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="7d05a-147">Computação</span><span class="sxs-lookup"><span data-stu-id="7d05a-147">Compute</span></span>

* <span data-ttu-id="7d05a-148">az sig image-version: adicionar --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="7d05a-148">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="7d05a-149">AZ PPG show: adicionou --outlocation-status para habilitar a busca do status de colocalização de todos os recursos no grupo de posicionamento por proximidade</span><span class="sxs-lookup"><span data-stu-id="7d05a-149">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="7d05a-150">az vmss create/update: suporte a reparos automáticos</span><span class="sxs-lookup"><span data-stu-id="7d05a-150">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="7d05a-151">[ALTERAÇÃO SIGNIFICATIVA] modelo de imagem AZ: renomear modelo para builder</span><span class="sxs-lookup"><span data-stu-id="7d05a-151">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="7d05a-152">AZ Image Builder Create: adicionou --Image-template</span><span class="sxs-lookup"><span data-stu-id="7d05a-152">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="7d05a-153">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7d05a-153">Cosmos DB</span></span>

* <span data-ttu-id="7d05a-154">Adicionou procedimento armazenado do SQL, UDF e disparar cmdlets</span><span class="sxs-lookup"><span data-stu-id="7d05a-154">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="7d05a-155">az cosmosdb create: adicionou --key-uri para dar suporte à adição de informações de criptografia do cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="7d05a-155">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="7d05a-156">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7d05a-156">KeyVault</span></span>

* <span data-ttu-id="7d05a-157">keyvault create: habilitou a exclusão reversível por padrão</span><span class="sxs-lookup"><span data-stu-id="7d05a-157">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="7d05a-158">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-158">Monitor</span></span>

* <span data-ttu-id="7d05a-159">az monitor metrics alert create: suporte a `~` em `--condition`</span><span class="sxs-lookup"><span data-stu-id="7d05a-159">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-160">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-160">Network</span></span>

* <span data-ttu-id="7d05a-161">az network application-gateway rewrite-rule create: suporte à configuração de URL</span><span class="sxs-lookup"><span data-stu-id="7d05a-161">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="7d05a-162">az network dns zone import: --zone-name não diferenciará maiúsculas de minúsculas no futuro</span><span class="sxs-lookup"><span data-stu-id="7d05a-162">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="7d05a-163">az network private-endpoint/private-link-service: removeu rótulo de visualização</span><span class="sxs-lookup"><span data-stu-id="7d05a-163">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="7d05a-164">az network bastion: suporte a bastions</span><span class="sxs-lookup"><span data-stu-id="7d05a-164">az network bastion: support bastion</span></span>
* <span data-ttu-id="7d05a-165">az network vnet list-available-ips: dar suporte à lista de IPs disponíveis em uma vnet</span><span class="sxs-lookup"><span data-stu-id="7d05a-165">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="7d05a-166">az network watcher flow-log create/list/delete/update: adicionou novos comandos para gerenciar o log de fluxo do Inspetor e expor o --local para identificá-lo explicitamente</span><span class="sxs-lookup"><span data-stu-id="7d05a-166">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="7d05a-167">az network watcher flow-log configure: preterido</span><span class="sxs-lookup"><span data-stu-id="7d05a-167">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="7d05a-168">az network watcher flow-log show: dá suporte a --location e --name para obter o resultado formatado por ARM, saída formatada antiga preterida</span><span class="sxs-lookup"><span data-stu-id="7d05a-168">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="7d05a-169">Política</span><span class="sxs-lookup"><span data-stu-id="7d05a-169">Policy</span></span>

* <span data-ttu-id="7d05a-170">az policy assignment create: correção do bug que gerou automaticamente o nome da atribuição de política, que excede o limite</span><span class="sxs-lookup"><span data-stu-id="7d05a-170">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="7d05a-171">RBAC</span><span class="sxs-lookup"><span data-stu-id="7d05a-171">RBAC</span></span>

* <span data-ttu-id="7d05a-172">az ad group show: correção do valor --group, que é tratado como um problema de regex</span><span class="sxs-lookup"><span data-stu-id="7d05a-172">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="7d05a-173">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-173">RDBMS</span></span>

* <span data-ttu-id="7d05a-174">Trocou a versão do zure-mgmt-rdbms SDK para 2.0.0</span><span class="sxs-lookup"><span data-stu-id="7d05a-174">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="7d05a-175">az postgres private-endpoint-connection: gerenciou conexões de ponto de extremidade privado do Postgres</span><span class="sxs-lookup"><span data-stu-id="7d05a-175">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="7d05a-176">az postgres private-link-resource: gerenciou recursos de link privado do Postgres</span><span class="sxs-lookup"><span data-stu-id="7d05a-176">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="7d05a-177">az mysql private-endpoint-connection: gerenciar conexões de ponto de extremidade privado do MySQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-177">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="7d05a-178">az mysql private-link-resource: gerenciou recursos de link privado do MySQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-178">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="7d05a-179">az mariadb private-endpoint-connection: gerenciou conexões de ponto de extremidade privado do MariaDB</span><span class="sxs-lookup"><span data-stu-id="7d05a-179">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="7d05a-180">az mariadb private-link-resource: gerenciou recursos de link privado do MariaDB</span><span class="sxs-lookup"><span data-stu-id="7d05a-180">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="7d05a-181">Atualizando testes de ponto de extremidade privado do RDBMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-181">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-182">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-182">SQL</span></span>

* <span data-ttu-id="7d05a-183">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span><span class="sxs-lookup"><span data-stu-id="7d05a-183">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="7d05a-184">(sql server create:) adicionou o sinalizador ' habilitar '/' desabilitar ' opcional public-network-access ao SQL Server create</span><span class="sxs-lookup"><span data-stu-id="7d05a-184">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="7d05a-185">(sql server update:) fez algumas alterações voltadas para o cliente</span><span class="sxs-lookup"><span data-stu-id="7d05a-185">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="7d05a-186">adicionou a propriedade minimal_tls_version para o banco de BD de MI e SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-186">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-187">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-187">Storage</span></span>

* <span data-ttu-id="7d05a-188">az storage blob delete-batch: sinalizador `--dryrun` de comportamento inadequado</span><span class="sxs-lookup"><span data-stu-id="7d05a-188">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="7d05a-189">az storage account network-rule add (correção de bug): a operação de adição deve ser idempotente</span><span class="sxs-lookup"><span data-stu-id="7d05a-189">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="7d05a-190">az storage account create/update: Adicionou suporte de preferência de roteamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-190">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="7d05a-191">Atualizou a versão do azure-mgmt-storage para 8.0.0</span><span class="sxs-lookup"><span data-stu-id="7d05a-191">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="7d05a-192">az storage container immutability create: adicionou o parâmetro --allow-protected-append-write</span><span class="sxs-lookup"><span data-stu-id="7d05a-192">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="7d05a-193">az storage account private-link-resource list: Adicionou suporte para lista de recursos de link privado para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-193">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="7d05a-194">az storage account private-endpoint-connection approve/reject/show/delete: Suporte para gerenciar conexões de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="7d05a-194">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="7d05a-195">az storage account blob-service-properties update: adicionou --enable-restore-policy e --restore-days</span><span class="sxs-lookup"><span data-stu-id="7d05a-195">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="7d05a-196">az storage blob restore: adicionou suporte para restaurar intervalos de blob</span><span class="sxs-lookup"><span data-stu-id="7d05a-196">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="7d05a-197">18 de fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="7d05a-197">February 18, 2020</span></span>

<span data-ttu-id="7d05a-198">Versão 2.1.0</span><span class="sxs-lookup"><span data-stu-id="7d05a-198">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-199">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-199">ACR</span></span>

* <span data-ttu-id="7d05a-200">Adicionar um novo argumento `--expose-token` a `az acr login`</span><span class="sxs-lookup"><span data-stu-id="7d05a-200">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="7d05a-201">Corrigir a saída incorreta de `az acr task identity show -n Name -r Registry -o table`</span><span class="sxs-lookup"><span data-stu-id="7d05a-201">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="7d05a-202">az acr login: Gerar CLIError se erros forem retornados pelo comando docker</span><span class="sxs-lookup"><span data-stu-id="7d05a-202">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-203">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-203">ACS</span></span>

* <span data-ttu-id="7d05a-204">aks create/update: adicionar a validação `--vnet-subnet-id`</span><span class="sxs-lookup"><span data-stu-id="7d05a-204">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="7d05a-205">Aladdin</span><span class="sxs-lookup"><span data-stu-id="7d05a-205">Aladdin</span></span>

* <span data-ttu-id="7d05a-206">Analisar os exemplos gerados no _help.py do comando</span><span class="sxs-lookup"><span data-stu-id="7d05a-206">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="7d05a-207">AMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-207">AMS</span></span>

* <span data-ttu-id="7d05a-208">az ams já está em GA</span><span class="sxs-lookup"><span data-stu-id="7d05a-208">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="7d05a-209">AppConfig</span><span class="sxs-lookup"><span data-stu-id="7d05a-209">AppConfig</span></span>

* <span data-ttu-id="7d05a-210">Revisar a mensagem de ajuda para excluir o filtro de chave/rótulo não compatível</span><span class="sxs-lookup"><span data-stu-id="7d05a-210">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="7d05a-211">Remover a marca de versão prévia da maioria dos comandos que excluem a identidade gerenciada e têm sinalizadores</span><span class="sxs-lookup"><span data-stu-id="7d05a-211">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="7d05a-212">Adicionar a chave gerenciada do cliente ao atualizar os repositórios</span><span class="sxs-lookup"><span data-stu-id="7d05a-212">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-213">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-213">AppService</span></span>

* <span data-ttu-id="7d05a-214">az webapp list-runtimes: Corrigir o bug de list-runtimes</span><span class="sxs-lookup"><span data-stu-id="7d05a-214">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="7d05a-215">Adicionar az webapp|functionapp config ssl create</span><span class="sxs-lookup"><span data-stu-id="7d05a-215">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="7d05a-216">Adicionar compatibilidade com aplicativos de funções v3 e nó 12</span><span class="sxs-lookup"><span data-stu-id="7d05a-216">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="7d05a-217">ARM</span><span class="sxs-lookup"><span data-stu-id="7d05a-217">ARM</span></span>

* <span data-ttu-id="7d05a-218">az policy assignment create: Corrigir a mensagem de erro quando o parâmetro `--policy` for inválido</span><span class="sxs-lookup"><span data-stu-id="7d05a-218">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="7d05a-219">az group deployment create: Corrigir o erro "stat: o caminho é muito longo para o Windows" ao usar o arquivo grande parameters.json</span><span class="sxs-lookup"><span data-stu-id="7d05a-219">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="7d05a-220">Backup</span><span class="sxs-lookup"><span data-stu-id="7d05a-220">Backup</span></span>

* <span data-ttu-id="7d05a-221">Corrigir o fluxo de recuperação de nível de item no OLR</span><span class="sxs-lookup"><span data-stu-id="7d05a-221">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="7d05a-222">Adicionar compatibilidade com restauração como arquivo aos bancos de dados SQL e SAP</span><span class="sxs-lookup"><span data-stu-id="7d05a-222">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="7d05a-223">Computação</span><span class="sxs-lookup"><span data-stu-id="7d05a-223">Compute</span></span>

* <span data-ttu-id="7d05a-224">vm/vmss/availability-set update: adicionar --ppg para permitir a atualização de ProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="7d05a-224">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="7d05a-225">vmss create: adicionar --data-disk-iops e --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="7d05a-225">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="7d05a-226">az vm host: remover a marca de versão prévia de `vm host` e `vm host group`</span><span class="sxs-lookup"><span data-stu-id="7d05a-226">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="7d05a-227">[ALTERAÇÃO SIGNIFICATIVA] Correção nº 10.728: `az vm create`: criar uma sub-rede automaticamente quando a vnet for especificada e não houver uma sub-rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-227">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="7d05a-228">Aumentar a robustez da lista de imagens de VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-228">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="7d05a-229">Eventhub</span><span class="sxs-lookup"><span data-stu-id="7d05a-229">Eventhub</span></span>

* <span data-ttu-id="7d05a-230">Compatibilidade com o Azure Stack para o perfil 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="7d05a-230">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="7d05a-231">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7d05a-231">KeyVault</span></span>

* <span data-ttu-id="7d05a-232">az keyvault key create: adicionar um novo valor `import` ao parâmetro `--ops`</span><span class="sxs-lookup"><span data-stu-id="7d05a-232">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="7d05a-233">az keyvault key list-versions: compatibilidade com o parâmetro `--id` para especificar chaves</span><span class="sxs-lookup"><span data-stu-id="7d05a-233">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="7d05a-234">Compatibilidade com conexões de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="7d05a-234">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-235">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-235">Network</span></span>

* <span data-ttu-id="7d05a-236">Avançar para azure-mgmt-network 9.0.0</span><span class="sxs-lookup"><span data-stu-id="7d05a-236">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="7d05a-237">az network private-link-service update/create: dá suporte a --enable-proxy-protocol</span><span class="sxs-lookup"><span data-stu-id="7d05a-237">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="7d05a-238">Adicionar o recurso de Monitor de conexão V2</span><span class="sxs-lookup"><span data-stu-id="7d05a-238">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="7d05a-239">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-239">Packaging</span></span>

* <span data-ttu-id="7d05a-240">[ALTERAÇÃO SIGNIFICATIVA] Fim da compatibilidade com o Python 2.7</span><span class="sxs-lookup"><span data-stu-id="7d05a-240">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="7d05a-241">Perfil</span><span class="sxs-lookup"><span data-stu-id="7d05a-241">Profile</span></span>

* <span data-ttu-id="7d05a-242">Visualização: Adicionar novos atributos `homeTenantId` e `managedByTenants` às contas de assinatura.</span><span class="sxs-lookup"><span data-stu-id="7d05a-242">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="7d05a-243">Executar `az login` novamente para as alterações entrarem em vigor</span><span class="sxs-lookup"><span data-stu-id="7d05a-243">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="7d05a-244">az login: Mostrar um aviso quando uma assinatura estiver listada de mais de um locatário e definir a primeira como padrão.</span><span class="sxs-lookup"><span data-stu-id="7d05a-244">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="7d05a-245">Para selecionar um locatário específico ao acessar essa assinatura, inclua `--tenant` em `az login`</span><span class="sxs-lookup"><span data-stu-id="7d05a-245">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-246">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-246">Role</span></span>

* <span data-ttu-id="7d05a-247">az role assignment create: Corrigir o erro em que atribuir uma função a uma entidade de serviço pelo nome de exibição gera um HTTP 400</span><span class="sxs-lookup"><span data-stu-id="7d05a-247">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-248">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-248">SQL</span></span>

* <span data-ttu-id="7d05a-249">Atualizar o cmdlet da Instância Gerenciada do SQL `az sql mi update` com dois novos parâmetros: nível e família</span><span class="sxs-lookup"><span data-stu-id="7d05a-249">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-250">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-250">Storage</span></span>

* <span data-ttu-id="7d05a-251">[ALTERAÇÃO DA FALHA] `az storage account create`: Alterar o tipo de conta de armazenamento padrão para StorageV2</span><span class="sxs-lookup"><span data-stu-id="7d05a-251">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="7d05a-252">4 de fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="7d05a-252">February 04, 2020</span></span>

<span data-ttu-id="7d05a-253">Versão 2.0.81</span><span class="sxs-lookup"><span data-stu-id="7d05a-253">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-254">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-254">ACS</span></span>

* <span data-ttu-id="7d05a-255">Adicionar suporte para definir portas alocadas de saída e tempos limite ociosos no balanceador de carga standard</span><span class="sxs-lookup"><span data-stu-id="7d05a-255">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="7d05a-256">Atualizar para a versão da API 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="7d05a-256">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-257">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-257">ACR</span></span>

* <span data-ttu-id="7d05a-258">A [ALTERAÇÃO DA FALHA] `az acr delete` será exibida</span><span class="sxs-lookup"><span data-stu-id="7d05a-258">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="7d05a-259">A [ALTERAÇÃO SIGNIFICATIVA] 'az acr task delete’ será exibida</span><span class="sxs-lookup"><span data-stu-id="7d05a-259">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="7d05a-260">Adicionar um novo grupo de comandos ‘az acr taskrun show/list/delete’ para o gerenciamento de taskrun</span><span class="sxs-lookup"><span data-stu-id="7d05a-260">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="7d05a-261">AKS</span><span class="sxs-lookup"><span data-stu-id="7d05a-261">AKS</span></span>

* <span data-ttu-id="7d05a-262">Cada cluster obtém uma entidade de serviço separada para aprimorar o isolamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-262">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="7d05a-263">AppConfig</span><span class="sxs-lookup"><span data-stu-id="7d05a-263">AppConfig</span></span>

* <span data-ttu-id="7d05a-264">Dar suporte à importação/exportação de referências keyvault de/a appservice</span><span class="sxs-lookup"><span data-stu-id="7d05a-264">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="7d05a-265">Dar suporte à importação/exportação de todos os rótulos de appconfig para appconfig</span><span class="sxs-lookup"><span data-stu-id="7d05a-265">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="7d05a-266">Validar nomes de chave e recursos antes de configurar e importar</span><span class="sxs-lookup"><span data-stu-id="7d05a-266">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="7d05a-267">Exponha a modificação do sku para o repositório de configurações.</span><span class="sxs-lookup"><span data-stu-id="7d05a-267">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="7d05a-268">Adicione o grupo de comandos à identidade gerenciada.</span><span class="sxs-lookup"><span data-stu-id="7d05a-268">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-269">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-269">AppService</span></span>

* <span data-ttu-id="7d05a-270">Azure Stack: comandos de superfície no perfil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="7d05a-270">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="7d05a-271">functionapp: adicionar a capacidade de criar aplicativos de funções Java no Linux</span><span class="sxs-lookup"><span data-stu-id="7d05a-271">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="7d05a-272">ARM</span><span class="sxs-lookup"><span data-stu-id="7d05a-272">ARM</span></span>

* <span data-ttu-id="7d05a-273">Correção de problema nº 10246: `az resource tag` falha quando o parâmetro `--ids` passado é a ID do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="7d05a-273">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="7d05a-274">Correção de problema nº 11658: o comando `az group export` não é compatível com os parâmetros `--query` e `--output`</span><span class="sxs-lookup"><span data-stu-id="7d05a-274">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="7d05a-275">Correção de problema nº 10279: O código de saída `az group deployment validate` é 0 quando a verificação falha</span><span class="sxs-lookup"><span data-stu-id="7d05a-275">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="7d05a-276">Correção de problema nº 9916: aprimorar a mensagem de erro do conflito entre a marca e outras condições de filtro para o comando `az resource list`</span><span class="sxs-lookup"><span data-stu-id="7d05a-276">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="7d05a-277">Adicionar novo parâmetro `--managed-by` para dar suporte à adição de informações managedBy para o comando `az group create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-277">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="7d05a-278">Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="7d05a-278">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="7d05a-279">Adicionar o subgrupo `monitor` para gerenciar o monitoramento do Log Analytics no cluster do Red Hat OpensShift no Azure</span><span class="sxs-lookup"><span data-stu-id="7d05a-279">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="7d05a-280">BotService</span><span class="sxs-lookup"><span data-stu-id="7d05a-280">BotService</span></span>

* <span data-ttu-id="7d05a-281">Correção de problema nº 11697: `az bot create` não é idempotente</span><span class="sxs-lookup"><span data-stu-id="7d05a-281">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="7d05a-282">Alterar testes de correção de nomes para serem executados somente em modo Ao vivo</span><span class="sxs-lookup"><span data-stu-id="7d05a-282">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="7d05a-283">CDN</span><span class="sxs-lookup"><span data-stu-id="7d05a-283">CDN</span></span>

* <span data-ttu-id="7d05a-284">Adicionar suporte ao recurso rulesEngine</span><span class="sxs-lookup"><span data-stu-id="7d05a-284">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="7d05a-285">Adicionar o novo grupo de comandos ‘cdn endpoint rule’ para gerenciar regras</span><span class="sxs-lookup"><span data-stu-id="7d05a-285">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="7d05a-286">Atualizar a versão azure-mgmt-cdn para a 4.0.0 para usar a versão da API 2019-04-15</span><span class="sxs-lookup"><span data-stu-id="7d05a-286">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="7d05a-287">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="7d05a-287">Deployment Manager</span></span>

* <span data-ttu-id="7d05a-288">Adicione a operação de lista para todos os recursos.</span><span class="sxs-lookup"><span data-stu-id="7d05a-288">Add list operation for all resources.</span></span>
* <span data-ttu-id="7d05a-289">Aprimore o recurso de etapa do novo tipo de etapa.</span><span class="sxs-lookup"><span data-stu-id="7d05a-289">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="7d05a-290">Atualize o pacote azure-mgmt-deploymentmanager para usar a versão 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="7d05a-290">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="7d05a-291">IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-291">IoT</span></span>

* <span data-ttu-id="7d05a-292">Substitua os comandos ‘IoT hub Job’.</span><span class="sxs-lookup"><span data-stu-id="7d05a-292">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="7d05a-293">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-293">IoT Central</span></span>

* <span data-ttu-id="7d05a-294">Dê suporte à atualização/criação de aplicativos com o novo nome do SKU ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="7d05a-294">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="7d05a-295">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7d05a-295">Key Vault</span></span>

* <span data-ttu-id="7d05a-296">Adicione um novo comando `az keyvault key download` para baixar chaves.</span><span class="sxs-lookup"><span data-stu-id="7d05a-296">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="7d05a-297">Diversos</span><span class="sxs-lookup"><span data-stu-id="7d05a-297">Misc</span></span>

* <span data-ttu-id="7d05a-298">Correção nº 6371: dar suporte à conclusão da variável de nome de arquivo e de ambiente em Bash</span><span class="sxs-lookup"><span data-stu-id="7d05a-298">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-299">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-299">Network</span></span>

* <span data-ttu-id="7d05a-300">Correção nº 2092: az network dns record-set add/remove: adicione um aviso quando record-set não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="7d05a-300">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="7d05a-301">No futuro, haverá suporte para um argumento extra para confirmar essa criação automática.</span><span class="sxs-lookup"><span data-stu-id="7d05a-301">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="7d05a-302">Política</span><span class="sxs-lookup"><span data-stu-id="7d05a-302">Policy</span></span>

* <span data-ttu-id="7d05a-303">Adicionar o novo comando `az policy metadata` para recuperar recursos avançados de metadados de política</span><span class="sxs-lookup"><span data-stu-id="7d05a-303">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="7d05a-304">`az policy remediation create`: Especifique se a conformidade deve ser reavaliada antes da correção com o parâmetro `--resource-discovery-mode`</span><span class="sxs-lookup"><span data-stu-id="7d05a-304">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="7d05a-305">Perfil</span><span class="sxs-lookup"><span data-stu-id="7d05a-305">Profile</span></span>

* <span data-ttu-id="7d05a-306">`az account get-access-token`: Adicionar parâmetro `--tenant` para adquirir o token do locatário diretamente, sem a necessidade de especificar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="7d05a-306">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="7d05a-307">RBAC</span><span class="sxs-lookup"><span data-stu-id="7d05a-307">RBAC</span></span>

* <span data-ttu-id="7d05a-308">[ALTERAÇÃO SIGNIFICATIVA] Correção nº 11883: `az role assignment create`: o escopo vazio exibirá erro</span><span class="sxs-lookup"><span data-stu-id="7d05a-308">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="7d05a-309">Segurança</span><span class="sxs-lookup"><span data-stu-id="7d05a-309">Security</span></span>

* <span data-ttu-id="7d05a-310">Adicione novos comandos `az atp show` e `az atp update` para exibir e gerenciar configurações avançadas de proteção contra ameaças para contas de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="7d05a-310">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-311">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-311">SQL</span></span>

* <span data-ttu-id="7d05a-312">`sql dw create`: substitua os parâmetros `--zone-redundant` e `--read-replica-count`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-312">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="7d05a-313">Esses parâmetros não se aplicam ao DataWarehouse.</span><span class="sxs-lookup"><span data-stu-id="7d05a-313">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="7d05a-314">[ALTERAÇÃO DA FALHA] `az sql db create`: Remova "WideWorldImportersStd" e "WideWorldImportersFull" como valores permitidos documentados para "az sql db create --sample-name".</span><span class="sxs-lookup"><span data-stu-id="7d05a-314">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="7d05a-315">Esses bancos de dados de exemplo sempre farão a criação falhar.</span><span class="sxs-lookup"><span data-stu-id="7d05a-315">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="7d05a-316">Adicione os novos comandos `sql db classification show/list/update/delete` e `sql db classification recommendation list/enable/disable` para gerenciar classificações de confidencialidade para bancos de dados SQL.</span><span class="sxs-lookup"><span data-stu-id="7d05a-316">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="7d05a-317">`az sql db audit-policy`: Correção para ações e grupos de auditoria vazios</span><span class="sxs-lookup"><span data-stu-id="7d05a-317">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-318">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-318">Storage</span></span>

* <span data-ttu-id="7d05a-319">Adicione um novo grupo de comandos `az storage share-rm` para usar o provedor de recursos Microsoft.Storage para operações de gerenciamento de compartilhamento de arquivo do Azure.</span><span class="sxs-lookup"><span data-stu-id="7d05a-319">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="7d05a-320">Correção de problema nº 11415: erro de permissão para `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-320">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="7d05a-321">Integre Azcopy 10.3.3 e dê suporte a Win32.</span><span class="sxs-lookup"><span data-stu-id="7d05a-321">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="7d05a-322">`az storage copy`: Adicione os parâmetros `--include-path`, `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="7d05a-322">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="7d05a-323">`az storage remove`: Altere os parâmetros `--inlcude` e `--exclude` para os parâmetros `--include-path`, `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="7d05a-323">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="7d05a-324">`az storage sync`: Adicione os parâmetros `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="7d05a-324">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="7d05a-325">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7d05a-325">ServiceFabric</span></span>

* <span data-ttu-id="7d05a-326">Adicione novos comandos para gerenciar o aplicativo e os serviços.</span><span class="sxs-lookup"><span data-stu-id="7d05a-326">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="7d05a-327">13 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="7d05a-327">January 13, 2020</span></span>

<span data-ttu-id="7d05a-328">Versão 2.0.80</span><span class="sxs-lookup"><span data-stu-id="7d05a-328">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="7d05a-329">Computação</span><span class="sxs-lookup"><span data-stu-id="7d05a-329">Compute</span></span>

* <span data-ttu-id="7d05a-330">atualização do disco: Adicionar --disk-encryption-set e --encryption-type</span><span class="sxs-lookup"><span data-stu-id="7d05a-330">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="7d05a-331">criação/atualização do instantâneo: Adicionar --disk-encryption-set e --encryption-type</span><span class="sxs-lookup"><span data-stu-id="7d05a-331">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-332">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-332">Storage</span></span>

* <span data-ttu-id="7d05a-333">Atualizar a versão do azure-mgmt-storage para 7.1.0</span><span class="sxs-lookup"><span data-stu-id="7d05a-333">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="7d05a-334">`az storage account create`: Adicionar `--encryption-key-type-for-table` e `--encryption-key-type-for-queue` para dar suporte ao Serviço de Criptografia de Tabela e de Fila</span><span class="sxs-lookup"><span data-stu-id="7d05a-334">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="7d05a-335">07 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="7d05a-335">January 07, 2020</span></span>

<span data-ttu-id="7d05a-336">Versão 2.0.79</span><span class="sxs-lookup"><span data-stu-id="7d05a-336">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-337">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-337">ACR</span></span>

* <span data-ttu-id="7d05a-338">[ALTERAÇÃO SIGNIFICATIVA] Remover o parâmetro '--os' para 'acr build', 'acr task create/update', 'acr run' e 'acr pack'.</span><span class="sxs-lookup"><span data-stu-id="7d05a-338">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="7d05a-339">Em vez disso, use '--platform'.</span><span class="sxs-lookup"><span data-stu-id="7d05a-339">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="7d05a-340">AppConfig</span><span class="sxs-lookup"><span data-stu-id="7d05a-340">AppConfig</span></span>

* <span data-ttu-id="7d05a-341">Adicionar suporte para importar/exportar sinalizadores de recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-341">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="7d05a-342">Adicione o novo comando 'az appconfig kv set-keyvault' para criar a referência do keyvault</span><span class="sxs-lookup"><span data-stu-id="7d05a-342">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="7d05a-343">Suporte a várias convenções de nomenclatura ao exportar os sinalizadores de recurso para o arquivo</span><span class="sxs-lookup"><span data-stu-id="7d05a-343">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-344">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-344">AppService</span></span>

* <span data-ttu-id="7d05a-345">Corrigir o problema #7154: Atualizar a documentação para o comando <> para usar acentos grave em vez de aspas simples</span><span class="sxs-lookup"><span data-stu-id="7d05a-345">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="7d05a-346">Corrigir o problema #11287: webapp up: Por padrão, faça o aplicativo criado usando 'should be 'SSL enabled'</span><span class="sxs-lookup"><span data-stu-id="7d05a-346">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="7d05a-347">Corrigir o problema #11592: Adicionar o sinalizador az webapp up para sites HTML estáticos</span><span class="sxs-lookup"><span data-stu-id="7d05a-347">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="7d05a-348">ARM</span><span class="sxs-lookup"><span data-stu-id="7d05a-348">ARM</span></span>

* <span data-ttu-id="7d05a-349">Corrigir `az resource tag`: As marcas do Cofre dos Serviços de Recuperação não podem ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="7d05a-349">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="7d05a-350">Backup</span><span class="sxs-lookup"><span data-stu-id="7d05a-350">Backup</span></span>

* <span data-ttu-id="7d05a-351">Novo comando 'backup protection undelete' adicionado para habilitar o recurso de exclusão reversível para carga de trabalho IaasVM</span><span class="sxs-lookup"><span data-stu-id="7d05a-351">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="7d05a-352">Novo parâmetro '--soft-delete-feature-state' adicionado para definir o comando propriedades do backup</span><span class="sxs-lookup"><span data-stu-id="7d05a-352">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="7d05a-353">Suporte de exclusão de disco adicionado para carga de trabalho IaasVM</span><span class="sxs-lookup"><span data-stu-id="7d05a-353">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="7d05a-354">Computação</span><span class="sxs-lookup"><span data-stu-id="7d05a-354">Compute</span></span>

* <span data-ttu-id="7d05a-355">Corrigir a falha `vm create` no perfil do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="7d05a-355">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="7d05a-356">parte final/listar definições de métricas de monitor de vm: suporte a métricas de consulta e definições de lista para uma vm.</span><span class="sxs-lookup"><span data-stu-id="7d05a-356">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="7d05a-357">Adicionar nova ação de comando de reaplicação para az vm</span><span class="sxs-lookup"><span data-stu-id="7d05a-357">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7d05a-358">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7d05a-358">HDInsight</span></span>

* <span data-ttu-id="7d05a-359">Suporte para criar um cluster Kafka com o Proxy REST do Kafka</span><span class="sxs-lookup"><span data-stu-id="7d05a-359">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="7d05a-360">Atualizar azure-mgmt-hdinsight para 1.3.0</span><span class="sxs-lookup"><span data-stu-id="7d05a-360">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="7d05a-361">Diversos.</span><span class="sxs-lookup"><span data-stu-id="7d05a-361">Misc.</span></span>

* <span data-ttu-id="7d05a-362">Adicionar comando de visualização `az version show` para mostrar as versões dos módulos e das extensões da CLI do Azure no formato JSON por padrão ou no formato configurado por --output</span><span class="sxs-lookup"><span data-stu-id="7d05a-362">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="7d05a-363">Hubs de Eventos</span><span class="sxs-lookup"><span data-stu-id="7d05a-363">Event Hubs</span></span>

* <span data-ttu-id="7d05a-364">[ALTERAÇÃO SIGNIFICATIVA] Remover a opção de status 'ReceiveDisabled' do comando 'az eventhubs eventhub update' e 'az eventhubs eventhub create'.</span><span class="sxs-lookup"><span data-stu-id="7d05a-364">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="7d05a-365">Essa opção não é válida para entidades do Hub de Eventos.</span><span class="sxs-lookup"><span data-stu-id="7d05a-365">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="7d05a-366">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="7d05a-366">Service Bus</span></span>

* <span data-ttu-id="7d05a-367">[ALTERAÇÃO SIGNIFICATIVA] Remover a opção de status 'ReceiveDisabled' do comando 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create' e 'az servicebus queue update'.</span><span class="sxs-lookup"><span data-stu-id="7d05a-367">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="7d05a-368">Essa opção não é válida para tópicos e filas do Barramento de Serviço.</span><span class="sxs-lookup"><span data-stu-id="7d05a-368">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="7d05a-369">RBAC</span><span class="sxs-lookup"><span data-stu-id="7d05a-369">RBAC</span></span>

* <span data-ttu-id="7d05a-370">Correção #11712: `az ad app/sp show` não devolve o código de saída 3 quando o aplicativo ou a entidade de serviço não existir</span><span class="sxs-lookup"><span data-stu-id="7d05a-370">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-371">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-371">Storage</span></span>

* <span data-ttu-id="7d05a-372">`az storage account create`: Remover o sinalizador de visualização do parâmetro --enable-hierarchical-namespace</span><span class="sxs-lookup"><span data-stu-id="7d05a-372">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="7d05a-373">Atualizar a versão azure-mgmt-storage para 7.0.0 para usar a versão de API 2019-06-01</span><span class="sxs-lookup"><span data-stu-id="7d05a-373">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="7d05a-374">Adicionar novos parâmetros `--enable-delete-retention` e `--delete-retention-days` para dar suporte ao gerenciamento da política de retenção de exclusão para a conta de armazenamento blob-service-properties.</span><span class="sxs-lookup"><span data-stu-id="7d05a-374">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="7d05a-375">17 de dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-375">December 17, 2019</span></span>

<span data-ttu-id="7d05a-376">2.0.78</span><span class="sxs-lookup"><span data-stu-id="7d05a-376">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-377">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-377">ACR</span></span>

* <span data-ttu-id="7d05a-378">Contexto local de suporte adicionado na execução da tarefa acr</span><span class="sxs-lookup"><span data-stu-id="7d05a-378">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-379">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-379">ACS</span></span>

* <span data-ttu-id="7d05a-380">[ALTERAÇÃO SIGNIFICATIVA]criar az openshift: renomear `--workspace-resource-id` para `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-380">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="7d05a-381">AMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-381">AMS</span></span>

* <span data-ttu-id="7d05a-382">Comandos de exibição atualizados para devolver 3 quando o recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="7d05a-382">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="7d05a-383">AppConfig</span><span class="sxs-lookup"><span data-stu-id="7d05a-383">AppConfig</span></span>

* <span data-ttu-id="7d05a-384">Bug corrigido ao acrescentar a versão de API à URL de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d05a-384">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="7d05a-385">A solução existente não funciona com a paginação.</span><span class="sxs-lookup"><span data-stu-id="7d05a-385">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="7d05a-386">Suporte adicionado para a exibição de idiomas além do inglês, pois nosso serviço de back-end é compatível com unicode para globalização.</span><span class="sxs-lookup"><span data-stu-id="7d05a-386">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-387">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-387">AppService</span></span>

* <span data-ttu-id="7d05a-388">Problema corrigido nº 11217: webapp: o upload ssl de configuração do az webapp deve ser compatível com o parâmetro do slot</span><span class="sxs-lookup"><span data-stu-id="7d05a-388">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="7d05a-389">Problema corrigido nº 10965: Erro: O nome não pode estar vazio.</span><span class="sxs-lookup"><span data-stu-id="7d05a-389">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="7d05a-390">Permitir remoção por ip_address e sub-rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-390">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="7d05a-391">Suporte adicionado para importar certificados do Key Vault `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="7d05a-391">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="7d05a-392">ARM</span><span class="sxs-lookup"><span data-stu-id="7d05a-392">ARM</span></span>

* <span data-ttu-id="7d05a-393">Pacote azure-mgmt-resource atualizado para usar 6.0.0</span><span class="sxs-lookup"><span data-stu-id="7d05a-393">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="7d05a-394">Suporte entre locatários para o comando `az group deployment create` adicionando o novo parâmetro `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="7d05a-394">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="7d05a-395">Novo parâmetro `--metadata` adicionado para dar suporte à adição de informações de metadados para definições de conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="7d05a-395">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="7d05a-396">Backup</span><span class="sxs-lookup"><span data-stu-id="7d05a-396">Backup</span></span>

* <span data-ttu-id="7d05a-397">Suporte de backup adicionado para carga de trabalho SQL e SAP Hana.</span><span class="sxs-lookup"><span data-stu-id="7d05a-397">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="7d05a-398">BotService</span><span class="sxs-lookup"><span data-stu-id="7d05a-398">BotService</span></span>

* <span data-ttu-id="7d05a-399">[ALTERAÇÃO SIGNIFICATIVA] Remover o sinalizador '--version ' do comando de visualização 'az bot create'.</span><span class="sxs-lookup"><span data-stu-id="7d05a-399">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="7d05a-400">Somente os bots do SDK v4 são compatíveis.</span><span class="sxs-lookup"><span data-stu-id="7d05a-400">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="7d05a-401">Verificação de disponibilidade de nome adicionada para 'az bot create'.</span><span class="sxs-lookup"><span data-stu-id="7d05a-401">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="7d05a-402">Suporte adicionado para atualizar a URL do ícone para um bot por meio de 'az bot update'.</span><span class="sxs-lookup"><span data-stu-id="7d05a-402">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="7d05a-403">Suporte adicionado para atualizar um canal Direct Line por meio de 'az bot directline update'.</span><span class="sxs-lookup"><span data-stu-id="7d05a-403">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="7d05a-404">Suporte ao sinalizador '--enable-enhanced-auth' adicionado para 'az bot directline create'.</span><span class="sxs-lookup"><span data-stu-id="7d05a-404">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="7d05a-405">Os seguintes grupos de comandos estão em GA e não estão em versão prévia: 'az bot authsetting'.</span><span class="sxs-lookup"><span data-stu-id="7d05a-405">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="7d05a-406">Os seguintes comandos em 'az bot' estão em GA e não na versão prévia: 'criar', 'preparar-implantar', 'mostrar', 'excluir', 'atualizar'.</span><span class="sxs-lookup"><span data-stu-id="7d05a-406">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="7d05a-407">Correção do valor 'az bot prepare-deploy' alterando '--proj-file-path ' para letras minúsculas (por exemplo, "Test. csproj" para "Test. csproj").</span><span class="sxs-lookup"><span data-stu-id="7d05a-407">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="7d05a-408">Computação</span><span class="sxs-lookup"><span data-stu-id="7d05a-408">Compute</span></span>

* <span data-ttu-id="7d05a-409">Criar/atualizar vmss: --scale-in-policy adicionado, que decide quais máquinas virtuais são escolhidas para remoção quando um VMSS é dimensionado.</span><span class="sxs-lookup"><span data-stu-id="7d05a-409">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="7d05a-410">atualização de vm/vmss: --priority adicionado.</span><span class="sxs-lookup"><span data-stu-id="7d05a-410">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="7d05a-411">atualização de vm/vmss: --max-price adicionado.</span><span class="sxs-lookup"><span data-stu-id="7d05a-411">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="7d05a-412">Grupo de comandos do conjunto de criptografia de disco adicionado (criar, mostrar, atualizar, excluir e listar).</span><span class="sxs-lookup"><span data-stu-id="7d05a-412">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="7d05a-413">criação de disco: --encryption-type e --disk-encryption-set adicionados.</span><span class="sxs-lookup"><span data-stu-id="7d05a-413">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="7d05a-414">vm/vmss create: --os-disk-encryption-set e --data-disk-encryption-sets adicionados.</span><span class="sxs-lookup"><span data-stu-id="7d05a-414">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-415">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-415">Core</span></span>

* <span data-ttu-id="7d05a-416">Suporte para Python 3.4 removido</span><span class="sxs-lookup"><span data-stu-id="7d05a-416">Removed support for Python 3.4</span></span>
* <span data-ttu-id="7d05a-417">Pesquisa de funções de plug-in em vários comandos</span><span class="sxs-lookup"><span data-stu-id="7d05a-417">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="7d05a-418">DLS</span><span class="sxs-lookup"><span data-stu-id="7d05a-418">DLS</span></span>

* <span data-ttu-id="7d05a-419">Versão atualizada do SDK do ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="7d05a-419">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="7d05a-420">Instalar</span><span class="sxs-lookup"><span data-stu-id="7d05a-420">Install</span></span>

* <span data-ttu-id="7d05a-421">Instalar suporte de script Python 3.8</span><span class="sxs-lookup"><span data-stu-id="7d05a-421">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="7d05a-422">IOT</span><span class="sxs-lookup"><span data-stu-id="7d05a-422">IOT</span></span>

* <span data-ttu-id="7d05a-423">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro--failover-region removido de failover manual.</span><span class="sxs-lookup"><span data-stu-id="7d05a-423">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="7d05a-424">Agora ele fará failover para a região secundária emparelhada atribuída geograficamente.</span><span class="sxs-lookup"><span data-stu-id="7d05a-424">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="7d05a-425">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7d05a-425">Key Vault</span></span>

* <span data-ttu-id="7d05a-426">Nº 8095 corrigido: `az keyvault storage remove`: melhorar a mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="7d05a-426">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="7d05a-427">Nº 8921 corrigido: `az keyvault key/secret/certificate list/list-deleted/list-versions`: corrigir o bug de validação no parâmetro `--maxresults`</span><span class="sxs-lookup"><span data-stu-id="7d05a-427">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="7d05a-428">Nº 10512 corrigido: `az keyvault set-policy`: melhorar a mensagem de erro quando nenhuma das `--object-id`, `--spn` ou `--upn` for especificada</span><span class="sxs-lookup"><span data-stu-id="7d05a-428">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="7d05a-429">Nº 10846 corrigido: `az keyvault secret show-deleted`: quando `--id` for especificado, `--name/-n` não será necessário</span><span class="sxs-lookup"><span data-stu-id="7d05a-429">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="7d05a-430">Nº 11084 corrigido: `az keyvault secret download`: melhorar a mensagem de ajuda do parâmetro `--encoding`</span><span class="sxs-lookup"><span data-stu-id="7d05a-430">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-431">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-431">Network</span></span>

* <span data-ttu-id="7d05a-432">Investigação de gateway de aplicativo de rede az: Suporte --port option adicionado para especificar uma porta para sondar servidores de back-end ao criar e atualizar</span><span class="sxs-lookup"><span data-stu-id="7d05a-432">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="7d05a-433">az network application-gateway url-path-map create/update: correção de bug para `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="7d05a-433">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="7d05a-434">az network application-gateway: Suporte `--rewrite-rule-set` adicionado</span><span class="sxs-lookup"><span data-stu-id="7d05a-434">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="7d05a-435">az network list-service-aliases: Foram adicionados aliases de serviço da lista de suporte que podem ser usados para políticas de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="7d05a-435">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="7d05a-436">importar zona dns da rede az: Suporte adicionado. @ no nome do registro</span><span class="sxs-lookup"><span data-stu-id="7d05a-436">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="7d05a-437">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-437">Packaging</span></span>

* <span data-ttu-id="7d05a-438">Compilações de back edge adicionadas para instalação de pip</span><span class="sxs-lookup"><span data-stu-id="7d05a-438">Added back edge builds for pip install</span></span>
* <span data-ttu-id="7d05a-439">Pacote eoan do Ubuntu adicionado</span><span class="sxs-lookup"><span data-stu-id="7d05a-439">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="7d05a-440">Política</span><span class="sxs-lookup"><span data-stu-id="7d05a-440">Policy</span></span>

* <span data-ttu-id="7d05a-441">Inclusão de compatibilidade com a API de Política, versão de 01/09/2019.</span><span class="sxs-lookup"><span data-stu-id="7d05a-441">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="7d05a-442">az policy set-definition: Agrupamento de suporte adicionado nas definições do conjunto de políticas com `--definition-groups` parâmetro</span><span class="sxs-lookup"><span data-stu-id="7d05a-442">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="7d05a-443">Redis</span><span class="sxs-lookup"><span data-stu-id="7d05a-443">Redis</span></span>

* <span data-ttu-id="7d05a-444">Adicionado o parâmetro de visualização `--replicas-per-master` ao comando `az redis create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-444">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="7d05a-445">Azure-MGMT-Redis adicionado do 6.0.0 para o 7.0.0rc1</span><span class="sxs-lookup"><span data-stu-id="7d05a-445">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="7d05a-446">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7d05a-446">ServiceFabric</span></span>

* <span data-ttu-id="7d05a-447">Corrigido em nó-tipo adicionar lógica, incluindo #10963: A adição do novo tipo de nó com nível de durabilidade Gold sempre gerará erro da CLI</span><span class="sxs-lookup"><span data-stu-id="7d05a-447">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="7d05a-448">Versão do ServiceFabricNodeVmExt atualizada para 1.1 no modelo de criação</span><span class="sxs-lookup"><span data-stu-id="7d05a-448">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-449">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-449">SQL</span></span>

* <span data-ttu-id="7d05a-450">Adicionados os parâmetros "--read-scale" e "--read-replicas" aos comandos criar e atualizar do BD SQL para dar suporte ao gerenciamento de escala de leitura.</span><span class="sxs-lookup"><span data-stu-id="7d05a-450">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-451">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-451">Storage</span></span>

* <span data-ttu-id="7d05a-452">Propriedade de compartilhamentos de arquivos grandes da versão GA para o comando criar e atualizar da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-452">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="7d05a-453">Suporte ao token SAS de delegação de usuário da versão GA</span><span class="sxs-lookup"><span data-stu-id="7d05a-453">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="7d05a-454">Novos comandos adicionados `az storage account blob-service-properties show` e `az storage account blob-service-properties update --enable-change-feed` para gerenciar Propriedades do serviço blob para a conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="7d05a-454">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="7d05a-455">[PRÓXIMA ALTERAÇÃO DA FALHA] `az storage copy`: `*` não há mais suporte para o caractere de como um curinga na URL, mas novos parâmetros--include-pattern e --exclude-pattern serão adicionados com suporte a curinga `*`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-455">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="7d05a-456">Problema corrigido nº 11043: Suporte adicionado para remover contêiner/compartilhamento inteiro no comando `az storage remove`</span><span class="sxs-lookup"><span data-stu-id="7d05a-456">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="7d05a-457">26 de novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-457">November 26, 2019</span></span>

<span data-ttu-id="7d05a-458">Versão 2.0.77</span><span class="sxs-lookup"><span data-stu-id="7d05a-458">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-459">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-459">ACR</span></span>

* <span data-ttu-id="7d05a-460">Parâmetro `--branch` preterido da criação/atualização da tarefa ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-460">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="7d05a-461">Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="7d05a-461">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="7d05a-462">Sinalizador `--workspace-resource-id` adicionado para permitir a criação do cluster do Red Hat OpenShift no Azure com monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-462">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="7d05a-463">`monitor_profile` adicionado para criar o cluster do Red Hat OpenShift no Azure com monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-463">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="7d05a-464">AKS</span><span class="sxs-lookup"><span data-stu-id="7d05a-464">AKS</span></span>

* <span data-ttu-id="7d05a-465">Operação de rotação de certificado de cluster de suporte adicionada usando "az aks rotate-certs".</span><span class="sxs-lookup"><span data-stu-id="7d05a-465">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="7d05a-466">AppConfig</span><span class="sxs-lookup"><span data-stu-id="7d05a-466">AppConfig</span></span>

* <span data-ttu-id="7d05a-467">Suporte adicionado para usar ":" para o separador `as az appconfig kv import`</span><span class="sxs-lookup"><span data-stu-id="7d05a-467">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="7d05a-468">Problema corrigido para listar valores de chave com vários rótulos incluindo o rótulo nulo.</span><span class="sxs-lookup"><span data-stu-id="7d05a-468">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="7d05a-469">SDK do plano de gerenciamento atualizado, azure-mgmt-appconfiguration, para a versão 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="7d05a-469">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="7d05a-470">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-470">AppService</span></span>

* <span data-ttu-id="7d05a-471">Problema corrigido nº 11100: AttributeError para az webapp up ao criar o plano de serviço</span><span class="sxs-lookup"><span data-stu-id="7d05a-471">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="7d05a-472">az webapp up: Forçar a criação ou a implantação em um site para linguagens com suporte, nenhum padrão usado.</span><span class="sxs-lookup"><span data-stu-id="7d05a-472">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="7d05a-473">Suporte adicionado para o Ambiente do Serviço de Aplicativo: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="7d05a-473">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="7d05a-474">Backup</span><span class="sxs-lookup"><span data-stu-id="7d05a-474">Backup</span></span>

* <span data-ttu-id="7d05a-475">Problema corrigido em list-associated-items da política de backup az.</span><span class="sxs-lookup"><span data-stu-id="7d05a-475">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="7d05a-476">Parâmetro BackupManagementType opcional adicionado.</span><span class="sxs-lookup"><span data-stu-id="7d05a-476">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="7d05a-477">Computação</span><span class="sxs-lookup"><span data-stu-id="7d05a-477">Compute</span></span>

* <span data-ttu-id="7d05a-478">Versão de API de computação, discos e instantâneos atualizados para 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="7d05a-478">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="7d05a-479">vmss create: melhoria para --orchestration-mode</span><span class="sxs-lookup"><span data-stu-id="7d05a-479">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="7d05a-480">sig image-definition create: --os-state adicionado para permitir a especificação se as máquinas virtuais criadas nessa imagem são 'Generalizadas' ou 'Especializadas'</span><span class="sxs-lookup"><span data-stu-id="7d05a-480">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="7d05a-481">sig image-definition create: --hyper-v-generation adicionado para permitir a especificação da geração do hipervisor</span><span class="sxs-lookup"><span data-stu-id="7d05a-481">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="7d05a-482">sig image-version create: --os-snapshot e --data-snapshots de suporte adicionados</span><span class="sxs-lookup"><span data-stu-id="7d05a-482">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="7d05a-483">image create: --data-disk-caching adicionado para permitir a especificação da configuração de cache de discos de dados</span><span class="sxs-lookup"><span data-stu-id="7d05a-483">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="7d05a-484">SDK de computação do Python atualizado para 10.0.0</span><span class="sxs-lookup"><span data-stu-id="7d05a-484">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="7d05a-485">vm/vmss create: 'Spot' adicionado à propriedade de enumeração 'Priority'</span><span class="sxs-lookup"><span data-stu-id="7d05a-485">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="7d05a-486">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro '--max-billing' renomeado para '--max-price', para a VM e o VMSS, a fim de que seja consistente com os cmdlets do Swagger e do PowerShell</span><span class="sxs-lookup"><span data-stu-id="7d05a-486">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="7d05a-487">vm monitor log show: suporte adicionado para consultar o log pelo workspace do Log Analytics vinculado.</span><span class="sxs-lookup"><span data-stu-id="7d05a-487">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="7d05a-488">IOT</span><span class="sxs-lookup"><span data-stu-id="7d05a-488">IOT</span></span>

* <span data-ttu-id="7d05a-489">Correção nº 2531: argumentos de conveniência adicionados para a atualização do hub.</span><span class="sxs-lookup"><span data-stu-id="7d05a-489">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="7d05a-490">Correção nº 8323: parâmetros ausentes adicionados para criar o ponto de extremidade personalizado de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="7d05a-490">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="7d05a-491">Corrigir bug de regressão: as alterações que substituem o ponto de extremidade de armazenamento padrão foram revertidas.</span><span class="sxs-lookup"><span data-stu-id="7d05a-491">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="7d05a-492">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7d05a-492">Key Vault</span></span>

* <span data-ttu-id="7d05a-493">Correção nº 11121: ao usar `az keyvault certificate list`, passar `--include-pending` agora não exige um valor de `true` ou `false`</span><span class="sxs-lookup"><span data-stu-id="7d05a-493">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="7d05a-494">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="7d05a-494">NetAppFiles</span></span>

* <span data-ttu-id="7d05a-495">azure-mgmt-netapp atualizado para 0.7.0 que inclui algumas propriedades de volume adicionais associadas a operações de replicação futuras</span><span class="sxs-lookup"><span data-stu-id="7d05a-495">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-496">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-496">Network</span></span>

* <span data-ttu-id="7d05a-497">application-gateway waf-config: preterido</span><span class="sxs-lookup"><span data-stu-id="7d05a-497">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="7d05a-498">application-gateway waf-policy: subgrupo managed-rules adicionado para gerenciar os conjuntos de regras e regras de exclusão gerenciados</span><span class="sxs-lookup"><span data-stu-id="7d05a-498">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="7d05a-499">application-gateway waf-policy: subgrupo policy-setting adicionado para gerenciar a configuração global de um waf-policy</span><span class="sxs-lookup"><span data-stu-id="7d05a-499">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="7d05a-500">[ALTERAÇÃO SIGNIFICATIVA] application-gateway waf-policy: subgrupo rule renomeado para custom-rule</span><span class="sxs-lookup"><span data-stu-id="7d05a-500">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="7d05a-501">application-gateway http-listener: --firewall-policy adicionado durante a criação</span><span class="sxs-lookup"><span data-stu-id="7d05a-501">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="7d05a-502">application-gateway url-path-map rule: --firewall-policy adicionado durante a criação</span><span class="sxs-lookup"><span data-stu-id="7d05a-502">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="7d05a-503">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-503">Packaging</span></span>

* <span data-ttu-id="7d05a-504">Wrapper az reescrito no Python</span><span class="sxs-lookup"><span data-stu-id="7d05a-504">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="7d05a-505">Suporte adicionado para Python 3.8</span><span class="sxs-lookup"><span data-stu-id="7d05a-505">Added support for Python 3.8</span></span>
* <span data-ttu-id="7d05a-506">Alterado para Python 3 para o pacote RPM</span><span class="sxs-lookup"><span data-stu-id="7d05a-506">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="7d05a-507">Perfil</span><span class="sxs-lookup"><span data-stu-id="7d05a-507">Profile</span></span>

* <span data-ttu-id="7d05a-508">Erro aperfeiçoado ao executar `az login -u {} -p {}` com a conta Microsoft</span><span class="sxs-lookup"><span data-stu-id="7d05a-508">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="7d05a-509">`SSLError` aperfeiçoado ao executar `az login` atrás de um proxy com o certificado raiz autoassinado</span><span class="sxs-lookup"><span data-stu-id="7d05a-509">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="7d05a-510">Correção nº 10578: `az login` trava quando mais de uma instância é iniciada ao mesmo tempo no Windows ou WSL</span><span class="sxs-lookup"><span data-stu-id="7d05a-510">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="7d05a-511">Correção nº 11059: `az login --allow-no-subscriptions` falhará se houver assinaturas no locatário</span><span class="sxs-lookup"><span data-stu-id="7d05a-511">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="7d05a-512">Correção nº 11238: após renomear uma assinatura, fazer logon com a MSI fará a mesma assinatura aparecer duas vezes</span><span class="sxs-lookup"><span data-stu-id="7d05a-512">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="7d05a-513">RBAC</span><span class="sxs-lookup"><span data-stu-id="7d05a-513">RBAC</span></span>

* <span data-ttu-id="7d05a-514">Correção nº 10996: erro aperfeiçoado para `--force-change-password-next-login` em `az ad user update` quando `--password` não for especificado</span><span class="sxs-lookup"><span data-stu-id="7d05a-514">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="7d05a-515">Redis</span><span class="sxs-lookup"><span data-stu-id="7d05a-515">Redis</span></span>

* <span data-ttu-id="7d05a-516">Correção nº 2902: evite definir configurações de memória ao atualizar o cache do SKU básico</span><span class="sxs-lookup"><span data-stu-id="7d05a-516">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="7d05a-517">Reservas</span><span class="sxs-lookup"><span data-stu-id="7d05a-517">Reservations</span></span>

* <span data-ttu-id="7d05a-518">Versão do SDK atualizada para 0.6.0</span><span class="sxs-lookup"><span data-stu-id="7d05a-518">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="7d05a-519">Informações de detalhes do plano de cobrança atualizadas após chamar Get-Gatalogs</span><span class="sxs-lookup"><span data-stu-id="7d05a-519">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="7d05a-520">Novo comando `az reservations reservation-order calculate` adicionado para calcular o preço de uma reserva</span><span class="sxs-lookup"><span data-stu-id="7d05a-520">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="7d05a-521">Novo comando `az reservations reservation-order purchase` adicionado para comprar uma nova reserva</span><span class="sxs-lookup"><span data-stu-id="7d05a-521">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="7d05a-522">Rest</span><span class="sxs-lookup"><span data-stu-id="7d05a-522">Rest</span></span>
* <span data-ttu-id="7d05a-523">`az rest` alterado para GA</span><span class="sxs-lookup"><span data-stu-id="7d05a-523">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-524">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-524">SQL</span></span>

* <span data-ttu-id="7d05a-525">azure-mgmt-sql atualizado para 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="7d05a-525">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-526">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-526">Storage</span></span>

* <span data-ttu-id="7d05a-527">storage account create: --enable-hierarchical-namespace adicionado para dar suporte à semântica do sistema de arquivos no serviço Blob.</span><span class="sxs-lookup"><span data-stu-id="7d05a-527">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="7d05a-528">Exceção não relacionada removida da mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="7d05a-528">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="7d05a-529">Problemas corrigidos com a mensagem de erro incorreta "Você não tem as permissões necessárias para executar essa operação."</span><span class="sxs-lookup"><span data-stu-id="7d05a-529">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="7d05a-530">quando bloqueado pelas regras de rede ou AuthenticationFailed.</span><span class="sxs-lookup"><span data-stu-id="7d05a-530">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="7d05a-531">4 de novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-531">November 4, 2019</span></span>

<span data-ttu-id="7d05a-532">Versão 2.0.76</span><span class="sxs-lookup"><span data-stu-id="7d05a-532">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-533">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-533">ACR</span></span>

* <span data-ttu-id="7d05a-534">O parâmetro de versão prévia `--pack-image-tag` foi adicionado ao comando `az acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-534">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="7d05a-535">Suporte adicionado para habilitar a auditoria na criação de um registro</span><span class="sxs-lookup"><span data-stu-id="7d05a-535">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="7d05a-536">Suporte adicionado para o RBAC com escopo de repositório</span><span class="sxs-lookup"><span data-stu-id="7d05a-536">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="7d05a-537">AKS</span><span class="sxs-lookup"><span data-stu-id="7d05a-537">AKS</span></span>

* <span data-ttu-id="7d05a-538">`--enable-cluster-autoscaler`, `--min-count` e `--max-count` foram adicionados ao comando `az aks create`, que habilita o dimensionamento automático do cluster para o pool de nós.</span><span class="sxs-lookup"><span data-stu-id="7d05a-538">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="7d05a-539">Foram adicionados os sinalizadores acima, bem como `--update-cluster-autoscaler` e `--disable-cluster-autoscaler` ao comando `az aks update`, permitindo atualizações do cluster de dimensionamento automático.</span><span class="sxs-lookup"><span data-stu-id="7d05a-539">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="7d05a-540">AppConfig</span><span class="sxs-lookup"><span data-stu-id="7d05a-540">AppConfig</span></span>

* <span data-ttu-id="7d05a-541">O grupo de comandos do recurso AppConfig foi adicionado para gerenciar os sinalizadores de recurso armazenados em uma Configuração de Aplicativos.</span><span class="sxs-lookup"><span data-stu-id="7d05a-541">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="7d05a-542">Foi corrigido um bug secundário do comando de exportação para arquivo appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="7d05a-542">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="7d05a-543">Foi interrompida a leitura de conteúdo do arquivo de destino durante a exportação.</span><span class="sxs-lookup"><span data-stu-id="7d05a-543">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-544">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-544">AppService</span></span>

* <span data-ttu-id="7d05a-545">`az appservice plan create`: Foi adicionado o suporte para definir 'persitecalling' no comando appservice plan create.</span><span class="sxs-lookup"><span data-stu-id="7d05a-545">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="7d05a-546">Foi corrigido um problema em que a operação webapp config ssl bind estava removendo as marcas existentes do recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-546">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="7d05a-547">Foi adicionado o sinalizador `--build-remote` para `az functionapp deployment source config-zip` para dar suporte à ação de build remoto durante a implantação do aplicativo de funções.</span><span class="sxs-lookup"><span data-stu-id="7d05a-547">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="7d05a-548">Foi alterada a versão do nó padrão em aplicativos de funções para ~10 para Windows</span><span class="sxs-lookup"><span data-stu-id="7d05a-548">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="7d05a-549">A propriedade `--runtime-version` foi adicionada a `az functionapp create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-549">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="7d05a-550">ARM</span><span class="sxs-lookup"><span data-stu-id="7d05a-550">ARM</span></span>

* <span data-ttu-id="7d05a-551">`az deployment/group deployment validate`: Foi adicionado o parâmetro `--handle-extended-json-format` para dar suporte a várias linhas e comentários no modelo JSON durante a implantação.</span><span class="sxs-lookup"><span data-stu-id="7d05a-551">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="7d05a-552">O azure-mgmt-resource passou a usar a 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="7d05a-552">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="7d05a-553">Backup</span><span class="sxs-lookup"><span data-stu-id="7d05a-553">Backup</span></span>

* <span data-ttu-id="7d05a-554">Foi adicionado o suporte de backup aos Arquivos do Azure</span><span class="sxs-lookup"><span data-stu-id="7d05a-554">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="7d05a-555">Computação</span><span class="sxs-lookup"><span data-stu-id="7d05a-555">Compute</span></span>

* <span data-ttu-id="7d05a-556">`az vm create`: foi adicionado um aviso ao especificar a rede acelerada e um adaptador de rede existente juntos.</span><span class="sxs-lookup"><span data-stu-id="7d05a-556">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="7d05a-557">`az vm create`: foi adicionado `--vmss` para especificar um conjunto de dimensionamento de máquinas virtuais existente ao qual a máquina virtual deve ser atribuída.</span><span class="sxs-lookup"><span data-stu-id="7d05a-557">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="7d05a-558">`az vm/vmss create`: foi adicionada uma cópia local do arquivo de alias de imagem para que ele possa ser acessado em um ambiente de rede restrita.</span><span class="sxs-lookup"><span data-stu-id="7d05a-558">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="7d05a-559">`az vmss create`: foi adicionado `--orchestration-mode` para especificar como as máquinas virtuais são gerenciadas pelo conjunto de dimensionamento.</span><span class="sxs-lookup"><span data-stu-id="7d05a-559">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="7d05a-560">`az vm/vmss update`: foi adicionado `--ultra-ssd-enabled` para permitir a atualização da configuração de SSD Ultra.</span><span class="sxs-lookup"><span data-stu-id="7d05a-560">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="7d05a-561">[ALTERAÇÃO DA FALHA] `az vm extension set`: foi corrigido o bug em que os usuários não podiam definir uma extensão em uma VM com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-561">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="7d05a-562">Foram adicionados os novos comandos `az vm image terms accept/cancel/show` para gerenciar os termos de imagem do Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7d05a-562">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="7d05a-563">O VMAccessForLinux foi atualizado para a versão 1.5</span><span class="sxs-lookup"><span data-stu-id="7d05a-563">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7d05a-564">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7d05a-564">CosmosDB</span></span>

* <span data-ttu-id="7d05a-565">[ALTERAÇÃO DA FALHA] `az sql container create`: `--partition-key-path` foi alterado para parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="7d05a-565">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="7d05a-566">[ALTERAÇÃO DA FALHA] `az gremlin graph create`: `--partition-key-path` foi alterado para parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="7d05a-566">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="7d05a-567">`az sql container create`: Adição de `--unique-key-policy` e `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="7d05a-567">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="7d05a-568">`az sql container create/update`: o esquema padrão `--idx` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="7d05a-568">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="7d05a-569">`gremlin graph create`: Adicionado `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="7d05a-569">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="7d05a-570">`gremlin graph create/update`: o esquema padrão `--idx` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="7d05a-570">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="7d05a-571">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="7d05a-571">Fixed typo in help message</span></span>
* <span data-ttu-id="7d05a-572">banco de dados: Foram adicionadas informações sobre preteridos</span><span class="sxs-lookup"><span data-stu-id="7d05a-572">database: Added deprecation information</span></span>
* <span data-ttu-id="7d05a-573">coleção: Foram adicionadas informações sobre preteridos</span><span class="sxs-lookup"><span data-stu-id="7d05a-573">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="7d05a-574">IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-574">IoT</span></span>

* <span data-ttu-id="7d05a-575">Um novo tipo de fonte de roteamento foi adicionado: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="7d05a-575">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="7d05a-576">Foi corrigido o erro de recursos ausentes no `az iot hub create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-576">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="7d05a-577">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7d05a-577">Key Vault</span></span>

* <span data-ttu-id="7d05a-578">Foi corrigido um erro inesperado quando o arquivo de certificado não existe</span><span class="sxs-lookup"><span data-stu-id="7d05a-578">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="7d05a-579">Foi corrigido o problema em que o `az keyvault recover/purge` não funcionava</span><span class="sxs-lookup"><span data-stu-id="7d05a-579">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="7d05a-580">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="7d05a-580">NetAppFiles</span></span>

* <span data-ttu-id="7d05a-581">O azure-mgmt-netapp foi atualizado para 0.6.0 para usar a versão da API 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="7d05a-581">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="7d05a-582">Essa nova versão da API inclui:</span><span class="sxs-lookup"><span data-stu-id="7d05a-582">This new API version includes:</span></span>

    - <span data-ttu-id="7d05a-583">A criação de volume `--protocol-types` agora aceita "NFSv4.1" não "NFSv4"</span><span class="sxs-lookup"><span data-stu-id="7d05a-583">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="7d05a-584">A propriedade da política de exportação de volume agora é chamada 'nfsv41' não 'nfsv4'</span><span class="sxs-lookup"><span data-stu-id="7d05a-584">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="7d05a-585">O volume `--creation-token` foi renomeado para `--file-path`</span><span class="sxs-lookup"><span data-stu-id="7d05a-585">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="7d05a-586">A data de criação do instantâneo agora é chamada apenas de 'criação'</span><span class="sxs-lookup"><span data-stu-id="7d05a-586">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-587">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-587">Network</span></span>

* <span data-ttu-id="7d05a-588">`az network private-dns link vnet create/update`: suporte à vinculação de rede virtual entre locatários.</span><span class="sxs-lookup"><span data-stu-id="7d05a-588">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="7d05a-589">[ALTERAÇÃO DA FALHA] `az network vnet subnet list`: `--resource-group` e `--vnet-name` foram alterados para serem obrigatórios agora.</span><span class="sxs-lookup"><span data-stu-id="7d05a-589">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="7d05a-590">`az network public-ip prefix create`: Suporte adicionado para especificar a versão do endereço IP (IPv4, IPv6) durante a criação</span><span class="sxs-lookup"><span data-stu-id="7d05a-590">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="7d05a-591">O azure-mgmt-network foi atualizado para 7.0.0 e a api-version para 2019-09-01</span><span class="sxs-lookup"><span data-stu-id="7d05a-591">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="7d05a-592">`az network vrouter`: Suporte adicionado para o novo roteador virtual de serviço e o emparelhamento do roteador virtual</span><span class="sxs-lookup"><span data-stu-id="7d05a-592">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="7d05a-593">`az network express-route gateway connection`: Adicionado o suporte para `--internet-security`</span><span class="sxs-lookup"><span data-stu-id="7d05a-593">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="7d05a-594">Perfil</span><span class="sxs-lookup"><span data-stu-id="7d05a-594">Profile</span></span>

* <span data-ttu-id="7d05a-595">Foi corrigido o problema em que o `az account get-access-token --resource-type ms-graph` não funcionava</span><span class="sxs-lookup"><span data-stu-id="7d05a-595">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="7d05a-596">O aviso foi removido de `az login`</span><span class="sxs-lookup"><span data-stu-id="7d05a-596">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="7d05a-597">RBAC</span><span class="sxs-lookup"><span data-stu-id="7d05a-597">RBAC</span></span>

* <span data-ttu-id="7d05a-598">Foi corrigido o problema em que o `az ad app update --id {} --display-name {}` não funcionava</span><span class="sxs-lookup"><span data-stu-id="7d05a-598">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="7d05a-599">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7d05a-599">ServiceFabric</span></span>

* <span data-ttu-id="7d05a-600">`az sf cluster create`: foi corrigido um problema que ocorria ao modificar o VMSS de computação do template.json do Linux e do Windows, do Service Fabric, de discos Standard para discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="7d05a-600">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-601">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-601">SQL</span></span>

* <span data-ttu-id="7d05a-602">Os parâmetros `--compute-model`, `--auto-pause-delay` e `--min-capacity` foram adicionados para dar suporte a operações CRUD para a nova oferta de Banco de Dados SQL: Modelo de computação sem servidor.</span><span class="sxs-lookup"><span data-stu-id="7d05a-602">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-603">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-603">Storage</span></span>

* <span data-ttu-id="7d05a-604">`az storage account create/update`: Foram adicionados o parâmetro --enable-files-adds e o grupo Argumentos de Propriedades do Azure Active Directory para dar suporte à Autenticação do Serviço de Domínio do Active Directory do Arquivos do Azure</span><span class="sxs-lookup"><span data-stu-id="7d05a-604">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="7d05a-605">O `az storage account keys list/renew` foi expandido para dar suporte à listagem ou à regeneração de chaves Kerberos da conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="7d05a-605">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="7d05a-606">15 de outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-606">October 15, 2019</span></span>

<span data-ttu-id="7d05a-607">Versão 2.0.75</span><span class="sxs-lookup"><span data-stu-id="7d05a-607">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="7d05a-608">AKS</span><span class="sxs-lookup"><span data-stu-id="7d05a-608">AKS</span></span>

* <span data-ttu-id="7d05a-609">Alteração do valor padrão `--load-balancer-sku` para `standard` se for compatível com a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="7d05a-609">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="7d05a-610">Alteração do valor padrão `--vm-set-type` para `virtualmachinescalesets` se for compatível com a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="7d05a-610">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="7d05a-611">AMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-611">AMS</span></span>

* <span data-ttu-id="7d05a-612">[ALTERAÇÃO SIGNIFICATIVA] Alteração do nome de `job start` para `job create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-612">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="7d05a-613">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--ask` de `content-key-policy create` para usar uma cadeia de 32 caracteres hexadecimais em vez do UTF8</span><span class="sxs-lookup"><span data-stu-id="7d05a-613">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-614">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-614">AppService</span></span>

* <span data-ttu-id="7d05a-615">Adição dos comandos `webapp config access-restriction show|set|add|remove`</span><span class="sxs-lookup"><span data-stu-id="7d05a-615">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="7d05a-616">Adição de um melhor tratamento de erro a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="7d05a-616">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="7d05a-617">Adição de suporte do SKU `Isolated` para `appservice plan update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-617">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="7d05a-618">ARM</span><span class="sxs-lookup"><span data-stu-id="7d05a-618">ARM</span></span>

* <span data-ttu-id="7d05a-619">Adição do parâmetro `--handle-extended-json-format``deployment create` para dar suporte a várias linhas e a comentários no modelo json</span><span class="sxs-lookup"><span data-stu-id="7d05a-619">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="7d05a-620">Computação</span><span class="sxs-lookup"><span data-stu-id="7d05a-620">Compute</span></span>

* <span data-ttu-id="7d05a-621">Parâmetro `--enable-agent` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-621">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="7d05a-622">Alteração de `vm create` para usar um SKU de IP público padrão automaticamente ao usar zonas</span><span class="sxs-lookup"><span data-stu-id="7d05a-622">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="7d05a-623">Alteração de `vm create` para criar automaticamente um nome de computador válido para uma VM, caso nenhum tenha sido fornecido</span><span class="sxs-lookup"><span data-stu-id="7d05a-623">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="7d05a-624">Adição do parâmetro `--computer-name-prefix` a `vmss create` para dar suporte ao prefixo de nome de computador personalizado de máquinas virtuais no VMSS</span><span class="sxs-lookup"><span data-stu-id="7d05a-624">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="7d05a-625">Adicione o parâmetro `--workspace` a `vm create` para habilitar o workspace de análise de logs automaticamente</span><span class="sxs-lookup"><span data-stu-id="7d05a-625">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="7d05a-626">Versão de API de galerias atualizadas para 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="7d05a-626">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-627">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-627">Core</span></span>

* <span data-ttu-id="7d05a-628">Adição da verificação de sintaxe para o parâmetro `--set` no comando de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="7d05a-628">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="7d05a-629">IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-629">IoT</span></span>

* <span data-ttu-id="7d05a-630">Correção de um problema em que o `iot hub show` retornaria incorretamente um erro com "recurso não encontrado"</span><span class="sxs-lookup"><span data-stu-id="7d05a-630">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="7d05a-631">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-631">Monitor</span></span>

* <span data-ttu-id="7d05a-632">Adição de suporte para CRUD a `monitor log-analytics workspace`</span><span class="sxs-lookup"><span data-stu-id="7d05a-632">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-633">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-633">Network</span></span>

* <span data-ttu-id="7d05a-634">Adição de suporte para vinculação virtual entre locatários para `network private-dns link vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-634">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="7d05a-635">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `network vnet subnet list` para exigir os parâmetros `--resource-group` e `--vnet-name`</span><span class="sxs-lookup"><span data-stu-id="7d05a-635">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-636">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-636">SQL</span></span>

* <span data-ttu-id="7d05a-637">Adição de comandos a `sql mi ad-admin` que dão suporte à configuração de um administrador do AAD em instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="7d05a-637">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-638">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-638">Storage</span></span>

* <span data-ttu-id="7d05a-639">Adição do parâmetro `--preserve-s2s-access-tier``storage copy` para preservar a camada de acesso durante a cópia do serviço para serviço</span><span class="sxs-lookup"><span data-stu-id="7d05a-639">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="7d05a-640">Adição do parâmetro `--enable-large-file-share` a `storage account [create|update]` para dar suporte a compartilhamentos de arquivos grandes para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-640">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="7d05a-641">24 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-641">September 24, 2019</span></span>

<span data-ttu-id="7d05a-642">Versão 2.0.74</span><span class="sxs-lookup"><span data-stu-id="7d05a-642">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-643">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-643">ACR</span></span>

* <span data-ttu-id="7d05a-644">Inclusão de um parâmetro `--type` obrigatório em `acr config retention update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-644">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="7d05a-645">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro renomeado `--name -n` foi alterado para `--registry -r ` para o grupo de comando `acr config`</span><span class="sxs-lookup"><span data-stu-id="7d05a-645">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="7d05a-646">AKS</span><span class="sxs-lookup"><span data-stu-id="7d05a-646">AKS</span></span>

* <span data-ttu-id="7d05a-647">Inclusão do parâmetro `--load-balancer-sku` no comando `aks create`, o que permite criar um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="7d05a-647">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="7d05a-648">Inclusão dos parâmetros `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` e `--load-balancer-outbound-ip-prefixes` nos comandos `aks [create|update]`, o que permite atualizar o perfil do balanceador de carga de um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="7d05a-648">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="7d05a-649">Inclusão do parâmetro `--vm-set-type` no comando `aks create`, o que permite especificar os tipos de VM de um cluster do AKS (vmas ou vmss)</span><span class="sxs-lookup"><span data-stu-id="7d05a-649">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="7d05a-650">ARM</span><span class="sxs-lookup"><span data-stu-id="7d05a-650">ARM</span></span>

* <span data-ttu-id="7d05a-651">Inclusão do parâmetro `--handle-extended-json-format` no comando `group deployment create` para compatibilidade com várias linhas e comentários no modelo JSON</span><span class="sxs-lookup"><span data-stu-id="7d05a-651">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="7d05a-652">Computação</span><span class="sxs-lookup"><span data-stu-id="7d05a-652">Compute</span></span>

* <span data-ttu-id="7d05a-653">Inclusão do parâmetro `--terminate-notification-time` nos comandos `vmss [create|update]` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="7d05a-653">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="7d05a-654">Inclusão do parâmetro `--enable-terminate-notification` no comando `vmss update` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="7d05a-654">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="7d05a-655">Inclusão dos parâmetros `--priority,`, `--eviction-policy,` e `--max-billing` nos comandos `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-655">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="7d05a-656">Alteração de `disk create` para permitir a especificação do tamanho exato do carregamento de disco</span><span class="sxs-lookup"><span data-stu-id="7d05a-656">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="7d05a-657">Inclusão de compatibilidade com instantâneos incrementais para discos gerenciados para `snapshot create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-657">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="7d05a-658">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7d05a-658">Cosmos DB</span></span>

* <span data-ttu-id="7d05a-659">Inclusão do parâmetro `--type <key-type>` no comando `cosmosdb keys list` para mostrar a chave, as chaves somente leitura ou cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="7d05a-659">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="7d05a-660">Adicionado o comando `cosmosdb keys regenerate`</span><span class="sxs-lookup"><span data-stu-id="7d05a-660">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="7d05a-661">[PRETERIDO] Comandos `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` e `cosmosdb list-read-only-keys` preteridos</span><span class="sxs-lookup"><span data-stu-id="7d05a-661">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="7d05a-662">EventGrid</span><span class="sxs-lookup"><span data-stu-id="7d05a-662">EventGrid</span></span>

* <span data-ttu-id="7d05a-663">Correção do texto de ajuda do ponto de extremidade para fazer referência ao parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="7d05a-663">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="7d05a-664">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7d05a-664">Key Vault</span></span>

* <span data-ttu-id="7d05a-665">Correção do problema em que fazer logon com um locatário (`login -t`) poderia causar uma falha no `keyvault create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-665">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="7d05a-666">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-666">Monitor</span></span>

* <span data-ttu-id="7d05a-667">Correção do problema em que o caractere `:` não era permitido no argumento `--condition` para `monitor metrics alert create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-667">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="7d05a-668">Política</span><span class="sxs-lookup"><span data-stu-id="7d05a-668">Policy</span></span>

* <span data-ttu-id="7d05a-669">Inclusão de compatibilidade com a API de Política, versão de 01/06/2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-669">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="7d05a-670">Inclusão do parâmetro `--enforcement-mode` no comando `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-670">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-671">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-671">Storage</span></span>

* <span data-ttu-id="7d05a-672">Inclusão do parâmetro `--blob-type` no comando `az storage copy`</span><span class="sxs-lookup"><span data-stu-id="7d05a-672">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="7d05a-673">10 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-673">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-674">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-674">ACR</span></span>

* <span data-ttu-id="7d05a-675">Adição do grupo de comandos `acr config retention` para configurar a política de retenção</span><span class="sxs-lookup"><span data-stu-id="7d05a-675">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="7d05a-676">AKS</span><span class="sxs-lookup"><span data-stu-id="7d05a-676">AKS</span></span>

* <span data-ttu-id="7d05a-677">Adição de suporte para integração do ACR com os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="7d05a-677">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="7d05a-678">Adição do parâmetro `--attach-acr` a `aks [create|update]` para anexar um ACR a um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="7d05a-678">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="7d05a-679">Adição do parâmetro `--detach-acr` a `aks update` para desanexar o ACR de um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="7d05a-679">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="7d05a-680">ARM</span><span class="sxs-lookup"><span data-stu-id="7d05a-680">ARM</span></span>

* <span data-ttu-id="7d05a-681">Atualização para uso da versão de API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="7d05a-681">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="7d05a-682">Lote</span><span class="sxs-lookup"><span data-stu-id="7d05a-682">Batch</span></span>

* <span data-ttu-id="7d05a-683">Adição de novas definições de configuração JSON de `--json-file` para `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="7d05a-683">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="7d05a-684">Adição de `MountConfigurations` para montagens do sistema de arquivos (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="7d05a-684">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="7d05a-685">Adição da propriedade opcional `publicIPs` a `NetworkConfiguration` para IPs públicos em pools (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="7d05a-685">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="7d05a-686">Adição de suporte para galerias de imagens compartilhadas a `--image`</span><span class="sxs-lookup"><span data-stu-id="7d05a-686">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="7d05a-687">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `--start-task-wait-for-success` em `batch pool create` para `true`</span><span class="sxs-lookup"><span data-stu-id="7d05a-687">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="7d05a-688">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `Scope` em `AutoUserSpecification` para sempre ser Pool (anteriormente, `Task` em nós do Windows e `Pool` em nós do Linux)</span><span class="sxs-lookup"><span data-stu-id="7d05a-688">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="7d05a-689">Esse argumento só pode ser definido em uma configuração JSON com `--json-file`</span><span class="sxs-lookup"><span data-stu-id="7d05a-689">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7d05a-690">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7d05a-690">HDInsight</span></span>

* <span data-ttu-id="7d05a-691">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="7d05a-691">GA release</span></span>
* <span data-ttu-id="7d05a-692">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--workernode-count/-c` de `az hdinsight resize` para ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d05a-692">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="7d05a-693">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7d05a-693">Key Vault</span></span>

* <span data-ttu-id="7d05a-694">Correção do problema em que as sub-redes não podiam ser excluídas das regras da rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-694">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="7d05a-695">Correção do problema em que sub-redes e endereços IP duplicados podiam ser adicionados às regras da rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-695">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-696">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-696">Network</span></span>

* <span data-ttu-id="7d05a-697">Adição do parâmetro `--interval` a `network watcher flow-log` para definir o valor do intervalo de análise de tráfego</span><span class="sxs-lookup"><span data-stu-id="7d05a-697">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="7d05a-698">Adição de `network application-gateway identity` para gerenciar a identidade do gateway</span><span class="sxs-lookup"><span data-stu-id="7d05a-698">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="7d05a-699">Adição de suporte para definir a ID do Key Vault como `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="7d05a-699">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="7d05a-700">Adicionado `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-700">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="7d05a-701">Política</span><span class="sxs-lookup"><span data-stu-id="7d05a-701">Policy</span></span>

* <span data-ttu-id="7d05a-702">Atualização para uso da versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="7d05a-702">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="7d05a-703">27 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-703">August 27, 2019</span></span>

<span data-ttu-id="7d05a-704">Versão 2.0.72</span><span class="sxs-lookup"><span data-stu-id="7d05a-704">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-705">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-705">ACR</span></span>

* <span data-ttu-id="7d05a-706">[ALTERAÇÃO SIGNIFICATIVA] Remoção da compatibilidade com o SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="7d05a-706">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="7d05a-707">Gerenciamento de API</span><span class="sxs-lookup"><span data-stu-id="7d05a-707">API Management</span></span>

* <span data-ttu-id="7d05a-708">[VERSÃO PRÉVIA] Adição do grupo de comandos `apim`</span><span class="sxs-lookup"><span data-stu-id="7d05a-708">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-709">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-709">AppService</span></span>

* <span data-ttu-id="7d05a-710">Correção do problema com o comando `webapp webjob continuous start` ao especificar um slot</span><span class="sxs-lookup"><span data-stu-id="7d05a-710">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="7d05a-711">Alteração de `webapp up` para detectar a pasta `env` e removê-la do arquivo usado para implantação</span><span class="sxs-lookup"><span data-stu-id="7d05a-711">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="7d05a-712">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7d05a-712">Keyvault</span></span>

* <span data-ttu-id="7d05a-713">Correção de um bug no `keyvault secret set` que ignorava o argumento `--expires`</span><span class="sxs-lookup"><span data-stu-id="7d05a-713">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-714">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-714">Network</span></span>

* <span data-ttu-id="7d05a-715">Adição de suporte para endereços IPv6 a argumentos `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="7d05a-715">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="7d05a-716">Adição de novos comandos `network private-endpoint [create|update|list-types]` para o gerenciamento de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="7d05a-716">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="7d05a-717">Adição do grupo de comandos `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="7d05a-717">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="7d05a-718">Adicionados os argumentos `--private-endpoint-network-policies` e `--private-link-service-network-policies` para `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-718">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="7d05a-719">RBAC</span><span class="sxs-lookup"><span data-stu-id="7d05a-719">RBAC</span></span>

* <span data-ttu-id="7d05a-720">Correção de um problema com `ad app update --homepage` em que a página inicial não era atualizada</span><span class="sxs-lookup"><span data-stu-id="7d05a-720">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="7d05a-721">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7d05a-721">ServiceFabric</span></span>

* <span data-ttu-id="7d05a-722">Adição de suporte para nomes de Key Vault grafados com maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="7d05a-722">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="7d05a-723">Correção de um problema ao usar certificados no Key Vault</span><span class="sxs-lookup"><span data-stu-id="7d05a-723">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="7d05a-724">Correção de um problema com o uso de arquivos de certificado PFX</span><span class="sxs-lookup"><span data-stu-id="7d05a-724">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="7d05a-725">Correção de um problema com `sf cluster certificate add` quando o grupo de recursos do Key Vault não era especificado</span><span class="sxs-lookup"><span data-stu-id="7d05a-725">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="7d05a-726">Correção de um problema em que `sf cluster set` não funcionava</span><span class="sxs-lookup"><span data-stu-id="7d05a-726">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="7d05a-727">SignalR</span><span class="sxs-lookup"><span data-stu-id="7d05a-727">SignalR</span></span>

* <span data-ttu-id="7d05a-728">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="7d05a-728">Added new commands:</span></span>
  * <span data-ttu-id="7d05a-729">`signalr cors`: gerenciar CORS do SignalR</span><span class="sxs-lookup"><span data-stu-id="7d05a-729">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="7d05a-730">`signalr restart`: reiniciar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="7d05a-730">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="7d05a-731">`signalr update`: atualizar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="7d05a-731">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="7d05a-732">Adicionado o argumento `--service-mode` para `signalr create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-732">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-733">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-733">Storage</span></span>

* <span data-ttu-id="7d05a-734">Adicionado o comando `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="7d05a-734">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="7d05a-735">13 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-735">August 13, 2019</span></span>

<span data-ttu-id="7d05a-736">Versão 2.0.71</span><span class="sxs-lookup"><span data-stu-id="7d05a-736">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-737">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-737">AppService</span></span>

* <span data-ttu-id="7d05a-738">Um problema de falha de slots com os comandos `webapp webjob continuous` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="7d05a-738">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="7d05a-739">BotService</span><span class="sxs-lookup"><span data-stu-id="7d05a-739">BotService</span></span>

* <span data-ttu-id="7d05a-740">[ALTERAÇÃO SIGNIFICATIVA] O suporte para a criação de bots SDK v3 foi removido</span><span class="sxs-lookup"><span data-stu-id="7d05a-740">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="7d05a-741">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="7d05a-741">CognitiveServices</span></span>

* <span data-ttu-id="7d05a-742">Adicionados os comandos `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="7d05a-742">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="7d05a-743">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7d05a-743">Cosmos DB</span></span>

* <span data-ttu-id="7d05a-744">Removido o aviso ao atualizar vários locais de gravação</span><span class="sxs-lookup"><span data-stu-id="7d05a-744">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="7d05a-745">Foram adicionados os comandos CRUD para o CosmosDB SQL, MongoDB, Cassandra, Gremlin e Recursos de tabela e taxa de transferência do recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-745">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7d05a-746">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7d05a-746">HDInsight</span></span>

<span data-ttu-id="7d05a-747">Esta versão contém um grande número de alterações da falha.</span><span class="sxs-lookup"><span data-stu-id="7d05a-747">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="7d05a-748">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="7d05a-748">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="7d05a-749">`--storage-default-container` renomeado para `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="7d05a-749">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="7d05a-750">`--storage-default-filesystem` renomeado para `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="7d05a-750">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="7d05a-751">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--name` de `application create` foi alterado para representar o nome do aplicativo em vez do nome do cluster</span><span class="sxs-lookup"><span data-stu-id="7d05a-751">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="7d05a-752">O argumento `--cluster-name` foi adicionado a `application create` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="7d05a-752">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="7d05a-753">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `application create`:</span><span class="sxs-lookup"><span data-stu-id="7d05a-753">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="7d05a-754">`--application-type` renomeado para `--type`</span><span class="sxs-lookup"><span data-stu-id="7d05a-754">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="7d05a-755">`--marketplace-identifier` renomeado para `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="7d05a-755">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="7d05a-756">`--https-endpoint-access-mode` renomeado para `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="7d05a-756">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="7d05a-757">Renomeado de `--https-endpoint-destination-port` para `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="7d05a-757">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="7d05a-758">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros removidos para `application create`:</span><span class="sxs-lookup"><span data-stu-id="7d05a-758">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="7d05a-759">[ALTERAÇÃO DA FALHA] Renomeado de `--target-instance-count` para `--workernode-count` para `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="7d05a-759">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="7d05a-760">[ALTERAÇÃO SIGNIFICATIVA] Todos os comandos no grupo `hdinsight script-action` foram alterados para usar o parâmetro `--name` como o nome da ação de script.</span><span class="sxs-lookup"><span data-stu-id="7d05a-760">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="7d05a-761">O argumento `--cluster-name` foi adicionado a todos os comandos `hdinsight script-action` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="7d05a-761">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="7d05a-762">[ALTERAÇÃO SIGNIFICATIVA] Renomeado de `--script-execution-id` para `--execution-id` para todos os comandos `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="7d05a-762">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="7d05a-763">[ALTERAÇÃO SIGNIFICATIVA]`hdinsight script-action show` renomeado para `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="7d05a-763">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="7d05a-764">[ALTERAÇÃO DA FALHA] Os parâmetros foram alterados para `hdinsight script-action execute --roles` para serem separados por espaços em vez de separados por vírgula</span><span class="sxs-lookup"><span data-stu-id="7d05a-764">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="7d05a-765">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro `--persisted` de `hdinsight script-action list` foi removido</span><span class="sxs-lookup"><span data-stu-id="7d05a-765">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="7d05a-766">O parâmetro `hdinsight create --cluster-configurations` foi alterado para aceitar um caminho para um arquivo JSON local ou uma cadeia de caracteres JSON</span><span class="sxs-lookup"><span data-stu-id="7d05a-766">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="7d05a-767">Adicionado o comando `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="7d05a-767">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="7d05a-768">Alterado `hdinsight monitor enable --workspace` para aceitar uma ID do workspace ou nome do workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="7d05a-768">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="7d05a-769">O argumento `hdinsight monitor enable --primary-key`, que será necessário caso uma ID do workspace seja fornecida como o parâmetro, foi adicionado</span><span class="sxs-lookup"><span data-stu-id="7d05a-769">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="7d05a-770">Foram adicionados mais exemplos e atualização das descrições das mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="7d05a-770">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="7d05a-771">Interativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-771">Interactive</span></span>

* <span data-ttu-id="7d05a-772">Um erro no carregamento foi corrigido</span><span class="sxs-lookup"><span data-stu-id="7d05a-772">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="7d05a-773">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="7d05a-773">Kubernetes</span></span>

* <span data-ttu-id="7d05a-774">Alterado para usar `https` se a porta do contêiner do painel estiver usando `https`</span><span class="sxs-lookup"><span data-stu-id="7d05a-774">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-775">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-775">Network</span></span>

* <span data-ttu-id="7d05a-776">O argumento `--yes` foi adicionado a `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="7d05a-776">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="7d05a-777">Perfil</span><span class="sxs-lookup"><span data-stu-id="7d05a-777">Profile</span></span>

* <span data-ttu-id="7d05a-778">O argumento `--resource-type` foi adicionado a `account get-access-token` para obter tokens de acesso de recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-778">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="7d05a-779">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7d05a-779">ServiceFabric</span></span>

* <span data-ttu-id="7d05a-780">Todas as versões de sistema operacional com suporte para criação do cluster sf foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="7d05a-780">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="7d05a-781">Foi corrigido o bug de validação do certificado primário</span><span class="sxs-lookup"><span data-stu-id="7d05a-781">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-782">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-782">Storage</span></span>

* <span data-ttu-id="7d05a-783">Adicionado o comando `storage copy`</span><span class="sxs-lookup"><span data-stu-id="7d05a-783">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="7d05a-784">30 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-784">July 30, 2019</span></span>

<span data-ttu-id="7d05a-785">Versão 2.0.70</span><span class="sxs-lookup"><span data-stu-id="7d05a-785">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-786">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-786">ACR</span></span>

* <span data-ttu-id="7d05a-787">Corrigido o problema #9952 (uma regressão no comando `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="7d05a-787">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="7d05a-788">Removido o nome da imagem do construtor padrão em `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="7d05a-788">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-789">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-789">Appservice</span></span>

* <span data-ttu-id="7d05a-790">Alterado `webapp config ssl` para mostrar uma mensagem se um recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="7d05a-790">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="7d05a-791">Corrigido o problema em que `functionapp create` não aceita o tipo de conta de armazenamento `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="7d05a-791">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="7d05a-792">Corrigido um problema em que `webapp up` falharia se fosse executado usando versões mais antigas do Python</span><span class="sxs-lookup"><span data-stu-id="7d05a-792">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-793">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-793">Network</span></span>

* <span data-ttu-id="7d05a-794">Removido parâmetro inválido `--ids` de `network nic ip-config add` (corrige o #9861)</span><span class="sxs-lookup"><span data-stu-id="7d05a-794">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="7d05a-795">Corrige o #9604.</span><span class="sxs-lookup"><span data-stu-id="7d05a-795">Fixes #9604.</span></span> <span data-ttu-id="7d05a-796">Adicionado o parâmetro `--root-certs` ao `network application-gateway http-settings [create|update]` para dar suporte a certificados raiz confiáveis associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="7d05a-796">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="7d05a-797">Fixado argumento `--subscription` para `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="7d05a-797">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="7d05a-798">RBAC</span><span class="sxs-lookup"><span data-stu-id="7d05a-798">RBAC</span></span>

* <span data-ttu-id="7d05a-799">Adicionado o comando `user update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-799">Added `user update` command</span></span>
* <span data-ttu-id="7d05a-800">[PRETERIDO] Preterido `--upn-or-object-id` de comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="7d05a-800">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="7d05a-801">Usar argumento de substituição `--id`</span><span class="sxs-lookup"><span data-stu-id="7d05a-801">Use replacement argument `--id`</span></span>
* <span data-ttu-id="7d05a-802">Adicionado argumento `--id` para comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="7d05a-802">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-803">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-803">SQL</span></span>

* <span data-ttu-id="7d05a-804">Adicionados comandos de gerenciamento para chaves de instância gerenciada e protetor de TDE</span><span class="sxs-lookup"><span data-stu-id="7d05a-804">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-805">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-805">Storage</span></span>

* <span data-ttu-id="7d05a-806">Adicionado o comando `storage remove`</span><span class="sxs-lookup"><span data-stu-id="7d05a-806">Added `storage remove` command</span></span>
* <span data-ttu-id="7d05a-807">Corrigido um problema com `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-807">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-808">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-808">VM</span></span>

* <span data-ttu-id="7d05a-809">Alterado `list-skus` para usar versão de API mais recente a fim de externar detalhes de zona</span><span class="sxs-lookup"><span data-stu-id="7d05a-809">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="7d05a-810">Alterado o padrão de `--single-placement-group` para `false` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-810">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="7d05a-811">Adicionada a capacidade de selecionar SKUs de armazenamento ZRS para `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-811">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="7d05a-812">Adicionado novo grupo de comandos `vm host` para dar suporte a hosts dedicados</span><span class="sxs-lookup"><span data-stu-id="7d05a-812">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="7d05a-813">Adicionados parâmetros `--host` e `--host-group` em `vm create` para definir o host dedicado da VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-813">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="7d05a-814">16 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-814">July 16, 2019</span></span>

<span data-ttu-id="7d05a-815">Versão 2.0.69</span><span class="sxs-lookup"><span data-stu-id="7d05a-815">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-816">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-816">Appservice</span></span>

* <span data-ttu-id="7d05a-817">Os comandos `webapp identity` foram alterados para retornar uma mensagem de erro apropriada se o nome do aplicativo ou ResourceGroupName for inválido</span><span class="sxs-lookup"><span data-stu-id="7d05a-817">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="7d05a-818">`webapp list` corrigido para retornar o valor correto para numberOfSites se nenhum ResourceGroup foi fornecido</span><span class="sxs-lookup"><span data-stu-id="7d05a-818">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="7d05a-819">Corrigidos os efeitos colaterais de `appservice plan create` e `webapp create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-819">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-820">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-820">Core</span></span>

* <span data-ttu-id="7d05a-821">Corrigido um problema em que `--subscription` aparecia apesar de não ser aplicável</span><span class="sxs-lookup"><span data-stu-id="7d05a-821">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="7d05a-822">Lote</span><span class="sxs-lookup"><span data-stu-id="7d05a-822">Batch</span></span>

* <span data-ttu-id="7d05a-823">[ALTERAÇÃO SIGNIFICATIVA]`batch pool node-agent-skus list` foi substituído por `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="7d05a-823">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="7d05a-824">Adicionado suporte para regras de segurança bloqueando o acesso de rede a um pool com base na porta de origem do tráfego ao usar a opção `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="7d05a-824">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="7d05a-825">Suporte adicionado para executar a tarefa no diretório de trabalho de contêiner ou no diretório de trabalho de tarefa em lotes ao usar a opção `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-825">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="7d05a-826">Corrigido o erro na opção `--application-package-references` de `batch pool create` em que ela funcionaria apenas com padrões</span><span class="sxs-lookup"><span data-stu-id="7d05a-826">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="7d05a-827">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="7d05a-827">Eventhubs</span></span>

* <span data-ttu-id="7d05a-828">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="7d05a-828">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="7d05a-829">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-829">RDBMS</span></span>

* <span data-ttu-id="7d05a-830">Adicionado um parâmetro opcional para especificar a réplica de SKU para criar o comando de réplica</span><span class="sxs-lookup"><span data-stu-id="7d05a-830">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="7d05a-831">Corrigido o problema com a falha no teste de CI com a criação de réplica de MySQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-831">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="7d05a-832">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="7d05a-832">Relay</span></span>

* <span data-ttu-id="7d05a-833">Corrigido o problema com a conexão híbrida quando a autorização do cliente desabilitava [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="7d05a-833">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="7d05a-834">Parâmetro `--requires-transport-security` adicionado a `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-834">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="7d05a-835">Barramento de serviço</span><span class="sxs-lookup"><span data-stu-id="7d05a-835">Servicebus</span></span>

* <span data-ttu-id="7d05a-836">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="7d05a-836">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-837">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-837">Storage</span></span>

* <span data-ttu-id="7d05a-838">Habilitar AADDS de arquivos para atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-838">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="7d05a-839">Problema corrigido `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="7d05a-839">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="7d05a-840">2 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-840">July 2, 2019</span></span>

<span data-ttu-id="7d05a-841">Versão 2.0.68</span><span class="sxs-lookup"><span data-stu-id="7d05a-841">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-842">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-842">Core</span></span>

* <span data-ttu-id="7d05a-843">Agora, os módulos de comando são consolidados em um único Python distribuível.</span><span class="sxs-lookup"><span data-stu-id="7d05a-843">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="7d05a-844">Isso substitui o uso direto de muitos pacotes `azure-cli-` no PyPI.</span><span class="sxs-lookup"><span data-stu-id="7d05a-844">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="7d05a-845">Assim, o tamanho da instalação será reduzido e apenas os usuários que tiverem instalado diretamente por meio do `pip` serão afetados.</span><span class="sxs-lookup"><span data-stu-id="7d05a-845">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-846">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-846">ACR</span></span>

* <span data-ttu-id="7d05a-847">Foi adicionado o suporte para gatilhos de temporizador para tarefa</span><span class="sxs-lookup"><span data-stu-id="7d05a-847">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-848">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-848">Appservice</span></span>

* <span data-ttu-id="7d05a-849">O `functionapp create` foi alterado para habilitar o Application Insights por padrão</span><span class="sxs-lookup"><span data-stu-id="7d05a-849">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="7d05a-850">[ALTERAÇÃO SIGNIFICATIVA] Foi removido o comando `functionapp devops-build` preterido.</span><span class="sxs-lookup"><span data-stu-id="7d05a-850">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="7d05a-851">Agora, use o novo comando `az functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="7d05a-851">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="7d05a-852">Foi adicionado o suporte ao plano de aplicativo de funções Consumo em Linux ao `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="7d05a-852">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="7d05a-853">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7d05a-853">Cosmos DB</span></span>

* <span data-ttu-id="7d05a-854">Foi adicionado o suporte para desabilitar a TTL</span><span class="sxs-lookup"><span data-stu-id="7d05a-854">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="7d05a-855">DLS</span><span class="sxs-lookup"><span data-stu-id="7d05a-855">DLS</span></span>

* <span data-ttu-id="7d05a-856">Versão atualizada do ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="7d05a-856">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="7d05a-857">Comentários</span><span class="sxs-lookup"><span data-stu-id="7d05a-857">Feedback</span></span>

* <span data-ttu-id="7d05a-858">Ao relatar um comando de extensão com falha, agora, o `az feedback` tenta abrir o navegador na URL do projeto/repositório da extensão por meio do índice</span><span class="sxs-lookup"><span data-stu-id="7d05a-858">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7d05a-859">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7d05a-859">HDInsight</span></span>

* <span data-ttu-id="7d05a-860">[ALTERAÇÃO SIGNIFICATIVA] O nome do grupo de comandos `oms` foi alterado para `monitor`</span><span class="sxs-lookup"><span data-stu-id="7d05a-860">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="7d05a-861">[ALTERAÇÃO SIGNIFICATIVA]`--http-password/-p` tornou-se um parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="7d05a-861">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="7d05a-862">Foram adicionados preenchedores para o preenchedor dos parâmetros `--cluster-admin-account` e `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="7d05a-862">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="7d05a-863">O parâmetro `cluster-users-group-dns` foi alterado para ser obrigatório quando `—esp` estiver presente</span><span class="sxs-lookup"><span data-stu-id="7d05a-863">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="7d05a-864">Foi adicionado um tempo limite para todos os preenchedores automáticos de argumento existentes</span><span class="sxs-lookup"><span data-stu-id="7d05a-864">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="7d05a-865">Foi adicionado um tempo limite para transformar o nome do recurso na ID de recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-865">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="7d05a-866">Os preenchedores automáticos foram alterados para selecionar recursos de qualquer grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="7d05a-866">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="7d05a-867">Pode ser um grupo de recursos diferente daquele especificado com `-g`</span><span class="sxs-lookup"><span data-stu-id="7d05a-867">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="7d05a-868">Foi adicionado o suporte para os parâmetros `--sub-domain-suffix` e `--disable_gateway_auth` no comando `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-868">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="7d05a-869">Serviços gerenciados</span><span class="sxs-lookup"><span data-stu-id="7d05a-869">Managed Services</span></span>

* <span data-ttu-id="7d05a-870">Introdução ao módulo de comando de serviço gerenciado em versão prévia</span><span class="sxs-lookup"><span data-stu-id="7d05a-870">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="7d05a-871">Perfil</span><span class="sxs-lookup"><span data-stu-id="7d05a-871">Profile</span></span>
* <span data-ttu-id="7d05a-872">Suprimir o argumento `--subscription` para o comando de logoff</span><span class="sxs-lookup"><span data-stu-id="7d05a-872">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="7d05a-873">RBAC</span><span class="sxs-lookup"><span data-stu-id="7d05a-873">RBAC</span></span>

* <span data-ttu-id="7d05a-874">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--password` foi removido de `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="7d05a-874">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="7d05a-875">Foi adicionado o parâmetro `--assignee-principal-type` ao comando `create` para evitar falhas intermitentes causadas pela latência de replicação do servidor do AAD Graph</span><span class="sxs-lookup"><span data-stu-id="7d05a-875">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="7d05a-876">Foi corrigida uma falha em `ad signed-in-user` ao listar objetos de propriedade</span><span class="sxs-lookup"><span data-stu-id="7d05a-876">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="7d05a-877">Foi corrigido um problema em que o `ad sp` não localizava o aplicativo certo de uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="7d05a-877">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="7d05a-878">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-878">RDBMS</span></span>

* <span data-ttu-id="7d05a-879">Foi adicionado o suporte à replicação para o MariaDB</span><span class="sxs-lookup"><span data-stu-id="7d05a-879">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-880">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-880">SQL</span></span>

* <span data-ttu-id="7d05a-881">Valores permitidos documentados para `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="7d05a-881">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-882">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-882">Storage</span></span>

* <span data-ttu-id="7d05a-883">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="7d05a-883">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="7d05a-884">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="7d05a-884">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="7d05a-885">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-885">VM</span></span>

* <span data-ttu-id="7d05a-886">Foi corrigido o bug em que o `vmss create` retornava uma mensagem de erro quando era executado com `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="7d05a-886">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="7d05a-887">Foi removida a validação do lado do cliente de `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-887">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="7d05a-888">Não falha quando `--single-placement-group` é definido como `true` e `--instance-count` é maior que 100 ou quando são especificadas zonas de disponibilidade, mas deixa essa validação para o serviço de computação</span><span class="sxs-lookup"><span data-stu-id="7d05a-888">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="7d05a-889">Foi corrigido o bug em que o `[vm|vmss] extension image list` falhava quando era usado com `--latest`</span><span class="sxs-lookup"><span data-stu-id="7d05a-889">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="7d05a-890">18 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-890">June 18, 2019</span></span>

<span data-ttu-id="7d05a-891">Versão 2.0.67</span><span class="sxs-lookup"><span data-stu-id="7d05a-891">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-892">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-892">Core</span></span>

<span data-ttu-id="7d05a-893">Esta versão apresenta uma nova marca [Versão prévia] para comunicar com mais clareza aos clientes quando um comando, um grupo de comandos ou um argumento está no status de versão prévia.</span><span class="sxs-lookup"><span data-stu-id="7d05a-893">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="7d05a-894">Anteriormente, essa informação era transmitida no texto de ajuda ou, implicitamente, pelo número da versão do módulo de comando.</span><span class="sxs-lookup"><span data-stu-id="7d05a-894">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="7d05a-895">A CLI removerá os números de versão dos pacotes individuais no futuro.</span><span class="sxs-lookup"><span data-stu-id="7d05a-895">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="7d05a-896">Se um comando estiver em versão prévia, todos os seus argumentos também estarão.</span><span class="sxs-lookup"><span data-stu-id="7d05a-896">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="7d05a-897">Se um grupo de comandos for rotulado com o status de versão prévia, então todos os seus comandos e argumentos também serão considerados em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="7d05a-897">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="7d05a-898">Como resultado dessa alteração, diversos grupos de comandos podem parecer surgir "de repente" com o status de versão prévia com esta liberação.</span><span class="sxs-lookup"><span data-stu-id="7d05a-898">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="7d05a-899">O que realmente aconteceu é que a maioria dos pacotes já estava com status de versão prévia, mas estão sendo consideradas GA com esta liberação</span><span class="sxs-lookup"><span data-stu-id="7d05a-899">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-900">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-900">ACR</span></span>
* <span data-ttu-id="7d05a-901">Adicionado o comando 'acr check-health'</span><span class="sxs-lookup"><span data-stu-id="7d05a-901">Added 'acr check-health' command</span></span>
* <span data-ttu-id="7d05a-902">Melhorado o tratamento de erro para tokens do AAD e para recuperar comandos externos</span><span class="sxs-lookup"><span data-stu-id="7d05a-902">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-903">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-903">ACS</span></span>
* <span data-ttu-id="7d05a-904">Comandos preteridos do ACS agora ficam ocultos da exibição da ajuda</span><span class="sxs-lookup"><span data-stu-id="7d05a-904">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="7d05a-905">AMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-905">AMS</span></span>
* <span data-ttu-id="7d05a-906">[ALTERAÇÃO SIGNIFICATIVA] Alterada para retornar cadeias de caracteres de tempo da ISO 8601 para archive-window-length e key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="7d05a-906">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-907">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-907">AppService</span></span>
* <span data-ttu-id="7d05a-908">Adicionado roteamento com base no local para `webapp deleted list` e `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="7d05a-908">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="7d05a-909">Corrigido problema em que a URL de destino registrada do webapp ("Não é possível iniciar o aplicativo em...") não era clicável no Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="7d05a-909">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="7d05a-910">Corrigido um problema em que a criação de aplicativos com algumas SKUs falhava com um erro de AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="7d05a-910">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="7d05a-911">Adicionada a pré-validação para o `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-911">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="7d05a-912">Corrigido o `[webapp|functionapp] traffic-routing` para usar o actionHostName correto</span><span class="sxs-lookup"><span data-stu-id="7d05a-912">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="7d05a-913">Adicionado o suporte de slot para comandos `functionapp`</span><span class="sxs-lookup"><span data-stu-id="7d05a-913">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="7d05a-914">Lote</span><span class="sxs-lookup"><span data-stu-id="7d05a-914">Batch</span></span>
* <span data-ttu-id="7d05a-915">Corrigida a regressão de autenticação do AAD causada pela geração de relatórios de erros superagressiva para autenticação de chave compartilhada</span><span class="sxs-lookup"><span data-stu-id="7d05a-915">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="7d05a-916">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7d05a-916">BatchAI</span></span>
* <span data-ttu-id="7d05a-917">Agora os comandos do BatchAI estão preteridos e ocultos</span><span class="sxs-lookup"><span data-stu-id="7d05a-917">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="7d05a-918">BotService</span><span class="sxs-lookup"><span data-stu-id="7d05a-918">BotService</span></span>
* <span data-ttu-id="7d05a-919">Adição das mensagens de aviso "suporte descontinuado"/"modo de manutenção" para os comandos compatíveis com a v3 do SDK</span><span class="sxs-lookup"><span data-stu-id="7d05a-919">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7d05a-920">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7d05a-920">CosmosDB</span></span>
* <span data-ttu-id="7d05a-921">[PRETERIDO] Preterido o comando `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="7d05a-921">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="7d05a-922">Adicionado o comando `cosmosdb keys list` – substitui o `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="7d05a-922">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="7d05a-923">`cosmsodb create/update`: Adicionado novo formato para --location a fim de permitir a configuração da propriedade "isZoneRedundant".</span><span class="sxs-lookup"><span data-stu-id="7d05a-923">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="7d05a-924">Formato antigo preterido</span><span class="sxs-lookup"><span data-stu-id="7d05a-924">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="7d05a-925">EventGrid</span><span class="sxs-lookup"><span data-stu-id="7d05a-925">EventGrid</span></span>
* <span data-ttu-id="7d05a-926">Adicionados comandos do `eventgrid domain` para operações de CRUD no domínio</span><span class="sxs-lookup"><span data-stu-id="7d05a-926">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="7d05a-927">Adicionados comandos do `eventgrid domain topic` para operações de CRUD nos tópicos do domínio</span><span class="sxs-lookup"><span data-stu-id="7d05a-927">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="7d05a-928">Adicionado argumento do `--odata-query` ao `eventgrid [topic|event-subscription] list` para filtrar os resultados usando a sintaxe do OData</span><span class="sxs-lookup"><span data-stu-id="7d05a-928">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="7d05a-929">`event-subscription create/update`: Adicionado o servicebusqueue como novos valores para o parâmetro `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="7d05a-929">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="7d05a-930">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para `--included-event-types All` com `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-930">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7d05a-931">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7d05a-931">HDInsight</span></span>
* <span data-ttu-id="7d05a-932">Adicionado suporte para o parâmetro `--ssh-public-key` no comando `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-932">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="7d05a-933">IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-933">IoT</span></span>
* <span data-ttu-id="7d05a-934">Adicionado suporte para regenerar as chaves da política de autorização</span><span class="sxs-lookup"><span data-stu-id="7d05a-934">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="7d05a-935">Adicionados SDK e suporte para o serviço de provisionamento de repositórios do DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="7d05a-935">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-936">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-936">Network</span></span>
* <span data-ttu-id="7d05a-937">Adicionado suporte de zona para o Gateway da NAT</span><span class="sxs-lookup"><span data-stu-id="7d05a-937">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="7d05a-938">Adicionado o comando `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="7d05a-938">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="7d05a-939">Corrigido o problema com o `dns zone import` em que os usuários não conseguiam importar registros do curinga A</span><span class="sxs-lookup"><span data-stu-id="7d05a-939">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="7d05a-940">Corrigido o problema com o `watcher flow-log configure` em que o registro de fluxo não podia ser habilitado em determinadas regiões</span><span class="sxs-lookup"><span data-stu-id="7d05a-940">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-941">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-941">Resource</span></span>
* <span data-ttu-id="7d05a-942">Adicionado o comando do `az rest` para fazer chamadas REST</span><span class="sxs-lookup"><span data-stu-id="7d05a-942">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="7d05a-943">Corrigido o erro ao usar o `policy assignment list` com um grupo de recursos ou o nível de assinatura `--scope`</span><span class="sxs-lookup"><span data-stu-id="7d05a-943">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="7d05a-944">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7d05a-944">ServiceBus</span></span>
* <span data-ttu-id="7d05a-945">Corrigido o problema com o `servicebus topic create --max-size`[nº9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="7d05a-945">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-946">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-946">SQL</span></span>
* <span data-ttu-id="7d05a-947">Alterado o `--location` para ser opcional para `sql [server|mi] create` – usa o local do grupo de recursos se não especificado</span><span class="sxs-lookup"><span data-stu-id="7d05a-947">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="7d05a-948">Corrigido o erro "objeto 'NoneType' não é iterável" para `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="7d05a-948">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="7d05a-949">SQLVm</span><span class="sxs-lookup"><span data-stu-id="7d05a-949">SQLVm</span></span>
* <span data-ttu-id="7d05a-950">[ALTERAÇÃO DA FALHA] Alterado `sql vm create` para exigir o parâmetro `--license-type`</span><span class="sxs-lookup"><span data-stu-id="7d05a-950">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="7d05a-951">Alterado para permitir a configuração da SKU da imagem do SQL ao criar ou atualizar uma VM do SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-951">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-952">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-952">Storage</span></span>
* <span data-ttu-id="7d05a-953">Corrigido o problema com a chave de conta ignorada para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="7d05a-953">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="7d05a-954">Corrigido o problema com o `storage blob sync` no Linux</span><span class="sxs-lookup"><span data-stu-id="7d05a-954">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-955">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-955">VM</span></span>
* <span data-ttu-id="7d05a-956">[VERSÃO PRÉVIA] Adicionados os comandos `vm image template` para criar imagens de VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-956">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="7d05a-957">4 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-957">June 4, 2019</span></span>

<span data-ttu-id="7d05a-958">Versão 2.0.66</span><span class="sxs-lookup"><span data-stu-id="7d05a-958">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-959">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-959">Core</span></span>
* <span data-ttu-id="7d05a-960">Foi corrigido o bug em que os comandos falhavam quando `--output yaml` era usado com `--query`</span><span class="sxs-lookup"><span data-stu-id="7d05a-960">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-961">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-961">ACR</span></span>
* <span data-ttu-id="7d05a-962">Foi adicionado o grupo de comando 'pack acr' para a criação de Tarefas de build rápida usando Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="7d05a-962">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-963">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-963">ACS</span></span>
* <span data-ttu-id="7d05a-964">Permitir a opção de habilitar/desabilitar o complemento kube-dashboard do AKS</span><span class="sxs-lookup"><span data-stu-id="7d05a-964">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="7d05a-965">Imprimir uma mensagem amigável quando a assinatura não estiver na lista de permissões para usar o Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="7d05a-965">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="7d05a-966">Lote</span><span class="sxs-lookup"><span data-stu-id="7d05a-966">Batch</span></span>
* <span data-ttu-id="7d05a-967">Melhoria no tratamento de erro quando você não está conectado a uma conta \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="7d05a-967">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="7d05a-968">IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-968">IoT</span></span>
* <span data-ttu-id="7d05a-969">Foi adicionado o suporte para failover manual</span><span class="sxs-lookup"><span data-stu-id="7d05a-969">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-970">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-970">Network</span></span>
* <span data-ttu-id="7d05a-971">Foram adicionados os comandos `network application-gateway waf-policy` para oferecer suporte às regras de WAF personalizadas.</span><span class="sxs-lookup"><span data-stu-id="7d05a-971">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="7d05a-972">Adicionados os argumentos `--waf-policy` e `--max-capacity` para `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-972">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="7d05a-973">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-973">Resource</span></span>
* <span data-ttu-id="7d05a-974">Melhoria da mensagem de erro do `deployment create` quando não há nenhum TTY disponível</span><span class="sxs-lookup"><span data-stu-id="7d05a-974">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-975">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-975">Role</span></span>
* <span data-ttu-id="7d05a-976">O texto da Ajuda foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="7d05a-976">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="7d05a-977">Computação</span><span class="sxs-lookup"><span data-stu-id="7d05a-977">Compute</span></span>
* <span data-ttu-id="7d05a-978">Foi adicionado o suporte para `vm create` para as VMs de uma imagem gerenciada com LUNs de disco de dados que não começam em 0 ou que ignoram números</span><span class="sxs-lookup"><span data-stu-id="7d05a-978">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="7d05a-979">21 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-979">May 21, 2019</span></span>

<span data-ttu-id="7d05a-980">Versão 2.0.65</span><span class="sxs-lookup"><span data-stu-id="7d05a-980">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-981">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-981">Core</span></span>
* <span data-ttu-id="7d05a-982">Foram adicionados comentários melhores para erros de autenticação</span><span class="sxs-lookup"><span data-stu-id="7d05a-982">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="7d05a-983">Corrigido um problema em que a CLI carregava extensões que não eram compatíveis com a versão do núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-983">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="7d05a-984">Corrigido um problema com a inicialização quando `clouds.config` está corrompido</span><span class="sxs-lookup"><span data-stu-id="7d05a-984">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-985">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-985">ACR</span></span>
* <span data-ttu-id="7d05a-986">Foi adicionado suporte das Identidades Gerenciadas para Tarefas</span><span class="sxs-lookup"><span data-stu-id="7d05a-986">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-987">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-987">ACS</span></span>
* <span data-ttu-id="7d05a-988">Corrigido o comando `openshift create` quando usado com o cliente AAD do consumidor</span><span class="sxs-lookup"><span data-stu-id="7d05a-988">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-989">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-989">AppService</span></span>
* <span data-ttu-id="7d05a-990">[PRETERIDO] Preterido o comando `functionapp devops-build` – Será removido na próxima versão</span><span class="sxs-lookup"><span data-stu-id="7d05a-990">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="7d05a-991">`functionapp devops-pipeline` foi alterado para buscar o log de build do Azure DevOps no modo detalhado</span><span class="sxs-lookup"><span data-stu-id="7d05a-991">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="7d05a-992">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--use_local_settings` foi removido do comando `functionapp devops-pipeline` – não estava operacional</span><span class="sxs-lookup"><span data-stu-id="7d05a-992">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="7d05a-993">`webapp up` foi alterado para retornar uma saída JSON se `--logs` não for usado</span><span class="sxs-lookup"><span data-stu-id="7d05a-993">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="7d05a-994">Foi adicionado suporte para escrever recursos padrão para a configuração local de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="7d05a-994">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="7d05a-995">Foi adicionado suporte para `webapp up` reimplantar um aplicativo sem usar o argumento `--location`</span><span class="sxs-lookup"><span data-stu-id="7d05a-995">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="7d05a-996">Corrigido um problema em que o valor do SKU gratuito não funcionava na criação do ASP do SKU gratuito do Linux</span><span class="sxs-lookup"><span data-stu-id="7d05a-996">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="7d05a-997">BotService</span><span class="sxs-lookup"><span data-stu-id="7d05a-997">BotService</span></span>
* <span data-ttu-id="7d05a-998">Alterado para permitir todas as capitalizações para parâmetros `--lang` em todos os comandos</span><span class="sxs-lookup"><span data-stu-id="7d05a-998">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="7d05a-999">Descrição atualizada do módulo de comando</span><span class="sxs-lookup"><span data-stu-id="7d05a-999">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="7d05a-1000">Consumo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1000">Consumption</span></span>
* <span data-ttu-id="7d05a-1001">O parâmetro obrigatório ausente foi adicionado para executar `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1001">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="7d05a-1002">IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-1002">IoT</span></span>
* <span data-ttu-id="7d05a-1003">Suporte adicionado para listar todas as chaves</span><span class="sxs-lookup"><span data-stu-id="7d05a-1003">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-1004">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1004">Network</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="7d05a-1006">O argumento `--nat-gateway` foi adicionado a `network vnet subnet [create|update]` para anexar a um gateway NAT</span><span class="sxs-lookup"><span data-stu-id="7d05a-1006">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="7d05a-1007">Corrigido o problema de `dns zone import`, em que os nomes de registro não correspondiam ao tipo de registro</span><span class="sxs-lookup"><span data-stu-id="7d05a-1007">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="7d05a-1008">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1008">RDBMS</span></span>
* <span data-ttu-id="7d05a-1009">Suporte a postgres e mysql adicionado para replicação geográfica</span><span class="sxs-lookup"><span data-stu-id="7d05a-1009">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="7d05a-1010">RBAC</span><span class="sxs-lookup"><span data-stu-id="7d05a-1010">RBAC</span></span>
* <span data-ttu-id="7d05a-1011">Adição de suporte do escopo de grupo de gerenciamento a `role assignment`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1011">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-1012">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1012">Storage</span></span>
* <span data-ttu-id="7d05a-1013">`storage blob sync`: adicionar um comando de sincronização ao armazenamento de blobs</span><span class="sxs-lookup"><span data-stu-id="7d05a-1013">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="7d05a-1014">Computação</span><span class="sxs-lookup"><span data-stu-id="7d05a-1014">Compute</span></span>
* <span data-ttu-id="7d05a-1015">`--computer-name` foi adicionado a `vm create` para configurar o nome do computador da VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1015">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="7d05a-1016">`--ssh-key-value` foi renomeado para `--ssh-key-values` para `[vm|vmss] create` – Agora, pode aceitar vários valores de chave pública ou caminhos ssh</span><span class="sxs-lookup"><span data-stu-id="7d05a-1016">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="7d05a-1017">__Observação__: Isso **não** é uma alteração da falha – `--ssh-key-value` será analisado corretamente, pois corresponde somente a `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1017">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="7d05a-1018">O argumento `--type` de `ppg create` foi alterado para ser opcional</span><span class="sxs-lookup"><span data-stu-id="7d05a-1018">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="7d05a-1019">6 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-1019">May 6, 2019</span></span>

<span data-ttu-id="7d05a-1020">Versão 2.0.64</span><span class="sxs-lookup"><span data-stu-id="7d05a-1020">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-1021">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1021">ACS</span></span>
* <span data-ttu-id="7d05a-1022">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--fqdn` foi removido dos comandos `openshift`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1022">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="7d05a-1023">Alterado para usar a versão da API do Red Hat OpenShift no Azure em disponibilidade geral</span><span class="sxs-lookup"><span data-stu-id="7d05a-1023">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="7d05a-1024">O sinalizador `customer-admin-group-id` foi adicionado a `openshift create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1024">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="7d05a-1025">[GA] `(PREVIEW)` foi removido da opção `aks create``--network-policy`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1025">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-1026">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-1026">Appservice</span></span>
* <span data-ttu-id="7d05a-1027">[PRETERIDO] O comando `functionapp devops-build` foi preterido</span><span class="sxs-lookup"><span data-stu-id="7d05a-1027">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="7d05a-1028">Renomeado para `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1028">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="7d05a-1029">Corrigido ao obter o nome de usuário correto para cloudshell que estava causando a falha em `webapp up`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1029">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="7d05a-1030">Documentação `appservice plan --sku` atualizada para refletir o appserviceplans com suporte</span><span class="sxs-lookup"><span data-stu-id="7d05a-1030">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="7d05a-1031">Adicionado argumentos opcionais para o grupo de recursos e plano a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1031">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="7d05a-1032">Adicionado suporte a `webapp ssh` para respeitar a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1032">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="7d05a-1033">Adicionado suporte `appserviceplan create` para a SKU gratuita do Linux</span><span class="sxs-lookup"><span data-stu-id="7d05a-1033">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="7d05a-1034">Alterado `webapp up` para ter uma suspensão de 30 segundos depois de definir appsetting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` para lidar com a inicialização a frio kudu</span><span class="sxs-lookup"><span data-stu-id="7d05a-1034">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="7d05a-1035">Adicionado suporte para runtime `powershell` a `functionapp create` no Windows</span><span class="sxs-lookup"><span data-stu-id="7d05a-1035">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="7d05a-1036">Adicionado o comando `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1036">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="7d05a-1037">Lote</span><span class="sxs-lookup"><span data-stu-id="7d05a-1037">Batch</span></span>
* <span data-ttu-id="7d05a-1038">Corrigido o bug no validador para as opções `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1038">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="7d05a-1039">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="7d05a-1039">Botservice</span></span>
* <span data-ttu-id="7d05a-1040">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para criar um Bot de Aplicativo Web vazio por padrão (ou seja, nenhum bot será implantado no Serviço de Aplicativo)</span><span class="sxs-lookup"><span data-stu-id="7d05a-1040">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="7d05a-1041">O sinalizador `--echo` foi adicionado ao `bot create` para usar o comportamento antigo com `-v v4`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1041">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="7d05a-1042">[ALTERAÇÃO SIGNIFICATIVA] O valor padrão de `--version` foi alterado para `v4`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1042">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="7d05a-1043">__OBSERVAÇÃO:__ `bot prepare-publish` ainda usa o padrão antigo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1043">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="7d05a-1044">[ALTERAÇÃO SIGNIFICATIVA]`--lang` foi alterado para não definir mais `Csharp` como padrão.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1044">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="7d05a-1045">Se o comando exigir `--lang` e ele não for fornecido, o comando será um erro</span><span class="sxs-lookup"><span data-stu-id="7d05a-1045">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="7d05a-1046">[ALTERAÇÃO SIGNIFICATIVA] Os argumentos `--appid` e `--password` foram alterados para `bot create` ser obrigatório e agora podem ser criados por meio de `ad app create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1046">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="7d05a-1047">Foi adicionada validação a `--appid` e `--password`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1047">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="7d05a-1048">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4` foi alterado para não criar ou usar uma Conta de Armazenamento ou o Application Insights</span><span class="sxs-lookup"><span data-stu-id="7d05a-1048">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="7d05a-1049">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v3` foi alterado para exigir uma região em que o Application Insights está disponível</span><span class="sxs-lookup"><span data-stu-id="7d05a-1049">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="7d05a-1050">[ALTERAÇÃO SIGNIFICATIVA] O `bot update` foi alterado para afetar somente as propriedades específicas de um bot</span><span class="sxs-lookup"><span data-stu-id="7d05a-1050">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="7d05a-1051">[ALTERAÇÃO SIGNIFICATIVA] Os sinalizadores `--lang` foram alterados para aceitar `Javascript` em vez de `Node`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1051">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="7d05a-1052">[ALTERAÇÃO SIGNIFICATIVA] O `Node` foi removido como um valor `--lang` permitido</span><span class="sxs-lookup"><span data-stu-id="7d05a-1052">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="7d05a-1053">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para não definir mais `SCM_DO_BUILD_DURING_DEPLOYMENT` como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1053">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="7d05a-1054">Todas as implantações por meio do Kudu atuarão de acordo com o comportamento padrão</span><span class="sxs-lookup"><span data-stu-id="7d05a-1054">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="7d05a-1055">O `bot download` foi alterado para os bots sem arquivos `.bot` para criar o arquivo de configuração específico a um idioma com os valores das Configurações de Aplicativo do bot</span><span class="sxs-lookup"><span data-stu-id="7d05a-1055">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="7d05a-1056">Adicionado o suporte `Typescript` para `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1056">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="7d05a-1057">Uma mensagem de aviso foi adicionada a `bot prepare-deploy` para os bots `Javascript` e `Typescript` para quando `--code-dir` não contiver `package.json`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1057">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="7d05a-1058">O `bot prepare-deploy` foi alterado para retornar `true`, se bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="7d05a-1058">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="7d05a-1059">O log detalhado foi adicionado a `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1059">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="7d05a-1060">Mais regiões disponíveis do Application Insights foram adicionadas ao `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1060">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="7d05a-1061">Configurar</span><span class="sxs-lookup"><span data-stu-id="7d05a-1061">Configure</span></span>
* <span data-ttu-id="7d05a-1062">Adicionado suporte para configurações de valor padrão do argumento baseado em pasta</span><span class="sxs-lookup"><span data-stu-id="7d05a-1062">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="7d05a-1063">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1063">Eventhubs</span></span>
* <span data-ttu-id="7d05a-1064">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1064">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="7d05a-1065">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1065">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-1066">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1066">Network</span></span>
* <span data-ttu-id="7d05a-1067">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--cache` foi substituído por `--defer` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1067">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="7d05a-1068">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="7d05a-1068">Policy Insights</span></span>
* <span data-ttu-id="7d05a-1069">Suporte adicionado a `--expand PolicyEvaluationDetails` para detalhes de avaliação de política de consulta no recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-1069">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-1070">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-1070">Role</span></span>
* <span data-ttu-id="7d05a-1071">[PRETERIDO] Alterado argumento ocultar '--password' `create-for-rbac` - suporte será removido em maio de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-1071">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="7d05a-1072">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="7d05a-1072">Service Bus</span></span>
* <span data-ttu-id="7d05a-1073">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1073">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="7d05a-1074">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1074">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="7d05a-1075">`topic [create|update]` foi fixado para permitir suporte a `--max-size` para valores de 10, 20, 40 e 80 GB com a SKU Premium</span><span class="sxs-lookup"><span data-stu-id="7d05a-1075">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-1076">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-1076">SQL</span></span>
* <span data-ttu-id="7d05a-1077">Adicionados os comandos `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1077">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-1078">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1078">VM</span></span>
* <span data-ttu-id="7d05a-1079">O `--protect-from-scale-in` e o `--protect-from-scale-set-actions` foram adicionados a `vmss update` para habilitar atualizações à política de proteção das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1079">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="7d05a-1080">Adicionado a `--instance-id` e `vmss update` para habilitar atualização genérica das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1080">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="7d05a-1081">`--instance-id` foi adicionado a `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1081">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="7d05a-1082">Adição do novo grupo de comandos `ppg` para gerenciar Grupos de Posicionamento de Proximidade</span><span class="sxs-lookup"><span data-stu-id="7d05a-1082">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="7d05a-1083">Adicionado a `--ppg`, `[vm|vmss] create` e `vm availability-set create` para gerenciar PPGs</span><span class="sxs-lookup"><span data-stu-id="7d05a-1083">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="7d05a-1084">Parâmetro `--hyper-v-generation` adicionado a `image create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1084">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="7d05a-1085">23 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-1085">April 23, 2019</span></span>

<span data-ttu-id="7d05a-1086">Versão 2.0.63</span><span class="sxs-lookup"><span data-stu-id="7d05a-1086">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-1087">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1087">ACS</span></span>
* <span data-ttu-id="7d05a-1088">Alterado `aks get-credentials` para solicitar substituição dos valores duplicados</span><span class="sxs-lookup"><span data-stu-id="7d05a-1088">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="7d05a-1089">Removido `(PREVIEW)` dos comandos de espaços de desenvolvimento "aks use-dev-espaces" e "aks remove-dev-espaces"</span><span class="sxs-lookup"><span data-stu-id="7d05a-1089">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="7d05a-1090">AMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1090">AMS</span></span>
* <span data-ttu-id="7d05a-1091">Corrigido o bug com a atualização de filtros de conta e de ativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1091">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-1092">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-1092">AppService</span></span>
* <span data-ttu-id="7d05a-1093">Adicionado suporte para o ASE e o tempo limite para `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1093">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="7d05a-1094">Adicionado suporte para o estabelecimento de CI CD em um pipeline do Azure DevOps de um repositório do Github para aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="7d05a-1094">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="7d05a-1095">Adicionado argumento `--github-pat` a `functionapp devops-build create` para aceitar o token de acesso pessoal do Github</span><span class="sxs-lookup"><span data-stu-id="7d05a-1095">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="7d05a-1096">Adicionado argumento `--github-repository` a `functionapp devops-build create` para aceitar o repositório Github que contém um código-fonte functionapp</span><span class="sxs-lookup"><span data-stu-id="7d05a-1096">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="7d05a-1097">Problema corrigido em que `az webapp up --logs` estava falhando com um erro e atualização da versão .NETCORE padrão para 2.1</span><span class="sxs-lookup"><span data-stu-id="7d05a-1097">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="7d05a-1098">Configurações de functionapp desnecessárias removidas durante a criação de um aplicativo de funções com plano de consumo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1098">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="7d05a-1099">Alterado `webapp up` para que a cadeia de caracteres padrão asp agora acrescente o número no final para criar um novo ASP com base nas opções de SKU</span><span class="sxs-lookup"><span data-stu-id="7d05a-1099">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="7d05a-1100">Adicionado `-b` como uma opção a `webapp up` para iniciar o aplicativo no navegador</span><span class="sxs-lookup"><span data-stu-id="7d05a-1100">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="7d05a-1101">Alterado `webapp deployment source config zip` para lidar com a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1101">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="7d05a-1102">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="7d05a-1102">Deployment Manager</span></span>
* <span data-ttu-id="7d05a-1103">[VERSÃO PRÉVIA] Criar e gerenciar artefatos que dão suporte a distribuições</span><span class="sxs-lookup"><span data-stu-id="7d05a-1103">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="7d05a-1104">Laboratório</span><span class="sxs-lookup"><span data-stu-id="7d05a-1104">Lab</span></span>
* <span data-ttu-id="7d05a-1105">Corrigido o bug que causa uma saída inicial</span><span class="sxs-lookup"><span data-stu-id="7d05a-1105">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-1106">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1106">Network</span></span>
* <span data-ttu-id="7d05a-1107">Adicionada delegação de servidor de nome automática a `dns zone create` no pai durante a criação da zona filho</span><span class="sxs-lookup"><span data-stu-id="7d05a-1107">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-1108">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-1108">Resource</span></span>
* <span data-ttu-id="7d05a-1109">[PRETERIDO] Argumentos `--link-id`, `--target-id` e `--filter-string` preteridos de `resource link`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1109">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="7d05a-1110">Use os argumentos `--link`, `--target` e `--filter`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1110">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="7d05a-1111">Corrigido o problema em que os comandos `resource link [create|update]` não funcionavam</span><span class="sxs-lookup"><span data-stu-id="7d05a-1111">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="7d05a-1112">Corrigido um problema em que a exclusão usando uma ID de recurso poderia causar falha no erro</span><span class="sxs-lookup"><span data-stu-id="7d05a-1112">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-1113">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-1113">SQL</span></span>
* <span data-ttu-id="7d05a-1114">Adicionado suporte para fuso horário personalizado nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="7d05a-1114">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="7d05a-1115">Alterado para permitir que o nome do pool Elástico seja usado com `sql db update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1115">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="7d05a-1116">Adicionado o suporte `--no-wait` para `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1116">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="7d05a-1117">Adicionado o comando `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1117">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-1118">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1118">Storage</span></span>
* <span data-ttu-id="7d05a-1119">Corrigido o problema com tokens SAS com codificação dupla em `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1119">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-1120">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1120">VM</span></span>
* <span data-ttu-id="7d05a-1121">Adicionado sinalizador `--skip-shutdown` a `vm|vmss stop` para desligar as VMs sem o desligamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1121">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="7d05a-1122">Adicionado argumento `--storage-account-type` a `sig image-version create` para definir o tipo de conta do perfil de publicação</span><span class="sxs-lookup"><span data-stu-id="7d05a-1122">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="7d05a-1123">Adicionado argumento `--target-regions` a `sig image-version create` para permitir definir os tipos de conta de armazenamento específico da região</span><span class="sxs-lookup"><span data-stu-id="7d05a-1123">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="7d05a-1124">9 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-1124">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-1125">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1125">Core</span></span>
* <span data-ttu-id="7d05a-1126">Correção do problema em que algumas extensões mostraram uma versão do `Unknown` e não podiam ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="7d05a-1126">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-1127">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1127">ACR</span></span>
* <span data-ttu-id="7d05a-1128">Adição de suporte para execução de uma imagem sem contexto</span><span class="sxs-lookup"><span data-stu-id="7d05a-1128">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="7d05a-1129">AMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1129">AMS</span></span>
* [PRETERIDO]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [ALTERAÇÃO SIGNIFICATIVA]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="7d05a-1132">Adição de suporte para novos parâmetros de criptografia em `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1132">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="7d05a-1133">Adição de novo parâmetro `--filters` a `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1133">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-1134">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-1134">AppService</span></span>
* <span data-ttu-id="7d05a-1135">Adicionado o suporte `--logs` para `webapp up`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1135">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="7d05a-1136">Correção de problemas do comando `functionapp devops-build create` de geração de `azure-pipelines.yml`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1136">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="7d05a-1137">Melhoria do tratamento de erros e indicadores `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1137">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="7d05a-1138">[ALTERAÇÃO SIGNIFICATIVA] Remoção do sinalizador `--local-git` para o comando `devops-build`; a detecção de git local e a manipulação são obrigatórias para a criação de pipelines do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="7d05a-1138">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="7d05a-1139">Adição de suporte para a criação de planos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="7d05a-1139">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="7d05a-1140">Adição da capacidade de trocar um plano sob um aplicativo de funções usando `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1140">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="7d05a-1141">Adição de suporte para configurações de expansão de plano Premium do Azure Functions</span><span class="sxs-lookup"><span data-stu-id="7d05a-1141">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="7d05a-1142">CDN</span><span class="sxs-lookup"><span data-stu-id="7d05a-1142">CDN</span></span>
* <span data-ttu-id="7d05a-1143">Adição de suporte para `Microsoft_Standard` e `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1143">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="7d05a-1144">Comentários</span><span class="sxs-lookup"><span data-stu-id="7d05a-1144">Feedback</span></span>
* <span data-ttu-id="7d05a-1145">Alteração de `feedback` para mostrar metadados em comandos executados recentemente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1145">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="7d05a-1146">Alteração de `feedback` para solicitar o auxílio do usuário no processo de criação de problema abrindo um navegador e usando um modelo de problema</span><span class="sxs-lookup"><span data-stu-id="7d05a-1146">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="7d05a-1147">Alteração do `feedback` para imprimir o corpo do problema ao executar com '--verbose'</span><span class="sxs-lookup"><span data-stu-id="7d05a-1147">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="7d05a-1148">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1148">Monitor</span></span>
* <span data-ttu-id="7d05a-1149">Correção de um problema em que “count” não era um valor permitido com `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1149">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="7d05a-1150">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1150">Network</span></span>
* <span data-ttu-id="7d05a-1151">Correção do formato de tabela que não estava sendo exibido com `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1151">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="7d05a-1152">Adição dos comandos `list-request-headers` e `list-response-headers` para `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1152">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="7d05a-1153">Adição do comando `list-server-variables` para `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1153">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="7d05a-1154">Correção de um problema em que a atualização do estado do link em uma porta express-route geraria uma exceção de atributo desconhecido `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1154">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="7d05a-1155">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1155">PrivateDNS</span></span>
* <span data-ttu-id="7d05a-1156">Adição de `network private-dns` para zonas de DNS privado</span><span class="sxs-lookup"><span data-stu-id="7d05a-1156">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-1157">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-1157">Resource</span></span>
* <span data-ttu-id="7d05a-1158">Correção do problema com `deployment create` e `group deployment create`, em que um arquivo de parâmetros com um conjunto vazio de parâmetros não funcionaria</span><span class="sxs-lookup"><span data-stu-id="7d05a-1158">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-1159">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-1159">Role</span></span>
* <span data-ttu-id="7d05a-1160">Correção de `create-for-rbac` para lidar corretamente com `--years`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1160">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="7d05a-1161">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `role assignment delete` para solicitar ao excluir todas as atribuições na assinatura incondicionalmente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1161">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-1162">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-1162">SQL</span></span>
* <span data-ttu-id="7d05a-1163">Atualização de `sql mi [create|update]` com as propriedades proxyOverride e publicDataEndpointEnabled</span><span class="sxs-lookup"><span data-stu-id="7d05a-1163">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-1164">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1164">Storage</span></span>
* <span data-ttu-id="7d05a-1165">[ALTERAÇÃO SIGNIFICATIVA] Remoção do resultado de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1165">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="7d05a-1166">Adição de `--full-uri` a `storage blob generate-sas` para criar o URI completo para o blob com SAS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1166">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="7d05a-1167">Adição de `--file-snapshot` a `storage file copy start` para copiar arquivo do instantâneo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1167">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="7d05a-1168">Alteração de `storage blob copy cancel` para mostrar apenas o erro em vez da exceção para NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="7d05a-1168">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="7d05a-1169">26 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-1169">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="7d05a-1170">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1170">Core</span></span>
* <span data-ttu-id="7d05a-1171">Correção de problemas com incompatibilidade da extensão de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1171">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="7d05a-1172">Agora o tratamento de erros encaminha os clientes para a página de problemas</span><span class="sxs-lookup"><span data-stu-id="7d05a-1172">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="7d05a-1173">Nuvem</span><span class="sxs-lookup"><span data-stu-id="7d05a-1173">Cloud</span></span>
* <span data-ttu-id="7d05a-1174">Erro de “assinatura não encontrada” corrigido em `cloud set`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1174">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-1175">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1175">ACR</span></span>
* <span data-ttu-id="7d05a-1176">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1176">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="7d05a-1177">`--auth-mode` adicionado aos comandos `acr build`, `acr run`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1177">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="7d05a-1178">Grupo de comandos “acr task credential” adicionado para gerenciar as credenciais de uma Tarefa</span><span class="sxs-lookup"><span data-stu-id="7d05a-1178">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="7d05a-1179">“--no-wait” adicionado ao comando `acr build`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1179">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-1180">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-1180">AppService</span></span>
* <span data-ttu-id="7d05a-1181">Bug corrigido onde `webapp up` não estava lidando corretamente com a execução do diretório vazio ou do cenário de código desconhecido</span><span class="sxs-lookup"><span data-stu-id="7d05a-1181">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="7d05a-1182">Bug corrigido onde os slots não funcionavam para `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1182">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="7d05a-1183">Serviço de BOT</span><span class="sxs-lookup"><span data-stu-id="7d05a-1183">BOT Service</span></span>
* <span data-ttu-id="7d05a-1184">`bot prepare-deploy` adicionado para se preparar para a implantação de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1184">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="7d05a-1185">`bot create --kind registration` alterado para mostrar a senha se ela não for fornecida</span><span class="sxs-lookup"><span data-stu-id="7d05a-1185">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="7d05a-1186">[ALTERAÇÃO SIGNIFICATIVA]`--endpoint` alterado em `bot create --kind registration` como padrão para uma cadeia de caracteres vazia, em vez de ser requerido</span><span class="sxs-lookup"><span data-stu-id="7d05a-1186">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="7d05a-1187">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1187">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="7d05a-1188">CDN</span><span class="sxs-lookup"><span data-stu-id="7d05a-1188">CDN</span></span>
* <span data-ttu-id="7d05a-1189">Adicionado o suporte ao `--no-wait` para `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1189">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [ALTERAÇÃO SIGNIFICATIVA]: `cdn endpoint create` alterado para o comportamento de cache da cadeia de consulta padrão.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="7d05a-1191">Não há mais padrão para "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="7d05a-1191">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="7d05a-1192">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="7d05a-1192">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7d05a-1193">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="7d05a-1193">Cosmosdb</span></span>
* <span data-ttu-id="7d05a-1194">Suporte adicionado para `--enable-multiple-write-locations` na atualização da conta</span><span class="sxs-lookup"><span data-stu-id="7d05a-1194">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="7d05a-1195">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7d05a-1195">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="7d05a-1196">Interativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1196">Interactive</span></span>
* <span data-ttu-id="7d05a-1197">Incompatibilidade corrigida com a extensão Interativa instalada por meio do azdev</span><span class="sxs-lookup"><span data-stu-id="7d05a-1197">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="7d05a-1198">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1198">Monitor</span></span>
* <span data-ttu-id="7d05a-1199">Alterado para permitir o valor de dimensão `*` para `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1199">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-1200">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1200">Network</span></span>
* <span data-ttu-id="7d05a-1201">Grupo de comandos `rewrite-rule` adicionado em `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1201">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="7d05a-1202">Perfil</span><span class="sxs-lookup"><span data-stu-id="7d05a-1202">Profile</span></span>
* <span data-ttu-id="7d05a-1203">Suporte de conta no nível do locatário para a identidade de serviço gerenciado adicionado em `login`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1203">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="7d05a-1204">Postgres</span><span class="sxs-lookup"><span data-stu-id="7d05a-1204">Postgres</span></span> 
* <span data-ttu-id="7d05a-1205">Adicionados os comandos postgresql `replica` e `restart server`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1205">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="7d05a-1206">Alterado para obter o local padrão do grupo de recursos quando não fornecido para criar servidores e adicionar validação para os dias de retenção</span><span class="sxs-lookup"><span data-stu-id="7d05a-1206">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-1207">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-1207">Resource</span></span>
* <span data-ttu-id="7d05a-1208">Saída da tabela aperfeiçoada para `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1208">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="7d05a-1209">Corrigido o problema com `deployment [create|validate]` onde o tipo secureObject não era reconhecido</span><span class="sxs-lookup"><span data-stu-id="7d05a-1209">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="7d05a-1210">Grafo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1210">Graph</span></span>
* <span data-ttu-id="7d05a-1211">Adicionado o suporte ao `--end-date` para `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1211">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="7d05a-1212">Suporte adicionado para acrescentar permissões com `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1212">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="7d05a-1213">Bug corrigido com `ad app permission list` quando não havia nenhuma permissão</span><span class="sxs-lookup"><span data-stu-id="7d05a-1213">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="7d05a-1214">`ad sp delete` alterado para ignorar a exclusão da atribuição de função se a conta atual não tem nenhuma assinatura</span><span class="sxs-lookup"><span data-stu-id="7d05a-1214">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="7d05a-1215">`ad app create` alterado para `--identifier-uris` passar para lista vazia como padrão se não fornecido</span><span class="sxs-lookup"><span data-stu-id="7d05a-1215">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-1216">armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1216">storage</span></span>
* <span data-ttu-id="7d05a-1217">`--snapshot` adicionado a `storage file download-batch` para baixar de um instantâneo de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1217">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="7d05a-1218">Barra de progresso `storage blob [download-batch|upload-batch]` alterada para ser menos detalhada e indicar o blob atual</span><span class="sxs-lookup"><span data-stu-id="7d05a-1218">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="7d05a-1219">Problema corrigido com `storage account update` ao atualizar os parâmetros de criptografia</span><span class="sxs-lookup"><span data-stu-id="7d05a-1219">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="7d05a-1220">Problema corrigido onde `storage blob show` falharia ao usar o oauth (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="7d05a-1220">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-1221">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1221">VM</span></span>
* <span data-ttu-id="7d05a-1222">Adicionado o comando `image update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1222">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="7d05a-1223">12 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-1223">March 12, 2019</span></span>

<span data-ttu-id="7d05a-1224">Versão 2.0.60</span><span class="sxs-lookup"><span data-stu-id="7d05a-1224">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-1225">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1225">Core</span></span>

* <span data-ttu-id="7d05a-1226">Foi corrigido um erro incorreto no `cloud set` sobre assinatura não encontrada.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1226">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-1227">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1227">ACR</span></span>

* <span data-ttu-id="7d05a-1228">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1228">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-1229">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1229">ACS</span></span>

* <span data-ttu-id="7d05a-1230">Alteração para ignorar o parâmetro `--listen-address` para `aks browse` se ele não for compatível com kubectl</span><span class="sxs-lookup"><span data-stu-id="7d05a-1230">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="7d05a-1231">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-1231">AppService</span></span>

* <span data-ttu-id="7d05a-1232">Adicionado `[webapp|functionapp] deployment list-publishing-credentials` para obter a URL de publicação do Kudu e suas credenciais.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1232">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="7d05a-1233">Removida a instrução de impressão errônea de `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1233">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="7d05a-1234">Corrigido `functionapp` para definir a imagem correta do runtime nos planos do Serviço de Aplicativo no Linux.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1234">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="7d05a-1235">Removida a marca de versão prévia do `webapp up` e adicionadas melhorias ao comando.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1235">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="7d05a-1236">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="7d05a-1236">Botservice</span></span>

* <span data-ttu-id="7d05a-1237">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1237">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="7d05a-1238">Adicionados `Microsoft-BotFramework-AppId` e `Microsoft-BotFramework-AppPassword` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1238">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="7d05a-1239">Removidas as aspas simples da saída de comando `bot publish`, no final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1239">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="7d05a-1240">Alterado `bot publish` para que seja assíncrono.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1240">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="7d05a-1241">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-1241">Container</span></span>

* <span data-ttu-id="7d05a-1242">Adicionado o argumento `--no-wait` para `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1242">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="7d05a-1243">EventHub</span><span class="sxs-lookup"><span data-stu-id="7d05a-1243">EventHub</span></span>

* <span data-ttu-id="7d05a-1244">Adicionado o sinalizador `--skip-empty-archives` a `eventhub create|update` para dar suporte a arquivos vazios na captura.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1244">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="7d05a-1245">Localizar</span><span class="sxs-lookup"><span data-stu-id="7d05a-1245">Find</span></span>

* <span data-ttu-id="7d05a-1246">Atualização de funcionalidade principal</span><span class="sxs-lookup"><span data-stu-id="7d05a-1246">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7d05a-1247">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7d05a-1247">HDInsight</span></span>

* <span data-ttu-id="7d05a-1248">Adicionado o parâmetro `--storage-account-managed-identity` a `hdinsight create` para oferecer suporte ao MSI do ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1248">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-1249">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1249">Network</span></span>

* <span data-ttu-id="7d05a-1250">Corrigido o problema com `vpn-connection update`, onde a atualização de uma conexão VPN entre gateways em assinaturas diferentes falharia.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1250">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="7d05a-1251">Rdbms</span><span class="sxs-lookup"><span data-stu-id="7d05a-1251">Rdbms</span></span>

* <span data-ttu-id="7d05a-1252">Correções secundárias para obter a localização padrão do grupo de recursos, quando não fornecida, para criar servidores e adicionar validação nos dias de retenção.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1252">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-1253">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-1253">Role</span></span>

* <span data-ttu-id="7d05a-1254">Corrigido `role definition update` para usar ID a fim de resolver a definição corretamente.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1254">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="7d05a-1255">Alterado `ad app credential reset` para remover a suposição de que a entidade de serviço do aplicativo já existe.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1255">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7d05a-1256">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7d05a-1256">Service Fabric</span></span>

* <span data-ttu-id="7d05a-1257">Corrigido o problema com o fato de `sf cluster list` não ser iterável.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1257">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="7d05a-1258">26 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-1258">February 26, 2019</span></span>

<span data-ttu-id="7d05a-1259">Versão 2.0.59</span><span class="sxs-lookup"><span data-stu-id="7d05a-1259">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-1260">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1260">Core</span></span>

* <span data-ttu-id="7d05a-1261">Corrigido o problema onde algumas instâncias usando `--subscription NAME` produziriam uma exceção</span><span class="sxs-lookup"><span data-stu-id="7d05a-1261">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-1262">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1262">ACR</span></span>

* <span data-ttu-id="7d05a-1263">Parâmetro `--target` adicionado para os comandos `acr build`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1263">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="7d05a-1264">Melhor tratamento de erros para os comandos de execução quando não conectado ao Azure</span><span class="sxs-lookup"><span data-stu-id="7d05a-1264">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-1265">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1265">ACS</span></span>

* <span data-ttu-id="7d05a-1266">Opção `--listen-address` adicionada a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1266">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-1267">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-1267">AppService</span></span>

* <span data-ttu-id="7d05a-1268">Adicionado o comando `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1268">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="7d05a-1269">Lote</span><span class="sxs-lookup"><span data-stu-id="7d05a-1269">Batch</span></span>
* <span data-ttu-id="7d05a-1270">[ALTERAÇÃO SIGNIFICATIVA] Comando `batch pool upgrade os` removido</span><span class="sxs-lookup"><span data-stu-id="7d05a-1270">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="7d05a-1271">[ALTERAÇÃO SIGNIFICATIVA] Propriedade `Pacakges` removida das respostas `Application`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1271">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="7d05a-1272">Comando `batch application package list` adicionado para listar os pacotes de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1272">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="7d05a-1273">[ALTERAÇÃO SIGNIFICATIVA]`--application-id` alterado para `--application-name` em todos os comandos `batch application`,</span><span class="sxs-lookup"><span data-stu-id="7d05a-1273">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="7d05a-1274">O argumento `--json-file` foi adicionado aos comandos para a solicitação de resposta da API bruta</span><span class="sxs-lookup"><span data-stu-id="7d05a-1274">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="7d05a-1275">Validação atualizada para incluir automaticamente `https://` em todos os pontos de extremidade, se ausente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1275">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7d05a-1276">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7d05a-1276">CosmosDB</span></span>

* <span data-ttu-id="7d05a-1277">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7d05a-1277">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="7d05a-1278">Kusto</span><span class="sxs-lookup"><span data-stu-id="7d05a-1278">Kusto</span></span>

* <span data-ttu-id="7d05a-1279">[ALTERAÇÃO SIGNIFICATIVA] Os tipos `hot_cache_period` e `soft_delete_period` foram alterados do banco de dados para o formato de duração ISO8601</span><span class="sxs-lookup"><span data-stu-id="7d05a-1279">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-1280">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1280">Network</span></span>

* <span data-ttu-id="7d05a-1281">Adicionado o argumento `--express-route-gateway-bypass` para `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1281">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="7d05a-1282">Foram adicionados os grupos de comando a partir das extensões `express-route`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1282">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="7d05a-1283">Os grupos de comando `express-route gateway` e `express-route port` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="7d05a-1283">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="7d05a-1284">Adicionado o argumento `--legacy-mode` para `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1284">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="7d05a-1285">Os argumentos `--allow-classic-operations` e `--express-route-port` foram adicionados a `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1285">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="7d05a-1286">Adicionado o argumento `--gateway-default-site` para `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1286">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="7d05a-1287">Os comandos `ipsec-policy` foram adicionados a `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1287">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-1288">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-1288">Resource</span></span>

* <span data-ttu-id="7d05a-1289">Foi corrigido o problema com `deployment create` em que o campo do tipo diferencia letras maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="7d05a-1289">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="7d05a-1290">Foi adicionado o suporte para arquivo de parâmetros de URI a `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1290">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="7d05a-1291">Foi adicionado o suporte para parâmetros de URI e definições a `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1291">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="7d05a-1292">Foi corrigido o tratamento de parâmetros e regras para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1292">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="7d05a-1293">Foi corrigido o problema com `resource show/update/delete/tag/invoke-action` em que as IDs de assinatura cruzada não respeitaram corretamente a ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="7d05a-1293">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-1294">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-1294">Role</span></span>

* <span data-ttu-id="7d05a-1295">Foi adicionado o suporte para as funções do aplicativo a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1295">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-1296">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1296">VM</span></span>

* <span data-ttu-id="7d05a-1297">Foi corrigido o problema com `vm create where ` – a rede acelerada não foi habilitada por padrão no Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="7d05a-1297">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="7d05a-1298">12 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-1298">February 12, 2019</span></span>

<span data-ttu-id="7d05a-1299">Versão 2.0.58</span><span class="sxs-lookup"><span data-stu-id="7d05a-1299">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-1300">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1300">Core</span></span>

* <span data-ttu-id="7d05a-1301">`az --version` agora exibe uma notificação se você tiver pacotes para atualização</span><span class="sxs-lookup"><span data-stu-id="7d05a-1301">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="7d05a-1302">A regressão em que `--ids` não pode ser usado com a saída JSON foi corrigida</span><span class="sxs-lookup"><span data-stu-id="7d05a-1302">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-1303">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1303">ACR</span></span>
* <span data-ttu-id="7d05a-1304">[ALTERAÇÃO SIGNIFICATIVA] O grupo de comandos `acr build-task` foi removido</span><span class="sxs-lookup"><span data-stu-id="7d05a-1304">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="7d05a-1305">[ALTERAÇÃO SIGNIFICATIVA] As opções `--tag` e `--manifest` de `acr repository delete` foram removidas</span><span class="sxs-lookup"><span data-stu-id="7d05a-1305">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-1306">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1306">ACS</span></span>
* <span data-ttu-id="7d05a-1307">Suporte adicionado a `aks [enable-addons|disable-addons]` para nomes que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="7d05a-1307">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="7d05a-1308">Suporte adicionado para a operação de atualização do Azure Active Directory usando `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1308">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="7d05a-1309">Um esclarecimento informando que `--output` é ignorado para `aks get-credentials` foi adicionado</span><span class="sxs-lookup"><span data-stu-id="7d05a-1309">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="7d05a-1310">AMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1310">AMS</span></span>
* <span data-ttu-id="7d05a-1311">Adicionados os comandos `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1311">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="7d05a-1312">Adicionados os comandos `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1312">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-1313">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-1313">Appservice</span></span>
* <span data-ttu-id="7d05a-1314">Foi adicionada a capacidade de criar e configurar funções usando contêineres de ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1314">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="7d05a-1315">Suporte adicionado para a atualização das configurações de aplicativos Web por meio de JSON</span><span class="sxs-lookup"><span data-stu-id="7d05a-1315">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="7d05a-1316">A ajuda foi aprimorada para `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1316">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="7d05a-1317">Suporte adicionado para o App Insights para auxiliar na criação de aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="7d05a-1317">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="7d05a-1318">Os problemas com o SSH do aplicativo Web foram corrigidos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1318">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="7d05a-1319">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="7d05a-1319">Botservice</span></span>
* <span data-ttu-id="7d05a-1320">A experiência do usuário para `bot publish` foi aprimorada</span><span class="sxs-lookup"><span data-stu-id="7d05a-1320">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="7d05a-1321">Foram adicionados avisos de tempos limite ao executar `npm install` durante `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1321">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="7d05a-1322">O caractere inválido `.` de `--name` em `az bot create` foi removido</span><span class="sxs-lookup"><span data-stu-id="7d05a-1322">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="7d05a-1323">Alteração para interromper a geração aleatória de nomes de recursos durante a criação do Armazenamento do Azure, Plano do Serviço de Aplicativo, Aplicativo Web/de funções e Application Insights</span><span class="sxs-lookup"><span data-stu-id="7d05a-1323">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="7d05a-1324">[PRETERIDO] O argumento `--proj-name` foi preterido em favor de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1324">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="7d05a-1325">`az bot publish` foi alterado para remover arquivos de implantação do Node.js do IIS buscados, caso eles já não existissem</span><span class="sxs-lookup"><span data-stu-id="7d05a-1325">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="7d05a-1326">Foi adicionado o argumento `--keep-node-modules` para `az bot publish` para não excluir a pasta `node_modules` no Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1326">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="7d05a-1327">O par chave-valor `"publishCommand"` foi adicionado à saída de `az bot create` durante a criação de uma função do Azure ou bot de aplicativo Web</span><span class="sxs-lookup"><span data-stu-id="7d05a-1327">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="7d05a-1328">O valor de `"publishCommand"` é um comando `az bot publish` que é automaticamente preenchido com os parâmetros necessários para publicar o bot recém-criado</span><span class="sxs-lookup"><span data-stu-id="7d05a-1328">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="7d05a-1329">O `"WEBSITE_NODE_DEFAULT_VERSION"` foi atualizado no modelo do ARM para que os bots de SDK v4 usem 10.14.1 em vez de 8.9.4</span><span class="sxs-lookup"><span data-stu-id="7d05a-1329">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="7d05a-1330">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7d05a-1330">Key Vault</span></span>
* <span data-ttu-id="7d05a-1331">Foi corrigido o problema com `keyvault secret backup`, em que alguns usuários recebiam um erro `unexpected_keyword` ao usar `--id`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1331">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="7d05a-1332">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1332">Monitor</span></span>
* <span data-ttu-id="7d05a-1333">`monitor metrics alert [create|update]` foi alterado para permitir o valor dimensional `*`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1333">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-1334">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1334">Network</span></span>
* <span data-ttu-id="7d05a-1335">`dns zone export` foi alterado para garantir que CNAMEs exportados fossem FQDNs</span><span class="sxs-lookup"><span data-stu-id="7d05a-1335">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="7d05a-1336">O parâmetro `--gateway-name` foi adicionado a `nic ip-config address-pool [add|remove]` para dar suporte a pools de endereços de back-end de gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1336">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="7d05a-1337">Os argumentos `--traffic-analytics` e `--workspace` foram adicionados a `network watcher flow-log configure` para dar suporte à análise de tráfego por meio de um espaço de trabalho do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="7d05a-1337">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="7d05a-1338">`--idle-timeout` e `--floating-ip` foram adicionados a `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1338">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="7d05a-1339">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="7d05a-1339">Policy Insights</span></span>
* <span data-ttu-id="7d05a-1340">Os comandos `policy remediation` foram adicionados para dar suporte a recursos de correção de política de recursos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1340">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="7d05a-1341">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1341">RDBMS</span></span>
* <span data-ttu-id="7d05a-1342">A mensagem e os parâmetros de comando de ajuda foram aprimorados</span><span class="sxs-lookup"><span data-stu-id="7d05a-1342">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="7d05a-1343">Redis</span><span class="sxs-lookup"><span data-stu-id="7d05a-1343">Redis</span></span>
* <span data-ttu-id="7d05a-1344">Foram adicionados comandos para gerenciar regras de firewall (criar, atualizar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="7d05a-1344">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="7d05a-1345">Foram adicionados comandos para gerenciar links do servidor (criar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="7d05a-1345">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="7d05a-1346">Foram adicionados comandos para gerenciar o agendamento de patches (criar, atualizar, excluir, mostrar)</span><span class="sxs-lookup"><span data-stu-id="7d05a-1346">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="7d05a-1347">Suporte adicionado para Zonas de Disponibilidade e versão mínima de TLS para criar Redis</span><span class="sxs-lookup"><span data-stu-id="7d05a-1347">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="7d05a-1348">[ALTERAÇÃO SIGNIFICATIVA] Os comandos `redis update-settings` e `redis list-all` foram removidos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1348">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="7d05a-1349">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro para `redis create`: “configurações de locatário” não é aceito no formato chave[=valor]</span><span class="sxs-lookup"><span data-stu-id="7d05a-1349">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="7d05a-1350">[PRETERIDO] Uma mensagem de aviso foi adicionada para preterir o comando `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1350">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-1351">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-1351">Role</span></span>
* <span data-ttu-id="7d05a-1352">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido dos comandos `vm` para esta localização</span><span class="sxs-lookup"><span data-stu-id="7d05a-1352">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="7d05a-1353">SQL VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1353">SQL VM</span></span>
* <span data-ttu-id="7d05a-1354">[PRETERIDO] O argumento `--boostrap-acc-pwd` foi preterido devido a um erro de digitação</span><span class="sxs-lookup"><span data-stu-id="7d05a-1354">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-1355">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1355">VM</span></span>
* <span data-ttu-id="7d05a-1356">`vm list-skus` foi alterado para permitir o uso de `--all` no lugar de `--all true`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1356">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="7d05a-1357">Adicionado `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1357">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="7d05a-1358">Foi corrigido o bug em que `vmss encryption enable` falhava se fosse executado anteriormente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1358">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="7d05a-1359">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido para os comandos `role`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1359">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="7d05a-1360">31 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-1360">January 31, 2019</span></span>

<span data-ttu-id="7d05a-1361">Versão 2.0.57</span><span class="sxs-lookup"><span data-stu-id="7d05a-1361">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-1362">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1362">Core</span></span>

* <span data-ttu-id="7d05a-1363">Hotfix para o [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="7d05a-1363">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="7d05a-1364">28 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-1364">January 28, 2019</span></span>

<span data-ttu-id="7d05a-1365">Versão 2.0.56</span><span class="sxs-lookup"><span data-stu-id="7d05a-1365">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-1366">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1366">ACR</span></span>
* <span data-ttu-id="7d05a-1367">Suporte adicionado para regras de rede virtual/IP</span><span class="sxs-lookup"><span data-stu-id="7d05a-1367">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-1368">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1368">ACS</span></span>
* <span data-ttu-id="7d05a-1369">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="7d05a-1369">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="7d05a-1370">Comandos do OpenShift gerenciado foram adicionados</span><span class="sxs-lookup"><span data-stu-id="7d05a-1370">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="7d05a-1371">Suporte adicionado para operações de atualização da entidade de serviço com `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1371">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="7d05a-1372">AMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1372">AMS</span></span>
* <span data-ttu-id="7d05a-1373">[ALTERAÇÃO SIGNIFICATIVA]`ams asset get-streaming-locators` renomeado para `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1373">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="7d05a-1374">[ALTERAÇÃO SIGNIFICATIVA]`ams streaming-locator get-content-keys` renomeado para `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1374">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-1375">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-1375">Appservice</span></span>
* <span data-ttu-id="7d05a-1376">Suporte adicionado para o App Insights no `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1376">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="7d05a-1377">Suporte adicionado para a criação do plano de serviço de aplicativo (incluindo Elástico Premium) para Aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="7d05a-1377">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="7d05a-1378">Foram corrigidos os problemas com de configuração de aplicativo com os planos Elástico Premium</span><span class="sxs-lookup"><span data-stu-id="7d05a-1378">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="7d05a-1379">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-1379">Container</span></span>
* <span data-ttu-id="7d05a-1380">Adicionado o comando `container start`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1380">Added `container start` command</span></span>
* <span data-ttu-id="7d05a-1381">Alteração para permitir o uso de valores decimais para CPU durante a criação do contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-1381">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="7d05a-1382">EventGrid</span><span class="sxs-lookup"><span data-stu-id="7d05a-1382">EventGrid</span></span>
* <span data-ttu-id="7d05a-1383">Parâmetro `--deadletter-endpoint` adicionado a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1383">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="7d05a-1384">Storagequeue e hybridconnection foram adicionados como novos valores para 'event-subscription [create|update] --endpoint-type\`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1384">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="7d05a-1385">Os parâmetros `--max-delivery-attempts` e `--event-ttl` foram adicionados a `event-subscription create` para especificar a política de repetição para eventos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1385">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="7d05a-1386">Uma mensagem de aviso foi adicionada a `event-subscription [create|update]` quando o webhook como destino for usado para uma assinatura de evento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1386">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="7d05a-1387">O parâmetro source-resource-id foi adicionado para todos os comandos relacionados a eventos e marcar todos os outros parâmetros relacionados ao recurso de origem como preteridos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1387">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7d05a-1388">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7d05a-1388">HDInsight</span></span>
* <span data-ttu-id="7d05a-1389">[ALTERAÇÃO SIGNIFICATIVA] Os parâmetros `--virtual-network` e `--subnet-name` de `hdinsight [application] create` foram removidos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1389">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="7d05a-1390">[ALTERAÇÃO SIGNIFICATIVA]`hdinsight create --storage-account` foi alterado para aceitar o nome ou ID da conta de armazenamento, em vez de pontos de extremidade de blob</span><span class="sxs-lookup"><span data-stu-id="7d05a-1390">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="7d05a-1391">Parâmetros `--vnet-name` e `--subnet-name` adicionados a `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1391">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="7d05a-1392">Suporte adicionado para a criptografia de disco e Enterprise Security Package ao `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1392">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="7d05a-1393">Adicionado o comando `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1393">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="7d05a-1394">Adicionado o comando `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1394">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="7d05a-1395">IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-1395">IoT</span></span>
* <span data-ttu-id="7d05a-1396">O formato de codificação foi adicionado ao comando routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="7d05a-1396">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="7d05a-1397">Kusto</span><span class="sxs-lookup"><span data-stu-id="7d05a-1397">Kusto</span></span>
* <span data-ttu-id="7d05a-1398">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="7d05a-1398">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="7d05a-1399">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1399">Monitor</span></span>
* <span data-ttu-id="7d05a-1400">A comparação de ID foi alterada para diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="7d05a-1400">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="7d05a-1401">Perfil</span><span class="sxs-lookup"><span data-stu-id="7d05a-1401">Profile</span></span>
* <span data-ttu-id="7d05a-1402">A conta de nível de locatário foi habilitada para a identidade de serviço gerenciada de `login`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1402">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-1403">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1403">Network</span></span>
* <span data-ttu-id="7d05a-1404">Foi corrigido o problema com `express-route update`: em que o argumento `--bandwidth` era ignorado</span><span class="sxs-lookup"><span data-stu-id="7d05a-1404">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="7d05a-1405">Foi corrigido o problema com `ddos-protection update` em que definir a compreensão levava ao rastreamento de pilha</span><span class="sxs-lookup"><span data-stu-id="7d05a-1405">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-1406">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-1406">Resource</span></span>
* <span data-ttu-id="7d05a-1407">Suporte adicionado para o arquivo de parâmetros de URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1407">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="7d05a-1408">Suporte adicionado para a identidade gerenciada à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1408">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="7d05a-1409">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-1409">SQL Virtual Machine</span></span>
* <span data-ttu-id="7d05a-1410">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="7d05a-1410">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-1411">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1411">Storage</span></span>
* <span data-ttu-id="7d05a-1412">Alteração na correção para atualizar apenas as propriedades que são alteradas no mesmo objeto</span><span class="sxs-lookup"><span data-stu-id="7d05a-1412">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="7d05a-1413">#8021 foi corrigido, dados binários são codificados em base 64 quando retornados</span><span class="sxs-lookup"><span data-stu-id="7d05a-1413">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-1414">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1414">VM</span></span>
* <span data-ttu-id="7d05a-1415">Alteração de `vm encryption enable` para validar o cofre de chaves de criptografia de disco e se esse cofre de chaves de criptografia de chave existe</span><span class="sxs-lookup"><span data-stu-id="7d05a-1415">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="7d05a-1416">O sinalizador `--force` foi adicionado a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1416">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="7d05a-1417">15 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="7d05a-1417">January 15, 2019</span></span>

<span data-ttu-id="7d05a-1418">Versão 2.0.55</span><span class="sxs-lookup"><span data-stu-id="7d05a-1418">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-1419">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1419">ACR</span></span>
* <span data-ttu-id="7d05a-1420">Alteração para permitir forçar o envio por push de um gráfico Helm que não existe</span><span class="sxs-lookup"><span data-stu-id="7d05a-1420">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="7d05a-1421">Alteração para permitir operações de runtime sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1421">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="7d05a-1422">[PRETERIDO] O parâmetro `--resource-group` foi preterido nos comandos:</span><span class="sxs-lookup"><span data-stu-id="7d05a-1422">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="7d05a-1423">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1423">ACS</span></span>
* <span data-ttu-id="7d05a-1424">Suporte adicionado para novas regiões ACI</span><span class="sxs-lookup"><span data-stu-id="7d05a-1424">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-1425">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-1425">Appservice</span></span>
* <span data-ttu-id="7d05a-1426">Foi corrigido o problema com o carregamento de certificados para aplicativos que são hospedados em um ASE, em que o RG do ASE e o RG do aplicativo são diferentes</span><span class="sxs-lookup"><span data-stu-id="7d05a-1426">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="7d05a-1427">Alteração de `webapp up` para usar a SKU P1V1 como padrão para Linux</span><span class="sxs-lookup"><span data-stu-id="7d05a-1427">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="7d05a-1428">`[webapp|functionapp] deployment source config-zip` foi corrigido para mostrar a mensagem de erro adequada quando uma implantação falhar</span><span class="sxs-lookup"><span data-stu-id="7d05a-1428">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="7d05a-1429">Adicionado o comando `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1429">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="7d05a-1430">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="7d05a-1430">Botservice</span></span>
* <span data-ttu-id="7d05a-1431">Atualizações de status de implantação foram adicionadas a `bot create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1431">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="7d05a-1432">Configurar</span><span class="sxs-lookup"><span data-stu-id="7d05a-1432">Configure</span></span>
* <span data-ttu-id="7d05a-1433">`none` foi adicionado como um formato de saída configurável</span><span class="sxs-lookup"><span data-stu-id="7d05a-1433">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7d05a-1434">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7d05a-1434">CosmosDB</span></span>
* <span data-ttu-id="7d05a-1435">Suporte adicionado para criar o banco de dados com taxa de transferência compartilhada</span><span class="sxs-lookup"><span data-stu-id="7d05a-1435">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7d05a-1436">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7d05a-1436">HDInsight</span></span>
* <span data-ttu-id="7d05a-1437">Foram adicionados comandos para o gerenciamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1437">Added commands for managing applications</span></span>
* <span data-ttu-id="7d05a-1438">Foram adicionados comandos para o gerenciamento de ações de script</span><span class="sxs-lookup"><span data-stu-id="7d05a-1438">Added commands for managing script actions</span></span>
* <span data-ttu-id="7d05a-1439">Foram adicionados comandos para o gerenciamento do Operations Management Suite (OMS)</span><span class="sxs-lookup"><span data-stu-id="7d05a-1439">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="7d05a-1440">Suporte adicionado para listar a utilização regional ao `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1440">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="7d05a-1441">[ALTERAÇÃO SIGNIFICATIVA] O tipo de cluster padrão de `hdinsight create` foi removido</span><span class="sxs-lookup"><span data-stu-id="7d05a-1441">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-1442">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1442">Network</span></span>
* <span data-ttu-id="7d05a-1443">Adicionados os argumentos `--custom-headers` e `--status-code-ranges` para `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1443">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="7d05a-1444">Novos tipos de roteamento foram adicionados: Subrede e múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="7d05a-1444">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="7d05a-1445">Adicionados os argumentos `--custom-headers` e `--subnets` para `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1445">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="7d05a-1446">Foi corrigido o problema no qual fornecer `--vnets ""` a `ddos-protection update` causava um erro</span><span class="sxs-lookup"><span data-stu-id="7d05a-1446">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-1447">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-1447">Role</span></span>
* <span data-ttu-id="7d05a-1448">[PRETERIDO] O argumento `--password` foi preterido para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1448">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="7d05a-1449">Como alternativa, use senhas seguras geradas pela CLI</span><span class="sxs-lookup"><span data-stu-id="7d05a-1449">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="7d05a-1450">Segurança</span><span class="sxs-lookup"><span data-stu-id="7d05a-1450">Security</span></span>
* <span data-ttu-id="7d05a-1451">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="7d05a-1451">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-1452">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1452">Storage</span></span>
* <span data-ttu-id="7d05a-1453">[ALTERAÇÃO SIGNIFICATIVA] O número padrão de resultados de `storage [blob|file|container|share] list` foi alterado para 5.000.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1453">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="7d05a-1454">Use `--num-results *` para o comportamento original de retornar todos os resultados</span><span class="sxs-lookup"><span data-stu-id="7d05a-1454">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="7d05a-1455">Parâmetro `--marker` adicionado a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1455">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="7d05a-1456">Um marcador de log foi adicionado para a próxima página ao STDERR de `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1456">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="7d05a-1457">O comando `storage blob service-properties update` foi adicionado com suporte para sites estáticos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1457">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-1458">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1458">VM</span></span>
* <span data-ttu-id="7d05a-1459">`vm [disk|unmanaged-disk]` e `vmss disk` foram alterados para que tenham parâmetros mais consistentes</span><span class="sxs-lookup"><span data-stu-id="7d05a-1459">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="7d05a-1460">Suporte adicionado para referência cruzada de imagem de locatário a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1460">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="7d05a-1461">O bug de configuração padrão foi corrigido em `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1461">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="7d05a-1462">O argumento `--provision-after-extensions` foi adicionado a `vmss extension set` para definir quais extensões deverão ser provisionadas antes da extensão ser definida</span><span class="sxs-lookup"><span data-stu-id="7d05a-1462">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="7d05a-1463">O argumento `--replica-count` foi adicionado a `sig image-version update` para definir a contagem de replicação padrão</span><span class="sxs-lookup"><span data-stu-id="7d05a-1463">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="7d05a-1464">Foi corrigido o bug com `image create --source` em que o disco do sistema operacional de origem era confundido com uma VM do mesmo nome, mesmo se a ID de recurso completa fosse fornecida</span><span class="sxs-lookup"><span data-stu-id="7d05a-1464">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="7d05a-1465">20 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-1465">December 20, 2018</span></span>

<span data-ttu-id="7d05a-1466">Versão 2.0.54</span><span class="sxs-lookup"><span data-stu-id="7d05a-1466">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="7d05a-1467">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-1467">Appservice</span></span>
* <span data-ttu-id="7d05a-1468">Corrigido o problema que causava falha na reimplantação do `webapp up`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1468">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="7d05a-1469">Adicionado suporte para listar e restaurar instantâneos de aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="7d05a-1469">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="7d05a-1470">Adicionado suporte para o sinalizador `--runtime` para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="7d05a-1470">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="7d05a-1471">IoT Central</span><span class="sxs-lookup"><span data-stu-id="7d05a-1471">IoTCentral</span></span>
* <span data-ttu-id="7d05a-1472">Corrigida a chamada à API do comando de atualização</span><span class="sxs-lookup"><span data-stu-id="7d05a-1472">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-1473">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-1473">Role</span></span>
* <span data-ttu-id="7d05a-1474">[ALTERAÇÃO SIGNIFICATIVA]`ad [app|sp] list` alterado para listar somente os 100 primeiros objetos por padrão</span><span class="sxs-lookup"><span data-stu-id="7d05a-1474">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-1475">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-1475">SQL</span></span>
* <span data-ttu-id="7d05a-1476">Adicionado suporte para ordenação personalizada nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="7d05a-1476">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-1477">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1477">VM</span></span>
* <span data-ttu-id="7d05a-1478">Parâmetro `---os-type` adicionado a `disk create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1478">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="7d05a-1479">18 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-1479">December 18, 2018</span></span>

<span data-ttu-id="7d05a-1480">Versão 2.0.53</span><span class="sxs-lookup"><span data-stu-id="7d05a-1480">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="7d05a-1481">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1481">ACR</span></span>
* <span data-ttu-id="7d05a-1482">Adicionado suporte para importação de imagem de Registros de Contêiner externos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1482">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="7d05a-1483">Simplificado o layout da tabela para a lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="7d05a-1483">Condensed the table layout for task list</span></span>
* <span data-ttu-id="7d05a-1484">Adicionado suporte para URLs do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="7d05a-1484">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-1485">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1485">ACS</span></span>
* <span data-ttu-id="7d05a-1486">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="7d05a-1486">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="7d05a-1487">Removido “(VISUALIZAÇÃO)” de argumentos do AAD para `aks create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1487">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="7d05a-1488">[PRETERIDO] Comandos `az acs` preteridos.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1488">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="7d05a-1489">O serviço ACS será desativado em 31 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="7d05a-1489">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="7d05a-1490">Adicionado suporte da Política de Rede durante a criação de novos clusters AKS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1490">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="7d05a-1491">Removido o requisito do argumento `--nodepool-name` para `aks scale` se houver apenas um pool de nós</span><span class="sxs-lookup"><span data-stu-id="7d05a-1491">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-1492">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-1492">Appservice</span></span>
* <span data-ttu-id="7d05a-1493">Corrigido o problema em que `webapp config container` não honra o parâmetro `--slot`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1493">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="7d05a-1494">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="7d05a-1494">Botservice</span></span>
* <span data-ttu-id="7d05a-1495">Suporte adicionado para análise do arquivo `.bot` ao chamar `bot show`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1495">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="7d05a-1496">Corrigido o bug de provisionamento do AppInsights</span><span class="sxs-lookup"><span data-stu-id="7d05a-1496">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="7d05a-1497">Corrigido o bug de espaço em branco ao lidar com caminhos de arquivo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1497">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="7d05a-1498">Reduzidas as chamadas de rede do Kudu</span><span class="sxs-lookup"><span data-stu-id="7d05a-1498">Reduced Kudu network calls</span></span>
* <span data-ttu-id="7d05a-1499">Melhorias de UX para comandos gerais</span><span class="sxs-lookup"><span data-stu-id="7d05a-1499">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="7d05a-1500">Consumo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1500">Consumption</span></span>
* <span data-ttu-id="7d05a-1501">Corrigidos os bugs da API de orçamento ao mostrar notificações</span><span class="sxs-lookup"><span data-stu-id="7d05a-1501">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7d05a-1502">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7d05a-1502">CosmosDB</span></span>
* <span data-ttu-id="7d05a-1503">Suporte adicionado para atualizar a conta de vários mestres para mestre único</span><span class="sxs-lookup"><span data-stu-id="7d05a-1503">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="7d05a-1504">Mapas</span><span class="sxs-lookup"><span data-stu-id="7d05a-1504">Maps</span></span>
* <span data-ttu-id="7d05a-1505">Adicionado suporte ao SKU S1 para `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1505">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-1506">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1506">Network</span></span>
* <span data-ttu-id="7d05a-1507">Adicionado suporte para `--format` e `--log-version` para `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1507">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="7d05a-1508">Corrigido o problema com `dns zone update` em que usar "" para limpar a resolução e o registro de redes virtuais não funcionava</span><span class="sxs-lookup"><span data-stu-id="7d05a-1508">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-1509">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-1509">Resource</span></span>
* <span data-ttu-id="7d05a-1510">Corrigido o tratamento do parâmetro de escopo para grupos de gerenciamento do `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1510">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="7d05a-1511">Adicionado o novo comando `resource wait`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1511">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-1512">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1512">Storage</span></span>
*  <span data-ttu-id="7d05a-1513">Adicionada a capacidade de atualizar a versão do esquema de log para serviços de armazenamento no `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1513">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-1514">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1514">VM</span></span>
* <span data-ttu-id="7d05a-1515">Corrigida a falha em `vm identity remove` quando a VM especificada não tem nenhuma identidade de serviço gerenciado atribuída</span><span class="sxs-lookup"><span data-stu-id="7d05a-1515">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="7d05a-1516">4 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-1516">December 4, 2018</span></span>

<span data-ttu-id="7d05a-1517">Versão 2.0.52</span><span class="sxs-lookup"><span data-stu-id="7d05a-1517">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="7d05a-1518">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1518">Core</span></span>
* <span data-ttu-id="7d05a-1519">Adicionado suporte para provisionamento de recursos de locatários cruzados para a entidade de serviço de multilocatários</span><span class="sxs-lookup"><span data-stu-id="7d05a-1519">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="7d05a-1520">Corrigido o bug onde as ids enviadas por pipe de um comando com a saída tsv eram analisados incorretamente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1520">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-1521">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-1521">Appservice</span></span>
* <span data-ttu-id="7d05a-1522">[VERSÃO PRÉVIA] Adicionado o comando `webapp up` que ajuda a criar e implantar conteúdo em aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1522">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="7d05a-1523">Corrigido um bug no aplicativo com base em contêiner do Windows devido à alteração de back-end</span><span class="sxs-lookup"><span data-stu-id="7d05a-1523">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-1524">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1524">Network</span></span>
* <span data-ttu-id="7d05a-1525">Adicionado o argumento `--exclusion` a `application-gateway waf-config set` para dar suporte a exclusões de WAF</span><span class="sxs-lookup"><span data-stu-id="7d05a-1525">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-1526">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-1526">Role</span></span>
* <span data-ttu-id="7d05a-1527">Adicionado suporte para identificadores personalizados para a credencial de senha</span><span class="sxs-lookup"><span data-stu-id="7d05a-1527">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="7d05a-1528">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1528">VM</span></span>
* <span data-ttu-id="7d05a-1529">[PRETERIDO] Parâmetro `vm extension [show|wait] --expand` preterido</span><span class="sxs-lookup"><span data-stu-id="7d05a-1529">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="7d05a-1530">Adicionado parâmetro `--force` a `vm restart` para reimplantar as VMs sem resposta</span><span class="sxs-lookup"><span data-stu-id="7d05a-1530">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="7d05a-1531">Alterado `[vm|vmss] create --authentication-type` para aceitar "todos" para criar uma VM com senha e autenticação SSH</span><span class="sxs-lookup"><span data-stu-id="7d05a-1531">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="7d05a-1532">Adicionado parâmetro `image create --os-disk-caching` para definir o cache de disco do sistema operacional para uma imagem</span><span class="sxs-lookup"><span data-stu-id="7d05a-1532">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="7d05a-1533">20 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-1533">November 20, 2018</span></span>

<span data-ttu-id="7d05a-1534">Versão 2.0.51</span><span class="sxs-lookup"><span data-stu-id="7d05a-1534">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="7d05a-1535">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1535">Core</span></span>
* <span data-ttu-id="7d05a-1536">Logon do MSI alterado para não reutilizar o nome da assinatura na identidade</span><span class="sxs-lookup"><span data-stu-id="7d05a-1536">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-1537">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1537">ACR</span></span>
* <span data-ttu-id="7d05a-1538">Token de contexto adicionado à etapa da tarefa</span><span class="sxs-lookup"><span data-stu-id="7d05a-1538">Added context token to task step</span></span>
* <span data-ttu-id="7d05a-1539">Suporte adicionado para definir segredos na execução do acr para espelhar a tarefa do acr</span><span class="sxs-lookup"><span data-stu-id="7d05a-1539">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="7d05a-1540">Suporte aprimorado para `--top` e `--orderby` para os comandos `show-tags` e `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1540">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-1541">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-1541">Appservice</span></span>
* <span data-ttu-id="7d05a-1542">Tempo limite padrão para a implantação do zip alterado para sondar o status aumentado para 5 minutos, também adicionando uma propriedade de tempo limite para personalizar esse valor</span><span class="sxs-lookup"><span data-stu-id="7d05a-1542">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="7d05a-1543">Padrão `node_version` atualizado.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1543">Updated the default `node_version`.</span></span> <span data-ttu-id="7d05a-1544">Redefinir a ação de troca de slots durante uma troca de duas fases preserva todas as configurações do aplicativo e cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="7d05a-1544">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="7d05a-1545">Verificação da SKU no lado do cliente removida para o Linux criar o plano do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1545">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="7d05a-1546">Erro corrigido ao tentar obter o status de implantação do zip</span><span class="sxs-lookup"><span data-stu-id="7d05a-1546">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="7d05a-1547">Iot Central</span><span class="sxs-lookup"><span data-stu-id="7d05a-1547">IotCentral</span></span>
* <span data-ttu-id="7d05a-1548">Verificação de disponibilidade do subdomínio adicionada ao criar um aplicativo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="7d05a-1548">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="7d05a-1549">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7d05a-1549">KeyVault</span></span>
* <span data-ttu-id="7d05a-1550">Bug corrigido em que os erros podem ter sido ignorados</span><span class="sxs-lookup"><span data-stu-id="7d05a-1550">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-1551">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1551">Network</span></span>
* <span data-ttu-id="7d05a-1552">Subcomandos `root-cert` adicionados a `application-gateway` para lidar com os certificados de raiz confiável</span><span class="sxs-lookup"><span data-stu-id="7d05a-1552">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="7d05a-1553">Opções `--min-capacity` e `--custom-error-pages` adicionadas a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="7d05a-1553">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="7d05a-1554">`--zones` adicionado para suporte da zona de disponibilidade a `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1554">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="7d05a-1555">Argumentos `--file-upload-limit`, `--max-request-body-size` e `--request-body-check` a `application-gateway waf-config set` adicionados</span><span class="sxs-lookup"><span data-stu-id="7d05a-1555">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="7d05a-1556">Rdbms</span><span class="sxs-lookup"><span data-stu-id="7d05a-1556">Rdbms</span></span>
* <span data-ttu-id="7d05a-1557">Comandos vnet do mariadb adicionados</span><span class="sxs-lookup"><span data-stu-id="7d05a-1557">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="7d05a-1558">Rbac</span><span class="sxs-lookup"><span data-stu-id="7d05a-1558">Rbac</span></span>
* <span data-ttu-id="7d05a-1559">Um problema corrigido ao tentar atualizar credenciais inalteradas em `ad app update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1559">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="7d05a-1560">Avisos de saída adicionados para comunicar alterações de falha em um futuro próximo para `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1560">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="7d05a-1561">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1561">Storage</span></span>
* <span data-ttu-id="7d05a-1562">Melhor manipulação de casos incomuns para os comandos da cópia de armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1562">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="7d05a-1563">Corrigido o problema em que `storage blob copy start-batch` não usava credenciais de logon quando as contas de origem e destino eram iguais</span><span class="sxs-lookup"><span data-stu-id="7d05a-1563">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="7d05a-1564">Bug corrigido com `storage [blob|file] url` em que `sas_token` não foi incorporado na URL</span><span class="sxs-lookup"><span data-stu-id="7d05a-1564">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="7d05a-1565">Aviso de alteração da falha adicionado a `[blob|container] list`: produzirá apenas os primeiros 5.000 resultados por padrão</span><span class="sxs-lookup"><span data-stu-id="7d05a-1565">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-1566">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1566">VM</span></span>
* <span data-ttu-id="7d05a-1567">Suporte adicionado a `[vm|vmss] create --storage-sku` para especificar a SKU da conta de armazenamento para o SO gerenciado e os discos de dados separadamente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1567">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="7d05a-1568">Parâmetros do nome da versão alterados de `sig image-version` para `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1568">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="7d05a-1569">Argumento `sig image-version` preterido `--image-version-name`, substituído por `--image-version`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1569">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="7d05a-1570">Suporte adicionado para usar o disco local do SO a `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1570">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="7d05a-1571">Adicionado o suporte ao `--no-wait` para `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1571">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="7d05a-1572">Adicionado o comando `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1572">Added `snapshot wait` command</span></span>
* <span data-ttu-id="7d05a-1573">Suporte adicionado para usar o nome da instância com `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1573">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="7d05a-1574">6 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-1574">November 6, 2018</span></span>

<span data-ttu-id="7d05a-1575">Versão 2.0.50</span><span class="sxs-lookup"><span data-stu-id="7d05a-1575">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-1576">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1576">Core</span></span>
* <span data-ttu-id="7d05a-1577">Foi adicionado suporte para o serviço principal sn + autenticação do emissor</span><span class="sxs-lookup"><span data-stu-id="7d05a-1577">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-1578">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1578">ACR</span></span>
* <span data-ttu-id="7d05a-1579">Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa</span><span class="sxs-lookup"><span data-stu-id="7d05a-1579">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="7d05a-1580">Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação</span><span class="sxs-lookup"><span data-stu-id="7d05a-1580">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-1581">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1581">ACS</span></span>
* <span data-ttu-id="7d05a-1582">[ALTERAÇÃO SIGNIFICATIVA]`enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão</span><span class="sxs-lookup"><span data-stu-id="7d05a-1582">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="7d05a-1583">Supervisor</span><span class="sxs-lookup"><span data-stu-id="7d05a-1583">Advisor</span></span>
* <span data-ttu-id="7d05a-1584">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="7d05a-1584">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="7d05a-1585">AMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1585">AMS</span></span>
* <span data-ttu-id="7d05a-1586">Novos grupos de comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="7d05a-1586">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="7d05a-1587">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="7d05a-1587">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="7d05a-1588">Adicionados parâmetros de criptografia com suporte para `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1588">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="7d05a-1589">O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido</span><span class="sxs-lookup"><span data-stu-id="7d05a-1589">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="7d05a-1590">Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1590">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="7d05a-1591">Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1591">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="7d05a-1592">Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1592">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="7d05a-1593">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming locator` foi substituído por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1593">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="7d05a-1594">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--content-keys` de `ams streaming locator` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="7d05a-1594">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="7d05a-1595">[ALTERAÇÃO SIGNIFICATIVA]`--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1595">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="7d05a-1596">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming policy` foi substituído por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1596">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="7d05a-1597">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1597">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="7d05a-1598">Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="7d05a-1598">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="7d05a-1599">Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado</span><span class="sxs-lookup"><span data-stu-id="7d05a-1599">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="7d05a-1600">[ALTERAÇÃO SIGNIFICATIVA]`--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1600">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="7d05a-1601">Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1601">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="7d05a-1602">Um ativo sem rótulo pode ser enviado assim: 'assetName='</span><span class="sxs-lookup"><span data-stu-id="7d05a-1602">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-1603">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-1603">AppService</span></span>
* <span data-ttu-id="7d05a-1604">Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido</span><span class="sxs-lookup"><span data-stu-id="7d05a-1604">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="7d05a-1605">Configurar</span><span class="sxs-lookup"><span data-stu-id="7d05a-1605">Configure</span></span>
* <span data-ttu-id="7d05a-1606">O YAML foi adicionado às opções de formato de saída</span><span class="sxs-lookup"><span data-stu-id="7d05a-1606">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="7d05a-1607">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-1607">Container</span></span>
* <span data-ttu-id="7d05a-1608">Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml</span><span class="sxs-lookup"><span data-stu-id="7d05a-1608">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="7d05a-1609">EventHub</span><span class="sxs-lookup"><span data-stu-id="7d05a-1609">EventHub</span></span>
* <span data-ttu-id="7d05a-1610">O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1610">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="7d05a-1611">Interativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1611">Interactive</span></span>
* <span data-ttu-id="7d05a-1612">O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1612">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="7d05a-1613">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1613">Monitor</span></span>
* <span data-ttu-id="7d05a-1614">Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) para `--condition` em `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1614">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-1615">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1615">Network</span></span>
* <span data-ttu-id="7d05a-1616">Os nomes de comandos `network interface-endpoint` foram preteridos em benefício de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1616">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="7d05a-1617">Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID</span><span class="sxs-lookup"><span data-stu-id="7d05a-1617">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="7d05a-1618">Foi corrigido um problema onde `--ip-tags` não funcionava corretamente com `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1618">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="7d05a-1619">Perfil</span><span class="sxs-lookup"><span data-stu-id="7d05a-1619">Profile</span></span>
* <span data-ttu-id="7d05a-1620">`--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado</span><span class="sxs-lookup"><span data-stu-id="7d05a-1620">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="7d05a-1621">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1621">RDBMS</span></span>
* <span data-ttu-id="7d05a-1622">Adicionados comandos da réplica mysql</span><span class="sxs-lookup"><span data-stu-id="7d05a-1622">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-1623">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-1623">Resource</span></span>
* <span data-ttu-id="7d05a-1624">Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1624">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-1625">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-1625">Role</span></span>
* <span data-ttu-id="7d05a-1626">Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais</span><span class="sxs-lookup"><span data-stu-id="7d05a-1626">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="7d05a-1627">`ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="7d05a-1627">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="7d05a-1628">Suporte adicionado para conceder permissões a aplicativos do AAD</span><span class="sxs-lookup"><span data-stu-id="7d05a-1628">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-1629">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1629">Storage</span></span>
* <span data-ttu-id="7d05a-1630">Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1630">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-1631">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1631">VM</span></span>
* <span data-ttu-id="7d05a-1632">O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem</span><span class="sxs-lookup"><span data-stu-id="7d05a-1632">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="7d05a-1633">O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido</span><span class="sxs-lookup"><span data-stu-id="7d05a-1633">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="7d05a-1634">O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado</span><span class="sxs-lookup"><span data-stu-id="7d05a-1634">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="7d05a-1635">`vm secret format` foi alterado para exigir a saída json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1635">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="7d05a-1636">Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido</span><span class="sxs-lookup"><span data-stu-id="7d05a-1636">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="7d05a-1637">Validação de argumento aprimorado para `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1637">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="7d05a-1638">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-1638">October 23, 2018</span></span>

<span data-ttu-id="7d05a-1639">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="7d05a-1639">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-1640">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1640">Core</span></span>
* <span data-ttu-id="7d05a-1641">Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1641">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="7d05a-1642">Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1642">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-1643">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1643">ACR</span></span>
* <span data-ttu-id="7d05a-1644">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="7d05a-1644">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="7d05a-1645">CDN</span><span class="sxs-lookup"><span data-stu-id="7d05a-1645">CDN</span></span>
* <span data-ttu-id="7d05a-1646">[ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="7d05a-1646">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="7d05a-1647">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="7d05a-1647">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="7d05a-1648">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-1648">Container</span></span>
* <span data-ttu-id="7d05a-1649">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="7d05a-1649">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="7d05a-1650">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="7d05a-1650">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="7d05a-1651">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1651">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="7d05a-1652">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="7d05a-1652">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="7d05a-1653">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="7d05a-1653">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="7d05a-1654">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="7d05a-1654">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="7d05a-1655">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1655">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7d05a-1656">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7d05a-1656">CosmosDB</span></span>
* <span data-ttu-id="7d05a-1657">Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1657">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="7d05a-1658">Interativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1658">Interactive</span></span>
* <span data-ttu-id="7d05a-1659">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="7d05a-1659">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="7d05a-1660">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-1660">IoT Central</span></span>
* <span data-ttu-id="7d05a-1661">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="7d05a-1661">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="7d05a-1662">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="7d05a-1662">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="7d05a-1663">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1663">Monitor</span></span>
* <span data-ttu-id="7d05a-1664">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="7d05a-1664">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="7d05a-1665">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="7d05a-1665">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="7d05a-1666">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1666">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="7d05a-1667">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="7d05a-1667">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="7d05a-1668">Adicionado `--namespace` como alias para a opção preterida `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1668">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="7d05a-1669">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="7d05a-1669">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="7d05a-1670">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="7d05a-1670">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="7d05a-1671">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1671">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="7d05a-1672">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="7d05a-1672">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="7d05a-1673">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1673">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-1674">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1674">Network</span></span>
* <span data-ttu-id="7d05a-1675">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="7d05a-1675">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="7d05a-1676">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="7d05a-1676">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="7d05a-1677">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7d05a-1677">ServiceBus</span></span>
* <span data-ttu-id="7d05a-1678">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="7d05a-1678">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-1679">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-1679">SQL</span></span>
* <span data-ttu-id="7d05a-1680">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="7d05a-1680">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-1681">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1681">Storage</span></span>
* <span data-ttu-id="7d05a-1682">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="7d05a-1682">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="7d05a-1683">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="7d05a-1683">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-1684">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1684">VM</span></span>
* <span data-ttu-id="7d05a-1685">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1685">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="7d05a-1686">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1686">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="7d05a-1687">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1687">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="7d05a-1688">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-1688">October 16, 2018</span></span>

<span data-ttu-id="7d05a-1689">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="7d05a-1689">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-1690">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1690">VM</span></span>
* <span data-ttu-id="7d05a-1691">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="7d05a-1691">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="7d05a-1692">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-1692">October 9, 2018</span></span>

<span data-ttu-id="7d05a-1693">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="7d05a-1693">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-1694">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1694">Core</span></span>
* <span data-ttu-id="7d05a-1695">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="7d05a-1695">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-1696">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1696">ACR</span></span>
* <span data-ttu-id="7d05a-1697">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="7d05a-1697">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-1698">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1698">ACS</span></span>
* <span data-ttu-id="7d05a-1699">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="7d05a-1699">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="7d05a-1700">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="7d05a-1700">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="7d05a-1701">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1701">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="7d05a-1702">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="7d05a-1702">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="7d05a-1703">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-1703">Container</span></span>
* <span data-ttu-id="7d05a-1704">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um runtime específico</span><span class="sxs-lookup"><span data-stu-id="7d05a-1704">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="7d05a-1705">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="7d05a-1705">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="7d05a-1706">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1706">Event Hub</span></span>
* <span data-ttu-id="7d05a-1707">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1707">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="7d05a-1708">[ALTERAÇÃO SIGNIFICATIVA]`list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="7d05a-1708">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="7d05a-1709">Extensões</span><span class="sxs-lookup"><span data-stu-id="7d05a-1709">Extensions</span></span>
* <span data-ttu-id="7d05a-1710">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="7d05a-1710">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7d05a-1711">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7d05a-1711">HDInsight</span></span>
* <span data-ttu-id="7d05a-1712">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="7d05a-1712">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="7d05a-1713">IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-1713">IoT</span></span>
* <span data-ttu-id="7d05a-1714">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="7d05a-1714">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="7d05a-1715">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7d05a-1715">KeyVault</span></span>
* <span data-ttu-id="7d05a-1716">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1716">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-1717">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1717">Network</span></span>
* <span data-ttu-id="7d05a-1718">Corrigido `network dns zone create`: O comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1718">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="7d05a-1719">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="7d05a-1719">See #6052</span></span>
* <span data-ttu-id="7d05a-1720">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1720">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="7d05a-1721">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="7d05a-1721">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="7d05a-1722">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1722">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="7d05a-1723">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1723">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="7d05a-1724">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1724">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="7d05a-1725">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1725">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-1726">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-1726">Role</span></span>
* <span data-ttu-id="7d05a-1727">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1727">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="7d05a-1728">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1728">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="7d05a-1729">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="7d05a-1729">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="7d05a-1730">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="7d05a-1730">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="7d05a-1731">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="7d05a-1731">Service Bus</span></span>
* <span data-ttu-id="7d05a-1732">[ALTERAÇÃO SIGNIFICATIVA]`list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="7d05a-1732">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-1733">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1733">VM</span></span>
* <span data-ttu-id="7d05a-1734">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1734">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="7d05a-1735">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1735">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="7d05a-1736">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1736">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="7d05a-1737">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1737">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="7d05a-1738">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1738">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="7d05a-1739">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="7d05a-1739">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="7d05a-1740">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-1740">September 21, 2018</span></span>

<span data-ttu-id="7d05a-1741">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="7d05a-1741">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-1742">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1742">ACR</span></span>
* <span data-ttu-id="7d05a-1743">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1743">Added ACR Task commands</span></span>
* <span data-ttu-id="7d05a-1744">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="7d05a-1744">Added quick run command</span></span>
* <span data-ttu-id="7d05a-1745">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1745">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="7d05a-1746">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1746">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="7d05a-1747">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="7d05a-1747">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="7d05a-1748">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="7d05a-1748">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-1749">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1749">ACS</span></span>
* <span data-ttu-id="7d05a-1750">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1750">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="7d05a-1751">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="7d05a-1751">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-1752">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-1752">AppService</span></span>

* <span data-ttu-id="7d05a-1753">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="7d05a-1753">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="7d05a-1754">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="7d05a-1754">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="7d05a-1755">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="7d05a-1755">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="7d05a-1756">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1756">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="7d05a-1757">Lote</span><span class="sxs-lookup"><span data-stu-id="7d05a-1757">Batch</span></span>
* <span data-ttu-id="7d05a-1758">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="7d05a-1758">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="7d05a-1759">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1759">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="7d05a-1760">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1760">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="7d05a-1761">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="7d05a-1761">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7d05a-1762">Lote AI</span><span class="sxs-lookup"><span data-stu-id="7d05a-1762">Batch AI</span></span> 
* <span data-ttu-id="7d05a-1763">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1763">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7d05a-1764">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1764">Cognitive Services</span></span>
* <span data-ttu-id="7d05a-1765">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1765">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="7d05a-1766">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1766">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="7d05a-1767">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1767">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="7d05a-1768">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1768">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="7d05a-1769">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1769">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="7d05a-1770">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1770">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="7d05a-1771">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-1771">Container</span></span>
* <span data-ttu-id="7d05a-1772">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="7d05a-1772">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="7d05a-1773">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1773">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="7d05a-1774">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="7d05a-1774">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="7d05a-1775">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="7d05a-1775">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="7d05a-1776">DataLake</span><span class="sxs-lookup"><span data-stu-id="7d05a-1776">Datalake</span></span>
* <span data-ttu-id="7d05a-1777">Comandos adicionados para regras da rede virtual</span><span class="sxs-lookup"><span data-stu-id="7d05a-1777">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="7d05a-1778">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1778">Interactive Shell</span></span>
* <span data-ttu-id="7d05a-1779">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1779">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="7d05a-1780">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1780">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="7d05a-1781">IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-1781">IoT</span></span>
* <span data-ttu-id="7d05a-1782">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-1782">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="7d05a-1783">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7d05a-1783">Key Vault</span></span>
* <span data-ttu-id="7d05a-1784">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="7d05a-1784">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-1785">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1785">Network</span></span>
* <span data-ttu-id="7d05a-1786">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="7d05a-1786">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="7d05a-1787">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="7d05a-1787">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="7d05a-1788">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="7d05a-1788">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="7d05a-1789">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="7d05a-1789">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="7d05a-1790">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1790">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="7d05a-1791">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1791">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="7d05a-1792">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1792">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="7d05a-1793">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1793">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="7d05a-1794">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1794">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="7d05a-1795">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1795">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="7d05a-1796">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1796">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="7d05a-1797">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1797">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="7d05a-1798">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1798">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="7d05a-1799">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1799">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="7d05a-1800">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1800">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="7d05a-1801">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="7d05a-1801">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="7d05a-1802">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1802">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="7d05a-1803">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="7d05a-1803">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="7d05a-1804">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1804">RDBMS</span></span>
* <span data-ttu-id="7d05a-1805">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="7d05a-1805">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="7d05a-1806">Reserva</span><span class="sxs-lookup"><span data-stu-id="7d05a-1806">Reservation</span></span>
* <span data-ttu-id="7d05a-1807">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="7d05a-1807">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="7d05a-1808">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="7d05a-1808">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="7d05a-1809">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1809">Manage App</span></span>
* <span data-ttu-id="7d05a-1810">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="7d05a-1810">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="7d05a-1811">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="7d05a-1811">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-1812">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-1812">Role</span></span>
* <span data-ttu-id="7d05a-1813">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="7d05a-1813">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="7d05a-1814">SignalR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1814">SignalR</span></span>
* <span data-ttu-id="7d05a-1815">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="7d05a-1815">First release</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-1816">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1816">Storage</span></span>
* <span data-ttu-id="7d05a-1817">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="7d05a-1817">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="7d05a-1818">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="7d05a-1818">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-1819">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1819">VM</span></span>
* <span data-ttu-id="7d05a-1820">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="7d05a-1820">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="7d05a-1821">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1821">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="7d05a-1822">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-1822">August 28, 2018</span></span>

<span data-ttu-id="7d05a-1823">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="7d05a-1823">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-1824">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1824">Core</span></span>

* <span data-ttu-id="7d05a-1825">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="7d05a-1825">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="7d05a-1826">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="7d05a-1826">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-1827">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1827">ACR</span></span>

* <span data-ttu-id="7d05a-1828">Adicionada uma solução alternativa para operações de runtime sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1828">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="7d05a-1829">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1829">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-1830">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1830">ACS</span></span>

* <span data-ttu-id="7d05a-1831">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1831">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="7d05a-1832">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="7d05a-1832">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-1833">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-1833">AppService</span></span>

* <span data-ttu-id="7d05a-1834">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="7d05a-1834">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="7d05a-1835">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1835">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="7d05a-1836">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1836">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="7d05a-1837">Backup</span><span class="sxs-lookup"><span data-stu-id="7d05a-1837">Backup</span></span>

* <span data-ttu-id="7d05a-1838">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1838">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="7d05a-1839">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="7d05a-1839">Bot Service</span></span>

* <span data-ttu-id="7d05a-1840">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="7d05a-1840">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7d05a-1841">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1841">Cognitive Services</span></span>

* <span data-ttu-id="7d05a-1842">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="7d05a-1842">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="7d05a-1843">IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-1843">IoT</span></span>

* <span data-ttu-id="7d05a-1844">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="7d05a-1844">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="7d05a-1845">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1845">Monitor</span></span>

* <span data-ttu-id="7d05a-1846">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="7d05a-1846">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="7d05a-1847">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1847">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-1848">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1848">Network</span></span>

* <span data-ttu-id="7d05a-1849">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1849">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-1850">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-1850">Resource</span></span>

* <span data-ttu-id="7d05a-1851">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1851">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-1852">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1852">Storage</span></span>

* <span data-ttu-id="7d05a-1853">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1853">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-1854">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1854">VM</span></span>

* <span data-ttu-id="7d05a-1855">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1855">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="7d05a-1856">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1856">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="7d05a-1857">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-1857">Auguest 14, 2018</span></span>

<span data-ttu-id="7d05a-1858">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="7d05a-1858">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-1859">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1859">Core</span></span>

* <span data-ttu-id="7d05a-1860">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1860">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="7d05a-1861">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="7d05a-1861">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="7d05a-1862">Telemetria</span><span class="sxs-lookup"><span data-stu-id="7d05a-1862">Telemetry</span></span>

* <span data-ttu-id="7d05a-1863">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="7d05a-1863">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-1864">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1864">ACR</span></span>

* <span data-ttu-id="7d05a-1865">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1865">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="7d05a-1866">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1866">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-1867">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1867">ACS</span></span>

* <span data-ttu-id="7d05a-1868">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="7d05a-1868">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="7d05a-1869">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1869">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="7d05a-1870">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="7d05a-1870">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="7d05a-1871">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="7d05a-1871">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="7d05a-1872">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="7d05a-1872">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="7d05a-1873">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-1873">AppService</span></span>

* <span data-ttu-id="7d05a-1874">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1874">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="7d05a-1875">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="7d05a-1875">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="7d05a-1876">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7d05a-1876">BatchAI</span></span>

* <span data-ttu-id="7d05a-1877">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1877">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="7d05a-1878">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-1878">Container</span></span>

* <span data-ttu-id="7d05a-1879">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-1879">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="7d05a-1880">IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-1880">IoT</span></span>

* <span data-ttu-id="7d05a-1881">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="7d05a-1881">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="7d05a-1882">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1882">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="7d05a-1883">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-1883">Iot Central</span></span>

* <span data-ttu-id="7d05a-1884">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="7d05a-1884">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="7d05a-1885">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7d05a-1885">KeyVault</span></span>


* <span data-ttu-id="7d05a-1886">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="7d05a-1886">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="7d05a-1887">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1887">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="7d05a-1888">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1888">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="7d05a-1889">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="7d05a-1889">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="7d05a-1890">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="7d05a-1890">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="7d05a-1891">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="7d05a-1891">Relay</span></span>

* <span data-ttu-id="7d05a-1892">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="7d05a-1892">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-1893">Sql</span><span class="sxs-lookup"><span data-stu-id="7d05a-1893">Sql</span></span>

* <span data-ttu-id="7d05a-1894">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1894">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-1895">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1895">Storage</span></span>

* <span data-ttu-id="7d05a-1896">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="7d05a-1896">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="7d05a-1897">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1897">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="7d05a-1898">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="7d05a-1898">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="7d05a-1899">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="7d05a-1899">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="7d05a-1900">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-1900">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-1901">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1901">VM</span></span>

* <span data-ttu-id="7d05a-1902">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="7d05a-1902">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="7d05a-1903">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-1903">July 31, 2018</span></span>

<span data-ttu-id="7d05a-1904">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="7d05a-1904">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-1905">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1905">ACR</span></span>

* <span data-ttu-id="7d05a-1906">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1906">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="7d05a-1907">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1907">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-1908">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1908">ACS</span></span>

* <span data-ttu-id="7d05a-1909">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="7d05a-1909">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="7d05a-1910">Lote</span><span class="sxs-lookup"><span data-stu-id="7d05a-1910">Batch</span></span>

* <span data-ttu-id="7d05a-1911">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="7d05a-1911">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="7d05a-1912">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-1912">Container</span></span>

* <span data-ttu-id="7d05a-1913">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="7d05a-1913">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-1914">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1914">Network</span></span>

* <span data-ttu-id="7d05a-1915">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="7d05a-1915">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="7d05a-1916">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-1916">Resource</span></span>

* <span data-ttu-id="7d05a-1917">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="7d05a-1917">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="7d05a-1918">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="7d05a-1918">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-1919">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-1919">Role</span></span>

* <span data-ttu-id="7d05a-1920">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="7d05a-1920">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="7d05a-1921">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1921">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="7d05a-1922">Search</span><span class="sxs-lookup"><span data-stu-id="7d05a-1922">Search</span></span>

* <span data-ttu-id="7d05a-1923">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="7d05a-1923">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="7d05a-1924">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="7d05a-1924">Service Bus</span></span>

* <span data-ttu-id="7d05a-1925">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="7d05a-1925">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="7d05a-1926">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="7d05a-1926">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="7d05a-1927">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1927">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="7d05a-1928">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1928">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-1929">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1929">Storage</span></span>

* <span data-ttu-id="7d05a-1930">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="7d05a-1930">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="7d05a-1931">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1931">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-1932">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1932">VM</span></span>

* <span data-ttu-id="7d05a-1933">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="7d05a-1933">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="7d05a-1934">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1934">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="7d05a-1935">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1935">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="7d05a-1936">[ALTERAÇÃO SIGNIFICATIVA]`[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="7d05a-1936">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="7d05a-1937">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-1937">July 18, 2018</span></span>

<span data-ttu-id="7d05a-1938">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="7d05a-1938">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-1939">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1939">Core</span></span>

* <span data-ttu-id="7d05a-1940">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="7d05a-1940">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="7d05a-1941">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="7d05a-1941">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="7d05a-1942">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1942">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-1943">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1943">ACR</span></span>

* <span data-ttu-id="7d05a-1944">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="7d05a-1944">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="7d05a-1945">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1945">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="7d05a-1946">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="7d05a-1946">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="7d05a-1947">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="7d05a-1947">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-1948">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1948">ACS</span></span>

* <span data-ttu-id="7d05a-1949">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="7d05a-1949">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-1950">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-1950">AppService</span></span>

* <span data-ttu-id="7d05a-1951">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="7d05a-1951">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="7d05a-1952">Lote</span><span class="sxs-lookup"><span data-stu-id="7d05a-1952">Batch</span></span>

* <span data-ttu-id="7d05a-1953">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="7d05a-1953">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="7d05a-1954">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="7d05a-1954">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7d05a-1955">Lote AI</span><span class="sxs-lookup"><span data-stu-id="7d05a-1955">Batch AI</span></span>

* <span data-ttu-id="7d05a-1956">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1956">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="7d05a-1957">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-1957">Container</span></span>

* <span data-ttu-id="7d05a-1958">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="7d05a-1958">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="7d05a-1959">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="7d05a-1959">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-1960">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-1960">Network</span></span>

* <span data-ttu-id="7d05a-1961">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1961">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="7d05a-1962">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1962">Added `network nic wait`</span></span>
* <span data-ttu-id="7d05a-1963">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1963">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="7d05a-1964">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1964">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="7d05a-1965">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-1965">Resource</span></span>

* <span data-ttu-id="7d05a-1966">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1966">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="7d05a-1967">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1967">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="7d05a-1968">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1968">Added `deployment wait` command</span></span>
* <span data-ttu-id="7d05a-1969">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="7d05a-1969">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-1970">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-1970">SQL</span></span>

* <span data-ttu-id="7d05a-1971">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1971">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="7d05a-1972">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1972">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="7d05a-1973">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1973">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-1974">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-1974">Storage</span></span>

* <span data-ttu-id="7d05a-1975">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="7d05a-1975">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-1976">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-1976">VM</span></span>

* <span data-ttu-id="7d05a-1977">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="7d05a-1977">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="7d05a-1978">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1978">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="7d05a-1979">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1979">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="7d05a-1980">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-1980">July 3, 2018</span></span>

<span data-ttu-id="7d05a-1981">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="7d05a-1981">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="7d05a-1982">AKS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1982">AKS</span></span>

* <span data-ttu-id="7d05a-1983">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="7d05a-1983">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="7d05a-1984">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-1984">July 3, 2018</span></span>

<span data-ttu-id="7d05a-1985">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="7d05a-1985">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-1986">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1986">Core</span></span>

* <span data-ttu-id="7d05a-1987">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-1987">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-1988">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-1988">ACR</span></span>

* <span data-ttu-id="7d05a-1989">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="7d05a-1989">Added polling build status</span></span>
* <span data-ttu-id="7d05a-1990">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="7d05a-1990">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="7d05a-1991">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="7d05a-1991">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-1992">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-1992">ACS</span></span>

* <span data-ttu-id="7d05a-1993">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="7d05a-1993">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="7d05a-1994">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="7d05a-1994">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="7d05a-1995">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1995">Updated options for `aks browse` command.</span></span> <span data-ttu-id="7d05a-1996">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="7d05a-1996">Added `--listen-port` support</span></span>
* <span data-ttu-id="7d05a-1997">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-1997">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="7d05a-1998">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="7d05a-1998">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="7d05a-1999">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="7d05a-1999">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-2000">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-2000">AppService</span></span>

* <span data-ttu-id="7d05a-2001">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2001">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="7d05a-2002">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="7d05a-2002">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="7d05a-2003">Backup</span><span class="sxs-lookup"><span data-stu-id="7d05a-2003">Backup</span></span>

* <span data-ttu-id="7d05a-2004">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="7d05a-2004">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="7d05a-2005">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7d05a-2005">BatchAI</span></span>

* <span data-ttu-id="7d05a-2006">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2006">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="7d05a-2007">Nuvem</span><span class="sxs-lookup"><span data-stu-id="7d05a-2007">Cloud</span></span>

* <span data-ttu-id="7d05a-2008">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="7d05a-2008">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="7d05a-2009">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-2009">Container</span></span>

* <span data-ttu-id="7d05a-2010">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="7d05a-2010">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="7d05a-2011">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="7d05a-2011">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="7d05a-2012">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="7d05a-2012">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="7d05a-2013">Extensão</span><span class="sxs-lookup"><span data-stu-id="7d05a-2013">Extension</span></span>

* <span data-ttu-id="7d05a-2014">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="7d05a-2014">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-2015">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-2015">Network</span></span>

* <span data-ttu-id="7d05a-2016">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="7d05a-2016">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="7d05a-2017">Rdbms</span><span class="sxs-lookup"><span data-stu-id="7d05a-2017">Rdbms</span></span>

* <span data-ttu-id="7d05a-2018">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2018">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-2019">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-2019">Resource</span></span>

* <span data-ttu-id="7d05a-2020">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="7d05a-2020">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2021">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2021">VM</span></span>

* <span data-ttu-id="7d05a-2022">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="7d05a-2022">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="7d05a-2023">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-2023">June 25, 2018</span></span>

<span data-ttu-id="7d05a-2024">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="7d05a-2024">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="7d05a-2025">CLI</span><span class="sxs-lookup"><span data-stu-id="7d05a-2025">CLI</span></span>

* <span data-ttu-id="7d05a-2026">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="7d05a-2026">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="7d05a-2027">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-2027">June 19, 2018</span></span>

<span data-ttu-id="7d05a-2028">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="7d05a-2028">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-2029">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2029">Core</span></span>

* <span data-ttu-id="7d05a-2030">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2030">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-2031">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-2031">ACR</span></span>

* <span data-ttu-id="7d05a-2032">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="7d05a-2032">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="7d05a-2033">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2033">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-2034">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2034">ACS</span></span>

* <span data-ttu-id="7d05a-2035">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2035">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="7d05a-2036">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="7d05a-2036">Added `--update` support</span></span>
* <span data-ttu-id="7d05a-2037">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2037">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="7d05a-2038">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="7d05a-2038">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="7d05a-2039">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="7d05a-2039">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="7d05a-2040">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2040">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="7d05a-2041">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2041">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="7d05a-2042">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2042">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-2043">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-2043">AppService</span></span>

* <span data-ttu-id="7d05a-2044">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="7d05a-2044">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="7d05a-2045">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2045">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="7d05a-2046">Lote</span><span class="sxs-lookup"><span data-stu-id="7d05a-2046">Batch</span></span>

* <span data-ttu-id="7d05a-2047">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="7d05a-2047">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7d05a-2048">Lote AI</span><span class="sxs-lookup"><span data-stu-id="7d05a-2048">Batch AI</span></span>

* <span data-ttu-id="7d05a-2049">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2049">Added support for workspaces.</span></span> <span data-ttu-id="7d05a-2050">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="7d05a-2050">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="7d05a-2051">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2051">Added support for experiments.</span></span> <span data-ttu-id="7d05a-2052">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="7d05a-2052">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="7d05a-2053">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="7d05a-2053">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="7d05a-2054">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2054">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="7d05a-2055">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2055">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="7d05a-2056">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2056">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="7d05a-2057">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="7d05a-2057">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="7d05a-2058">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="7d05a-2058">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="7d05a-2059">[ALTERAÇÃO SIGNIFICATIVA]`--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2059">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="7d05a-2060">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2060">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="7d05a-2061">[ALTERAÇÃO SIGNIFICATIVA]`--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2061">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="7d05a-2062">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2062">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="7d05a-2063">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2063">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="7d05a-2064">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2064">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="7d05a-2065">[ALTERAÇÃO SIGNIFICATIVA]`--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2065">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="7d05a-2066">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="7d05a-2066">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="7d05a-2067">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="7d05a-2067">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="7d05a-2068">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="7d05a-2068">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="7d05a-2069">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="7d05a-2069">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="7d05a-2070">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="7d05a-2070">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="7d05a-2071">Mapas</span><span class="sxs-lookup"><span data-stu-id="7d05a-2071">Maps</span></span>

* <span data-ttu-id="7d05a-2072">[ALTERAÇÃO SIGNIFICATIVA]`maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2072">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-2073">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-2073">Network</span></span>

* <span data-ttu-id="7d05a-2074">Suporte adicionado para `https` a `network lb probe create` [nº6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="7d05a-2074">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="7d05a-2075">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2075">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="7d05a-2076">#6502</span><span class="sxs-lookup"><span data-stu-id="7d05a-2076">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="7d05a-2077">Reservas</span><span class="sxs-lookup"><span data-stu-id="7d05a-2077">Reservations</span></span>

* <span data-ttu-id="7d05a-2078">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2078">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="7d05a-2079">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2079">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="7d05a-2080">[ALTERAÇÃO SIGNIFICATIVA]`kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2080">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="7d05a-2081">[ALTERAÇÃO SIGNIFICATIVA]`capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2081">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="7d05a-2082">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2082">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="7d05a-2083">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2083">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-2084">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-2084">Role</span></span>

* <span data-ttu-id="7d05a-2085">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="7d05a-2085">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-2086">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-2086">SQL</span></span>

* <span data-ttu-id="7d05a-2087">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="7d05a-2087">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-2088">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2088">Storage</span></span>

* <span data-ttu-id="7d05a-2089">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="7d05a-2089">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2090">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2090">VM</span></span>

* <span data-ttu-id="7d05a-2091">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2091">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="7d05a-2092">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2092">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="7d05a-2093">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="7d05a-2093">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="7d05a-2094">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-2094">June 13, 2018</span></span>

<span data-ttu-id="7d05a-2095">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="7d05a-2095">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-2096">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2096">Core</span></span>

* <span data-ttu-id="7d05a-2097">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="7d05a-2097">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="7d05a-2098">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-2098">June 13, 2018</span></span>

<span data-ttu-id="7d05a-2099">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="7d05a-2099">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="7d05a-2100">AKS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2100">AKS</span></span>

* <span data-ttu-id="7d05a-2101">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2101">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="7d05a-2102">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="7d05a-2102">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="7d05a-2103">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2103">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="7d05a-2104">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2104">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="7d05a-2105">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2105">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-2106">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-2106">AppService</span></span>

* <span data-ttu-id="7d05a-2107">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="7d05a-2107">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="7d05a-2108">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-2108">June 5, 2018</span></span>

<span data-ttu-id="7d05a-2109">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="7d05a-2109">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="7d05a-2110">Interativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2110">Interactive</span></span>

* <span data-ttu-id="7d05a-2111">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2111">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="7d05a-2112">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-2112">June 5, 2018</span></span>

<span data-ttu-id="7d05a-2113">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="7d05a-2113">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-2114">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2114">Core</span></span>

* <span data-ttu-id="7d05a-2115">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="7d05a-2115">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="7d05a-2116">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="7d05a-2116">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-2117">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-2117">ACR</span></span>

* <span data-ttu-id="7d05a-2118">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="7d05a-2118">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="7d05a-2119">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2119">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="7d05a-2120">AKS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2120">AKS</span></span>

* <span data-ttu-id="7d05a-2121">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="7d05a-2121">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="7d05a-2122">Lote</span><span class="sxs-lookup"><span data-stu-id="7d05a-2122">Batch</span></span>

* <span data-ttu-id="7d05a-2123">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="7d05a-2123">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="7d05a-2124">IOT</span><span class="sxs-lookup"><span data-stu-id="7d05a-2124">IOT</span></span>

* <span data-ttu-id="7d05a-2125">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="7d05a-2125">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-2126">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-2126">Network</span></span>

* <span data-ttu-id="7d05a-2127">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="7d05a-2127">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="7d05a-2128">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="7d05a-2128">Policy Insights</span></span>

* <span data-ttu-id="7d05a-2129">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="7d05a-2129">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="7d05a-2130">ARM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2130">ARM</span></span>

* <span data-ttu-id="7d05a-2131">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2131">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-2132">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-2132">SQL</span></span>

* <span data-ttu-id="7d05a-2133">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="7d05a-2133">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="7d05a-2134">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="7d05a-2134">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="7d05a-2135">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2135">Storage</span></span>

* <span data-ttu-id="7d05a-2136">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2136">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2137">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2137">VM</span></span>

* <span data-ttu-id="7d05a-2138">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2138">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="7d05a-2139">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2139">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="7d05a-2140">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2140">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="7d05a-2141">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-2141">May 22, 2018</span></span>

<span data-ttu-id="7d05a-2142">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="7d05a-2142">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-2143">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2143">Core</span></span>

* <span data-ttu-id="7d05a-2144">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2144">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-2145">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2145">ACS</span></span>

* <span data-ttu-id="7d05a-2146">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="7d05a-2146">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="7d05a-2147">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="7d05a-2147">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-2148">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-2148">AppService</span></span>

* <span data-ttu-id="7d05a-2149">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="7d05a-2149">Improved generic update commands</span></span>
* <span data-ttu-id="7d05a-2150">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2150">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="7d05a-2151">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-2151">Container</span></span>

* <span data-ttu-id="7d05a-2152">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="7d05a-2152">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="7d05a-2153">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-2153">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="7d05a-2154">Extensão</span><span class="sxs-lookup"><span data-stu-id="7d05a-2154">Extension</span></span>

* <span data-ttu-id="7d05a-2155">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="7d05a-2155">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="7d05a-2156">Interativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2156">Interactive</span></span>

* <span data-ttu-id="7d05a-2157">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="7d05a-2157">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="7d05a-2158">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="7d05a-2158">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="7d05a-2159">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7d05a-2159">KeyVault</span></span>

* <span data-ttu-id="7d05a-2160">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="7d05a-2160">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-2161">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-2161">Network</span></span>

* <span data-ttu-id="7d05a-2162">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="7d05a-2162">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="7d05a-2163">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="7d05a-2163">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-2164">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-2164">SQL</span></span>

* <span data-ttu-id="7d05a-2165">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="7d05a-2165">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="7d05a-2166">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2166">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="7d05a-2167">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="7d05a-2167">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="7d05a-2168">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d05a-2168">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="7d05a-2169">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="7d05a-2169">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="7d05a-2170">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2170">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="7d05a-2171">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2171">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="7d05a-2172">`edition`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2172">`edition`.</span></span> <span data-ttu-id="7d05a-2173">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2173">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="7d05a-2174">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2174">`elasticPoolName`.</span></span> <span data-ttu-id="7d05a-2175">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2175">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="7d05a-2176">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="7d05a-2176">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="7d05a-2177">`edition`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2177">`edition`.</span></span> <span data-ttu-id="7d05a-2178">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2178">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="7d05a-2179">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2179">`dtu`.</span></span> <span data-ttu-id="7d05a-2180">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2180">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="7d05a-2181">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2181">`databaseDtuMin`.</span></span> <span data-ttu-id="7d05a-2182">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2182">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="7d05a-2183">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2183">`databaseDtuMax`.</span></span> <span data-ttu-id="7d05a-2184">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2184">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="7d05a-2185">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2185">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="7d05a-2186">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2186">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-2187">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2187">Storage</span></span>

* <span data-ttu-id="7d05a-2188">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2188">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="7d05a-2189">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="7d05a-2189">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2190">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2190">VM</span></span>

* <span data-ttu-id="7d05a-2191">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2191">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="7d05a-2192">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2192">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="7d05a-2193">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2193">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="7d05a-2194">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="7d05a-2194">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="7d05a-2195">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2195">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="7d05a-2196">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-2196">May 7, 2018</span></span>

<span data-ttu-id="7d05a-2197">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="7d05a-2197">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-2198">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2198">Core</span></span>

* <span data-ttu-id="7d05a-2199">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="7d05a-2199">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="7d05a-2200">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="7d05a-2200">Added limited support for positional arguments</span></span>
* <span data-ttu-id="7d05a-2201">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2201">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="7d05a-2202">#5591</span><span class="sxs-lookup"><span data-stu-id="7d05a-2202">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="7d05a-2203">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2203">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="7d05a-2204">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="7d05a-2204">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="7d05a-2205">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2205">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="7d05a-2206">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2206">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="7d05a-2207">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="7d05a-2207">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-2208">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-2208">ACR</span></span>

* <span data-ttu-id="7d05a-2209">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-2209">Added ACR Build commands</span></span>
* <span data-ttu-id="7d05a-2210">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="7d05a-2210">Improved resource not found error messages</span></span>
* <span data-ttu-id="7d05a-2211">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="7d05a-2211">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="7d05a-2212">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="7d05a-2212">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="7d05a-2213">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="7d05a-2213">Improved repository commands error messages</span></span>
* <span data-ttu-id="7d05a-2214">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="7d05a-2214">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-2215">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2215">ACS</span></span>

* <span data-ttu-id="7d05a-2216">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="7d05a-2216">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="7d05a-2217">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="7d05a-2217">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="7d05a-2218">AMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2218">AMS</span></span>

* <span data-ttu-id="7d05a-2219">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="7d05a-2219">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-2220">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-2220">Appservice</span></span>

* <span data-ttu-id="7d05a-2221">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="7d05a-2221">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="7d05a-2222">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2222">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="7d05a-2223">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="7d05a-2223">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="7d05a-2224">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="7d05a-2224">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7d05a-2225">Lote AI</span><span class="sxs-lookup"><span data-stu-id="7d05a-2225">Batch AI</span></span>

* <span data-ttu-id="7d05a-2226">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="7d05a-2226">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7d05a-2227">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2227">Cognitive Services</span></span>

* <span data-ttu-id="7d05a-2228">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create`[#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="7d05a-2228">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="7d05a-2229">Consumo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2229">Consumption</span></span>

* <span data-ttu-id="7d05a-2230">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2230">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="7d05a-2231">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-2231">Container</span></span>

* <span data-ttu-id="7d05a-2232">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="7d05a-2232">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="7d05a-2233">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7d05a-2233">Cosmos DB</span></span>

* <span data-ttu-id="7d05a-2234">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7d05a-2234">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="7d05a-2235">DMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2235">DMS</span></span>

* <span data-ttu-id="7d05a-2236">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="7d05a-2236">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="7d05a-2237">Extensão</span><span class="sxs-lookup"><span data-stu-id="7d05a-2237">Extension</span></span>

* <span data-ttu-id="7d05a-2238">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2238">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="7d05a-2239">Interativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2239">Interactive</span></span>

* <span data-ttu-id="7d05a-2240">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="7d05a-2240">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="7d05a-2241">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="7d05a-2241">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="7d05a-2242">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="7d05a-2242">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="7d05a-2243">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="7d05a-2243">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="7d05a-2244">Laboratório</span><span class="sxs-lookup"><span data-stu-id="7d05a-2244">Lab</span></span>

* <span data-ttu-id="7d05a-2245">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="7d05a-2245">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-2246">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-2246">Network</span></span>

* <span data-ttu-id="7d05a-2247">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="7d05a-2247">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="7d05a-2248">Perfil</span><span class="sxs-lookup"><span data-stu-id="7d05a-2248">Profile</span></span>

* <span data-ttu-id="7d05a-2249">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="7d05a-2249">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="7d05a-2250">[ALTERAÇÃO SIGNIFICATIVA]`--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="7d05a-2250">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="7d05a-2251">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2251">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="7d05a-2252">Redis</span><span class="sxs-lookup"><span data-stu-id="7d05a-2252">Redis</span></span>

* <span data-ttu-id="7d05a-2253">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2253">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="7d05a-2254">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2254">Deprecated `redis list-all`.</span></span> <span data-ttu-id="7d05a-2255">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2255">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="7d05a-2256">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2256">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="7d05a-2257">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2257">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-2258">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-2258">Role</span></span>

* <span data-ttu-id="7d05a-2259">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="7d05a-2259">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-2260">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2260">Storage</span></span>

* <span data-ttu-id="7d05a-2261">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="7d05a-2261">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="7d05a-2262">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="7d05a-2262">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="7d05a-2263">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2263">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="7d05a-2264">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="7d05a-2264">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="7d05a-2265">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="7d05a-2265">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2266">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2266">VM</span></span>

* <span data-ttu-id="7d05a-2267">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="7d05a-2267">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="7d05a-2268">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="7d05a-2268">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="7d05a-2269">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="7d05a-2269">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="7d05a-2270">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2270">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="7d05a-2271">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="7d05a-2271">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="7d05a-2272">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="7d05a-2272">Added write accelerator support</span></span>
* <span data-ttu-id="7d05a-2273">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2273">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="7d05a-2274">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="7d05a-2274">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="7d05a-2275">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="7d05a-2275">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="7d05a-2276">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-2276">April 10, 2018</span></span>

<span data-ttu-id="7d05a-2277">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="7d05a-2277">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-2278">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-2278">ACR</span></span>

* <span data-ttu-id="7d05a-2279">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="7d05a-2279">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-2280">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2280">ACS</span></span>

* <span data-ttu-id="7d05a-2281">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2281">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-2282">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-2282">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="7d05a-2284">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="7d05a-2284">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="7d05a-2285">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7d05a-2285">BatchAI</span></span>

* <span data-ttu-id="7d05a-2286">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="7d05a-2286">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="7d05a-2287">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="7d05a-2287">Job level mounting</span></span>
  - <span data-ttu-id="7d05a-2288">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2288">Environment variables with secret values</span></span>
  - <span data-ttu-id="7d05a-2289">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="7d05a-2289">Performance counters settings</span></span>
  - <span data-ttu-id="7d05a-2290">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="7d05a-2290">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="7d05a-2291">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="7d05a-2291">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="7d05a-2292">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="7d05a-2292">Usage and limits reporting</span></span>
  - <span data-ttu-id="7d05a-2293">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2293">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="7d05a-2294">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="7d05a-2294">Support for custom images</span></span>
  - <span data-ttu-id="7d05a-2295">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="7d05a-2295">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="7d05a-2296">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="7d05a-2296">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="7d05a-2297">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="7d05a-2297">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="7d05a-2298">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="7d05a-2298">National clouds are supported</span></span>
* <span data-ttu-id="7d05a-2299">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="7d05a-2299">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="7d05a-2300">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="7d05a-2300">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="7d05a-2301">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="7d05a-2301">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="7d05a-2302">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2302">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="7d05a-2303">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="7d05a-2303">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="7d05a-2304">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="7d05a-2304">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="7d05a-2305">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2305">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="7d05a-2306">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2306">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="7d05a-2307">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="7d05a-2307">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="7d05a-2308">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2308">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="7d05a-2309">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="7d05a-2309">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="7d05a-2310">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2310">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="7d05a-2311">[ALTERAÇÃO SIGNIFICATIVA]`--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2311">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="7d05a-2312">Cobrança</span><span class="sxs-lookup"><span data-stu-id="7d05a-2312">Billing</span></span>

* <span data-ttu-id="7d05a-2313">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="7d05a-2313">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="7d05a-2314">Consumo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2314">Consumption</span></span>

* <span data-ttu-id="7d05a-2315">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2315">Added `marketplace` commands</span></span>
* <span data-ttu-id="7d05a-2316">[ALTERAÇÃO SIGNIFICATIVA]`reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2316">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="7d05a-2317">[ALTERAÇÃO SIGNIFICATIVA]`reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2317">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="7d05a-2318">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2318">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="7d05a-2319">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2319">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="7d05a-2320">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2320">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="7d05a-2321">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-2321">Container</span></span>

* <span data-ttu-id="7d05a-2322">Adição dos parâmetros de montagem de volume do Repositório Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2322">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="7d05a-2323">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="7d05a-2323">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="7d05a-2324">Extensão</span><span class="sxs-lookup"><span data-stu-id="7d05a-2324">Extension</span></span>

* <span data-ttu-id="7d05a-2325">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="7d05a-2325">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="7d05a-2326">Interativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2326">Interactive</span></span>

* <span data-ttu-id="7d05a-2327">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2327">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="7d05a-2328">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="7d05a-2328">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="7d05a-2329">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2329">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-2330">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-2330">Network</span></span>

* <span data-ttu-id="7d05a-2331">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="7d05a-2331">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="7d05a-2332">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2332">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="7d05a-2333">#4910</span><span class="sxs-lookup"><span data-stu-id="7d05a-2333">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="7d05a-2334">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2334">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="7d05a-2335">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2335">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="7d05a-2336">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2336">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="7d05a-2337">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2337">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="7d05a-2338">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2338">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="7d05a-2339">Perfil</span><span class="sxs-lookup"><span data-stu-id="7d05a-2339">Profile</span></span>

* <span data-ttu-id="7d05a-2340">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2340">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="7d05a-2341">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2341">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="7d05a-2342">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2342">RDBMS</span></span>

* <span data-ttu-id="7d05a-2343">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2343">Added `georestore` command</span></span>
* <span data-ttu-id="7d05a-2344">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2344">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-2345">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-2345">Resource</span></span>

* <span data-ttu-id="7d05a-2346">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2346">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="7d05a-2347">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2347">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-2348">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-2348">SQL</span></span>

* <span data-ttu-id="7d05a-2349">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2349">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-2350">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2350">Storage</span></span>

* <span data-ttu-id="7d05a-2351">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="7d05a-2351">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2352">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2352">VM</span></span>

* <span data-ttu-id="7d05a-2353">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2353">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="7d05a-2354">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2354">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="7d05a-2356">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2356">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="7d05a-2357">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2357">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="7d05a-2358">#5718</span><span class="sxs-lookup"><span data-stu-id="7d05a-2358">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="7d05a-2359">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="7d05a-2359">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="7d05a-2360">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-2360">March 27, 2018</span></span>

<span data-ttu-id="7d05a-2361">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="7d05a-2361">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-2362">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2362">Core</span></span>

* <span data-ttu-id="7d05a-2363">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="7d05a-2363">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-2364">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2364">ACS</span></span>

* <span data-ttu-id="7d05a-2365">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="7d05a-2365">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-2366">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-2366">Appservice</span></span>

* <span data-ttu-id="7d05a-2367">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2367">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="7d05a-2368">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2368">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="7d05a-2369">Backup</span><span class="sxs-lookup"><span data-stu-id="7d05a-2369">Backup</span></span>

* <span data-ttu-id="7d05a-2370">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2370">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="7d05a-2371">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="7d05a-2371">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="7d05a-2372">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="7d05a-2372">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="7d05a-2373">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2373">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="7d05a-2374">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-2374">Container</span></span>

* <span data-ttu-id="7d05a-2375">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2375">Added `container exec` command.</span></span> <span data-ttu-id="7d05a-2376">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="7d05a-2376">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="7d05a-2377">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-2377">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="7d05a-2378">Extensão</span><span class="sxs-lookup"><span data-stu-id="7d05a-2378">Extension</span></span>

* <span data-ttu-id="7d05a-2379">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="7d05a-2379">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="7d05a-2380">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2380">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="7d05a-2381">[ALTERAÇÃO SIGNIFICATIVA]`extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="7d05a-2381">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="7d05a-2382">Interativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2382">Interactive</span></span>

* <span data-ttu-id="7d05a-2383">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2383">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="7d05a-2384">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2384">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="7d05a-2385">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2385">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="7d05a-2386">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="7d05a-2386">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="7d05a-2387">Laboratório</span><span class="sxs-lookup"><span data-stu-id="7d05a-2387">Lab</span></span>

* <span data-ttu-id="7d05a-2388">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2388">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="7d05a-2389">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2389">Monitor</span></span>

* <span data-ttu-id="7d05a-2390">Adicionado suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [nº5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="7d05a-2390">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="7d05a-2391">Corrigido [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="7d05a-2391">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="7d05a-2392">Suporte adicionado para `--namespace` a `metrics list-definitions` [nº5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="7d05a-2392">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-2393">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-2393">Network</span></span>

* <span data-ttu-id="7d05a-2394">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="7d05a-2394">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="7d05a-2395">Perfil</span><span class="sxs-lookup"><span data-stu-id="7d05a-2395">Profile</span></span>

* <span data-ttu-id="7d05a-2396">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2396">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="7d05a-2397">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2397">RDBMS</span></span>

* <span data-ttu-id="7d05a-2398">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="7d05a-2398">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-2399">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-2399">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="7d05a-2401">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-2401">Role</span></span>

* <span data-ttu-id="7d05a-2402">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2402">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="7d05a-2403">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="7d05a-2403">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="7d05a-2404">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2404">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="7d05a-2405">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2405">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="7d05a-2406">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2406">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-2407">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2407">Storage</span></span>

* <span data-ttu-id="7d05a-2408">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="7d05a-2408">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="7d05a-2409">Corrigido [#4049](https://github.com/Azure/azure-cli/issues/4049): problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="7d05a-2409">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2410">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2410">VM</span></span>

* <span data-ttu-id="7d05a-2411">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="7d05a-2411">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="7d05a-2412">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2412">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="7d05a-2413">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="7d05a-2413">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="7d05a-2414">[ALTERAÇÃO SIGNIFICATIVA]`vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="7d05a-2414">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="7d05a-2415">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-2415">March 13, 2018</span></span>

<span data-ttu-id="7d05a-2416">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="7d05a-2416">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-2417">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-2417">ACR</span></span>

* <span data-ttu-id="7d05a-2418">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2418">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="7d05a-2419">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2419">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="7d05a-2420">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="7d05a-2420">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-2421">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2421">ACS</span></span>

* <span data-ttu-id="7d05a-2422">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="7d05a-2422">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="7d05a-2423">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="7d05a-2423">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="7d05a-2424">Supervisor</span><span class="sxs-lookup"><span data-stu-id="7d05a-2424">Advisor</span></span>

* <span data-ttu-id="7d05a-2425">[ALTERAÇÃO SIGNIFICATIVA]`advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2425">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="7d05a-2426">[ALTERAÇÃO SIGNIFICATIVA]`advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2426">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="7d05a-2427">[ALTERAÇÃO SIGNIFICATIVA]`advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="7d05a-2427">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="7d05a-2428">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2428">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="7d05a-2429">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2429">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-2430">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-2430">Appservice</span></span>

* <span data-ttu-id="7d05a-2431">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2431">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="7d05a-2432">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="7d05a-2432">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="7d05a-2433">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2433">Eventhubs</span></span>

* <span data-ttu-id="7d05a-2434">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="7d05a-2434">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="7d05a-2435">Extensão</span><span class="sxs-lookup"><span data-stu-id="7d05a-2435">Extension</span></span>

* <span data-ttu-id="7d05a-2436">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="7d05a-2436">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="7d05a-2437">Interativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2437">Interactive</span></span>

* <span data-ttu-id="7d05a-2438">Corrigido [#5625](https://github.com/Azure/azure-cli/issues/5625): manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="7d05a-2438">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="7d05a-2439">Corrigido [#3016](https://github.com/Azure/azure-cli/issues/3016): histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2439">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="7d05a-2440">Corrigido [#5688](https://github.com/Azure/azure-cli/issues/5688): as conclusões não aparecerão se o carregamento da tabela de comando encontrar uma exceção</span><span class="sxs-lookup"><span data-stu-id="7d05a-2440">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="7d05a-2441">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="7d05a-2441">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="7d05a-2442">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2442">Monitor</span></span>

* <span data-ttu-id="7d05a-2443">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2443">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="7d05a-2444">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2444">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="7d05a-2445">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2445">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="7d05a-2446">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2446">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-2447">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-2447">Network</span></span>

* <span data-ttu-id="7d05a-2448">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2448">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="7d05a-2449">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="7d05a-2449">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="7d05a-2450">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="7d05a-2450">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="7d05a-2451">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2451">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="7d05a-2452">Perfil</span><span class="sxs-lookup"><span data-stu-id="7d05a-2452">Profile</span></span>

* <span data-ttu-id="7d05a-2453">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2453">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="7d05a-2454">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2454">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="7d05a-2455">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2455">RDBMS</span></span>

* <span data-ttu-id="7d05a-2456">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="7d05a-2456">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="7d05a-2457">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="7d05a-2457">Service Bus</span></span>

* <span data-ttu-id="7d05a-2458">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="7d05a-2458">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-2459">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2459">Storage</span></span>

* <span data-ttu-id="7d05a-2460">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="7d05a-2460">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="7d05a-2461">Corrigido [#5286](https://github.com/Azure/azure-cli/issues/5286): os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="7d05a-2461">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2462">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2462">VM</span></span>

* <span data-ttu-id="7d05a-2463">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="7d05a-2463">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="7d05a-2464">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2464">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="7d05a-2465">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2465">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="7d05a-2466">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="7d05a-2466">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="7d05a-2467">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-2467">February 27, 2018</span></span>

<span data-ttu-id="7d05a-2468">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="7d05a-2468">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-2469">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2469">Core</span></span>

* <span data-ttu-id="7d05a-2470">Corrigido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="7d05a-2470">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="7d05a-2471">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="7d05a-2471">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="7d05a-2472">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2472">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-2473">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2473">ACS</span></span>

* <span data-ttu-id="7d05a-2474">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="7d05a-2474">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="7d05a-2475">Problema corrigido: permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="7d05a-2475">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="7d05a-2476">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2476">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="7d05a-2477">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2477">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-2478">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-2478">Appservice</span></span>

* <span data-ttu-id="7d05a-2479">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="7d05a-2479">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="7d05a-2480">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="7d05a-2480">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7d05a-2481">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2481">Cognitive Services</span></span>

* <span data-ttu-id="7d05a-2482">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2482">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="7d05a-2483">Consumo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2483">Consumption</span></span>

* <span data-ttu-id="7d05a-2484">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="7d05a-2484">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="7d05a-2485">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="7d05a-2485">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="7d05a-2486">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-2486">Container</span></span>

* <span data-ttu-id="7d05a-2487">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="7d05a-2487">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-2488">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-2488">Network</span></span>

* <span data-ttu-id="7d05a-2489">Corrigido [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2489">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-2490">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-2490">Resource</span></span>

* <span data-ttu-id="7d05a-2491">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="7d05a-2491">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-2492">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-2492">Role</span></span>

* <span data-ttu-id="7d05a-2493">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="7d05a-2493">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-2494">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-2494">SQL</span></span>

* <span data-ttu-id="7d05a-2495">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="7d05a-2495">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-2496">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2496">Storage</span></span>

* <span data-ttu-id="7d05a-2497">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2497">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2498">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2498">VM</span></span>

* <span data-ttu-id="7d05a-2499">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2499">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="7d05a-2500">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-2500">February 13, 2018</span></span>

<span data-ttu-id="7d05a-2501">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="7d05a-2501">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-2502">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2502">Core</span></span>

* <span data-ttu-id="7d05a-2503">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="7d05a-2503">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-2504">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2504">ACS</span></span>

* <span data-ttu-id="7d05a-2505">[ALTERAÇÃO SIGNIFICATIVA]`aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="7d05a-2505">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="7d05a-2506">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2506">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="7d05a-2507">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="7d05a-2507">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="7d05a-2508">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2508">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="7d05a-2509">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="7d05a-2509">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="7d05a-2510">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2510">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="7d05a-2511">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="7d05a-2511">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="7d05a-2512">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2512">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-2513">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-2513">Appservice</span></span>

* <span data-ttu-id="7d05a-2514">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="7d05a-2514">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="7d05a-2515">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2515">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="7d05a-2516">CDN</span><span class="sxs-lookup"><span data-stu-id="7d05a-2516">CDN</span></span>

* <span data-ttu-id="7d05a-2517">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2517">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="7d05a-2518">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-2518">Container</span></span>

* <span data-ttu-id="7d05a-2519">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="7d05a-2519">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="7d05a-2520">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-2520">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7d05a-2521">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7d05a-2521">CosmosDB</span></span>

* <span data-ttu-id="7d05a-2522">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2522">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="7d05a-2523">Extensão</span><span class="sxs-lookup"><span data-stu-id="7d05a-2523">Extension</span></span>

* <span data-ttu-id="7d05a-2524">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2524">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="7d05a-2525">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2525">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="7d05a-2526">Comentários</span><span class="sxs-lookup"><span data-stu-id="7d05a-2526">Feedback</span></span>

* <span data-ttu-id="7d05a-2527">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="7d05a-2527">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="7d05a-2528">Interativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2528">Interactive</span></span>

* <span data-ttu-id="7d05a-2529">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="7d05a-2529">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="7d05a-2530">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="7d05a-2530">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="7d05a-2531">IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-2531">IoT</span></span>

* <span data-ttu-id="7d05a-2532">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="7d05a-2532">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="7d05a-2533">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="7d05a-2533">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="7d05a-2534">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2534">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="7d05a-2535">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="7d05a-2535">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="7d05a-2536">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2536">Monitor</span></span>

* <span data-ttu-id="7d05a-2537">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2537">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-2538">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-2538">Network</span></span>

* <span data-ttu-id="7d05a-2539">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="7d05a-2539">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="7d05a-2540">Perfil</span><span class="sxs-lookup"><span data-stu-id="7d05a-2540">Profile</span></span>

* <span data-ttu-id="7d05a-2541">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2541">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-2542">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-2542">Resource</span></span>

* <span data-ttu-id="7d05a-2543">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="7d05a-2543">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-2544">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-2544">Role</span></span>

* <span data-ttu-id="7d05a-2545">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2545">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-2546">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-2546">SQL</span></span>

* <span data-ttu-id="7d05a-2547">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2547">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="7d05a-2548">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2548">Added `sql db rename`</span></span>
* <span data-ttu-id="7d05a-2549">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="7d05a-2549">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-2550">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2550">Storage</span></span>

* <span data-ttu-id="7d05a-2551">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="7d05a-2551">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2552">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2552">VM</span></span>

* <span data-ttu-id="7d05a-2553">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="7d05a-2553">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="7d05a-2554">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="7d05a-2554">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="7d05a-2555">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2555">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="7d05a-2556">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-2556">January 31, 2018</span></span>

<span data-ttu-id="7d05a-2557">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="7d05a-2557">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-2558">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2558">Core</span></span>

* <span data-ttu-id="7d05a-2559">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="7d05a-2559">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="7d05a-2560">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="7d05a-2560">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="7d05a-2561">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2561">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="7d05a-2562">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="7d05a-2562">Use `--verbose` to see</span></span>
* <span data-ttu-id="7d05a-2563">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="7d05a-2563">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-2564">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2564">ACS</span></span>

* <span data-ttu-id="7d05a-2565">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="7d05a-2565">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="7d05a-2566">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2566">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-2567">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-2567">Appservice</span></span>

* <span data-ttu-id="7d05a-2568">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2568">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="7d05a-2569">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="7d05a-2569">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="7d05a-2570">CDN</span><span class="sxs-lookup"><span data-stu-id="7d05a-2570">CDN</span></span>

* <span data-ttu-id="7d05a-2571">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2571">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7d05a-2572">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7d05a-2572">CosmosDB</span></span>

* <span data-ttu-id="7d05a-2573">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="7d05a-2573">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="7d05a-2574">Interativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2574">Interactive</span></span>

* <span data-ttu-id="7d05a-2575">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="7d05a-2575">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-2576">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-2576">Network</span></span>

* <span data-ttu-id="7d05a-2577">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2577">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="7d05a-2578">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="7d05a-2578">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="7d05a-2579">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2579">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="7d05a-2580">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2580">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="7d05a-2581">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2581">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="7d05a-2582">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="7d05a-2582">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="7d05a-2583">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="7d05a-2583">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="7d05a-2584">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="7d05a-2584">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="7d05a-2585">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2585">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="7d05a-2586">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2586">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="7d05a-2587">Perfil</span><span class="sxs-lookup"><span data-stu-id="7d05a-2587">Profile</span></span>

* <span data-ttu-id="7d05a-2588">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="7d05a-2588">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-2589">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-2589">Resource</span></span>

* <span data-ttu-id="7d05a-2590">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2590">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-2591">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2591">Storage</span></span>

* <span data-ttu-id="7d05a-2592">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="7d05a-2592">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="7d05a-2593">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="7d05a-2593">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="7d05a-2594">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2594">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="7d05a-2595">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2595">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="7d05a-2596">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="7d05a-2596">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2597">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2597">VM</span></span>

* <span data-ttu-id="7d05a-2598">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="7d05a-2598">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="7d05a-2599">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="7d05a-2599">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="7d05a-2600">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2600">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="7d05a-2601">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2601">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="7d05a-2602">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="7d05a-2602">January 17, 2018</span></span>

<span data-ttu-id="7d05a-2603">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="7d05a-2603">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-2604">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-2604">ACR</span></span>

* <span data-ttu-id="7d05a-2605">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="7d05a-2605">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="7d05a-2606">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="7d05a-2606">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-2607">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2607">ACS</span></span>

* <span data-ttu-id="7d05a-2608">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2608">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="7d05a-2609">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="7d05a-2609">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-2610">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-2610">Appservice</span></span>

* <span data-ttu-id="7d05a-2611">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2611">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="7d05a-2612">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2612">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="7d05a-2613">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2613">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="7d05a-2614">Backup</span><span class="sxs-lookup"><span data-stu-id="7d05a-2614">Backup</span></span>

* <span data-ttu-id="7d05a-2615">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="7d05a-2615">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="7d05a-2616">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2616">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="7d05a-2617">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="7d05a-2617">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="7d05a-2618">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="7d05a-2618">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="7d05a-2619">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="7d05a-2619">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="7d05a-2620">Lote</span><span class="sxs-lookup"><span data-stu-id="7d05a-2620">Batch</span></span>

* <span data-ttu-id="7d05a-2621">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="7d05a-2621">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="7d05a-2622">Nuvem</span><span class="sxs-lookup"><span data-stu-id="7d05a-2622">Cloud</span></span>

* <span data-ttu-id="7d05a-2623">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="7d05a-2623">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="7d05a-2624">Consumo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2624">Consumption</span></span>

* <span data-ttu-id="7d05a-2625">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2625">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="7d05a-2626">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2626">Event Grid</span></span>

* <span data-ttu-id="7d05a-2627">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2627">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="7d05a-2628">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2628">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="7d05a-2629">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2629">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="7d05a-2630">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2630">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="7d05a-2631">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2631">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="7d05a-2632">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2632">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="7d05a-2633">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2633">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="7d05a-2634">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="7d05a-2634">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="7d05a-2635">Interativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2635">Interactive</span></span>

* <span data-ttu-id="7d05a-2636">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="7d05a-2636">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="7d05a-2637">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="7d05a-2637">Fixed errors on startup</span></span>
* <span data-ttu-id="7d05a-2638">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2638">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="7d05a-2639">IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-2639">IoT</span></span>

* <span data-ttu-id="7d05a-2640">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2640">Added support for device provisioning service</span></span>
* <span data-ttu-id="7d05a-2641">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="7d05a-2641">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="7d05a-2642">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-2642">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="7d05a-2643">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2643">Monitor</span></span>

* <span data-ttu-id="7d05a-2644">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2644">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="7d05a-2645">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2645">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="7d05a-2646">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="7d05a-2646">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-2647">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-2647">Network</span></span>

* <span data-ttu-id="7d05a-2648">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2648">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="7d05a-2649">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2649">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="7d05a-2650">Perfil</span><span class="sxs-lookup"><span data-stu-id="7d05a-2650">Profile</span></span>

* <span data-ttu-id="7d05a-2651">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="7d05a-2651">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-2652">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-2652">Role</span></span>

* <span data-ttu-id="7d05a-2653">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="7d05a-2653">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7d05a-2654">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7d05a-2654">Service Fabric</span></span>

* <span data-ttu-id="7d05a-2655">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="7d05a-2655">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="7d05a-2656">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2656">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2657">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2657">VM</span></span>

* <span data-ttu-id="7d05a-2658">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2658">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="7d05a-2659">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="7d05a-2659">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="7d05a-2660">[ALTERAÇÃO SIGNIFICATIVA]`externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="7d05a-2660">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="7d05a-2661">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="7d05a-2661">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="7d05a-2662">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="7d05a-2662">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="7d05a-2663">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2663">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="7d05a-2664">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2664">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="7d05a-2665">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2665">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="7d05a-2666">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="7d05a-2666">December 19, 2017</span></span>

<span data-ttu-id="7d05a-2667">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="7d05a-2667">Version 2.0.23</span></span>

* <span data-ttu-id="7d05a-2668">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="7d05a-2668">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="7d05a-2669">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-2669">Container</span></span>

* <span data-ttu-id="7d05a-2670">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-2670">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-2671">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-2671">Network</span></span>

* <span data-ttu-id="7d05a-2672">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2672">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="7d05a-2673">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2673">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-2674">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2674">Storage</span></span>

* <span data-ttu-id="7d05a-2675">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="7d05a-2675">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2676">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2676">VM</span></span>

* <span data-ttu-id="7d05a-2677">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="7d05a-2677">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="7d05a-2678">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="7d05a-2678">December 5, 2017</span></span>

<span data-ttu-id="7d05a-2679">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="7d05a-2679">Version 2.0.22</span></span>

* <span data-ttu-id="7d05a-2680">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2680">Removed `az component` commands.</span></span> <span data-ttu-id="7d05a-2681">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2681">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-2682">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2682">Core</span></span>
* <span data-ttu-id="7d05a-2683">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="7d05a-2683">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="7d05a-2684">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="7d05a-2684">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-2685">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2685">ACS</span></span>

* <span data-ttu-id="7d05a-2686">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="7d05a-2686">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="7d05a-2687">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2687">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="7d05a-2688">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="7d05a-2688">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="7d05a-2689">Supervisor</span><span class="sxs-lookup"><span data-stu-id="7d05a-2689">Advisor</span></span>

* <span data-ttu-id="7d05a-2690">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="7d05a-2690">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-2691">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-2691">Appservice</span></span>

* <span data-ttu-id="7d05a-2692">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2692">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="7d05a-2693">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2693">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="7d05a-2694">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2694">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="7d05a-2695">Consumo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2695">Consumption</span></span>

* <span data-ttu-id="7d05a-2696">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="7d05a-2696">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="7d05a-2697">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-2697">Container</span></span>

* <span data-ttu-id="7d05a-2698">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="7d05a-2698">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="7d05a-2699">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2699">Monitor</span></span>

* <span data-ttu-id="7d05a-2700">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="7d05a-2700">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-2701">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-2701">Resource</span></span>

* <span data-ttu-id="7d05a-2702">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2702">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-2703">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-2703">Role</span></span>

* <span data-ttu-id="7d05a-2704">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2704">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="7d05a-2705">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="7d05a-2705">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="7d05a-2706">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2706">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-2707">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-2707">SQL</span></span>

* <span data-ttu-id="7d05a-2708">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="7d05a-2708">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="7d05a-2709">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="7d05a-2709">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2710">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2710">VM</span></span>

* <span data-ttu-id="7d05a-2711">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2711">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="7d05a-2712">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="7d05a-2712">November 14, 2017</span></span>

<span data-ttu-id="7d05a-2713">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="7d05a-2713">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-2714">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-2714">ACR</span></span>

* <span data-ttu-id="7d05a-2715">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="7d05a-2715">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="7d05a-2716">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2716">ACS</span></span>

* <span data-ttu-id="7d05a-2717">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2717">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="7d05a-2718">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2718">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="7d05a-2719">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2719">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="7d05a-2720">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="7d05a-2720">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="7d05a-2721">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="7d05a-2721">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-2722">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-2722">Appservice</span></span>

* <span data-ttu-id="7d05a-2723">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="7d05a-2723">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="7d05a-2724">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2724">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="7d05a-2725">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2725">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="7d05a-2726">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2726">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="7d05a-2727">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="7d05a-2727">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="7d05a-2728">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2728">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="7d05a-2729">Lote</span><span class="sxs-lookup"><span data-stu-id="7d05a-2729">Batch</span></span>

* <span data-ttu-id="7d05a-2730">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2730">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="7d05a-2731">Batchai</span><span class="sxs-lookup"><span data-stu-id="7d05a-2731">Batchai</span></span>

* <span data-ttu-id="7d05a-2732">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2732">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="7d05a-2733">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2733">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="7d05a-2734">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2734">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="7d05a-2735">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2735">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="7d05a-2736">Nuvem</span><span class="sxs-lookup"><span data-stu-id="7d05a-2736">Cloud</span></span>

* <span data-ttu-id="7d05a-2737">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="7d05a-2737">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="7d05a-2738">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-2738">Container</span></span>

* <span data-ttu-id="7d05a-2739">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="7d05a-2739">Added support to open multiple ports</span></span>
* <span data-ttu-id="7d05a-2740">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="7d05a-2740">Added container group restart policy</span></span>
* <span data-ttu-id="7d05a-2741">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="7d05a-2741">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="7d05a-2742">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="7d05a-2742">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7d05a-2743">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7d05a-2743">Data Lake Analytics</span></span>

* <span data-ttu-id="7d05a-2744">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="7d05a-2744">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7d05a-2745">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7d05a-2745">Data Lake Store</span></span>

* <span data-ttu-id="7d05a-2746">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="7d05a-2746">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="7d05a-2747">Extensão</span><span class="sxs-lookup"><span data-stu-id="7d05a-2747">Extension</span></span>

* <span data-ttu-id="7d05a-2748">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="7d05a-2748">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="7d05a-2749">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="7d05a-2749">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="7d05a-2750">IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-2750">IoT</span></span>

* <span data-ttu-id="7d05a-2751">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="7d05a-2751">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="7d05a-2752">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2752">Monitor</span></span>

* <span data-ttu-id="7d05a-2753">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2753">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-2754">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-2754">Network</span></span>

* <span data-ttu-id="7d05a-2755">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="7d05a-2755">Added support for CAA DNS records</span></span>
* <span data-ttu-id="7d05a-2756">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2756">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="7d05a-2757">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="7d05a-2757">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="7d05a-2758">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2758">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="7d05a-2759">Reservas</span><span class="sxs-lookup"><span data-stu-id="7d05a-2759">Reservations</span></span>

* <span data-ttu-id="7d05a-2760">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="7d05a-2760">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-2761">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-2761">Resource</span></span>

* <span data-ttu-id="7d05a-2762">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-2762">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-2763">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-2763">SQL</span></span>

* <span data-ttu-id="7d05a-2764">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2764">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-2765">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2765">Storage</span></span>

* <span data-ttu-id="7d05a-2766">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="7d05a-2766">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="7d05a-2767">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="7d05a-2767">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="7d05a-2768">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2768">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="7d05a-2769">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2769">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="7d05a-2770">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2770">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="7d05a-2771">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2771">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="7d05a-2772">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2772">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2773">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2773">VM</span></span>

* <span data-ttu-id="7d05a-2774">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2774">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="7d05a-2775">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="7d05a-2775">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="7d05a-2776">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="7d05a-2776">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="7d05a-2777">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2777">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="7d05a-2778">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2778">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="7d05a-2779">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="7d05a-2779">October 24, 2017</span></span>

<span data-ttu-id="7d05a-2780">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="7d05a-2780">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-2781">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2781">Core</span></span>

* <span data-ttu-id="7d05a-2782">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2782">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-2783">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-2783">ACR</span></span>

* <span data-ttu-id="7d05a-2784">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2784">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="7d05a-2785">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="7d05a-2785">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="7d05a-2786">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="7d05a-2786">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-2787">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2787">ACS</span></span>

* <span data-ttu-id="7d05a-2788">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="7d05a-2788">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="7d05a-2789">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="7d05a-2789">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-2790">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-2790">Appservice</span></span>

* <span data-ttu-id="7d05a-2791">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2791">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="7d05a-2792">Componente</span><span class="sxs-lookup"><span data-stu-id="7d05a-2792">Component</span></span>

* <span data-ttu-id="7d05a-2793">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="7d05a-2793">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="7d05a-2794">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2794">Monitor</span></span>

* <span data-ttu-id="7d05a-2795">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2795">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-2796">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-2796">Resource</span></span>

* <span data-ttu-id="7d05a-2797">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2797">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="7d05a-2798">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="7d05a-2798">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2799">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2799">VM</span></span>

* <span data-ttu-id="7d05a-2800">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2800">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="7d05a-2801">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="7d05a-2801">October 9, 2017</span></span>

<span data-ttu-id="7d05a-2802">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="7d05a-2802">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-2803">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2803">Core</span></span>

* <span data-ttu-id="7d05a-2804">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="7d05a-2804">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-2805">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-2805">Appservice</span></span>

* <span data-ttu-id="7d05a-2806">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2806">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="7d05a-2807">Lote</span><span class="sxs-lookup"><span data-stu-id="7d05a-2807">Batch</span></span>

* <span data-ttu-id="7d05a-2808">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="7d05a-2808">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="7d05a-2809">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="7d05a-2809">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="7d05a-2810">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="7d05a-2810">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="7d05a-2811">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="7d05a-2811">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="7d05a-2812">Batchai</span><span class="sxs-lookup"><span data-stu-id="7d05a-2812">Batchai</span></span>

* <span data-ttu-id="7d05a-2813">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="7d05a-2813">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="7d05a-2814">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7d05a-2814">Keyvault</span></span>

* <span data-ttu-id="7d05a-2815">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2815">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="7d05a-2816">(#4448)</span><span class="sxs-lookup"><span data-stu-id="7d05a-2816">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="7d05a-2817">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-2817">Network</span></span>

* <span data-ttu-id="7d05a-2818">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="7d05a-2818">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="7d05a-2819">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="7d05a-2819">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-2820">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-2820">Resource</span></span>

* <span data-ttu-id="7d05a-2821">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2821">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="7d05a-2822">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="7d05a-2822">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="7d05a-2823">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2823">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="7d05a-2824">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-2824">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-2825">Sql</span><span class="sxs-lookup"><span data-stu-id="7d05a-2825">Sql</span></span>

* <span data-ttu-id="7d05a-2826">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="7d05a-2826">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="7d05a-2827">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2827">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="7d05a-2828">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="7d05a-2828">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-2829">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2829">Storage</span></span>

* <span data-ttu-id="7d05a-2830">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2830">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2831">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2831">Vm</span></span>

* <span data-ttu-id="7d05a-2832">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="7d05a-2832">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="7d05a-2833">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2833">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="7d05a-2834">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2834">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="7d05a-2835">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2835">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="7d05a-2836">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2836">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="7d05a-2837">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="7d05a-2837">September 22, 2017</span></span>

<span data-ttu-id="7d05a-2838">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="7d05a-2838">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-2839">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-2839">Resource</span></span>

* <span data-ttu-id="7d05a-2840">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="7d05a-2840">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="7d05a-2841">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="7d05a-2841">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="7d05a-2842">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2842">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="7d05a-2843">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2843">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-2844">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-2844">Network</span></span>

* <span data-ttu-id="7d05a-2845">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2845">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="7d05a-2846">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2846">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="7d05a-2847">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2847">Added `asg` application security group commands</span></span>
* <span data-ttu-id="7d05a-2848">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2848">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="7d05a-2849">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2849">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="7d05a-2850">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2850">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="7d05a-2851">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2851">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-2852">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2852">Storage</span></span>

* <span data-ttu-id="7d05a-2853">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="7d05a-2853">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="7d05a-2854">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2854">Eventgrid</span></span>

* <span data-ttu-id="7d05a-2855">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="7d05a-2855">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-2856">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-2856">SQL</span></span>

* <span data-ttu-id="7d05a-2857">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="7d05a-2857">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="7d05a-2858">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="7d05a-2858">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="7d05a-2859">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2859">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="7d05a-2860">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7d05a-2860">Keyvault</span></span>

* <span data-ttu-id="7d05a-2861">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="7d05a-2861">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2862">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2862">VM</span></span>

* <span data-ttu-id="7d05a-2863">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2863">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="7d05a-2864">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="7d05a-2864">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="7d05a-2865">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2865">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="7d05a-2866">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2866">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="7d05a-2867">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2867">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="7d05a-2868">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2868">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-2869">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2869">ACS</span></span>

* <span data-ttu-id="7d05a-2870">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2870">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-2871">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-2871">Appservice</span></span>

* <span data-ttu-id="7d05a-2872">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2872">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="7d05a-2873">Backup</span><span class="sxs-lookup"><span data-stu-id="7d05a-2873">Backup</span></span>

* <span data-ttu-id="7d05a-2874">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="7d05a-2874">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="7d05a-2875">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="7d05a-2875">September 11, 2017</span></span>

<span data-ttu-id="7d05a-2876">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="7d05a-2876">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="7d05a-2877">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2877">Core</span></span>

* <span data-ttu-id="7d05a-2878">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="7d05a-2878">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="7d05a-2879">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="7d05a-2879">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-2880">Acs</span><span class="sxs-lookup"><span data-stu-id="7d05a-2880">Acs</span></span>

* <span data-ttu-id="7d05a-2881">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2881">Added `acs list-locations` command</span></span>
* <span data-ttu-id="7d05a-2882">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="7d05a-2882">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-2883">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-2883">Appservice</span></span>

* <span data-ttu-id="7d05a-2884">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2884">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="7d05a-2885">CDN</span><span class="sxs-lookup"><span data-stu-id="7d05a-2885">CDN</span></span>

* <span data-ttu-id="7d05a-2886">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2886">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="7d05a-2887">Extensão</span><span class="sxs-lookup"><span data-stu-id="7d05a-2887">Extension</span></span>

* <span data-ttu-id="7d05a-2888">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="7d05a-2888">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="7d05a-2889">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7d05a-2889">Keyvault</span></span>

* <span data-ttu-id="7d05a-2890">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2890">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-2891">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-2891">Network</span></span>

* <span data-ttu-id="7d05a-2892">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2892">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="7d05a-2893">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2893">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="7d05a-2894">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2894">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="7d05a-2895">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2895">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="7d05a-2896">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2896">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-2897">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-2897">Resource</span></span>

* <span data-ttu-id="7d05a-2898">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2898">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="7d05a-2899">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2899">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="7d05a-2900">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="7d05a-2900">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="7d05a-2901">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="7d05a-2901">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-2902">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-2902">SQL</span></span>

* <span data-ttu-id="7d05a-2903">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2903">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2904">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2904">VM</span></span>

* <span data-ttu-id="7d05a-2905">Corrigido: não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="7d05a-2905">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="7d05a-2906">Corrigido: usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="7d05a-2906">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="7d05a-2907">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2907">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="7d05a-2908">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="7d05a-2908">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="7d05a-2909">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="7d05a-2909">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="7d05a-2910">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="7d05a-2910">August 31, 2017</span></span>

<span data-ttu-id="7d05a-2911">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="7d05a-2911">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="7d05a-2912">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7d05a-2912">Keyvault</span></span>

* <span data-ttu-id="7d05a-2913">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2913">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="7d05a-2914">Sf</span><span class="sxs-lookup"><span data-stu-id="7d05a-2914">Sf</span></span>

* <span data-ttu-id="7d05a-2915">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="7d05a-2915">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-2916">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2916">Storage</span></span>

* <span data-ttu-id="7d05a-2917">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="7d05a-2917">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="7d05a-2918">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="7d05a-2918">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="7d05a-2919">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="7d05a-2919">August 28, 2017</span></span>

<span data-ttu-id="7d05a-2920">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="7d05a-2920">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="7d05a-2921">CLI</span><span class="sxs-lookup"><span data-stu-id="7d05a-2921">CLI</span></span>

* <span data-ttu-id="7d05a-2922">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2922">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-2923">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2923">ACS</span></span>

* <span data-ttu-id="7d05a-2924">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="7d05a-2924">Corrected preview regions</span></span>
* <span data-ttu-id="7d05a-2925">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2925">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="7d05a-2926">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="7d05a-2926">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-2927">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-2927">Appservice</span></span>

* <span data-ttu-id="7d05a-2928">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2928">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="7d05a-2929">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2929">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="7d05a-2930">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2930">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="7d05a-2931">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-2931">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="7d05a-2932">Corrigido: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="7d05a-2932">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="7d05a-2933">IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-2933">IoT</span></span>

* <span data-ttu-id="7d05a-2934">Corrigido #3934: a criação de uma política não limpa mais as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="7d05a-2934">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-2935">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-2935">Network</span></span>

* <span data-ttu-id="7d05a-2936">[ALTERAÇÃO SIGNIFICATIVA]`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2936">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="7d05a-2937">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2937">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="7d05a-2938">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2938">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="7d05a-2939">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2939">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="7d05a-2940">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2940">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="7d05a-2941">Perfil</span><span class="sxs-lookup"><span data-stu-id="7d05a-2941">Profile</span></span>

* <span data-ttu-id="7d05a-2942">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="7d05a-2942">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7d05a-2943">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7d05a-2943">Service Fabric</span></span>

* <span data-ttu-id="7d05a-2944">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="7d05a-2944">Preview release</span></span>
* <span data-ttu-id="7d05a-2945">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="7d05a-2945">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="7d05a-2946">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="7d05a-2946">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="7d05a-2947">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="7d05a-2947">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-2948">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2948">Storage</span></span>

* <span data-ttu-id="7d05a-2949">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="7d05a-2949">Enabled setting blob tier</span></span>
* <span data-ttu-id="7d05a-2950">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="7d05a-2950">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="7d05a-2951">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="7d05a-2951">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="7d05a-2952">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="7d05a-2952">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="7d05a-2953">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2953">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="7d05a-2954">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="7d05a-2954">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2955">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2955">VM</span></span>

* <span data-ttu-id="7d05a-2956">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2956">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="7d05a-2957">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="7d05a-2957">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="7d05a-2958">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2958">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="7d05a-2959">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="7d05a-2959">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="7d05a-2960">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="7d05a-2960">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="7d05a-2961">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2961">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="7d05a-2962">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="7d05a-2962">August 15, 2017</span></span>

<span data-ttu-id="7d05a-2963">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="7d05a-2963">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-2964">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2964">ACS</span></span>

* <span data-ttu-id="7d05a-2965">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="7d05a-2965">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-2966">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-2966">Appservice</span></span>

* <span data-ttu-id="7d05a-2967">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="7d05a-2967">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="7d05a-2968">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2968">Event Grid</span></span>

* <span data-ttu-id="7d05a-2969">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="7d05a-2969">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="7d05a-2970">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="7d05a-2970">August 11, 2017</span></span>

<span data-ttu-id="7d05a-2971">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="7d05a-2971">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-2972">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-2972">ACS</span></span>

* <span data-ttu-id="7d05a-2973">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="7d05a-2973">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="7d05a-2974">Lote</span><span class="sxs-lookup"><span data-stu-id="7d05a-2974">Batch</span></span>

* <span data-ttu-id="7d05a-2975">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="7d05a-2975">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="7d05a-2976">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="7d05a-2976">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="7d05a-2977">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-2977">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="7d05a-2978">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://”</span><span class="sxs-lookup"><span data-stu-id="7d05a-2978">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="7d05a-2979">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="7d05a-2979">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="7d05a-2980">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="7d05a-2980">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="7d05a-2981">Componente</span><span class="sxs-lookup"><span data-stu-id="7d05a-2981">Component</span></span>

* <span data-ttu-id="7d05a-2982">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="7d05a-2982">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="7d05a-2983">Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-2983">Container</span></span>

* <span data-ttu-id="7d05a-2984">`create`: corrigido o problema em que o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="7d05a-2984">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="7d05a-2985">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7d05a-2985">Data Lake Store</span></span>

* <span data-ttu-id="7d05a-2986">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2986">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="7d05a-2987">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2987">Event Grid</span></span>

* <span data-ttu-id="7d05a-2988">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="7d05a-2988">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-2989">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-2989">Network</span></span>

* <span data-ttu-id="7d05a-2990">`lb`: corrigido o problema em que os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="7d05a-2990">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="7d05a-2991">`application-gateway {subresource} delete`: corrigido o problema em que `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="7d05a-2991">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="7d05a-2992">`application-gateway http-settings update`: corrigido o problema em que `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="7d05a-2992">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="7d05a-2993">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="7d05a-2993">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="7d05a-2994">Perfil</span><span class="sxs-lookup"><span data-stu-id="7d05a-2994">Profile</span></span>

* <span data-ttu-id="7d05a-2995">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="7d05a-2995">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-2996">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-2996">Storage</span></span>

* <span data-ttu-id="7d05a-2997">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="7d05a-2997">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-2998">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-2998">VM</span></span>

* <span data-ttu-id="7d05a-2999">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="7d05a-2999">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="7d05a-3000">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3000">Exposed `list-skus` command</span></span>
* <span data-ttu-id="7d05a-3001">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="7d05a-3001">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="7d05a-3002">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="7d05a-3002">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="7d05a-3003">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="7d05a-3003">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="7d05a-3004">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="7d05a-3004">July 28, 2017</span></span>

<span data-ttu-id="7d05a-3005">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="7d05a-3005">Version 2.0.12</span></span>

* <span data-ttu-id="7d05a-3006">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-3006">Added container commands</span></span>
* <span data-ttu-id="7d05a-3007">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="7d05a-3007">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="7d05a-3008">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-3008">Core</span></span>

* <span data-ttu-id="7d05a-3009">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="7d05a-3009">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="7d05a-3010">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="7d05a-3010">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="7d05a-3011">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="7d05a-3011">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="7d05a-3012">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3012">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="7d05a-3013">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="7d05a-3013">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="7d05a-3014">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3014">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="7d05a-3015">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3015">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="7d05a-3016">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3016">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="7d05a-3017">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3017">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="7d05a-3018">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="7d05a-3018">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="7d05a-3019">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="7d05a-3019">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="7d05a-3020">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3020">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="7d05a-3021">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="7d05a-3021">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="7d05a-3022">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="7d05a-3022">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="7d05a-3023">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="7d05a-3023">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="7d05a-3024">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3024">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="7d05a-3025">ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-3025">ACR</span></span>

* <span data-ttu-id="7d05a-3026">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="7d05a-3026">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="7d05a-3027">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="7d05a-3027">Support SKU update for managed registries</span></span>
* <span data-ttu-id="7d05a-3028">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="7d05a-3028">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="7d05a-3029">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-3029">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="7d05a-3030">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-3030">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="7d05a-3031">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="7d05a-3031">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-3032">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-3032">ACS</span></span>

* <span data-ttu-id="7d05a-3033">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="7d05a-3033">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-3034">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-3034">Appservice</span></span>

* <span data-ttu-id="7d05a-3035">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="7d05a-3035">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="7d05a-3036">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="7d05a-3036">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="7d05a-3037">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3037">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="7d05a-3038">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3038">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="7d05a-3039">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3039">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="7d05a-3040">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3040">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="7d05a-3041">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3041">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="7d05a-3042">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3042">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="7d05a-3043">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="7d05a-3043">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="7d05a-3044">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3044">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="7d05a-3045">Lote</span><span class="sxs-lookup"><span data-stu-id="7d05a-3045">Batch</span></span>

* <span data-ttu-id="7d05a-3046">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="7d05a-3046">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="7d05a-3047">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3047">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="7d05a-3048">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3048">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="7d05a-3049">CDN</span><span class="sxs-lookup"><span data-stu-id="7d05a-3049">CDN</span></span>

* <span data-ttu-id="7d05a-3050">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="7d05a-3050">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="7d05a-3051">Nuvem</span><span class="sxs-lookup"><span data-stu-id="7d05a-3051">Cloud</span></span>

* <span data-ttu-id="7d05a-3052">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="7d05a-3052">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="7d05a-3053">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="7d05a-3053">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="7d05a-3054">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="7d05a-3054">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="7d05a-3055">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="7d05a-3055">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="7d05a-3056">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3056">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7d05a-3057">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7d05a-3057">CosmosDB</span></span>

* <span data-ttu-id="7d05a-3058">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="7d05a-3058">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="7d05a-3059">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="7d05a-3059">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7d05a-3060">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7d05a-3060">Data Lake Analytics</span></span>

* <span data-ttu-id="7d05a-3061">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3061">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="7d05a-3062">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3062">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="7d05a-3063">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3063">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7d05a-3064">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7d05a-3064">Data Lake Store</span></span>

* <span data-ttu-id="7d05a-3065">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3065">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="7d05a-3066">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="7d05a-3066">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="7d05a-3067">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="7d05a-3067">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="7d05a-3068">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7d05a-3068">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="7d05a-3069">Interativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-3069">Interactive</span></span>

* <span data-ttu-id="7d05a-3070">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="7d05a-3070">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="7d05a-3071">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="7d05a-3071">Increased test coverage</span></span>
* <span data-ttu-id="7d05a-3072">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="7d05a-3072">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="7d05a-3073">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3073">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="7d05a-3074">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3074">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="7d05a-3075">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3075">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="7d05a-3076">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3076">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="7d05a-3077">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3077">Added `--progress` flag</span></span>
* <span data-ttu-id="7d05a-3078">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="7d05a-3078">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="7d05a-3079">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3079">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="7d05a-3080">IoT</span><span class="sxs-lookup"><span data-stu-id="7d05a-3080">IoT</span></span>

* <span data-ttu-id="7d05a-3081">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="7d05a-3081">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="7d05a-3082">(#3934)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3082">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="7d05a-3083">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="7d05a-3083">Key vault</span></span>

* <span data-ttu-id="7d05a-3084">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="7d05a-3084">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="7d05a-3085">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3085">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="7d05a-3086">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3086">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="7d05a-3087">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3087">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="7d05a-3088">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3088">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="7d05a-3089">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3089">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="7d05a-3090">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="7d05a-3090">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="7d05a-3091">(#3307)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3091">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="7d05a-3092">Laboratório</span><span class="sxs-lookup"><span data-stu-id="7d05a-3092">Lab</span></span>

* <span data-ttu-id="7d05a-3093">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3093">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="7d05a-3094">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3094">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="7d05a-3095">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-3095">Monitor</span></span>

* <span data-ttu-id="7d05a-3096">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3096">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="7d05a-3097">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3097">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="7d05a-3098">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3098">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="7d05a-3099">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3099">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="7d05a-3100">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3100">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="7d05a-3101">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="7d05a-3101">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="7d05a-3102">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="7d05a-3102">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="7d05a-3103">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="7d05a-3103">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="7d05a-3104">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="7d05a-3104">`location` no longer required</span></span>
  * <span data-ttu-id="7d05a-3105">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="7d05a-3105">Add name and ID support for target</span></span>
  * <span data-ttu-id="7d05a-3106">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3106">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="7d05a-3107">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="7d05a-3107">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="7d05a-3108">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="7d05a-3108">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="7d05a-3109">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="7d05a-3109">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="7d05a-3110">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3110">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="7d05a-3111">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3111">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-3112">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-3112">Network</span></span>

* <span data-ttu-id="7d05a-3113">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3113">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="7d05a-3114">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3114">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="7d05a-3115">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="7d05a-3115">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="7d05a-3116">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="7d05a-3116">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="7d05a-3117">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3117">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="7d05a-3118">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3118">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="7d05a-3119">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3119">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="7d05a-3120">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3120">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="7d05a-3121">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3121">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="7d05a-3122">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3122">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="7d05a-3123">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3123">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="7d05a-3124">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3124">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="7d05a-3125">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3125">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="7d05a-3126">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3126">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="7d05a-3127">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3127">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="7d05a-3128">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3128">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="7d05a-3129">Adicionado o suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para --dns-servers</span><span class="sxs-lookup"><span data-stu-id="7d05a-3129">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="7d05a-3130">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3130">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="7d05a-3131">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3131">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="7d05a-3132">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3132">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="7d05a-3133">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3133">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="7d05a-3134">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3134">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="7d05a-3135">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3135">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="7d05a-3136">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="7d05a-3136">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="7d05a-3137">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="7d05a-3137">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="7d05a-3138">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="7d05a-3138">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="7d05a-3139">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="7d05a-3139">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="7d05a-3140">Perfil</span><span class="sxs-lookup"><span data-stu-id="7d05a-3140">Profile</span></span>

* <span data-ttu-id="7d05a-3141">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="7d05a-3141">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="7d05a-3142">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="7d05a-3142">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="7d05a-3143">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="7d05a-3143">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="7d05a-3144">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="7d05a-3144">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="7d05a-3145">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="7d05a-3145">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="7d05a-3146">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7d05a-3146">RDBMS</span></span>

* <span data-ttu-id="7d05a-3147">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3147">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="7d05a-3148">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3148">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="7d05a-3149">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3149">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="7d05a-3150">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3150">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-3151">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-3151">Resource</span></span>

* <span data-ttu-id="7d05a-3152">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3152">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="7d05a-3153">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3153">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="7d05a-3154">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3154">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="7d05a-3155">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3155">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="7d05a-3156">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3156">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="7d05a-3157">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3157">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="7d05a-3158">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3158">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="7d05a-3159">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3159">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-3160">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-3160">Role</span></span>

* <span data-ttu-id="7d05a-3161">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3161">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="7d05a-3162">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3162">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="7d05a-3163">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3163">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="7d05a-3164">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3164">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="7d05a-3165">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3165">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7d05a-3166">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7d05a-3166">Service Fabric</span></span>
* <span data-ttu-id="7d05a-3167">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3167">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="7d05a-3168">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3168">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="7d05a-3169">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3169">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-3170">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-3170">SQL</span></span>

* <span data-ttu-id="7d05a-3171">Removido o parâmetro `sql server create` `--identity` desfeito</span><span class="sxs-lookup"><span data-stu-id="7d05a-3171">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="7d05a-3172">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3172">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="7d05a-3173">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3173">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-3174">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-3174">Storage</span></span>

* <span data-ttu-id="7d05a-3175">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3175">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="7d05a-3176">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="7d05a-3176">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="7d05a-3177">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3177">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="7d05a-3178">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3178">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="7d05a-3179">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3179">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="7d05a-3180">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3180">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-3181">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-3181">VM</span></span>

* <span data-ttu-id="7d05a-3182">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="7d05a-3182">Support configuring nsg</span></span>
* <span data-ttu-id="7d05a-3183">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="7d05a-3183">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="7d05a-3184">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="7d05a-3184">Support managed service identities</span></span>
* <span data-ttu-id="7d05a-3185">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3185">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="7d05a-3186">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="7d05a-3186">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="7d05a-3187">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="7d05a-3187">May 10, 2017</span></span>

<span data-ttu-id="7d05a-3188">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="7d05a-3188">Version 2.0.6</span></span>

* <span data-ttu-id="7d05a-3189">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7d05a-3189">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="7d05a-3190">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3190">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="7d05a-3191">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7d05a-3191">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="7d05a-3192">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="7d05a-3192">Include Cognitive Services module</span></span>
* <span data-ttu-id="7d05a-3193">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7d05a-3193">Include Service Fabric module</span></span>
* <span data-ttu-id="7d05a-3194">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3194">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="7d05a-3195">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="7d05a-3195">Add support for CDN commands</span></span>
* <span data-ttu-id="7d05a-3196">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="7d05a-3196">Remove Container module</span></span>
* <span data-ttu-id="7d05a-3197">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3197">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="7d05a-3198">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3198">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="7d05a-3199">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-3199">Core</span></span>

* <span data-ttu-id="7d05a-3200">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="7d05a-3200">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="7d05a-3201">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3201">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="7d05a-3202">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3202">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="7d05a-3203">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3203">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="7d05a-3204">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3204">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="7d05a-3205">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3205">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="7d05a-3206">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3206">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="7d05a-3207">núcleo: permitir que o caminho do arquivo accessTokens.json seja configurável por meio de uma variável de ambiente ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3207">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="7d05a-3208">núcleo: permitir que padrões configurados sejam aplicados em argumentos opcionais ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3208">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="7d05a-3209">núcleo: desempenho aprimorado</span><span class="sxs-lookup"><span data-stu-id="7d05a-3209">core: Improved performance</span></span>
* <span data-ttu-id="7d05a-3210">núcleo: certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="7d05a-3210">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="7d05a-3211">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="7d05a-3211">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-3212">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-3212">ACS</span></span>

* <span data-ttu-id="7d05a-3213">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d05a-3213">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="7d05a-3214">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="7d05a-3214">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="7d05a-3215">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="7d05a-3215">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="7d05a-3216">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3216">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-3217">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-3217">AppService</span></span>

* <span data-ttu-id="7d05a-3218">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="7d05a-3218">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="7d05a-3219">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="7d05a-3219">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="7d05a-3220">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3220">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="7d05a-3221">Exposição de argumentos para configurar a implantação e as “pilhas em runtime” em webapp create</span><span class="sxs-lookup"><span data-stu-id="7d05a-3221">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="7d05a-3222">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="7d05a-3222">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="7d05a-3223">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3223">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="7d05a-3224">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="7d05a-3224">support slot swap with preview</span></span>
* <span data-ttu-id="7d05a-3225">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3225">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="7d05a-3226">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3226">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7d05a-3227">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7d05a-3227">CosmosDB</span></span>

* <span data-ttu-id="7d05a-3228">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7d05a-3228">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="7d05a-3229">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="7d05a-3229">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="7d05a-3230">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="7d05a-3230">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="7d05a-3231">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="7d05a-3231">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7d05a-3232">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7d05a-3232">Data Lake Analytics</span></span>

* <span data-ttu-id="7d05a-3233">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="7d05a-3233">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="7d05a-3234">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="7d05a-3234">Add support for new catalog item type: package.</span></span> <span data-ttu-id="7d05a-3235">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3235">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="7d05a-3236">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="7d05a-3236">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="7d05a-3237">Tabela</span><span class="sxs-lookup"><span data-stu-id="7d05a-3237">Table</span></span>
  * <span data-ttu-id="7d05a-3238">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="7d05a-3238">Table valued function</span></span>
  * <span data-ttu-id="7d05a-3239">Visualizar</span><span class="sxs-lookup"><span data-stu-id="7d05a-3239">View</span></span>
  * <span data-ttu-id="7d05a-3240">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="7d05a-3240">Table Statistics.</span></span> <span data-ttu-id="7d05a-3241">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="7d05a-3241">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7d05a-3242">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7d05a-3242">Data Lake Store</span></span>

* <span data-ttu-id="7d05a-3243">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="7d05a-3243">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="7d05a-3244">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3244">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="7d05a-3245">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="7d05a-3245">missed help for access show.</span></span> <span data-ttu-id="7d05a-3246">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="7d05a-3246">adding it.</span></span> <span data-ttu-id="7d05a-3247">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3247">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="7d05a-3248">Localizar</span><span class="sxs-lookup"><span data-stu-id="7d05a-3248">Find</span></span>

* <span data-ttu-id="7d05a-3249">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="7d05a-3249">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="7d05a-3250">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7d05a-3250">KeyVault</span></span>

* <span data-ttu-id="7d05a-3251">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="7d05a-3251">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="7d05a-3252">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois estes parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="7d05a-3252">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="7d05a-3253">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="7d05a-3253">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="7d05a-3254">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="7d05a-3254">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="7d05a-3255">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3255">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="7d05a-3256">Laboratório</span><span class="sxs-lookup"><span data-stu-id="7d05a-3256">Lab</span></span>

* <span data-ttu-id="7d05a-3257">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="7d05a-3257">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="7d05a-3258">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="7d05a-3258">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="7d05a-3259">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="7d05a-3259">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="7d05a-3260">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="7d05a-3260">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="7d05a-3261">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="7d05a-3261">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="7d05a-3262">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="7d05a-3262">Monitor</span></span>

* <span data-ttu-id="7d05a-3263">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3263">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="7d05a-3264">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3264">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="7d05a-3265">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-3265">Network</span></span>

* <span data-ttu-id="7d05a-3266">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3266">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="7d05a-3267">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3267">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="7d05a-3268">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-3268">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="7d05a-3269">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d05a-3269">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="7d05a-3270">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="7d05a-3270">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="7d05a-3271">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="7d05a-3271">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="7d05a-3272">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="7d05a-3272">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="7d05a-3273">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="7d05a-3273">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="7d05a-3274">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3274">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="7d05a-3275">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="7d05a-3275">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="7d05a-3276">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3276">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="7d05a-3277">BC: corrigido um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3277">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="7d05a-3278">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="7d05a-3278">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="7d05a-3279">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="7d05a-3279">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="7d05a-3280">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="7d05a-3280">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="7d05a-3281">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="7d05a-3281">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="7d05a-3282">Perfil</span><span class="sxs-lookup"><span data-stu-id="7d05a-3282">Profile</span></span>

* <span data-ttu-id="7d05a-3283">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3283">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="7d05a-3284">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3284">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="7d05a-3285">Redis</span><span class="sxs-lookup"><span data-stu-id="7d05a-3285">Redis</span></span>

* <span data-ttu-id="7d05a-3286">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="7d05a-3286">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="7d05a-3287">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="7d05a-3287">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="7d05a-3288">Recurso</span><span class="sxs-lookup"><span data-stu-id="7d05a-3288">Resource</span></span>

* <span data-ttu-id="7d05a-3289">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3289">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="7d05a-3290">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3290">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="7d05a-3291">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3291">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="7d05a-3292">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="7d05a-3292">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="7d05a-3293">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3293">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="7d05a-3294">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="7d05a-3294">Add docs for az lock update.</span></span> <span data-ttu-id="7d05a-3295">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3295">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="7d05a-3296">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="7d05a-3296">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="7d05a-3297">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3297">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="7d05a-3298">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="7d05a-3298">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="7d05a-3299">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3299">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="7d05a-3300">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3300">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="7d05a-3301">Função</span><span class="sxs-lookup"><span data-stu-id="7d05a-3301">Role</span></span>

* <span data-ttu-id="7d05a-3302">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3302">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="7d05a-3303">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3303">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="7d05a-3304">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3304">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="7d05a-3305">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="7d05a-3305">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="7d05a-3306">SQL</span><span class="sxs-lookup"><span data-stu-id="7d05a-3306">SQL</span></span>

* <span data-ttu-id="7d05a-3307">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="7d05a-3307">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="7d05a-3308">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3308">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="7d05a-3309">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-3309">Storage</span></span>

* <span data-ttu-id="7d05a-3310">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3310">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="7d05a-3311">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="7d05a-3311">Add support for incremental blob copy</span></span>
* <span data-ttu-id="7d05a-3312">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="7d05a-3312">Add support for large block blob upload</span></span>
* <span data-ttu-id="7d05a-3313">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="7d05a-3313">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-3314">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-3314">VM</span></span>

* <span data-ttu-id="7d05a-3315">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="7d05a-3315">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="7d05a-3316">observação: em comandos da VM em nuvens soberanas, evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="7d05a-3316">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="7d05a-3317">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="7d05a-3317">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="7d05a-3318">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="7d05a-3318">az vm/vmss disk</span></span>
  3. <span data-ttu-id="7d05a-3319">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="7d05a-3319">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="7d05a-3320">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="7d05a-3320">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="7d05a-3321">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3321">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="7d05a-3322">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="7d05a-3322">April 3, 2017</span></span>

<span data-ttu-id="7d05a-3323">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="7d05a-3323">Version 2.0.2</span></span>

<span data-ttu-id="7d05a-3324">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="7d05a-3324">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="7d05a-3325">Núcleo</span><span class="sxs-lookup"><span data-stu-id="7d05a-3325">Core</span></span>

* <span data-ttu-id="7d05a-3326">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="7d05a-3326">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="7d05a-3327">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3327">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="7d05a-3328">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3328">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="7d05a-3329">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3329">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="7d05a-3330">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3330">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="7d05a-3331">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="7d05a-3331">Add prompting for missing template parameters.</span></span> <span data-ttu-id="7d05a-3332">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3332">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="7d05a-3333">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="7d05a-3333">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="7d05a-3334">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="7d05a-3334">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="7d05a-3335">ACS</span><span class="sxs-lookup"><span data-stu-id="7d05a-3335">ACS</span></span>

* <span data-ttu-id="7d05a-3336">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3336">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="7d05a-3337">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="7d05a-3337">Add support for ssh key password prompting.</span></span> <span data-ttu-id="7d05a-3338">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3338">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="7d05a-3339">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="7d05a-3339">Add support for windows clusters.</span></span> <span data-ttu-id="7d05a-3340">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3340">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="7d05a-3341">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="7d05a-3341">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="7d05a-3342">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3342">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="7d05a-3343">AppService</span><span class="sxs-lookup"><span data-stu-id="7d05a-3343">AppService</span></span>

* <span data-ttu-id="7d05a-3344">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3344">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="7d05a-3345">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3345">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="7d05a-3346">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3346">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="7d05a-3347">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3347">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="7d05a-3348">DataLake</span><span class="sxs-lookup"><span data-stu-id="7d05a-3348">DataLake</span></span>

* <span data-ttu-id="7d05a-3349">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7d05a-3349">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="7d05a-3350">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7d05a-3350">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="7d05a-3351">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="7d05a-3351">DocuemntDB</span></span>

* <span data-ttu-id="7d05a-3352">DocumentDB: adicionado suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3352">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="7d05a-3353">VM</span><span class="sxs-lookup"><span data-stu-id="7d05a-3353">VM</span></span>

* <span data-ttu-id="7d05a-3354">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3354">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="7d05a-3355">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3355">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="7d05a-3356">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3356">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="7d05a-3357">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3357">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="7d05a-3358">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3358">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="7d05a-3359">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3359">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="7d05a-3360">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="7d05a-3360">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="7d05a-3361">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="7d05a-3361">February 27, 2017</span></span>

<span data-ttu-id="7d05a-3362">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="7d05a-3362">Version 2.0.0</span></span>

<span data-ttu-id="7d05a-3363">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="7d05a-3363">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="7d05a-3364">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3364">Container Service (acs)</span></span>
- <span data-ttu-id="7d05a-3365">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3365">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="7d05a-3366">Rede</span><span class="sxs-lookup"><span data-stu-id="7d05a-3366">Networking</span></span>
- <span data-ttu-id="7d05a-3367">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="7d05a-3367">Storage</span></span>

<span data-ttu-id="7d05a-3368">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3368">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="7d05a-3369">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="7d05a-3369">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="7d05a-3370">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="7d05a-3370">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="7d05a-3371">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="7d05a-3371">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="7d05a-3372">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3372">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="7d05a-3373">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="7d05a-3373">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="7d05a-3374">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3374">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="7d05a-3375">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="7d05a-3375">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="7d05a-3376">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="7d05a-3376">Provide feedback from the command line with the `az feedback` command</span></span>

