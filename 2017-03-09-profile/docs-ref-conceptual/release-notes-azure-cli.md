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
ms.openlocfilehash: e893b99349bbf2a5eec8af254158eb07001f1da7
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="b6d7d-104">Notas de versão da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="b6d7d-104">Azure CLI 2.0 release notes</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="b6d7d-105">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="b6d7d-105">August 28, 2017</span></span>

<span data-ttu-id="b6d7d-106">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="b6d7d-106">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="b6d7d-107">CLI</span><span class="sxs-lookup"><span data-stu-id="b6d7d-107">CLI</span></span>

* <span data-ttu-id="b6d7d-108">Adicionada uma observação legal para `--version`.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-108">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="b6d7d-109">ACS</span><span class="sxs-lookup"><span data-stu-id="b6d7d-109">ACS</span></span>

* <span data-ttu-id="b6d7d-110">Corrigidas as regiões de visualização.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-110">Corrected preview regions.</span></span>
* <span data-ttu-id="b6d7d-111">Corrigida a formatação padrão de `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-111">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="b6d7d-112">Otimização de saída de comando do ACS.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-112">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="b6d7d-113">AppService</span><span class="sxs-lookup"><span data-stu-id="b6d7d-113">Appservice</span></span>

* <span data-ttu-id="b6d7d-114">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-114">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="b6d7d-115">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-115">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="b6d7d-116">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-116">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="b6d7d-117">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6d7d-117">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="b6d7d-118">Correção: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="b6d7d-118">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="b6d7d-119">IoT</span><span class="sxs-lookup"><span data-stu-id="b6d7d-119">IoT</span></span>

* <span data-ttu-id="b6d7d-120">Correção #3934: Criação de política não limpa as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="b6d7d-120">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="b6d7d-121">Rede</span><span class="sxs-lookup"><span data-stu-id="b6d7d-121">Network</span></span>

* <span data-ttu-id="b6d7d-122">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-122">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="b6d7d-123">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-123">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="b6d7d-124">Adicionado suporte para vários IP e intervalos de porta para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-124">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="b6d7d-125">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-125">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="b6d7d-126">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-126">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="b6d7d-127">Perfil</span><span class="sxs-lookup"><span data-stu-id="b6d7d-127">Profile</span></span>

* <span data-ttu-id="b6d7d-128">Exposto `--msi` e `--msi-port` para logon com a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="b6d7d-128">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="b6d7d-129">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="b6d7d-129">Service Fabric</span></span>

* <span data-ttu-id="b6d7d-130">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="b6d7d-130">Preview release</span></span>
* <span data-ttu-id="b6d7d-131">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="b6d7d-131">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="b6d7d-132">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="b6d7d-132">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="b6d7d-133">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="b6d7d-133">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="b6d7d-134">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="b6d7d-134">Storage</span></span>

* <span data-ttu-id="b6d7d-135">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="b6d7d-135">Enabled setting blob tier</span></span>
* <span data-ttu-id="b6d7d-136">Adicionados os argumentos `--bypass` e `--default-action` para `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="b6d7d-136">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="b6d7d-137">Comandos adicionados para adicionar as regras de rede virtual e com base em IP para `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-137">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="b6d7d-138">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="b6d7d-138">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="b6d7d-139">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-139">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="b6d7d-140">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="b6d7d-140">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="b6d7d-141">VM</span><span class="sxs-lookup"><span data-stu-id="b6d7d-141">VM</span></span>

* <span data-ttu-id="b6d7d-142">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-142">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="b6d7d-143">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="b6d7d-143">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="b6d7d-144">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-144">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="b6d7d-145">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="b6d7d-145">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="b6d7d-146">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="b6d7d-146">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="b6d7d-147">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-147">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="b6d7d-148">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="b6d7d-148">August 15, 2017</span></span>

<span data-ttu-id="b6d7d-149">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="b6d7d-149">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="b6d7d-150">ACS</span><span class="sxs-lookup"><span data-stu-id="b6d7d-150">ACS</span></span>

* <span data-ttu-id="b6d7d-151">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="b6d7d-151">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="b6d7d-152">AppService</span><span class="sxs-lookup"><span data-stu-id="b6d7d-152">Appservice</span></span>

* <span data-ttu-id="b6d7d-153">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="b6d7d-153">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="b6d7d-154">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="b6d7d-154">Event Grid</span></span>

* <span data-ttu-id="b6d7d-155">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="b6d7d-155">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="b6d7d-156">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="b6d7d-156">August 11, 2017</span></span>

<span data-ttu-id="b6d7d-157">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="b6d7d-157">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="b6d7d-158">ACS</span><span class="sxs-lookup"><span data-stu-id="b6d7d-158">ACS</span></span>

* <span data-ttu-id="b6d7d-159">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="b6d7d-159">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="b6d7d-160">Batch</span><span class="sxs-lookup"><span data-stu-id="b6d7d-160">Batch</span></span>

* <span data-ttu-id="b6d7d-161">Atualizado para o SDK 3.1.0 do Lote e SDK 4.1.0 do Gerenciamento de Lote</span><span class="sxs-lookup"><span data-stu-id="b6d7d-161">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="b6d7d-162">Adicionado um novo comando que mostra as contagens de tarefa de um trabalho</span><span class="sxs-lookup"><span data-stu-id="b6d7d-162">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="b6d7d-163">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="b6d7d-163">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="b6d7d-164">Ponto de extremidade de conta de lote agora dá suporte ao prefixo conta do Lote “https://” opcional</span><span class="sxs-lookup"><span data-stu-id="b6d7d-164">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="b6d7d-165">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="b6d7d-165">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="b6d7d-166">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="b6d7d-166">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="b6d7d-167">Componente</span><span class="sxs-lookup"><span data-stu-id="b6d7d-167">Component</span></span>

* <span data-ttu-id="b6d7d-168">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="b6d7d-168">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="b6d7d-169">Contêiner</span><span class="sxs-lookup"><span data-stu-id="b6d7d-169">Container</span></span>

* <span data-ttu-id="b6d7d-170">`create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="b6d7d-170">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="b6d7d-171">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="b6d7d-171">Data Lake Store</span></span>

* <span data-ttu-id="b6d7d-172">Habilitado o controle de progresso</span><span class="sxs-lookup"><span data-stu-id="b6d7d-172">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="b6d7d-173">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="b6d7d-173">Event Grid</span></span>

* <span data-ttu-id="b6d7d-174">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="b6d7d-174">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="b6d7d-175">Rede</span><span class="sxs-lookup"><span data-stu-id="b6d7d-175">Network</span></span>

* <span data-ttu-id="b6d7d-176">`lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="b6d7d-176">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="b6d7d-177">`application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="b6d7d-177">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="b6d7d-178">`application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="b6d7d-178">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="b6d7d-179">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-179">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="b6d7d-180">Perfil</span><span class="sxs-lookup"><span data-stu-id="b6d7d-180">Profile</span></span>

* <span data-ttu-id="b6d7d-181">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="b6d7d-181">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="b6d7d-182">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="b6d7d-182">Storage</span></span>

* <span data-ttu-id="b6d7d-183">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="b6d7d-183">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="b6d7d-184">VM</span><span class="sxs-lookup"><span data-stu-id="b6d7d-184">VM</span></span>

* <span data-ttu-id="b6d7d-185">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="b6d7d-185">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="b6d7d-186">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-186">Exposed `list-skus` command</span></span>
* <span data-ttu-id="b6d7d-187">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="b6d7d-187">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="b6d7d-188">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="b6d7d-188">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="b6d7d-189">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="b6d7d-189">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="b6d7d-190">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="b6d7d-190">July 28, 2017</span></span>

<span data-ttu-id="b6d7d-191">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="b6d7d-191">Version 2.0.12</span></span>

* <span data-ttu-id="b6d7d-192">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="b6d7d-192">Added container commands</span></span>
* <span data-ttu-id="b6d7d-193">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="b6d7d-193">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="b6d7d-194">Núcleo</span><span class="sxs-lookup"><span data-stu-id="b6d7d-194">Core</span></span>

* <span data-ttu-id="b6d7d-195">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="b6d7d-195">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="b6d7d-196">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="b6d7d-196">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="b6d7d-197">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="b6d7d-197">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="b6d7d-198">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-198">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="b6d7d-199">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="b6d7d-199">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="b6d7d-200">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-200">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="b6d7d-201">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-201">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="b6d7d-202">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-202">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="b6d7d-203">Aprimorado a desativação de áudio de argumentos de análise e acrescentar histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-203">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="b6d7d-204">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="b6d7d-204">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="b6d7d-205">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="b6d7d-205">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="b6d7d-206">Corrigida a idempotência fixa para criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-206">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="b6d7d-207">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="b6d7d-207">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="b6d7d-208">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="b6d7d-208">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="b6d7d-209">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="b6d7d-209">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="b6d7d-210">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-210">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="b6d7d-211">ACR</span><span class="sxs-lookup"><span data-stu-id="b6d7d-211">ACR</span></span>

* <span data-ttu-id="b6d7d-212">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="b6d7d-212">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="b6d7d-213">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="b6d7d-213">Support SKU update for managed registries</span></span>
* <span data-ttu-id="b6d7d-214">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="b6d7d-214">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="b6d7d-215">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="b6d7d-215">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="b6d7d-216">Adicionada autenticação do AAD adicionada com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="b6d7d-216">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="b6d7d-217">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="b6d7d-217">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="b6d7d-218">ACS</span><span class="sxs-lookup"><span data-stu-id="b6d7d-218">ACS</span></span>

* <span data-ttu-id="b6d7d-219">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="b6d7d-219">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="b6d7d-220">AppService</span><span class="sxs-lookup"><span data-stu-id="b6d7d-220">Appservice</span></span>

* <span data-ttu-id="b6d7d-221">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="b6d7d-221">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="b6d7d-222">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="b6d7d-222">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="b6d7d-223">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-223">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="b6d7d-224">Máscara de senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-224">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="b6d7d-225">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-225">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="b6d7d-226">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-226">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="b6d7d-227">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-227">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="b6d7d-228">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-228">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="b6d7d-229">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-229">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="b6d7d-230">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-230">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="b6d7d-231">Batch</span><span class="sxs-lookup"><span data-stu-id="b6d7d-231">Batch</span></span>

* <span data-ttu-id="b6d7d-232">Atualizado para o SDK 3.0.0 do Lote com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="b6d7d-232">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="b6d7d-233">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-233">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="b6d7d-234">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-234">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="b6d7d-235">CDN</span><span class="sxs-lookup"><span data-stu-id="b6d7d-235">CDN</span></span>

* <span data-ttu-id="b6d7d-236">Fornecida uma mensagem de erro mais adequada para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existe.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-236">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="b6d7d-237">Nuvem</span><span class="sxs-lookup"><span data-stu-id="b6d7d-237">Cloud</span></span>

* <span data-ttu-id="b6d7d-238">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="b6d7d-238">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="b6d7d-239">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="b6d7d-239">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="b6d7d-240">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="b6d7d-240">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="b6d7d-241">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="b6d7d-241">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="b6d7d-242">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-242">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="b6d7d-243">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="b6d7d-243">CosmosDB</span></span>

* <span data-ttu-id="b6d7d-244">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="b6d7d-244">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="b6d7d-245">Adicionado suporte para o TTL padrão de coleção.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-245">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="b6d7d-246">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="b6d7d-246">Data Lake Analytics</span></span>

* <span data-ttu-id="b6d7d-247">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-247">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="b6d7d-248">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-248">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="b6d7d-249">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-249">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="b6d7d-250">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="b6d7d-250">Data Lake Store</span></span>

* <span data-ttu-id="b6d7d-251">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-251">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="b6d7d-252">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="b6d7d-252">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="b6d7d-253">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-253">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="b6d7d-254">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="b6d7d-254">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="b6d7d-255">Interativo</span><span class="sxs-lookup"><span data-stu-id="b6d7d-255">Interactive</span></span>

* <span data-ttu-id="b6d7d-256">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="b6d7d-256">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="b6d7d-257">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="b6d7d-257">Increased test coverage</span></span>
* <span data-ttu-id="b6d7d-258">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="b6d7d-258">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="b6d7d-259">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-259">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="b6d7d-260">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-260">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="b6d7d-261">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-261">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="b6d7d-262">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-262">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="b6d7d-263">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-263">Added `--progress` flag</span></span>
* <span data-ttu-id="b6d7d-264">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="b6d7d-264">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="b6d7d-265">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-265">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="b6d7d-266">IoT</span><span class="sxs-lookup"><span data-stu-id="b6d7d-266">IoT</span></span>

* <span data-ttu-id="b6d7d-267">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-267">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="b6d7d-268">(#3934)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-268">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="b6d7d-269">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="b6d7d-269">Key vault</span></span>

* <span data-ttu-id="b6d7d-270">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="b6d7d-270">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="b6d7d-271">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-271">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="b6d7d-272">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-272">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="b6d7d-273">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-273">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="b6d7d-274">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-274">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="b6d7d-275">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-275">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="b6d7d-276">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-276">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="b6d7d-277">(#3307)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-277">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="b6d7d-278">Laboratório</span><span class="sxs-lookup"><span data-stu-id="b6d7d-278">Lab</span></span>

* <span data-ttu-id="b6d7d-279">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-279">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="b6d7d-280">Adicionada o formatador de tabela `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-280">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="b6d7d-281">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="b6d7d-281">Monitor</span></span>

* <span data-ttu-id="b6d7d-282">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-282">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="b6d7d-283">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-283">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="b6d7d-284">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-284">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="b6d7d-285">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-285">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="b6d7d-286">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-286">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="b6d7d-287">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="b6d7d-287">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="b6d7d-288">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="b6d7d-288">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="b6d7d-289">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="b6d7d-289">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="b6d7d-290">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="b6d7d-290">`location` no longer required</span></span>
  * <span data-ttu-id="b6d7d-291">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="b6d7d-291">Add name and ID support for target</span></span>
  * <span data-ttu-id="b6d7d-292">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-292">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="b6d7d-293">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="b6d7d-293">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="b6d7d-294">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="b6d7d-294">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="b6d7d-295">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="b6d7d-295">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="b6d7d-296">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-296">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="b6d7d-297">Argumentos de conveniência adicional e exemplos para `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-297">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="b6d7d-298">Rede</span><span class="sxs-lookup"><span data-stu-id="b6d7d-298">Network</span></span>

* <span data-ttu-id="b6d7d-299">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-299">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="b6d7d-300">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-300">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="b6d7d-301">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="b6d7d-301">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="b6d7d-302">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="b6d7d-302">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="b6d7d-303">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-303">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="b6d7d-304">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-304">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="b6d7d-305">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-305">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="b6d7d-306">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-306">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="b6d7d-307">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-307">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="b6d7d-308">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-308">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="b6d7d-309">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-309">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="b6d7d-310">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-310">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="b6d7d-311">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-311">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="b6d7d-312">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-312">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="b6d7d-313">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-313">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="b6d7d-314">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-314">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="b6d7d-315">Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS</span><span class="sxs-lookup"><span data-stu-id="b6d7d-315">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="b6d7d-316">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-316">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="b6d7d-317">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-317">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="b6d7d-318">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-318">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="b6d7d-319">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-319">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="b6d7d-320">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-320">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="b6d7d-321">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-321">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="b6d7d-322">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="b6d7d-322">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="b6d7d-323">Usar o pool padrão de pool de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="b6d7d-323">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="b6d7d-324">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="b6d7d-324">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="b6d7d-325">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="b6d7d-325">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="b6d7d-326">Perfil</span><span class="sxs-lookup"><span data-stu-id="b6d7d-326">Profile</span></span>

* <span data-ttu-id="b6d7d-327">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="b6d7d-327">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="b6d7d-328">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="b6d7d-328">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="b6d7d-329">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="b6d7d-329">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="b6d7d-330">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="b6d7d-330">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="b6d7d-331">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="b6d7d-331">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="b6d7d-332">RDBMS</span><span class="sxs-lookup"><span data-stu-id="b6d7d-332">RDBMS</span></span>

* <span data-ttu-id="b6d7d-333">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-333">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="b6d7d-334">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-334">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="b6d7d-335">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-335">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="b6d7d-336">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-336">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="b6d7d-337">Recurso</span><span class="sxs-lookup"><span data-stu-id="b6d7d-337">Resource</span></span>

* <span data-ttu-id="b6d7d-338">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-338">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="b6d7d-339">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-339">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="b6d7d-340">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-340">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="b6d7d-341">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-341">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="b6d7d-342">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-342">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="b6d7d-343">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-343">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="b6d7d-344">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-344">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="b6d7d-345">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-345">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="b6d7d-346">Função</span><span class="sxs-lookup"><span data-stu-id="b6d7d-346">Role</span></span>

* <span data-ttu-id="b6d7d-347">Suporte à saída para no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-347">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="b6d7d-348">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-348">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="b6d7d-349">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-349">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="b6d7d-350">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-350">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="b6d7d-351">Adicionada a integração do cofre da chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-351">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="b6d7d-352">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="b6d7d-352">Service Fabric</span></span>
* <span data-ttu-id="b6d7d-353">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-353">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="b6d7d-354">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-354">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="b6d7d-355">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-355">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="b6d7d-356">SQL</span><span class="sxs-lookup"><span data-stu-id="b6d7d-356">SQL</span></span>

* <span data-ttu-id="b6d7d-357">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-357">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="b6d7d-358">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-358">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="b6d7d-359">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-359">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="b6d7d-360">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="b6d7d-360">Storage</span></span>

* <span data-ttu-id="b6d7d-361">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-361">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="b6d7d-362">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="b6d7d-362">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="b6d7d-363">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-363">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="b6d7d-364">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-364">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="b6d7d-365">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-365">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="b6d7d-366">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-366">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="b6d7d-367">VM</span><span class="sxs-lookup"><span data-stu-id="b6d7d-367">VM</span></span>

* <span data-ttu-id="b6d7d-368">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="b6d7d-368">Support configuring nsg</span></span>
* <span data-ttu-id="b6d7d-369">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="b6d7d-369">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="b6d7d-370">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="b6d7d-370">Support managed service identities</span></span>
* <span data-ttu-id="b6d7d-371">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-371">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="b6d7d-372">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="b6d7d-372">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="b6d7d-373">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="b6d7d-373">May 10, 2017</span></span>

<span data-ttu-id="b6d7d-374">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="b6d7d-374">Version 2.0.6</span></span>

* <span data-ttu-id="b6d7d-375">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="b6d7d-375">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="b6d7d-376">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-376">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="b6d7d-377">Inclusão dos módulos Data Lake Analytics e Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-377">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="b6d7d-378">Inclusão do módulo Serviços Cognitivos.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-378">Include Cognitive Services module.</span></span>
* <span data-ttu-id="b6d7d-379">Inclusão do módulo Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-379">Include Service Fabric module.</span></span>
* <span data-ttu-id="b6d7d-380">Inclusão do módulo Interativo (renomeação de az-shell).</span><span class="sxs-lookup"><span data-stu-id="b6d7d-380">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="b6d7d-381">Adição de suporte para comandos CDN.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-381">Add support for CDN commands.</span></span>
* <span data-ttu-id="b6d7d-382">Remoção do módulo Contêiner.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-382">Remove Container module.</span></span>
* <span data-ttu-id="b6d7d-383">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-383">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="b6d7d-384">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-384">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="b6d7d-385">Núcleo</span><span class="sxs-lookup"><span data-stu-id="b6d7d-385">Core</span></span>

* <span data-ttu-id="b6d7d-386">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="b6d7d-386">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="b6d7d-387">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-387">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="b6d7d-388">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-388">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="b6d7d-389">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-389">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="b6d7d-390">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-390">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="b6d7d-391">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-391">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="b6d7d-392">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-392">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="b6d7d-393">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-393">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="b6d7d-394">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-394">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="b6d7d-395">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="b6d7d-395">core: Improved performance</span></span>
* <span data-ttu-id="b6d7d-396">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="b6d7d-396">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="b6d7d-397">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="b6d7d-397">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="b6d7d-398">ACS</span><span class="sxs-lookup"><span data-stu-id="b6d7d-398">ACS</span></span>

* <span data-ttu-id="b6d7d-399">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6d7d-399">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="b6d7d-400">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="b6d7d-400">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="b6d7d-401">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="b6d7d-401">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="b6d7d-402">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-402">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="b6d7d-403">AppService</span><span class="sxs-lookup"><span data-stu-id="b6d7d-403">AppService</span></span>

* <span data-ttu-id="b6d7d-404">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-404">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="b6d7d-405">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="b6d7d-405">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="b6d7d-406">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-406">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="b6d7d-407">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="b6d7d-407">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="b6d7d-408">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="b6d7d-408">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="b6d7d-409">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-409">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="b6d7d-410">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="b6d7d-410">support slot swap with preview</span></span>
* <span data-ttu-id="b6d7d-411">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-411">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="b6d7d-412">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-412">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="b6d7d-413">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="b6d7d-413">CosmosDB</span></span>

* <span data-ttu-id="b6d7d-414">Renomeação do módulo DocumentDB para CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-414">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="b6d7d-415">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="b6d7d-415">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="b6d7d-416">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="b6d7d-416">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="b6d7d-417">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="b6d7d-417">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="b6d7d-418">Análises Data Lake</span><span class="sxs-lookup"><span data-stu-id="b6d7d-418">Data Lake Analytics</span></span>

* <span data-ttu-id="b6d7d-419">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-419">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="b6d7d-420">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-420">Add support for new catalog item type: package.</span></span> <span data-ttu-id="b6d7d-421">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-421">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="b6d7d-422">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="b6d7d-422">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="b6d7d-423">Tabela</span><span class="sxs-lookup"><span data-stu-id="b6d7d-423">Table</span></span>
  * <span data-ttu-id="b6d7d-424">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="b6d7d-424">Table valued function</span></span>
  * <span data-ttu-id="b6d7d-425">Visualizar</span><span class="sxs-lookup"><span data-stu-id="b6d7d-425">View</span></span>
  * <span data-ttu-id="b6d7d-426">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-426">Table Statistics.</span></span> <span data-ttu-id="b6d7d-427">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-427">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="b6d7d-428">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="b6d7d-428">Data Lake Store</span></span>

* <span data-ttu-id="b6d7d-429">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-429">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="b6d7d-430">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-430">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="b6d7d-431">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-431">missed help for access show.</span></span> <span data-ttu-id="b6d7d-432">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-432">adding it.</span></span> <span data-ttu-id="b6d7d-433">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-433">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="b6d7d-434">Localizar</span><span class="sxs-lookup"><span data-stu-id="b6d7d-434">Find</span></span>

* <span data-ttu-id="b6d7d-435">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="b6d7d-435">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="b6d7d-436">KeyVault</span><span class="sxs-lookup"><span data-stu-id="b6d7d-436">KeyVault</span></span>

* <span data-ttu-id="b6d7d-437">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="b6d7d-437">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="b6d7d-438">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-438">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="b6d7d-439">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="b6d7d-439">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="b6d7d-440">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-440">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="b6d7d-441">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-441">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="b6d7d-442">Laboratório</span><span class="sxs-lookup"><span data-stu-id="b6d7d-442">Lab</span></span>

* <span data-ttu-id="b6d7d-443">Adição dos comandos create, show, delete e list ao ambiente do laboratório.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-443">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="b6d7d-444">Adição dos comandos show e list para exibir modelos ARM no laboratório.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-444">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="b6d7d-445">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-445">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="b6d7d-446">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-446">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="b6d7d-447">Adição de comandos para gerenciar segredos em um Laboratório.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-447">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="b6d7d-448">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="b6d7d-448">Monitor</span></span>

* <span data-ttu-id="b6d7d-449">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-449">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="b6d7d-450">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-450">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="b6d7d-451">Rede</span><span class="sxs-lookup"><span data-stu-id="b6d7d-451">Network</span></span>

* <span data-ttu-id="b6d7d-452">Adição do comando `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-452">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="b6d7d-453">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-453">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="b6d7d-454">Adição de suporte para drenagem de conexão do Gateway de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-454">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="b6d7d-455">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-455">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="b6d7d-456">Adição de suporte para filtros de rota e regras do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-456">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="b6d7d-457">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-457">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="b6d7d-458">Adição de suporte para seletores de tráfego baseados em política da conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-458">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="b6d7d-459">Adição de suporte para políticas IPsec da conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-459">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="b6d7d-460">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-460">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="b6d7d-461">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="b6d7d-461">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="b6d7d-462">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-462">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="b6d7d-463">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="b6d7d-463">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="b6d7d-464">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-464">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="b6d7d-465">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-465">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="b6d7d-466">Correção de um bug em que `traffic-manager endpoint update` não funciona.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-466">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="b6d7d-467">Adição de comandos de visualização “network watcher”.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-467">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="b6d7d-468">Perfil</span><span class="sxs-lookup"><span data-stu-id="b6d7d-468">Profile</span></span>

* <span data-ttu-id="b6d7d-469">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-469">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="b6d7d-470">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-470">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="b6d7d-471">Redis</span><span class="sxs-lookup"><span data-stu-id="b6d7d-471">Redis</span></span>

* <span data-ttu-id="b6d7d-472">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="b6d7d-472">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="b6d7d-473">Preterição do comando “update-settings”.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-473">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="b6d7d-474">Recurso</span><span class="sxs-lookup"><span data-stu-id="b6d7d-474">Resource</span></span>

* <span data-ttu-id="b6d7d-475">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-475">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="b6d7d-476">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-476">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="b6d7d-477">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-477">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="b6d7d-478">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-478">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="b6d7d-479">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-479">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="b6d7d-480">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-480">Add docs for az lock update.</span></span> <span data-ttu-id="b6d7d-481">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-481">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="b6d7d-482">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-482">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="b6d7d-483">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-483">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="b6d7d-484">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-484">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="b6d7d-485">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-485">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="b6d7d-486">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-486">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="b6d7d-487">Função</span><span class="sxs-lookup"><span data-stu-id="b6d7d-487">Role</span></span>

* <span data-ttu-id="b6d7d-488">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-488">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="b6d7d-489">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-489">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="b6d7d-490">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-490">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="b6d7d-491">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="b6d7d-491">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="b6d7d-492">SQL</span><span class="sxs-lookup"><span data-stu-id="b6d7d-492">SQL</span></span>

* <span data-ttu-id="b6d7d-493">Adição dos comandos az sql server list-usages e az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-493">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="b6d7d-494">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-494">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="b6d7d-495">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="b6d7d-495">Storage</span></span>

* <span data-ttu-id="b6d7d-496">Localização padrão da localização do grupo de recursos de `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-496">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="b6d7d-497">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="b6d7d-497">Add support for incremental blob copy</span></span>
* <span data-ttu-id="b6d7d-498">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="b6d7d-498">Add support for large block blob upload</span></span>
* <span data-ttu-id="b6d7d-499">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="b6d7d-499">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="b6d7d-500">VM</span><span class="sxs-lookup"><span data-stu-id="b6d7d-500">VM</span></span>

* <span data-ttu-id="b6d7d-501">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="b6d7d-501">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="b6d7d-502">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="b6d7d-502">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="b6d7d-503">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="b6d7d-503">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="b6d7d-504">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="b6d7d-504">az vm/vmss disk</span></span>
  3. <span data-ttu-id="b6d7d-505">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="b6d7d-505">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="b6d7d-506">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="b6d7d-506">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="b6d7d-507">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-507">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="b6d7d-508">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="b6d7d-508">April 3, 2017</span></span>

<span data-ttu-id="b6d7d-509">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="b6d7d-509">Version 2.0.2</span></span>

<span data-ttu-id="b6d7d-510">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-510">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="b6d7d-511">Núcleo</span><span class="sxs-lookup"><span data-stu-id="b6d7d-511">Core</span></span>

* <span data-ttu-id="b6d7d-512">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-512">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="b6d7d-513">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-513">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="b6d7d-514">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-514">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="b6d7d-515">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-515">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="b6d7d-516">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-516">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="b6d7d-517">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-517">Add prompting for missing template parameters.</span></span> <span data-ttu-id="b6d7d-518">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-518">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="b6d7d-519">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="b6d7d-519">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="b6d7d-520">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="b6d7d-520">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="b6d7d-521">ACS</span><span class="sxs-lookup"><span data-stu-id="b6d7d-521">ACS</span></span>

* <span data-ttu-id="b6d7d-522">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([&#2554;](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-522">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="b6d7d-523">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-523">Add support for ssh key password prompting.</span></span> <span data-ttu-id="b6d7d-524">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-524">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="b6d7d-525">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-525">Add support for windows clusters.</span></span> <span data-ttu-id="b6d7d-526">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-526">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="b6d7d-527">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-527">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="b6d7d-528">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-528">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="b6d7d-529">AppService</span><span class="sxs-lookup"><span data-stu-id="b6d7d-529">AppService</span></span>

* <span data-ttu-id="b6d7d-530">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-530">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="b6d7d-531">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-531">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="b6d7d-532">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-532">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="b6d7d-533">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-533">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="b6d7d-534">DataLake</span><span class="sxs-lookup"><span data-stu-id="b6d7d-534">DataLake</span></span>

* <span data-ttu-id="b6d7d-535">Versão inicial do módulo do Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-535">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="b6d7d-536">Versão inicial do módulo do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-536">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="b6d7d-537">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="b6d7d-537">DocuemntDB</span></span>

* <span data-ttu-id="b6d7d-538">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-538">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="b6d7d-539">VM</span><span class="sxs-lookup"><span data-stu-id="b6d7d-539">VM</span></span>

* <span data-ttu-id="b6d7d-540">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-540">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="b6d7d-541">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-541">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="b6d7d-542">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-542">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="b6d7d-543">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-543">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="b6d7d-544">Conjunto de dimensionamento de máquinas virtuais: suporte à * para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-544">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="b6d7d-545">Adicionar --secrets para o conjunto de dimensionamento de máquinas virtuais e VM ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-545">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="b6d7d-546">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="b6d7d-546">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="b6d7d-547">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="b6d7d-547">February 27, 2017</span></span>

<span data-ttu-id="b6d7d-548">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="b6d7d-548">Version 2.0.0</span></span>

<span data-ttu-id="b6d7d-549">Essa versão da CLI do Azure 2.0 é a primeira versão “Disponível”.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-549">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="b6d7d-550">A disponibilidade se aplica a esses módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="b6d7d-550">General availability applies to these command modules:</span></span>
- <span data-ttu-id="b6d7d-551">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-551">Container Service (acs)</span></span>
- <span data-ttu-id="b6d7d-552">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-552">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="b6d7d-553">Rede</span><span class="sxs-lookup"><span data-stu-id="b6d7d-553">Networking</span></span>
- <span data-ttu-id="b6d7d-554">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="b6d7d-554">Storage</span></span>

<span data-ttu-id="b6d7d-555">Esses módulos de comando podem ser usados na produção e são compatíveis com o SLA do Microsoft padrão.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-555">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="b6d7d-556">Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="b6d7d-556">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="b6d7d-557">Você pode fazer perguntas sobre [StackOverflow usando a marcação azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) ou entrar em contato com a equipe do produto pelo endereço [ azfeedback@microsoft.com ](mailto:azfeedback@microsoft.com). Você pode fornecer comentários a partir da linha de comando com o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-557">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="b6d7d-558">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-558">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="b6d7d-559">Para verificar a versão da CLI, utilize `az --version`.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-559">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="b6d7d-560">A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-560">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="b6d7d-561">Alguns dos módulos de comando têm um “b*n*” ou “rc*n*” pós-fixado.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-561">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="b6d7d-562">Esses módulos de comando ainda estão em visualização e estarão disponíveis no futuro.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-562">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="b6d7d-563">Também temos compilações de visualização diárias da CLI.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-563">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="b6d7d-564">Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="b6d7d-564">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="b6d7d-565">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="b6d7d-565">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="b6d7d-566">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="b6d7d-566">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="b6d7d-567">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="b6d7d-567">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="b6d7d-568">Forneça comentários a partir da linha de comando com o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="b6d7d-568">Provide feedback from the command line with the `az feedback` command.</span></span>

