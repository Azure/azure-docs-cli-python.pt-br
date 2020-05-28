---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 05/19/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: c95a635cc58afcc7956c230d0e3f47351fa0893d
ms.sourcegitcommit: d05660a42b2a77c4b05a7f96c386e656bd2db0fe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "83569180"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="10322-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="10322-103">Azure CLI release notes</span></span>

## <a name="may-19-2020"></a><span data-ttu-id="10322-104">19 de maio de 2020</span><span class="sxs-lookup"><span data-stu-id="10322-104">May 19, 2020</span></span>

<span data-ttu-id="10322-105">Versão 2.6.0</span><span class="sxs-lookup"><span data-stu-id="10322-105">Version 2.6.0</span></span>

### <a name="acr"></a><span data-ttu-id="10322-106">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-106">ACR</span></span>

* <span data-ttu-id="10322-107">Adiciona tempo limite padrão de 5 minutos para solicitações ao ACR</span><span class="sxs-lookup"><span data-stu-id="10322-107">Add default timeout of 5 minutes for any requests to ACR</span></span>
* <span data-ttu-id="10322-108">Suporte para desabilitar o acesso à redes públicas</span><span class="sxs-lookup"><span data-stu-id="10322-108">Support disable public network access</span></span>
* <span data-ttu-id="10322-109">`az acr token create`: expõe o argumento --days</span><span class="sxs-lookup"><span data-stu-id="10322-109">`az acr token create`: expose --days argument</span></span>
* <span data-ttu-id="10322-110">`az acr import`: aceita valores do argumento --source que contêm logon no nome do servidor por meio da correção final do cliente</span><span class="sxs-lookup"><span data-stu-id="10322-110">`az acr import`: accept --source argument values which contain login in server name through client end correction</span></span>

### <a name="acs"></a><span data-ttu-id="10322-111">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-111">ACS</span></span>

* <span data-ttu-id="10322-112">Correção de bug: remover limpeza de campos para campos que não existem mais</span><span class="sxs-lookup"><span data-stu-id="10322-112">Bug fix: remove fields cleanup for fields that no longer exist</span></span>

### <a name="aks"></a><span data-ttu-id="10322-113">AKS</span><span class="sxs-lookup"><span data-stu-id="10322-113">AKS</span></span>

* <span data-ttu-id="10322-114">Atualiza o tempo de atividade do contexto de ajuda de comando do SLA</span><span class="sxs-lookup"><span data-stu-id="10322-114">Update uptime-sla command help context</span></span>
* <span data-ttu-id="10322-115">Remove a verificação do intervalo para a atualização da contagem de minutos do dimensionador automático</span><span class="sxs-lookup"><span data-stu-id="10322-115">Remove range check for updating min count for autoscaler</span></span>
* <span data-ttu-id="10322-116">Corrige o problema que fazia com que a CLI falhasse quando o usuário especificava apenas a senha do Windows</span><span class="sxs-lookup"><span data-stu-id="10322-116">Fix that cli doe not fail when user only specifies Windows password</span></span>

### <a name="ams"></a><span data-ttu-id="10322-117">AMS</span><span class="sxs-lookup"><span data-stu-id="10322-117">AMS</span></span>

* <span data-ttu-id="10322-118">`az ams transform create`: Adiciona a capacidade de criar uma transformação com um FaceDetector predefinido</span><span class="sxs-lookup"><span data-stu-id="10322-118">`az ams transform create`: Add ability to create a transform with a FaceDetector preset</span></span>
* <span data-ttu-id="10322-119">`az ams content-key-policy create`: Adiciona a capacidade de criar uma política de chave de conteúdo do FairPlay com uma configuração de aluguel offline</span><span class="sxs-lookup"><span data-stu-id="10322-119">`az ams content-key-policy create` : Add ability to create a FairPlay content key policy with an offline rental configuration</span></span>

### <a name="appconfig"></a><span data-ttu-id="10322-120">AppConfig</span><span class="sxs-lookup"><span data-stu-id="10322-120">AppConfig</span></span>

* <span data-ttu-id="10322-121">Correção de bug para valores de chave da lista com campos</span><span class="sxs-lookup"><span data-stu-id="10322-121">Bug fix for list key values with fields</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-122">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-122">AppService</span></span>

* <span data-ttu-id="10322-123">`az functionapp create`: AzureWebJobsDashboard será definido somente se AppInsights estiver desabilitado</span><span class="sxs-lookup"><span data-stu-id="10322-123">`az functionapp create`: AzureWebJobsDashboard will only be set if AppInsights is disabled</span></span>
* <span data-ttu-id="10322-124">Correção #10664 – Integração VNet – Problema de Verificação de Localização e Correção #13257-AZ Web App falha quando o RG precisar ser criado</span><span class="sxs-lookup"><span data-stu-id="10322-124">Fix #10664- VNet Integration - Location Check Issue & fix #13257- az webapp up failing when RG needs to be created</span></span>
* <span data-ttu-id="10322-125">`az webapp|functionapp config ssl import`: Pesquisa o cofre de chaves em grupos de recursos na assinatura e aprimora a ajuda e os exemplos.</span><span class="sxs-lookup"><span data-stu-id="10322-125">`az webapp|functionapp config ssl import`: Lookup key vault across resources groups in subscription and improve help and examples.</span></span>
* <span data-ttu-id="10322-126">Integra o contexto local para o serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="10322-126">Onboard local context for app service</span></span>

### <a name="arm"></a><span data-ttu-id="10322-127">ARM</span><span class="sxs-lookup"><span data-stu-id="10322-127">ARM</span></span>

* <span data-ttu-id="10322-128">`az deployment`: Corrige o problema que faz com que o templateLink não seja retornado ao implantar ou validar o template-uri</span><span class="sxs-lookup"><span data-stu-id="10322-128">`az deployment`: Fix the problem that the templateLink will not be returned when deploying or validating template-uri</span></span>
* <span data-ttu-id="10322-129">`az deployment`: Corrige o problema que faz com que implantação/validação não dê suporte ao caractere codificado especialmente</span><span class="sxs-lookup"><span data-stu-id="10322-129">`az deployment`: Fix the problem that deployment/validate does not support specially encoded character</span></span>
* <span data-ttu-id="10322-130">`az deployment sub/group what-if`: Corrige o alinhamento de matriz e o tratamento de erro</span><span class="sxs-lookup"><span data-stu-id="10322-130">`az deployment sub/group what-if`: Fix array alignment and error handling</span></span>
* <span data-ttu-id="10322-131">`az deployment operation`: Modifica as informações preteridas</span><span class="sxs-lookup"><span data-stu-id="10322-131">`az deployment operation`: Modify the deprecate information</span></span>

### <a name="aro"></a><span data-ttu-id="10322-132">ARO</span><span class="sxs-lookup"><span data-stu-id="10322-132">ARO</span></span>

* <span data-ttu-id="10322-133">Adiciona exemplos para az aro create, list, list-credentials, show, delete</span><span class="sxs-lookup"><span data-stu-id="10322-133">Add examples to az aro create, list, list-credentials, show, delete</span></span>
* <span data-ttu-id="10322-134">Adiciona a função generate_random_id</span><span class="sxs-lookup"><span data-stu-id="10322-134">Add generate_random_id function</span></span>

### <a name="backup"></a><span data-ttu-id="10322-135">Backup</span><span class="sxs-lookup"><span data-stu-id="10322-135">Backup</span></span>

* <span data-ttu-id="10322-136">Permite FriendlyName ao habilitar proteção para o comando AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="10322-136">Allow FriendlyName in enable protection for AzureFileShare command</span></span>
* <span data-ttu-id="10322-137">Correção do comando restore-disks da IaasVM</span><span class="sxs-lookup"><span data-stu-id="10322-137">Fix in IaasVM restore-disks Command</span></span>
* <span data-ttu-id="10322-138">Adiciona o BackupManagementType "MAB" ao comando item list</span><span class="sxs-lookup"><span data-stu-id="10322-138">Add "MAB" BackupManagementType to item list command</span></span>
* <span data-ttu-id="10322-139">Adiciona suporte para a repetição de tentativas de atualização da política para itens com falha.</span><span class="sxs-lookup"><span data-stu-id="10322-139">Add support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="10322-140">Adiciona a funcionalidade de Retomada de Proteção para as Máquinas Virtuais do Azure</span><span class="sxs-lookup"><span data-stu-id="10322-140">Add Resume Protection functionality for Azure Virtual Machine</span></span>
* <span data-ttu-id="10322-141">Adiciona suporte para especificar o ResourceGroup para armazenar instantRP durante a Criação ou Modificação de Política</span><span class="sxs-lookup"><span data-stu-id="10322-141">Add support to specify ResourceGroup for storing instantRP during Create or Modify Policy</span></span>

### <a name="ci"></a><span data-ttu-id="10322-142">CI</span><span class="sxs-lookup"><span data-stu-id="10322-142">CI</span></span>

* <span data-ttu-id="10322-143">Suporte para flake8 3.8.0</span><span class="sxs-lookup"><span data-stu-id="10322-143">Support flake8 3.8.0</span></span>

### <a name="compute"></a><span data-ttu-id="10322-144">Computação</span><span class="sxs-lookup"><span data-stu-id="10322-144">Compute</span></span>

* <span data-ttu-id="10322-145">Novo comando az vm auto-shutdown</span><span class="sxs-lookup"><span data-stu-id="10322-145">New command az vm auto-shutdown</span></span>
* <span data-ttu-id="10322-146">`az vm list-skus`: Atualização do comportamento --zone, retorna SKUs de todos os tipos agora</span><span class="sxs-lookup"><span data-stu-id="10322-146">`az vm list-skus`: Update --zone behavior, return all type skus now</span></span>

### <a name="core"></a><span data-ttu-id="10322-147">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-147">Core</span></span>

* <span data-ttu-id="10322-148">Atualiza o status de ativado/desativado do contexto local para o nível de usuário global</span><span class="sxs-lookup"><span data-stu-id="10322-148">Update local context on/off status to global user level</span></span>

### <a name="extension"></a><span data-ttu-id="10322-149">Extensão</span><span class="sxs-lookup"><span data-stu-id="10322-149">Extension</span></span>

* <span data-ttu-id="10322-150">`az extension add`: Adiciona --system para habilitar a instalação de extensões em um caminho do sistema</span><span class="sxs-lookup"><span data-stu-id="10322-150">`az extension add`: Add --system to enable installing extensions in a system path</span></span>
* <span data-ttu-id="10322-151">Suporte para .egg-info para armazenar metadados de extensão de tipo de roda</span><span class="sxs-lookup"><span data-stu-id="10322-151">Support .egg-info to store wheel type extension metadata</span></span>

### <a name="iot"></a><span data-ttu-id="10322-152">IoT</span><span class="sxs-lookup"><span data-stu-id="10322-152">IoT</span></span>

* <span data-ttu-id="10322-153">`az iot`: Atualiza a mensagem de reconhecimento de extensão da primeira execução do módulo de comando IoT para a ID precisa e moderna não preterida `azure-iot`.</span><span class="sxs-lookup"><span data-stu-id="10322-153">`az iot`: Update the IoT command module first run extension awareness message to the accurate, non-deprecated modern Id `azure-iot`.</span></span>

### <a name="iot-hub"></a><span data-ttu-id="10322-154">Hub IoT</span><span class="sxs-lookup"><span data-stu-id="10322-154">IoT Hub</span></span>

* <span data-ttu-id="10322-155">Suporte para comandos de isolamento de rede e API 2020-03-01</span><span class="sxs-lookup"><span data-stu-id="10322-155">Support for 2020-03-01 API and Network Isolation commands</span></span>

### <a name="netappfiles"></a><span data-ttu-id="10322-156">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="10322-156">NetAppFiles</span></span>

* <span data-ttu-id="10322-157">`az volume create`: Adiciona snapshot-id como um parâmetro para criar volume – isso permitirá que os usuários criem um volume por meio de um instantâneo existente.</span><span class="sxs-lookup"><span data-stu-id="10322-157">`az volume create`: Adds snapshot-id as a parameter to create volume this will allow users to create a volume from existing snapshot.</span></span>

### <a name="network"></a><span data-ttu-id="10322-158">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-158">Network</span></span>

* <span data-ttu-id="10322-159">Corrige o valor TTL alterado não destinado ao DNS add-record</span><span class="sxs-lookup"><span data-stu-id="10322-159">Fix ttl value changed unintended for dns add-record</span></span>
* <span data-ttu-id="10322-160">`az network public-ip create`: Informa os clientes sobre futuras alterações da falha</span><span class="sxs-lookup"><span data-stu-id="10322-160">`az network public-ip create`: Inform customers of a coming breaking change</span></span>
* <span data-ttu-id="10322-161">Suporte para comandos genéricos para cenários de link privado</span><span class="sxs-lookup"><span data-stu-id="10322-161">Support generic commands for private link scenario</span></span>
* <span data-ttu-id="10322-162">`az network private-endpoint-connection`: Suporte para tipos mysql, postgre e mariadb</span><span class="sxs-lookup"><span data-stu-id="10322-162">`az network private-endpoint-connection`: Support mysql, postgre and mariadb types</span></span>
* <span data-ttu-id="10322-163">`az network private-endpoint-connection`: Suporte para tipos cosmosdb</span><span class="sxs-lookup"><span data-stu-id="10322-163">`az network private-endpoint-connection`: Support cosmosdb types</span></span>
* <span data-ttu-id="10322-164">`az network private-endpoint`: pretere --group-ids e redireciona para --group-id</span><span class="sxs-lookup"><span data-stu-id="10322-164">`az network private-endpoint`: deprecate --group-ids and redirect to --group-id</span></span>

### <a name="output"></a><span data-ttu-id="10322-165">Saída</span><span class="sxs-lookup"><span data-stu-id="10322-165">Output</span></span>

* <span data-ttu-id="10322-166">Mostra instruções de atualização em localizar, comentários e --help</span><span class="sxs-lookup"><span data-stu-id="10322-166">Show update instruction in find, feedback and --help</span></span>

### <a name="packaging"></a><span data-ttu-id="10322-167">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="10322-167">Packaging</span></span>

* <span data-ttu-id="10322-168">Cria pacotes MSI/Homebrew com dependências resolvidas de requirements.txt</span><span class="sxs-lookup"><span data-stu-id="10322-168">Build MSI/Homebrew packages with dependecies resolved from requirements.txt</span></span>

### <a name="rbac"></a><span data-ttu-id="10322-169">RBAC</span><span class="sxs-lookup"><span data-stu-id="10322-169">RBAC</span></span>

* <span data-ttu-id="10322-170">`az ad sp credential reset`: corrige a geração de credenciais fracas</span><span class="sxs-lookup"><span data-stu-id="10322-170">`az ad sp credential reset`: fix weak credential generation</span></span>

### <a name="storage"></a><span data-ttu-id="10322-171">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-171">Storage</span></span>

* <span data-ttu-id="10322-172">`az storage account file-service-properties update/show`: Adiciona suporte a propriedades de arquivo para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-172">`az storage account file-service-properties update/show`: Add File Properties Support for Storage Account</span></span>
* <span data-ttu-id="10322-173">`az storage container create`: Correção #13373 ao adicionar o validador para acesso público</span><span class="sxs-lookup"><span data-stu-id="10322-173">`az storage container create`: Fix #13373 by adding validator for public access</span></span>
* <span data-ttu-id="10322-174">Adiciona suporte a ADLS Gen2 track2</span><span class="sxs-lookup"><span data-stu-id="10322-174">Add ADLS Gen2 track2 support</span></span>
* <span data-ttu-id="10322-175">`az storage blob sync`: Dar suporte à `--connection-string`</span><span class="sxs-lookup"><span data-stu-id="10322-175">`az storage blob sync`: Support `--connection-string`</span></span>
* <span data-ttu-id="10322-176">`az storage blob sync`: Corrige a mensagem de erro incorreta quando azcopy não consegue encontrar o local de instalação</span><span class="sxs-lookup"><span data-stu-id="10322-176">`az storage blob sync`: Fix the incorrect error message when azcopy cannot find the installation location</span></span>

## <a name="april-30-2020"></a><span data-ttu-id="10322-177">30 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="10322-177">April 30, 2020</span></span>

<span data-ttu-id="10322-178">Versão 2.5.1</span><span class="sxs-lookup"><span data-stu-id="10322-178">Version 2.5.1</span></span>

### <a name="acr"></a><span data-ttu-id="10322-179">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-179">ACR</span></span>

* <span data-ttu-id="10322-180">`az acr check-health`: correção de "DOCKER_PULL_ERROR" no Windows</span><span class="sxs-lookup"><span data-stu-id="10322-180">`az acr check-health`: Fix "DOCKER_PULL_ERROR" on Windows</span></span>

### <a name="compute"></a><span data-ttu-id="10322-181">Computação</span><span class="sxs-lookup"><span data-stu-id="10322-181">Compute</span></span>

* <span data-ttu-id="10322-182">`az vm list-ip-addresses`: Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="10322-182">`az vm list-ip-addresses`: Error handling</span></span>
* <span data-ttu-id="10322-183">Correção de um bug de criação de VM caso endpoint_vm_image_alias_doc não estivesse definido no perfil de nuvem</span><span class="sxs-lookup"><span data-stu-id="10322-183">Fix a bug of vm create if endpoint_vm_image_alias_doc is not set in cloud profile</span></span>
* <span data-ttu-id="10322-184">`az vmss create`: adição de --os-disk-size-gb</span><span class="sxs-lookup"><span data-stu-id="10322-184">`az vmss create`: Add --os-disk-size-gb</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="10322-185">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="10322-185">Cosmos DB</span></span>

* <span data-ttu-id="10322-186">`az cosmosdb create/update`: adição de suporte a --enable-public-network</span><span class="sxs-lookup"><span data-stu-id="10322-186">`az cosmosdb create/update`: add --enable-public-network support</span></span>

### <a name="extension"></a><span data-ttu-id="10322-187">Extensão</span><span class="sxs-lookup"><span data-stu-id="10322-187">Extension</span></span>

* <span data-ttu-id="10322-188">Correção do carregamento de metadados errados para a extensão de tipo roda</span><span class="sxs-lookup"><span data-stu-id="10322-188">Fix loading wrong metadata for wheel type extension</span></span>

### <a name="packaging"></a><span data-ttu-id="10322-189">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="10322-189">Packaging</span></span>

* <span data-ttu-id="10322-190">Adição de script az para Git Bash/Cygwin no Windows</span><span class="sxs-lookup"><span data-stu-id="10322-190">Add az script for Git Bash/Cygwin on Windows</span></span>

### <a name="sql"></a><span data-ttu-id="10322-191">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-191">SQL</span></span>

* <span data-ttu-id="10322-192">`az sql instance-pool`: adição de grupo de comando de pools de instância</span><span class="sxs-lookup"><span data-stu-id="10322-192">`az sql instance-pool`: Add instance pools command group</span></span>

### <a name="storage"></a><span data-ttu-id="10322-193">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-193">Storage</span></span>

* <span data-ttu-id="10322-194">Atualização do pacote azure-multiapi-storage para 0.3.0</span><span class="sxs-lookup"><span data-stu-id="10322-194">Upgrade package azure-multiapi-storage to 0.3.0</span></span>
* <span data-ttu-id="10322-195">Dá suporte ao GZRS para a criação e atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-195">Support GZRS for storage account creation and update</span></span>
* <span data-ttu-id="10322-196">`az storage account failover`: adição de suporte para failover da conta de armazenamento de GRS/GZRS</span><span class="sxs-lookup"><span data-stu-id="10322-196">`az storage account failover`: Add support for grs/gzrs storage account failover</span></span>
* <span data-ttu-id="10322-197">`az storage blob upload`: adição do parâmetro --encryption-scope para dar suporte à especificação da informação do escopo da criptografia</span><span class="sxs-lookup"><span data-stu-id="10322-197">`az storage blob upload`: Add --encryption-scope parameter to support specifying encryption scope information</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="10322-198">28 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="10322-198">April 28, 2020</span></span>

<span data-ttu-id="10322-199">Versão 2.5.0</span><span class="sxs-lookup"><span data-stu-id="10322-199">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="10322-200">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-200">ACS</span></span>

* <span data-ttu-id="10322-201">[ALTERAÇÃO SIGNIFICATIVA] az openshift create: remove o parâmetro --vnet-peer.</span><span class="sxs-lookup"><span data-stu-id="10322-201">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="10322-202">`az openshift create`: adição de sinalizadores para dar suporte a clusters privados.</span><span class="sxs-lookup"><span data-stu-id="10322-202">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="10322-203">`az openshift`: atualização para a versão `2019-10-27-preview` da API.</span><span class="sxs-lookup"><span data-stu-id="10322-203">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="10322-204">`az openshift`: adição do comando `update`.</span><span class="sxs-lookup"><span data-stu-id="10322-204">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="10322-205">AKS</span><span class="sxs-lookup"><span data-stu-id="10322-205">AKS</span></span>

* <span data-ttu-id="10322-206">`az aks create`: adição do suporte para Windows</span><span class="sxs-lookup"><span data-stu-id="10322-206">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-207">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-207">AppService</span></span>

* <span data-ttu-id="10322-208">`az webapp deployment source config-zip`: remoção da suspensão após request.get()</span><span class="sxs-lookup"><span data-stu-id="10322-208">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="10322-209">ARM</span><span class="sxs-lookup"><span data-stu-id="10322-209">ARM</span></span>

* <span data-ttu-id="10322-210">Adição de comandos What-If de implantação de modelo</span><span class="sxs-lookup"><span data-stu-id="10322-210">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="10322-211">ARO</span><span class="sxs-lookup"><span data-stu-id="10322-211">ARO</span></span>

* <span data-ttu-id="10322-212">`az aro`: correção da saída da tabela</span><span class="sxs-lookup"><span data-stu-id="10322-212">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="10322-213">CI</span><span class="sxs-lookup"><span data-stu-id="10322-213">CI</span></span>

* <span data-ttu-id="10322-214">Integração do pytest e preterição do nose para o teste de automação</span><span class="sxs-lookup"><span data-stu-id="10322-214">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="10322-215">Computação</span><span class="sxs-lookup"><span data-stu-id="10322-215">Compute</span></span>

* <span data-ttu-id="10322-216">`az vmss disk detach`: correção do problema de NoneType do disco de dados</span><span class="sxs-lookup"><span data-stu-id="10322-216">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="10322-217">`az vm availability-set list`: suporte à exibição da lista de VM</span><span class="sxs-lookup"><span data-stu-id="10322-217">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="10322-218">`az vm list-skus`: correção do problema de exibição do formato de tabela</span><span class="sxs-lookup"><span data-stu-id="10322-218">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="10322-219">KeyVault</span><span class="sxs-lookup"><span data-stu-id="10322-219">KeyVault</span></span>

* <span data-ttu-id="10322-220">Adição de novo parâmetro `--enable-rbac-authorization` durante a criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="10322-220">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-221">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-221">Monitor</span></span>

* <span data-ttu-id="10322-222">Suporte aos recursos de CMK do cluster de LA</span><span class="sxs-lookup"><span data-stu-id="10322-222">Support LA cluster CMK features</span></span>
* <span data-ttu-id="10322-223">`az monitor log-analytics workspace linked-storage`: dá suporte aos recursos BYOS</span><span class="sxs-lookup"><span data-stu-id="10322-223">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="10322-224">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-224">Network</span></span>

* <span data-ttu-id="10322-225">`az network security-partner`: suporte para provedor de segurança de parceiros</span><span class="sxs-lookup"><span data-stu-id="10322-225">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="10322-226">Privatedns</span><span class="sxs-lookup"><span data-stu-id="10322-226">Privatedns</span></span>

* <span data-ttu-id="10322-227">Adição do recurso na zona DNS privada para importar o arquivo da zona de exportação</span><span class="sxs-lookup"><span data-stu-id="10322-227">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="10322-228">21 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="10322-228">April 21, 2020</span></span>

<span data-ttu-id="10322-229">Versão 2.4.0</span><span class="sxs-lookup"><span data-stu-id="10322-229">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="10322-230">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-230">ACR</span></span>

* <span data-ttu-id="10322-231">`az acr run --cmd`: desabilitar a substituição do diretório de trabalho</span><span class="sxs-lookup"><span data-stu-id="10322-231">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="10322-232">Suporte ao ponto de extremidade dos dados dedicados</span><span class="sxs-lookup"><span data-stu-id="10322-232">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="10322-233">AKS</span><span class="sxs-lookup"><span data-stu-id="10322-233">AKS</span></span>

* <span data-ttu-id="10322-234">`az aks list -o table` deve mostrar privateFqdn como fqdn para clusters privados</span><span class="sxs-lookup"><span data-stu-id="10322-234">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="10322-235">Adicionar --uptime-sla</span><span class="sxs-lookup"><span data-stu-id="10322-235">Add --uptime-sla</span></span>
* <span data-ttu-id="10322-236">Atualizar pacote containerservice</span><span class="sxs-lookup"><span data-stu-id="10322-236">Update containerservice package</span></span>
* <span data-ttu-id="10322-237">Adicionar suporte ao IP público do nó</span><span class="sxs-lookup"><span data-stu-id="10322-237">Add node public IP support</span></span>
* <span data-ttu-id="10322-238">Corrigir erros de digitação no comando de ajuda</span><span class="sxs-lookup"><span data-stu-id="10322-238">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="10322-239">AppConfig</span><span class="sxs-lookup"><span data-stu-id="10322-239">AppConfig</span></span>

* <span data-ttu-id="10322-240">Resolver referência do cofre de chaves para os comandos kv list e export</span><span class="sxs-lookup"><span data-stu-id="10322-240">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="10322-241">Correção de bug para valores de chave da lista</span><span class="sxs-lookup"><span data-stu-id="10322-241">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-242">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-242">AppService</span></span>

* <span data-ttu-id="10322-243">`az functionapp create`: mudou a maneira como o linuxFxVersion estava sendo definido para os aplicativos de funções dotnet linux.</span><span class="sxs-lookup"><span data-stu-id="10322-243">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="10322-244">Isso deve corrigir um bug que estava impedindo a criação de aplicativos de consumo em dotnet linux</span><span class="sxs-lookup"><span data-stu-id="10322-244">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="10322-245">[ALTERAÇÃO DA FALHA] `az webapp create`: correção para manter o AppSettings existente com o az webapp create</span><span class="sxs-lookup"><span data-stu-id="10322-245">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="10322-246">[ALTERAÇÃO DA FALHA] `az webapp up`: correção para criar o RG para o comando az webapp up ao usar o sinalizador -g</span><span class="sxs-lookup"><span data-stu-id="10322-246">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="10322-247">[ALTERAÇÃO DA FALHA] `az webapp config`: correção para mostrar valores de saída não JSON com o az webapp config connection-string list</span><span class="sxs-lookup"><span data-stu-id="10322-247">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="10322-248">ARM</span><span class="sxs-lookup"><span data-stu-id="10322-248">ARM</span></span>

* <span data-ttu-id="10322-249">`az deployment create/validate`: adicionar o parâmetro `--no-prompt` para dar suporte à ação de ignorar o prompt de parâmetros ausentes para o modelo do Resource Manager</span><span class="sxs-lookup"><span data-stu-id="10322-249">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="10322-250">`az deployment group/mg/sub/tenant validate`: dar suporte aos comentários no arquivo de parâmetro de implantação</span><span class="sxs-lookup"><span data-stu-id="10322-250">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="10322-251">`az deployment`: remover `is_preview` para o parâmetro `--handle-extended-json-format`</span><span class="sxs-lookup"><span data-stu-id="10322-251">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="10322-252">`az deployment group/mg/sub/tenant cancel`: dar suporte para cancelar a implantação do modelo do Resource Manager</span><span class="sxs-lookup"><span data-stu-id="10322-252">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="10322-253">`az deployment group/mg/sub/tenant validate`: melhorar a mensagem de erro quando a verificação de implantação falhar</span><span class="sxs-lookup"><span data-stu-id="10322-253">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="10322-254">`az deployment-scripts`: adicionar novos comandos para DeploymentScripts</span><span class="sxs-lookup"><span data-stu-id="10322-254">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="10322-255">`az resource tag`: adicionar o parâmetro `--is-incremental` para dar suporte à adição de marcas ao recurso de maneira incremental</span><span class="sxs-lookup"><span data-stu-id="10322-255">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="10322-256">ARO</span><span class="sxs-lookup"><span data-stu-id="10322-256">ARO</span></span>

* <span data-ttu-id="10322-257">`az aro`:  adicionar módulo de comando aro do Azure RedHat OpenShift V4</span><span class="sxs-lookup"><span data-stu-id="10322-257">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="10322-258">Lote</span><span class="sxs-lookup"><span data-stu-id="10322-258">Batch</span></span>

* <span data-ttu-id="10322-259">Atualizar a API do Lote</span><span class="sxs-lookup"><span data-stu-id="10322-259">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="10322-260">Computação</span><span class="sxs-lookup"><span data-stu-id="10322-260">Compute</span></span>

* <span data-ttu-id="10322-261">`az sig image-version create`: adicionar o tipo da conta de armazenamento Premium_LRS</span><span class="sxs-lookup"><span data-stu-id="10322-261">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="10322-262">`az vmss update`: corrigir problema de atualização de notificação de término</span><span class="sxs-lookup"><span data-stu-id="10322-262">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="10322-263">`az vm/vmss create`: adicionar suporte para a versão de imagem especializada</span><span class="sxs-lookup"><span data-stu-id="10322-263">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="10322-264">Versão da API SIG 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="10322-264">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="10322-265">`az sig image-version create`: Adicionar --target-region-encryption</span><span class="sxs-lookup"><span data-stu-id="10322-265">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="10322-266">Os testes de correção falham quando executados em série, pois o nome do keyvault está duplicado no cache global na memória</span><span class="sxs-lookup"><span data-stu-id="10322-266">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="10322-267">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="10322-267">CosmosDB</span></span>

* <span data-ttu-id="10322-268">Dar suporte à `az cosmosdb private-link-resource/private-endpoint-connection`</span><span class="sxs-lookup"><span data-stu-id="10322-268">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="10322-269">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="10322-269">IoT Central</span></span>

* <span data-ttu-id="10322-270">Preterir `az iotcentral`</span><span class="sxs-lookup"><span data-stu-id="10322-270">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="10322-271">Adicionar o módulo de comando `az iot central`</span><span class="sxs-lookup"><span data-stu-id="10322-271">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-272">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-272">Monitor</span></span>

* <span data-ttu-id="10322-273">Dar suporte ao cenário de link privado para monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-273">Support private link scenario for monitor</span></span>
* <span data-ttu-id="10322-274">Corrigir a maneira incorreta de simulação em test_monitor_general_operations.py</span><span class="sxs-lookup"><span data-stu-id="10322-274">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="10322-275">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-275">Network</span></span>

* <span data-ttu-id="10322-276">Preterir o sku para o comando de atualização de ip público</span><span class="sxs-lookup"><span data-stu-id="10322-276">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="10322-277">`az network private-endpoint`: dar suporte ao grupo de zona dns privada</span><span class="sxs-lookup"><span data-stu-id="10322-277">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="10322-278">Habilitar o recurso de contexto local para o parâmetro vnet/sub-rede</span><span class="sxs-lookup"><span data-stu-id="10322-278">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="10322-279">Corrigir o exemplo de uso incorreto em test_nw_flow_log_delete</span><span class="sxs-lookup"><span data-stu-id="10322-279">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="10322-280">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="10322-280">Packaging</span></span>

* <span data-ttu-id="10322-281">Descartar o suporte para o pacote Ubuntu/Disco</span><span class="sxs-lookup"><span data-stu-id="10322-281">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="10322-282">RBAC</span><span class="sxs-lookup"><span data-stu-id="10322-282">RBAC</span></span>

* <span data-ttu-id="10322-283">`az ad app create/update`: dar suporte a --optional-claims como um parâmetro</span><span class="sxs-lookup"><span data-stu-id="10322-283">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="10322-284">RDBMS</span><span class="sxs-lookup"><span data-stu-id="10322-284">RDBMS</span></span>

* <span data-ttu-id="10322-285">Adicionar comandos do administrador do Azure Active Directory para PostgreSQL e MySQL</span><span class="sxs-lookup"><span data-stu-id="10322-285">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="10322-286">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="10322-286">Service Fabric</span></span>

* <span data-ttu-id="10322-287">Correção nº 12891: `az sf application update --application-parameters` remove parâmetros antigos que não estão na solicitação</span><span class="sxs-lookup"><span data-stu-id="10322-287">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="10322-288">Correção nº 12470 az sf create cluster, corrigir bugs na atualização de durabilidade e confiabilidade e encontrar vmss corretamente por meio do código, dado um nome de tipo de nó</span><span class="sxs-lookup"><span data-stu-id="10322-288">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="10322-289">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-289">SQL</span></span>

* <span data-ttu-id="10322-290">Adicionar `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span><span class="sxs-lookup"><span data-stu-id="10322-290">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="10322-291">`az sql midb`: atualizar/mostrar política de retenção de longo prazo, mostrar/excluir backups de retenção de longo prazo, restaurar backup de retenção de longo prazo</span><span class="sxs-lookup"><span data-stu-id="10322-291">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="10322-292">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-292">Storage</span></span>

* <span data-ttu-id="10322-293">Atualizar azure-mgmt-storage para 9.0.0</span><span class="sxs-lookup"><span data-stu-id="10322-293">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="10322-294">`az storage logging off`: dar suporte à desativação do registro em log de uma conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-294">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="10322-295">`az storage account update`: habilitar rotação automática de chave para CMK</span><span class="sxs-lookup"><span data-stu-id="10322-295">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="10322-296">`az storage account encryption-scope create/update/list/show`: adicionar suporte para personalizar o escopo de criptografia</span><span class="sxs-lookup"><span data-stu-id="10322-296">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="10322-297">`az storage container create`: adicionar --default-encryption-scope e --deny-encryption-scope-override a fim de definir o escopo de criptografia para o nível de contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-297">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="10322-298">Pesquisa</span><span class="sxs-lookup"><span data-stu-id="10322-298">Survey</span></span>

* <span data-ttu-id="10322-299">Adicionar opção para desligar o link de pesquisa</span><span class="sxs-lookup"><span data-stu-id="10322-299">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="10322-300">1º de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="10322-300">April 01, 2020</span></span>

<span data-ttu-id="10322-301">Versão 2.3.1</span><span class="sxs-lookup"><span data-stu-id="10322-301">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="10322-302">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-302">ACR</span></span>

* <span data-ttu-id="10322-303">Corrigir a versão errada do azure-mgmt-containerregistry para Linux</span><span class="sxs-lookup"><span data-stu-id="10322-303">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="10322-304">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-304">Profile</span></span>

* <span data-ttu-id="10322-305">az login: Corrigir falha de logon com perfis de nuvem diferentes de `latest`</span><span class="sxs-lookup"><span data-stu-id="10322-305">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="10322-306">31 de março de 2020</span><span class="sxs-lookup"><span data-stu-id="10322-306">March 31, 2020</span></span>

<span data-ttu-id="10322-307">Versão 2.3.0</span><span class="sxs-lookup"><span data-stu-id="10322-307">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="10322-308">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-308">ACR</span></span>

* <span data-ttu-id="10322-309">'az acr task update': exceção de ponteiro nulo</span><span class="sxs-lookup"><span data-stu-id="10322-309">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="10322-310">`az acr import`: Modificar a mensagem de ajuda e de erro para esclarecer o uso de --source e --registry</span><span class="sxs-lookup"><span data-stu-id="10322-310">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="10322-311">Adicionar um validador para o argumento 'registry_name'</span><span class="sxs-lookup"><span data-stu-id="10322-311">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="10322-312">`az acr login`: remover o sinalizador de visualização em '--expose-token'</span><span class="sxs-lookup"><span data-stu-id="10322-312">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="10322-313">O parâmetro de branch 'az acr task create/update' de [ALTERAÇÃO SIGNIFICATIVA] foi removido</span><span class="sxs-lookup"><span data-stu-id="10322-313">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="10322-314">O cliente 'az acr task update' agora pode atualizar o contexto, o token do git e/ou os gatilhos individualmente</span><span class="sxs-lookup"><span data-stu-id="10322-314">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="10322-315">'az acr agentpool': novo recurso</span><span class="sxs-lookup"><span data-stu-id="10322-315">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="10322-316">AKS</span><span class="sxs-lookup"><span data-stu-id="10322-316">AKS</span></span>

* <span data-ttu-id="10322-317">Corrigir apiServerAccessProfile ao atualizar --api-server-authorized-ip-ranges</span><span class="sxs-lookup"><span data-stu-id="10322-317">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="10322-318">aks update: Substituir IPs de saída por valores de entrada ao atualizar</span><span class="sxs-lookup"><span data-stu-id="10322-318">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="10322-319">Não criar SPN para clusters MSI e dar suporte à anexação de ACR a clusters MSI</span><span class="sxs-lookup"><span data-stu-id="10322-319">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="10322-320">AMS</span><span class="sxs-lookup"><span data-stu-id="10322-320">AMS</span></span>

* <span data-ttu-id="10322-321">Correção nº. 12469: a adição da política de chave de conteúdo Fairplay falha devido a problemas com o parâmetro 'ask'</span><span class="sxs-lookup"><span data-stu-id="10322-321">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="10322-322">AppConfig</span><span class="sxs-lookup"><span data-stu-id="10322-322">AppConfig</span></span>

* <span data-ttu-id="10322-323">Adicionar --skip-keyvault a kv export</span><span class="sxs-lookup"><span data-stu-id="10322-323">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-324">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-324">AppService</span></span>

* <span data-ttu-id="10322-325">Correção nº 12509: remover a marca para az webapp up por padrão</span><span class="sxs-lookup"><span data-stu-id="10322-325">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="10322-326">az functionapp create: o menu de ajuda de --runtime-version foi atualizado e um aviso foi adicionado quando o usuário especifica --runtime-version para dotnet</span><span class="sxs-lookup"><span data-stu-id="10322-326">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="10322-327">az functionapp create: atualizado o modo como o javaVersion estava sendo definido para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="10322-327">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="10322-328">ARM</span><span class="sxs-lookup"><span data-stu-id="10322-328">ARM</span></span>

* <span data-ttu-id="10322-329">az deployment create/validate: usar --handle-extended-json-format por padrão</span><span class="sxs-lookup"><span data-stu-id="10322-329">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="10322-330">az lock create: adicionar exemplos de criação de subrecurso na documentação da ajuda</span><span class="sxs-lookup"><span data-stu-id="10322-330">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="10322-331">az deployment {group/mg/sub/tenant} list: dar suporte à filtragem de provisioningState</span><span class="sxs-lookup"><span data-stu-id="10322-331">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="10322-332">az deployment: corrigir o bug de análise para o comentário no último argumento</span><span class="sxs-lookup"><span data-stu-id="10322-332">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="10322-333">Backup</span><span class="sxs-lookup"><span data-stu-id="10322-333">Backup</span></span>

* <span data-ttu-id="10322-334">Adicionadas várias funcionalidades de restauração de arquivo</span><span class="sxs-lookup"><span data-stu-id="10322-334">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="10322-335">Adicionado suporte para backup somente de discos do SO</span><span class="sxs-lookup"><span data-stu-id="10322-335">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="10322-336">Adicionado o parâmetro restore-as-unmanaged-disk para especificar a restauração não gerenciada</span><span class="sxs-lookup"><span data-stu-id="10322-336">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="10322-337">Computação</span><span class="sxs-lookup"><span data-stu-id="10322-337">Compute</span></span>

* <span data-ttu-id="10322-338">az vm create: adicionar opção NONE de --nsg-rule</span><span class="sxs-lookup"><span data-stu-id="10322-338">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="10322-339">az vmss create/update: remover a marca de visualização de reparos automáticos do vmss</span><span class="sxs-lookup"><span data-stu-id="10322-339">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="10322-340">az vm update: dar suporte a --workspace</span><span class="sxs-lookup"><span data-stu-id="10322-340">az vm update: Support --workspace</span></span>
* <span data-ttu-id="10322-341">Corrigir um bug no código de inicialização de VirtualMachineScaleSetExtension</span><span class="sxs-lookup"><span data-stu-id="10322-341">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="10322-342">Atualizar a versão do VMAccessAgent para 2.4</span><span class="sxs-lookup"><span data-stu-id="10322-342">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="10322-343">az vmss set-orchestration-service-state: dar suporte para o estado de definição do serviço de orquestração do vmss</span><span class="sxs-lookup"><span data-stu-id="10322-343">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="10322-344">Atualizar a API do disco para a versão 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="10322-344">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="10322-345">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span><span class="sxs-lookup"><span data-stu-id="10322-345">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="10322-346">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="10322-346">Cosmos DB</span></span>

* <span data-ttu-id="10322-347">Corrigir a ausência da opção --type para redirecionamentos de preterimento</span><span class="sxs-lookup"><span data-stu-id="10322-347">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="10322-348">Docker</span><span class="sxs-lookup"><span data-stu-id="10322-348">Docker</span></span>

* <span data-ttu-id="10322-349">Atualizar para Alpine 3.11 e Python 3.6.10</span><span class="sxs-lookup"><span data-stu-id="10322-349">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="10322-350">Extensão</span><span class="sxs-lookup"><span data-stu-id="10322-350">Extension</span></span>

* <span data-ttu-id="10322-351">Permitir carregar extensões no caminho do sistema por meio de pacotes</span><span class="sxs-lookup"><span data-stu-id="10322-351">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="10322-352">HDInsight</span><span class="sxs-lookup"><span data-stu-id="10322-352">HDInsight</span></span>

* <span data-ttu-id="10322-353">(az hdinsight create:) dar suporte à especificação da versão de TLS mínima pelos clientes usando o parâmetro `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="10322-353">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="10322-354">O valor permitido é 1.0,1.1,1.2</span><span class="sxs-lookup"><span data-stu-id="10322-354">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="10322-355">IoT</span><span class="sxs-lookup"><span data-stu-id="10322-355">IoT</span></span>

* <span data-ttu-id="10322-356">Adicionar codeowner</span><span class="sxs-lookup"><span data-stu-id="10322-356">Add codeowner</span></span>
* <span data-ttu-id="10322-357">az iot hub create : alterar o SKU padrão de F1 para S1</span><span class="sxs-lookup"><span data-stu-id="10322-357">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="10322-358">iot hub: dar suporte a IotHub no perfil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="10322-358">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="10322-359">IoT Central</span><span class="sxs-lookup"><span data-stu-id="10322-359">IoTCentral</span></span>

* <span data-ttu-id="10322-360">Atualizar detalhes do erro, atualizar modelo de aplicativo padrão e a mensagem de aviso</span><span class="sxs-lookup"><span data-stu-id="10322-360">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="10322-361">KeyVault</span><span class="sxs-lookup"><span data-stu-id="10322-361">KeyVault</span></span>

* <span data-ttu-id="10322-362">Suporte para backup/restauração de certificado</span><span class="sxs-lookup"><span data-stu-id="10322-362">Support certificate backup/restore</span></span>
* <span data-ttu-id="10322-363">keyvault create/update: Suporte a --retention-days</span><span class="sxs-lookup"><span data-stu-id="10322-363">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="10322-364">Não exibir mais chaves/segredos gerenciados durante a listagem</span><span class="sxs-lookup"><span data-stu-id="10322-364">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="10322-365">az keyvault create: suporte a `--network-acls`, `--network-acls-ips` e `--network-acls-vnets` para especificar regras de rede ao criar o cofre</span><span class="sxs-lookup"><span data-stu-id="10322-365">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="10322-366">Bloqueio</span><span class="sxs-lookup"><span data-stu-id="10322-366">Lock</span></span>

* <span data-ttu-id="10322-367">az lock delete fix bug: az lock delete não funciona no Microsoft.DocumentDB</span><span class="sxs-lookup"><span data-stu-id="10322-367">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-368">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-368">Monitor</span></span>

* <span data-ttu-id="10322-369">az monitor clone: suporte a regras de métrica de clone de um recurso para outro</span><span class="sxs-lookup"><span data-stu-id="10322-369">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="10322-370">Corrigir IcM179210086: não é possível criar um alerta de métrica personalizado para a métrica de Application Insights</span><span class="sxs-lookup"><span data-stu-id="10322-370">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="10322-371">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="10322-371">NetAppFiles</span></span>

* <span data-ttu-id="10322-372">az volume create: permitir volumes de proteção de dados adicionando operações de replicação: approve, suspend, resume, status, remove</span><span class="sxs-lookup"><span data-stu-id="10322-372">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="10322-373">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-373">Network</span></span>

* <span data-ttu-id="10322-374">az network application-gateway waf-policy managed-rule rule-set add: dar suporte a Microsoft_BotManagerRuleSet</span><span class="sxs-lookup"><span data-stu-id="10322-374">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="10322-375">network watcher flow-log show: corrigir informações erradas em preterimento</span><span class="sxs-lookup"><span data-stu-id="10322-375">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="10322-376">dar suporte a nomes de host no ouvinte do gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="10322-376">support host names in application gateway listener</span></span>
* <span data-ttu-id="10322-377">az network nat gateway: dar suporte para criar um recurso vazio sem IP público nem prefixo de IP público</span><span class="sxs-lookup"><span data-stu-id="10322-377">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="10322-378">Dar suporte à geração de gateway de VPN</span><span class="sxs-lookup"><span data-stu-id="10322-378">Support vpn gateway generation</span></span>
* <span data-ttu-id="10322-379">Dar suporte a `--if-none-match` em `az network dns record-set {} add-record`</span><span class="sxs-lookup"><span data-stu-id="10322-379">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="10322-380">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="10322-380">Packaging</span></span>

* <span data-ttu-id="10322-381">Remover o suporte ao Python 3.5</span><span class="sxs-lookup"><span data-stu-id="10322-381">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="10322-382">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-382">Profile</span></span>

* <span data-ttu-id="10322-383">az login: Mostrar aviso para erro de MFA</span><span class="sxs-lookup"><span data-stu-id="10322-383">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="10322-384">RDBMS</span><span class="sxs-lookup"><span data-stu-id="10322-384">RDBMS</span></span>

* <span data-ttu-id="10322-385">Adicionar comandos de gerenciamento de chaves de criptografia de dados do servidor para PostgreSQL e MySQL</span><span class="sxs-lookup"><span data-stu-id="10322-385">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="10322-386">10 de março de 2020</span><span class="sxs-lookup"><span data-stu-id="10322-386">March 10, 2020</span></span>

<span data-ttu-id="10322-387">Versão 2.2.0</span><span class="sxs-lookup"><span data-stu-id="10322-387">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="10322-388">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-388">ACR</span></span>

* <span data-ttu-id="10322-389">Correção: `az acr login` gerava erro incorretamente</span><span class="sxs-lookup"><span data-stu-id="10322-389">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="10322-390">Adicionou o novo comando `az acr helm install-cli`</span><span class="sxs-lookup"><span data-stu-id="10322-390">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="10322-391">Adicionou link privado e suporte do CMK</span><span class="sxs-lookup"><span data-stu-id="10322-391">Add private link and CMK support</span></span>
* <span data-ttu-id="10322-392">Adicionou o comando 'private-link-resource list'</span><span class="sxs-lookup"><span data-stu-id="10322-392">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="10322-393">AKS</span><span class="sxs-lookup"><span data-stu-id="10322-393">AKS</span></span>

* <span data-ttu-id="10322-394">correção da busca do AKS no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="10322-394">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="10322-395">az aks: correção dos erros de complemento de monitoramento e de agentpool NoneType</span><span class="sxs-lookup"><span data-stu-id="10322-395">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="10322-396">Adicionou --nodepool-tags ao pool de nós ao criar o cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="10322-396">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="10322-397">Adicionou --tags ao adicionar ou atualizar um pool de nós para o cluster</span><span class="sxs-lookup"><span data-stu-id="10322-397">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="10322-398">AKS create: adicionou `--enable-private-cluster`</span><span class="sxs-lookup"><span data-stu-id="10322-398">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="10322-399">Adicionou --nodepool-labels ao criar o cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="10322-399">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="10322-400">Adicionou --labels ao adicionar um novo pool de nós ao cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="10322-400">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="10322-401">Adicionou / ausente na URL do painel</span><span class="sxs-lookup"><span data-stu-id="10322-401">add missing / in the dashboard url</span></span>
* <span data-ttu-id="10322-402">Suporte para criar clusters do AKS habilitando identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="10322-402">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="10322-403">az aks: validou o plug-in de rede como "Azure" ou "Kubenet"</span><span class="sxs-lookup"><span data-stu-id="10322-403">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="10322-404">az aks: adicionou suporte da chave da sessão do AAD</span><span class="sxs-lookup"><span data-stu-id="10322-404">az aks: Add aad session key support</span></span>
* <span data-ttu-id="10322-405">[ALTERAÇÃO SIGNIFICATIVA] AZ AKS: suporte para alterações de MSI para GF e BF para omsagent (Monitoramento de contêiner) (#1)</span><span class="sxs-lookup"><span data-stu-id="10322-405">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="10322-406">az aks use-dev-spaces: adicionou a opção de tipo de ponto de extremidade ao comando use-dev-spaces para personalizar o ponto de extremidade criado em um controlador Azure Dev Spaces</span><span class="sxs-lookup"><span data-stu-id="10322-406">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="10322-407">AppConfig</span><span class="sxs-lookup"><span data-stu-id="10322-407">AppConfig</span></span>

* <span data-ttu-id="10322-408">Desbloqueou usando "KV set" para adicionar o recurso e a referência do keyvault...</span><span class="sxs-lookup"><span data-stu-id="10322-408">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-409">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-409">AppService</span></span>

* <span data-ttu-id="10322-410">az webapp create: correção do problema ao executar o comando com --runtime</span><span class="sxs-lookup"><span data-stu-id="10322-410">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="10322-411">az functionapp deployment source config-zip: adicionou uma mensagem de erro se o grupo de recursos ou o nome da função forem inválidos/não existirem</span><span class="sxs-lookup"><span data-stu-id="10322-411">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="10322-412">functionapp create: correção da mensagem de aviso que aparece com `functionapp create` hoje, que cita um sinalizador de `--functions_version`, mas usa erroneamente `_` em vez de `-` no nome do sinalizador</span><span class="sxs-lookup"><span data-stu-id="10322-412">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="10322-413">az functionapp create: atualizou o modo como linuxFxVersion e o nome da imagem de contêiner eram definidos para aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="10322-413">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="10322-414">az functionapp deployment source config-zip: correção de um problema causado pelas configurações do aplicativo que alterava a condição de corrida durante a implantação do zip, provocando erros 5xx durante a implantação</span><span class="sxs-lookup"><span data-stu-id="10322-414">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="10322-415">Correção #5720946: AZ WebApp backup falha ao definir o nome</span><span class="sxs-lookup"><span data-stu-id="10322-415">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="10322-416">ARM</span><span class="sxs-lookup"><span data-stu-id="10322-416">ARM</span></span>

* <span data-ttu-id="10322-417">az resource: aprimorou os exemplos do módulo de recurso</span><span class="sxs-lookup"><span data-stu-id="10322-417">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="10322-418">az policy assignment list: suporte à listagem de atribuições de política no escopo do Grupo de Gerenciamento</span><span class="sxs-lookup"><span data-stu-id="10322-418">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="10322-419">Adicionou `az deployment group` e `az deployment operation group` para a implantação de modelos nos grupos de recursos.</span><span class="sxs-lookup"><span data-stu-id="10322-419">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="10322-420">Esta é uma duplicata de `az group deployment` e `az group deployment operation`</span><span class="sxs-lookup"><span data-stu-id="10322-420">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="10322-421">Adicionou `az deployment sub` e `az deployment operation sub` para a implantação de modelos no escopo da assinatura.</span><span class="sxs-lookup"><span data-stu-id="10322-421">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="10322-422">Esta é uma duplicata de `az deployment` e `az deployment operation`</span><span class="sxs-lookup"><span data-stu-id="10322-422">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="10322-423">Adicionou `az deployment mg` e `az deployment operation mg` para implantação de modelos nos grupos de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="10322-423">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="10322-424">Adicionou `az deployment tenant` e `az deployment operation tenant` para implantação de modelos no escopo do locatário.</span><span class="sxs-lookup"><span data-stu-id="10322-424">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="10322-425">az policy assignment create: adicionou descrição ao parâmetro `--location`</span><span class="sxs-lookup"><span data-stu-id="10322-425">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="10322-426">az group deployment create: adicionou o parâmetro `--aux-tenants` para dar suporte a locatários cruzados</span><span class="sxs-lookup"><span data-stu-id="10322-426">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="10322-427">CDN</span><span class="sxs-lookup"><span data-stu-id="10322-427">CDN</span></span>

* <span data-ttu-id="10322-428">Adicionou comandos do WAF da CDN</span><span class="sxs-lookup"><span data-stu-id="10322-428">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="10322-429">Computação</span><span class="sxs-lookup"><span data-stu-id="10322-429">Compute</span></span>

* <span data-ttu-id="10322-430">az sig image-version: adicionar --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="10322-430">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="10322-431">AZ PPG show: adicionou --outlocation-status para habilitar a busca do status de colocalização de todos os recursos no grupo de posicionamento por proximidade</span><span class="sxs-lookup"><span data-stu-id="10322-431">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="10322-432">az vmss create/update: suporte a reparos automáticos</span><span class="sxs-lookup"><span data-stu-id="10322-432">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="10322-433">[ALTERAÇÃO SIGNIFICATIVA] modelo de imagem AZ: renomear modelo para builder</span><span class="sxs-lookup"><span data-stu-id="10322-433">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="10322-434">AZ Image Builder Create: adicionou --Image-template</span><span class="sxs-lookup"><span data-stu-id="10322-434">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="10322-435">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="10322-435">Cosmos DB</span></span>

* <span data-ttu-id="10322-436">Adicionou procedimento armazenado do SQL, UDF e disparar cmdlets</span><span class="sxs-lookup"><span data-stu-id="10322-436">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="10322-437">az cosmosdb create: adicionou --key-uri para dar suporte à adição de informações de criptografia do cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="10322-437">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="10322-438">KeyVault</span><span class="sxs-lookup"><span data-stu-id="10322-438">KeyVault</span></span>

* <span data-ttu-id="10322-439">keyvault create: habilitou a exclusão reversível por padrão</span><span class="sxs-lookup"><span data-stu-id="10322-439">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-440">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-440">Monitor</span></span>

* <span data-ttu-id="10322-441">az monitor metrics alert create: suporte a `~` em `--condition`</span><span class="sxs-lookup"><span data-stu-id="10322-441">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="10322-442">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-442">Network</span></span>

* <span data-ttu-id="10322-443">az network application-gateway rewrite-rule create: suporte à configuração de URL</span><span class="sxs-lookup"><span data-stu-id="10322-443">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="10322-444">az network dns zone import: --zone-name não diferenciará maiúsculas de minúsculas no futuro</span><span class="sxs-lookup"><span data-stu-id="10322-444">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="10322-445">az network private-endpoint/private-link-service: removeu rótulo de visualização</span><span class="sxs-lookup"><span data-stu-id="10322-445">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="10322-446">az network bastion: suporte a bastions</span><span class="sxs-lookup"><span data-stu-id="10322-446">az network bastion: support bastion</span></span>
* <span data-ttu-id="10322-447">az network vnet list-available-ips: dar suporte à lista de IPs disponíveis em uma vnet</span><span class="sxs-lookup"><span data-stu-id="10322-447">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="10322-448">az network watcher flow-log create/list/delete/update: adicionou novos comandos para gerenciar o log de fluxo do Inspetor e expor o --local para identificá-lo explicitamente</span><span class="sxs-lookup"><span data-stu-id="10322-448">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="10322-449">az network watcher flow-log configure: preterido</span><span class="sxs-lookup"><span data-stu-id="10322-449">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="10322-450">az network watcher flow-log show: dá suporte a --location e --name para obter o resultado formatado por ARM, saída formatada antiga preterida</span><span class="sxs-lookup"><span data-stu-id="10322-450">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="10322-451">Política</span><span class="sxs-lookup"><span data-stu-id="10322-451">Policy</span></span>

* <span data-ttu-id="10322-452">az policy assignment create: correção do bug que gerou automaticamente o nome da atribuição de política, que excede o limite</span><span class="sxs-lookup"><span data-stu-id="10322-452">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="10322-453">RBAC</span><span class="sxs-lookup"><span data-stu-id="10322-453">RBAC</span></span>

* <span data-ttu-id="10322-454">az ad group show: correção do valor --group, que é tratado como um problema de regex</span><span class="sxs-lookup"><span data-stu-id="10322-454">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="10322-455">RDBMS</span><span class="sxs-lookup"><span data-stu-id="10322-455">RDBMS</span></span>

* <span data-ttu-id="10322-456">Trocou a versão do zure-mgmt-rdbms SDK para 2.0.0</span><span class="sxs-lookup"><span data-stu-id="10322-456">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="10322-457">az postgres private-endpoint-connection: gerenciou conexões de ponto de extremidade privado do Postgres</span><span class="sxs-lookup"><span data-stu-id="10322-457">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="10322-458">az postgres private-link-resource: gerenciou recursos de link privado do Postgres</span><span class="sxs-lookup"><span data-stu-id="10322-458">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="10322-459">az mysql private-endpoint-connection: gerenciar conexões de ponto de extremidade privado do MySQL</span><span class="sxs-lookup"><span data-stu-id="10322-459">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="10322-460">az mysql private-link-resource: gerenciou recursos de link privado do MySQL</span><span class="sxs-lookup"><span data-stu-id="10322-460">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="10322-461">az mariadb private-endpoint-connection: gerenciou conexões de ponto de extremidade privado do MariaDB</span><span class="sxs-lookup"><span data-stu-id="10322-461">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="10322-462">az mariadb private-link-resource: gerenciou recursos de link privado do MariaDB</span><span class="sxs-lookup"><span data-stu-id="10322-462">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="10322-463">Atualizando testes de ponto de extremidade privado do RDBMS</span><span class="sxs-lookup"><span data-stu-id="10322-463">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="10322-464">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-464">SQL</span></span>

* <span data-ttu-id="10322-465">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span><span class="sxs-lookup"><span data-stu-id="10322-465">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="10322-466">(sql server create:) adicionou o sinalizador ' habilitar '/' desabilitar ' opcional public-network-access ao SQL Server create</span><span class="sxs-lookup"><span data-stu-id="10322-466">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="10322-467">(sql server update:) fez algumas alterações voltadas para o cliente</span><span class="sxs-lookup"><span data-stu-id="10322-467">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="10322-468">adicionou a propriedade minimal_tls_version para o banco de BD de MI e SQL</span><span class="sxs-lookup"><span data-stu-id="10322-468">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="10322-469">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-469">Storage</span></span>

* <span data-ttu-id="10322-470">az storage blob delete-batch: sinalizador `--dryrun` de comportamento inadequado</span><span class="sxs-lookup"><span data-stu-id="10322-470">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="10322-471">az storage account network-rule add (correção de bug): a operação de adição deve ser idempotente</span><span class="sxs-lookup"><span data-stu-id="10322-471">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="10322-472">az storage account create/update: Adicionou suporte de preferência de roteamento</span><span class="sxs-lookup"><span data-stu-id="10322-472">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="10322-473">Atualizou a versão do azure-mgmt-storage para 8.0.0</span><span class="sxs-lookup"><span data-stu-id="10322-473">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="10322-474">az storage container immutability create: adicionou o parâmetro --allow-protected-append-write</span><span class="sxs-lookup"><span data-stu-id="10322-474">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="10322-475">az storage account private-link-resource list: Adicionou suporte para lista de recursos de link privado para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-475">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="10322-476">az storage account private-endpoint-connection approve/reject/show/delete: Suporte para gerenciar conexões de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="10322-476">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="10322-477">az storage account blob-service-properties update: adicionou --enable-restore-policy e --restore-days</span><span class="sxs-lookup"><span data-stu-id="10322-477">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="10322-478">az storage blob restore: adicionou suporte para restaurar intervalos de blob</span><span class="sxs-lookup"><span data-stu-id="10322-478">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="10322-479">18 de fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="10322-479">February 18, 2020</span></span>

<span data-ttu-id="10322-480">Versão 2.1.0</span><span class="sxs-lookup"><span data-stu-id="10322-480">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="10322-481">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-481">ACR</span></span>

* <span data-ttu-id="10322-482">Adicionar um novo argumento `--expose-token` a `az acr login`</span><span class="sxs-lookup"><span data-stu-id="10322-482">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="10322-483">Corrigir a saída incorreta de `az acr task identity show -n Name -r Registry -o table`</span><span class="sxs-lookup"><span data-stu-id="10322-483">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="10322-484">az acr login: Gerar CLIError se erros forem retornados pelo comando docker</span><span class="sxs-lookup"><span data-stu-id="10322-484">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="10322-485">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-485">ACS</span></span>

* <span data-ttu-id="10322-486">aks create/update: adicionar a validação `--vnet-subnet-id`</span><span class="sxs-lookup"><span data-stu-id="10322-486">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="10322-487">Aladdin</span><span class="sxs-lookup"><span data-stu-id="10322-487">Aladdin</span></span>

* <span data-ttu-id="10322-488">Analisar os exemplos gerados no _help.py do comando</span><span class="sxs-lookup"><span data-stu-id="10322-488">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="10322-489">AMS</span><span class="sxs-lookup"><span data-stu-id="10322-489">AMS</span></span>

* <span data-ttu-id="10322-490">az ams já está em GA</span><span class="sxs-lookup"><span data-stu-id="10322-490">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="10322-491">AppConfig</span><span class="sxs-lookup"><span data-stu-id="10322-491">AppConfig</span></span>

* <span data-ttu-id="10322-492">Revisar a mensagem de ajuda para excluir o filtro de chave/rótulo não compatível</span><span class="sxs-lookup"><span data-stu-id="10322-492">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="10322-493">Remover a marca de versão prévia da maioria dos comandos que excluem a identidade gerenciada e têm sinalizadores</span><span class="sxs-lookup"><span data-stu-id="10322-493">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="10322-494">Adicionar a chave gerenciada do cliente ao atualizar os repositórios</span><span class="sxs-lookup"><span data-stu-id="10322-494">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-495">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-495">AppService</span></span>

* <span data-ttu-id="10322-496">az webapp list-runtimes: Corrigir o bug de list-runtimes</span><span class="sxs-lookup"><span data-stu-id="10322-496">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="10322-497">Adicionar az webapp|functionapp config ssl create</span><span class="sxs-lookup"><span data-stu-id="10322-497">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="10322-498">Adicionar compatibilidade com aplicativos de funções v3 e nó 12</span><span class="sxs-lookup"><span data-stu-id="10322-498">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="10322-499">ARM</span><span class="sxs-lookup"><span data-stu-id="10322-499">ARM</span></span>

* <span data-ttu-id="10322-500">az policy assignment create: Corrigir a mensagem de erro quando o parâmetro `--policy` for inválido</span><span class="sxs-lookup"><span data-stu-id="10322-500">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="10322-501">az group deployment create: Corrigir o erro "stat: o caminho é muito longo para o Windows" ao usar o arquivo grande parameters.json</span><span class="sxs-lookup"><span data-stu-id="10322-501">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="10322-502">Backup</span><span class="sxs-lookup"><span data-stu-id="10322-502">Backup</span></span>

* <span data-ttu-id="10322-503">Corrigir o fluxo de recuperação de nível de item no OLR</span><span class="sxs-lookup"><span data-stu-id="10322-503">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="10322-504">Adicionar compatibilidade com restauração como arquivo aos bancos de dados SQL e SAP</span><span class="sxs-lookup"><span data-stu-id="10322-504">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="10322-505">Computação</span><span class="sxs-lookup"><span data-stu-id="10322-505">Compute</span></span>

* <span data-ttu-id="10322-506">vm/vmss/availability-set update: adicionar --ppg para permitir a atualização de ProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="10322-506">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="10322-507">vmss create: adicionar --data-disk-iops e --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="10322-507">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="10322-508">az vm host: remover a marca de versão prévia de `vm host` e `vm host group`</span><span class="sxs-lookup"><span data-stu-id="10322-508">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="10322-509">[ALTERAÇÃO SIGNIFICATIVA] Correção nº 10.728: `az vm create`: criar uma sub-rede automaticamente quando a vnet for especificada e não houver uma sub-rede</span><span class="sxs-lookup"><span data-stu-id="10322-509">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="10322-510">Aumentar a robustez da lista de imagens de VM</span><span class="sxs-lookup"><span data-stu-id="10322-510">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="10322-511">Eventhub</span><span class="sxs-lookup"><span data-stu-id="10322-511">Eventhub</span></span>

* <span data-ttu-id="10322-512">Compatibilidade com o Azure Stack para o perfil 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="10322-512">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="10322-513">KeyVault</span><span class="sxs-lookup"><span data-stu-id="10322-513">KeyVault</span></span>

* <span data-ttu-id="10322-514">az keyvault key create: adicionar um novo valor `import` ao parâmetro `--ops`</span><span class="sxs-lookup"><span data-stu-id="10322-514">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="10322-515">az keyvault key list-versions: compatibilidade com o parâmetro `--id` para especificar chaves</span><span class="sxs-lookup"><span data-stu-id="10322-515">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="10322-516">Compatibilidade com conexões de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="10322-516">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="10322-517">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-517">Network</span></span>

* <span data-ttu-id="10322-518">Avançar para azure-mgmt-network 9.0.0</span><span class="sxs-lookup"><span data-stu-id="10322-518">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="10322-519">az network private-link-service update/create: dá suporte a --enable-proxy-protocol</span><span class="sxs-lookup"><span data-stu-id="10322-519">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="10322-520">Adicionar o recurso de Monitor de conexão V2</span><span class="sxs-lookup"><span data-stu-id="10322-520">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="10322-521">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="10322-521">Packaging</span></span>

* <span data-ttu-id="10322-522">[ALTERAÇÃO SIGNIFICATIVA] Fim da compatibilidade com o Python 2.7</span><span class="sxs-lookup"><span data-stu-id="10322-522">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="10322-523">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-523">Profile</span></span>

* <span data-ttu-id="10322-524">Visualização: Adicionar novos atributos `homeTenantId` e `managedByTenants` às contas de assinatura.</span><span class="sxs-lookup"><span data-stu-id="10322-524">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="10322-525">Executar `az login` novamente para as alterações entrarem em vigor</span><span class="sxs-lookup"><span data-stu-id="10322-525">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="10322-526">az login: Mostrar um aviso quando uma assinatura estiver listada de mais de um locatário e definir a primeira como padrão.</span><span class="sxs-lookup"><span data-stu-id="10322-526">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="10322-527">Para selecionar um locatário específico ao acessar essa assinatura, inclua `--tenant` em `az login`</span><span class="sxs-lookup"><span data-stu-id="10322-527">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="10322-528">Função</span><span class="sxs-lookup"><span data-stu-id="10322-528">Role</span></span>

* <span data-ttu-id="10322-529">az role assignment create: Corrigir o erro em que atribuir uma função a uma entidade de serviço pelo nome de exibição gera um HTTP 400</span><span class="sxs-lookup"><span data-stu-id="10322-529">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="10322-530">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-530">SQL</span></span>

* <span data-ttu-id="10322-531">Atualizar o cmdlet da Instância Gerenciada do SQL `az sql mi update` com dois novos parâmetros: nível e família</span><span class="sxs-lookup"><span data-stu-id="10322-531">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="10322-532">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-532">Storage</span></span>

* <span data-ttu-id="10322-533">[ALTERAÇÃO DA FALHA] `az storage account create`: Alterar o tipo de conta de armazenamento padrão para StorageV2</span><span class="sxs-lookup"><span data-stu-id="10322-533">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="10322-534">4 de fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="10322-534">February 04, 2020</span></span>

<span data-ttu-id="10322-535">Versão 2.0.81</span><span class="sxs-lookup"><span data-stu-id="10322-535">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="10322-536">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-536">ACS</span></span>

* <span data-ttu-id="10322-537">Adicionar suporte para definir portas alocadas de saída e tempos limite ociosos no balanceador de carga standard</span><span class="sxs-lookup"><span data-stu-id="10322-537">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="10322-538">Atualizar para a versão da API 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="10322-538">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="10322-539">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-539">ACR</span></span>

* <span data-ttu-id="10322-540">A [ALTERAÇÃO DA FALHA] `az acr delete` será exibida</span><span class="sxs-lookup"><span data-stu-id="10322-540">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="10322-541">A [ALTERAÇÃO SIGNIFICATIVA] 'az acr task delete’ será exibida</span><span class="sxs-lookup"><span data-stu-id="10322-541">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="10322-542">Adicionar um novo grupo de comandos ‘az acr taskrun show/list/delete’ para o gerenciamento de taskrun</span><span class="sxs-lookup"><span data-stu-id="10322-542">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="10322-543">AKS</span><span class="sxs-lookup"><span data-stu-id="10322-543">AKS</span></span>

* <span data-ttu-id="10322-544">Cada cluster obtém uma entidade de serviço separada para aprimorar o isolamento</span><span class="sxs-lookup"><span data-stu-id="10322-544">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="10322-545">AppConfig</span><span class="sxs-lookup"><span data-stu-id="10322-545">AppConfig</span></span>

* <span data-ttu-id="10322-546">Dar suporte à importação/exportação de referências keyvault de/a appservice</span><span class="sxs-lookup"><span data-stu-id="10322-546">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="10322-547">Dar suporte à importação/exportação de todos os rótulos de appconfig para appconfig</span><span class="sxs-lookup"><span data-stu-id="10322-547">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="10322-548">Validar nomes de chave e recursos antes de configurar e importar</span><span class="sxs-lookup"><span data-stu-id="10322-548">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="10322-549">Exponha a modificação do sku para o repositório de configurações.</span><span class="sxs-lookup"><span data-stu-id="10322-549">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="10322-550">Adicione o grupo de comandos à identidade gerenciada.</span><span class="sxs-lookup"><span data-stu-id="10322-550">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-551">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-551">AppService</span></span>

* <span data-ttu-id="10322-552">Azure Stack: comandos de superfície no perfil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="10322-552">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="10322-553">functionapp: adicionar a capacidade de criar aplicativos de funções Java no Linux</span><span class="sxs-lookup"><span data-stu-id="10322-553">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="10322-554">ARM</span><span class="sxs-lookup"><span data-stu-id="10322-554">ARM</span></span>

* <span data-ttu-id="10322-555">Correção de problema nº 10246: `az resource tag` falha quando o parâmetro `--ids` passado é a ID do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="10322-555">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="10322-556">Correção de problema nº 11658: o comando `az group export` não é compatível com os parâmetros `--query` e `--output`</span><span class="sxs-lookup"><span data-stu-id="10322-556">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="10322-557">Correção de problema nº 10279: O código de saída `az group deployment validate` é 0 quando a verificação falha</span><span class="sxs-lookup"><span data-stu-id="10322-557">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="10322-558">Correção de problema nº 9916: aprimorar a mensagem de erro do conflito entre a marca e outras condições de filtro para o comando `az resource list`</span><span class="sxs-lookup"><span data-stu-id="10322-558">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="10322-559">Adicionar novo parâmetro `--managed-by` para dar suporte à adição de informações managedBy para o comando `az group create`</span><span class="sxs-lookup"><span data-stu-id="10322-559">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="10322-560">Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="10322-560">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="10322-561">Adicionar o subgrupo `monitor` para gerenciar o monitoramento do Log Analytics no cluster do Red Hat OpensShift no Azure</span><span class="sxs-lookup"><span data-stu-id="10322-561">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="10322-562">BotService</span><span class="sxs-lookup"><span data-stu-id="10322-562">BotService</span></span>

* <span data-ttu-id="10322-563">Correção de problema nº 11697: `az bot create` não é idempotente</span><span class="sxs-lookup"><span data-stu-id="10322-563">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="10322-564">Alterar testes de correção de nomes para serem executados somente em modo Ao vivo</span><span class="sxs-lookup"><span data-stu-id="10322-564">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="10322-565">CDN</span><span class="sxs-lookup"><span data-stu-id="10322-565">CDN</span></span>

* <span data-ttu-id="10322-566">Adicionar suporte ao recurso rulesEngine</span><span class="sxs-lookup"><span data-stu-id="10322-566">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="10322-567">Adicionar o novo grupo de comandos ‘cdn endpoint rule’ para gerenciar regras</span><span class="sxs-lookup"><span data-stu-id="10322-567">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="10322-568">Atualizar a versão azure-mgmt-cdn para a 4.0.0 para usar a versão da API 2019-04-15</span><span class="sxs-lookup"><span data-stu-id="10322-568">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="10322-569">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="10322-569">Deployment Manager</span></span>

* <span data-ttu-id="10322-570">Adicione a operação de lista para todos os recursos.</span><span class="sxs-lookup"><span data-stu-id="10322-570">Add list operation for all resources.</span></span>
* <span data-ttu-id="10322-571">Aprimore o recurso de etapa do novo tipo de etapa.</span><span class="sxs-lookup"><span data-stu-id="10322-571">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="10322-572">Atualize o pacote azure-mgmt-deploymentmanager para usar a versão 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="10322-572">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="10322-573">IoT</span><span class="sxs-lookup"><span data-stu-id="10322-573">IoT</span></span>

* <span data-ttu-id="10322-574">Substitua os comandos ‘IoT hub Job’.</span><span class="sxs-lookup"><span data-stu-id="10322-574">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="10322-575">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="10322-575">IoT Central</span></span>

* <span data-ttu-id="10322-576">Dê suporte à atualização/criação de aplicativos com o novo nome do SKU ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="10322-576">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="10322-577">Key Vault</span><span class="sxs-lookup"><span data-stu-id="10322-577">Key Vault</span></span>

* <span data-ttu-id="10322-578">Adicione um novo comando `az keyvault key download` para baixar chaves.</span><span class="sxs-lookup"><span data-stu-id="10322-578">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="10322-579">Diversos</span><span class="sxs-lookup"><span data-stu-id="10322-579">Misc</span></span>

* <span data-ttu-id="10322-580">Correção nº 6371: dar suporte à conclusão da variável de nome de arquivo e de ambiente em Bash</span><span class="sxs-lookup"><span data-stu-id="10322-580">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="10322-581">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-581">Network</span></span>

* <span data-ttu-id="10322-582">Correção nº 2092: az network dns record-set add/remove: adicione um aviso quando record-set não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="10322-582">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="10322-583">No futuro, haverá suporte para um argumento extra para confirmar essa criação automática.</span><span class="sxs-lookup"><span data-stu-id="10322-583">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="10322-584">Política</span><span class="sxs-lookup"><span data-stu-id="10322-584">Policy</span></span>

* <span data-ttu-id="10322-585">Adicionar o novo comando `az policy metadata` para recuperar recursos avançados de metadados de política</span><span class="sxs-lookup"><span data-stu-id="10322-585">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="10322-586">`az policy remediation create`: Especifique se a conformidade deve ser reavaliada antes da correção com o parâmetro `--resource-discovery-mode`</span><span class="sxs-lookup"><span data-stu-id="10322-586">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="10322-587">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-587">Profile</span></span>

* <span data-ttu-id="10322-588">`az account get-access-token`: Adicionar parâmetro `--tenant` para adquirir o token do locatário diretamente, sem a necessidade de especificar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="10322-588">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="10322-589">RBAC</span><span class="sxs-lookup"><span data-stu-id="10322-589">RBAC</span></span>

* <span data-ttu-id="10322-590">[ALTERAÇÃO SIGNIFICATIVA] Correção nº 11883: `az role assignment create`: o escopo vazio exibirá erro</span><span class="sxs-lookup"><span data-stu-id="10322-590">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="10322-591">Segurança</span><span class="sxs-lookup"><span data-stu-id="10322-591">Security</span></span>

* <span data-ttu-id="10322-592">Adicione novos comandos `az atp show` e `az atp update` para exibir e gerenciar configurações avançadas de proteção contra ameaças para contas de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="10322-592">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="10322-593">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-593">SQL</span></span>

* <span data-ttu-id="10322-594">`sql dw create`: substitua os parâmetros `--zone-redundant` e `--read-replica-count`.</span><span class="sxs-lookup"><span data-stu-id="10322-594">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="10322-595">Esses parâmetros não se aplicam ao DataWarehouse.</span><span class="sxs-lookup"><span data-stu-id="10322-595">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="10322-596">[ALTERAÇÃO DA FALHA] `az sql db create`: Remova "WideWorldImportersStd" e "WideWorldImportersFull" como valores permitidos documentados para "az sql db create --sample-name".</span><span class="sxs-lookup"><span data-stu-id="10322-596">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="10322-597">Esses bancos de dados de exemplo sempre farão a criação falhar.</span><span class="sxs-lookup"><span data-stu-id="10322-597">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="10322-598">Adicione os novos comandos `sql db classification show/list/update/delete` e `sql db classification recommendation list/enable/disable` para gerenciar classificações de confidencialidade para bancos de dados SQL.</span><span class="sxs-lookup"><span data-stu-id="10322-598">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="10322-599">`az sql db audit-policy`: Correção para ações e grupos de auditoria vazios</span><span class="sxs-lookup"><span data-stu-id="10322-599">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="10322-600">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-600">Storage</span></span>

* <span data-ttu-id="10322-601">Adicione um novo grupo de comandos `az storage share-rm` para usar o provedor de recursos Microsoft.Storage para operações de gerenciamento de compartilhamento de arquivo do Azure.</span><span class="sxs-lookup"><span data-stu-id="10322-601">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="10322-602">Correção de problema nº 11415: erro de permissão para `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="10322-602">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="10322-603">Integre Azcopy 10.3.3 e dê suporte a Win32.</span><span class="sxs-lookup"><span data-stu-id="10322-603">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="10322-604">`az storage copy`: Adicione os parâmetros `--include-path`, `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="10322-604">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="10322-605">`az storage remove`: Altere os parâmetros `--inlcude` e `--exclude` para os parâmetros `--include-path`, `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="10322-605">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="10322-606">`az storage sync`: Adicione os parâmetros `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="10322-606">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="10322-607">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="10322-607">ServiceFabric</span></span>

* <span data-ttu-id="10322-608">Adicione novos comandos para gerenciar o aplicativo e os serviços.</span><span class="sxs-lookup"><span data-stu-id="10322-608">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="10322-609">13 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="10322-609">January 13, 2020</span></span>

<span data-ttu-id="10322-610">Versão 2.0.80</span><span class="sxs-lookup"><span data-stu-id="10322-610">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="10322-611">Computação</span><span class="sxs-lookup"><span data-stu-id="10322-611">Compute</span></span>

* <span data-ttu-id="10322-612">atualização do disco: Adicionar --disk-encryption-set e --encryption-type</span><span class="sxs-lookup"><span data-stu-id="10322-612">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="10322-613">criação/atualização do instantâneo: Adicionar --disk-encryption-set e --encryption-type</span><span class="sxs-lookup"><span data-stu-id="10322-613">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="10322-614">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-614">Storage</span></span>

* <span data-ttu-id="10322-615">Atualizar a versão do azure-mgmt-storage para 7.1.0</span><span class="sxs-lookup"><span data-stu-id="10322-615">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="10322-616">`az storage account create`: Adicionar `--encryption-key-type-for-table` e `--encryption-key-type-for-queue` para dar suporte ao Serviço de Criptografia de Tabela e de Fila</span><span class="sxs-lookup"><span data-stu-id="10322-616">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="10322-617">07 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="10322-617">January 07, 2020</span></span>

<span data-ttu-id="10322-618">Versão 2.0.79</span><span class="sxs-lookup"><span data-stu-id="10322-618">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="10322-619">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-619">ACR</span></span>

* <span data-ttu-id="10322-620">[ALTERAÇÃO SIGNIFICATIVA] Remover o parâmetro '--os' para 'acr build', 'acr task create/update', 'acr run' e 'acr pack'.</span><span class="sxs-lookup"><span data-stu-id="10322-620">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="10322-621">Em vez disso, use '--platform'.</span><span class="sxs-lookup"><span data-stu-id="10322-621">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="10322-622">AppConfig</span><span class="sxs-lookup"><span data-stu-id="10322-622">AppConfig</span></span>

* <span data-ttu-id="10322-623">Adicionar suporte para importar/exportar sinalizadores de recurso</span><span class="sxs-lookup"><span data-stu-id="10322-623">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="10322-624">Adicione o novo comando 'az appconfig kv set-keyvault' para criar a referência do keyvault</span><span class="sxs-lookup"><span data-stu-id="10322-624">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="10322-625">Suporte a várias convenções de nomenclatura ao exportar os sinalizadores de recurso para o arquivo</span><span class="sxs-lookup"><span data-stu-id="10322-625">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-626">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-626">AppService</span></span>

* <span data-ttu-id="10322-627">Corrigir o problema #7154: Atualizar a documentação para o comando <> para usar acentos grave em vez de aspas simples</span><span class="sxs-lookup"><span data-stu-id="10322-627">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="10322-628">Corrigir o problema #11287: webapp up: Por padrão, faça o aplicativo criado usando 'should be 'SSL enabled'</span><span class="sxs-lookup"><span data-stu-id="10322-628">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="10322-629">Corrigir o problema #11592: Adicionar o sinalizador az webapp up para sites HTML estáticos</span><span class="sxs-lookup"><span data-stu-id="10322-629">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="10322-630">ARM</span><span class="sxs-lookup"><span data-stu-id="10322-630">ARM</span></span>

* <span data-ttu-id="10322-631">Corrigir `az resource tag`: As marcas do Cofre dos Serviços de Recuperação não podem ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="10322-631">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="10322-632">Backup</span><span class="sxs-lookup"><span data-stu-id="10322-632">Backup</span></span>

* <span data-ttu-id="10322-633">Novo comando 'backup protection undelete' adicionado para habilitar o recurso de exclusão reversível para carga de trabalho IaasVM</span><span class="sxs-lookup"><span data-stu-id="10322-633">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="10322-634">Novo parâmetro '--soft-delete-feature-state' adicionado para definir o comando propriedades do backup</span><span class="sxs-lookup"><span data-stu-id="10322-634">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="10322-635">Suporte de exclusão de disco adicionado para carga de trabalho IaasVM</span><span class="sxs-lookup"><span data-stu-id="10322-635">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="10322-636">Computação</span><span class="sxs-lookup"><span data-stu-id="10322-636">Compute</span></span>

* <span data-ttu-id="10322-637">Corrigir a falha `vm create` no perfil do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="10322-637">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="10322-638">parte final/listar definições de métricas de monitor de vm: suporte a métricas de consulta e definições de lista para uma vm.</span><span class="sxs-lookup"><span data-stu-id="10322-638">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="10322-639">Adicionar nova ação de comando de reaplicação para az vm</span><span class="sxs-lookup"><span data-stu-id="10322-639">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="10322-640">HDInsight</span><span class="sxs-lookup"><span data-stu-id="10322-640">HDInsight</span></span>

* <span data-ttu-id="10322-641">Suporte para criar um cluster Kafka com o Proxy REST do Kafka</span><span class="sxs-lookup"><span data-stu-id="10322-641">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="10322-642">Atualizar azure-mgmt-hdinsight para 1.3.0</span><span class="sxs-lookup"><span data-stu-id="10322-642">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="10322-643">Diversos.</span><span class="sxs-lookup"><span data-stu-id="10322-643">Misc.</span></span>

* <span data-ttu-id="10322-644">Adicionar comando de visualização `az version show` para mostrar as versões dos módulos e das extensões da CLI do Azure no formato JSON por padrão ou no formato configurado por --output</span><span class="sxs-lookup"><span data-stu-id="10322-644">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="10322-645">Hubs de Eventos</span><span class="sxs-lookup"><span data-stu-id="10322-645">Event Hubs</span></span>

* <span data-ttu-id="10322-646">[ALTERAÇÃO SIGNIFICATIVA] Remover a opção de status 'ReceiveDisabled' do comando 'az eventhubs eventhub update' e 'az eventhubs eventhub create'.</span><span class="sxs-lookup"><span data-stu-id="10322-646">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="10322-647">Essa opção não é válida para entidades do Hub de Eventos.</span><span class="sxs-lookup"><span data-stu-id="10322-647">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="10322-648">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="10322-648">Service Bus</span></span>

* <span data-ttu-id="10322-649">[ALTERAÇÃO SIGNIFICATIVA] Remover a opção de status 'ReceiveDisabled' do comando 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create' e 'az servicebus queue update'.</span><span class="sxs-lookup"><span data-stu-id="10322-649">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="10322-650">Essa opção não é válida para tópicos e filas do Barramento de Serviço.</span><span class="sxs-lookup"><span data-stu-id="10322-650">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="10322-651">RBAC</span><span class="sxs-lookup"><span data-stu-id="10322-651">RBAC</span></span>

* <span data-ttu-id="10322-652">Correção #11712: `az ad app/sp show` não devolve o código de saída 3 quando o aplicativo ou a entidade de serviço não existir</span><span class="sxs-lookup"><span data-stu-id="10322-652">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="10322-653">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-653">Storage</span></span>

* <span data-ttu-id="10322-654">`az storage account create`: Remover o sinalizador de visualização do parâmetro --enable-hierarchical-namespace</span><span class="sxs-lookup"><span data-stu-id="10322-654">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="10322-655">Atualizar a versão azure-mgmt-storage para 7.0.0 para usar a versão de API 2019-06-01</span><span class="sxs-lookup"><span data-stu-id="10322-655">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="10322-656">Adicionar novos parâmetros `--enable-delete-retention` e `--delete-retention-days` para dar suporte ao gerenciamento da política de retenção de exclusão para a conta de armazenamento blob-service-properties.</span><span class="sxs-lookup"><span data-stu-id="10322-656">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="10322-657">17 de dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-657">December 17, 2019</span></span>

<span data-ttu-id="10322-658">2.0.78</span><span class="sxs-lookup"><span data-stu-id="10322-658">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="10322-659">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-659">ACR</span></span>

* <span data-ttu-id="10322-660">Contexto local de suporte adicionado na execução da tarefa acr</span><span class="sxs-lookup"><span data-stu-id="10322-660">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="10322-661">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-661">ACS</span></span>

* <span data-ttu-id="10322-662">[ALTERAÇÃO SIGNIFICATIVA]criar az openshift: renomear `--workspace-resource-id` para `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="10322-662">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="10322-663">AMS</span><span class="sxs-lookup"><span data-stu-id="10322-663">AMS</span></span>

* <span data-ttu-id="10322-664">Comandos de exibição atualizados para devolver 3 quando o recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="10322-664">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="10322-665">AppConfig</span><span class="sxs-lookup"><span data-stu-id="10322-665">AppConfig</span></span>

* <span data-ttu-id="10322-666">Bug corrigido ao acrescentar a versão de API à URL de solicitação.</span><span class="sxs-lookup"><span data-stu-id="10322-666">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="10322-667">A solução existente não funciona com a paginação.</span><span class="sxs-lookup"><span data-stu-id="10322-667">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="10322-668">Suporte adicionado para a exibição de idiomas além do inglês, pois nosso serviço de back-end é compatível com unicode para globalização.</span><span class="sxs-lookup"><span data-stu-id="10322-668">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-669">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-669">AppService</span></span>

* <span data-ttu-id="10322-670">Problema corrigido nº 11217: webapp: o upload ssl de configuração do az webapp deve ser compatível com o parâmetro do slot</span><span class="sxs-lookup"><span data-stu-id="10322-670">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="10322-671">Problema corrigido nº 10965: Erro: O nome não pode estar vazio.</span><span class="sxs-lookup"><span data-stu-id="10322-671">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="10322-672">Permitir remoção por ip_address e sub-rede</span><span class="sxs-lookup"><span data-stu-id="10322-672">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="10322-673">Suporte adicionado para importar certificados do Key Vault `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="10322-673">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="10322-674">ARM</span><span class="sxs-lookup"><span data-stu-id="10322-674">ARM</span></span>

* <span data-ttu-id="10322-675">Pacote azure-mgmt-resource atualizado para usar 6.0.0</span><span class="sxs-lookup"><span data-stu-id="10322-675">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="10322-676">Suporte entre locatários para o comando `az group deployment create` adicionando o novo parâmetro `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="10322-676">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="10322-677">Novo parâmetro `--metadata` adicionado para dar suporte à adição de informações de metadados para definições de conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="10322-677">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="10322-678">Backup</span><span class="sxs-lookup"><span data-stu-id="10322-678">Backup</span></span>

* <span data-ttu-id="10322-679">Suporte de backup adicionado para carga de trabalho SQL e SAP Hana.</span><span class="sxs-lookup"><span data-stu-id="10322-679">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="10322-680">BotService</span><span class="sxs-lookup"><span data-stu-id="10322-680">BotService</span></span>

* <span data-ttu-id="10322-681">[ALTERAÇÃO SIGNIFICATIVA] Remover o sinalizador '--version ' do comando de visualização 'az bot create'.</span><span class="sxs-lookup"><span data-stu-id="10322-681">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="10322-682">Somente os bots do SDK v4 são compatíveis.</span><span class="sxs-lookup"><span data-stu-id="10322-682">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="10322-683">Verificação de disponibilidade de nome adicionada para 'az bot create'.</span><span class="sxs-lookup"><span data-stu-id="10322-683">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="10322-684">Suporte adicionado para atualizar a URL do ícone para um bot por meio de 'az bot update'.</span><span class="sxs-lookup"><span data-stu-id="10322-684">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="10322-685">Suporte adicionado para atualizar um canal Direct Line por meio de 'az bot directline update'.</span><span class="sxs-lookup"><span data-stu-id="10322-685">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="10322-686">Suporte ao sinalizador '--enable-enhanced-auth' adicionado para 'az bot directline create'.</span><span class="sxs-lookup"><span data-stu-id="10322-686">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="10322-687">Os seguintes grupos de comandos estão em GA e não estão em versão prévia: 'az bot authsetting'.</span><span class="sxs-lookup"><span data-stu-id="10322-687">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="10322-688">Os seguintes comandos em 'az bot' estão em GA e não na versão prévia: 'criar', 'preparar-implantar', 'mostrar', 'excluir', 'atualizar'.</span><span class="sxs-lookup"><span data-stu-id="10322-688">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="10322-689">Correção do valor 'az bot prepare-deploy' alterando '--proj-file-path ' para letras minúsculas (por exemplo, "Test. csproj" para "Test. csproj").</span><span class="sxs-lookup"><span data-stu-id="10322-689">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="10322-690">Computação</span><span class="sxs-lookup"><span data-stu-id="10322-690">Compute</span></span>

* <span data-ttu-id="10322-691">Criar/atualizar vmss: --scale-in-policy adicionado, que decide quais máquinas virtuais são escolhidas para remoção quando um VMSS é dimensionado.</span><span class="sxs-lookup"><span data-stu-id="10322-691">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="10322-692">atualização de vm/vmss: --priority adicionado.</span><span class="sxs-lookup"><span data-stu-id="10322-692">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="10322-693">atualização de vm/vmss: --max-price adicionado.</span><span class="sxs-lookup"><span data-stu-id="10322-693">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="10322-694">Grupo de comandos do conjunto de criptografia de disco adicionado (criar, mostrar, atualizar, excluir e listar).</span><span class="sxs-lookup"><span data-stu-id="10322-694">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="10322-695">criação de disco: --encryption-type e --disk-encryption-set adicionados.</span><span class="sxs-lookup"><span data-stu-id="10322-695">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="10322-696">vm/vmss create: --os-disk-encryption-set e --data-disk-encryption-sets adicionados.</span><span class="sxs-lookup"><span data-stu-id="10322-696">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="10322-697">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-697">Core</span></span>

* <span data-ttu-id="10322-698">Suporte para Python 3.4 removido</span><span class="sxs-lookup"><span data-stu-id="10322-698">Removed support for Python 3.4</span></span>
* <span data-ttu-id="10322-699">Pesquisa de funções de plug-in em vários comandos</span><span class="sxs-lookup"><span data-stu-id="10322-699">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="10322-700">DLS</span><span class="sxs-lookup"><span data-stu-id="10322-700">DLS</span></span>

* <span data-ttu-id="10322-701">Versão atualizada do SDK do ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="10322-701">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="10322-702">Instalar</span><span class="sxs-lookup"><span data-stu-id="10322-702">Install</span></span>

* <span data-ttu-id="10322-703">Instalar suporte de script Python 3.8</span><span class="sxs-lookup"><span data-stu-id="10322-703">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="10322-704">IOT</span><span class="sxs-lookup"><span data-stu-id="10322-704">IOT</span></span>

* <span data-ttu-id="10322-705">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro--failover-region removido de failover manual.</span><span class="sxs-lookup"><span data-stu-id="10322-705">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="10322-706">Agora ele fará failover para a região secundária emparelhada atribuída geograficamente.</span><span class="sxs-lookup"><span data-stu-id="10322-706">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="10322-707">Key Vault</span><span class="sxs-lookup"><span data-stu-id="10322-707">Key Vault</span></span>

* <span data-ttu-id="10322-708">Nº 8095 corrigido: `az keyvault storage remove`: melhorar a mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="10322-708">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="10322-709">Nº 8921 corrigido: `az keyvault key/secret/certificate list/list-deleted/list-versions`: corrigir o bug de validação no parâmetro `--maxresults`</span><span class="sxs-lookup"><span data-stu-id="10322-709">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="10322-710">Nº 10512 corrigido: `az keyvault set-policy`: melhorar a mensagem de erro quando nenhuma das `--object-id`, `--spn` ou `--upn` for especificada</span><span class="sxs-lookup"><span data-stu-id="10322-710">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="10322-711">Nº 10846 corrigido: `az keyvault secret show-deleted`: quando `--id` for especificado, `--name/-n` não será necessário</span><span class="sxs-lookup"><span data-stu-id="10322-711">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="10322-712">Nº 11084 corrigido: `az keyvault secret download`: melhorar a mensagem de ajuda do parâmetro `--encoding`</span><span class="sxs-lookup"><span data-stu-id="10322-712">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="10322-713">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-713">Network</span></span>

* <span data-ttu-id="10322-714">Investigação de gateway de aplicativo de rede az: Suporte --port option adicionado para especificar uma porta para sondar servidores de back-end ao criar e atualizar</span><span class="sxs-lookup"><span data-stu-id="10322-714">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="10322-715">az network application-gateway url-path-map create/update: correção de bug para `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="10322-715">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="10322-716">az network application-gateway: Suporte `--rewrite-rule-set` adicionado</span><span class="sxs-lookup"><span data-stu-id="10322-716">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="10322-717">az network list-service-aliases: Foram adicionados aliases de serviço da lista de suporte que podem ser usados para políticas de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="10322-717">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="10322-718">importar zona dns da rede az: Suporte adicionado. @ no nome do registro</span><span class="sxs-lookup"><span data-stu-id="10322-718">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="10322-719">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="10322-719">Packaging</span></span>

* <span data-ttu-id="10322-720">Compilações de back edge adicionadas para instalação de pip</span><span class="sxs-lookup"><span data-stu-id="10322-720">Added back edge builds for pip install</span></span>
* <span data-ttu-id="10322-721">Pacote eoan do Ubuntu adicionado</span><span class="sxs-lookup"><span data-stu-id="10322-721">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="10322-722">Política</span><span class="sxs-lookup"><span data-stu-id="10322-722">Policy</span></span>

* <span data-ttu-id="10322-723">Inclusão de compatibilidade com a API de Política, versão de 01/09/2019.</span><span class="sxs-lookup"><span data-stu-id="10322-723">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="10322-724">az policy set-definition: Agrupamento de suporte adicionado nas definições do conjunto de políticas com `--definition-groups` parâmetro</span><span class="sxs-lookup"><span data-stu-id="10322-724">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="10322-725">Redis</span><span class="sxs-lookup"><span data-stu-id="10322-725">Redis</span></span>

* <span data-ttu-id="10322-726">Adicionado o parâmetro de visualização `--replicas-per-master` ao comando `az redis create`</span><span class="sxs-lookup"><span data-stu-id="10322-726">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="10322-727">Azure-MGMT-Redis adicionado do 6.0.0 para o 7.0.0rc1</span><span class="sxs-lookup"><span data-stu-id="10322-727">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="10322-728">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="10322-728">ServiceFabric</span></span>

* <span data-ttu-id="10322-729">Corrigido em nó-tipo adicionar lógica, incluindo #10963: A adição do novo tipo de nó com nível de durabilidade Gold sempre gerará erro da CLI</span><span class="sxs-lookup"><span data-stu-id="10322-729">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="10322-730">Versão do ServiceFabricNodeVmExt atualizada para 1.1 no modelo de criação</span><span class="sxs-lookup"><span data-stu-id="10322-730">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="10322-731">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-731">SQL</span></span>

* <span data-ttu-id="10322-732">Adicionados os parâmetros "--read-scale" e "--read-replicas" aos comandos criar e atualizar do BD SQL para dar suporte ao gerenciamento de escala de leitura.</span><span class="sxs-lookup"><span data-stu-id="10322-732">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="10322-733">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-733">Storage</span></span>

* <span data-ttu-id="10322-734">Propriedade de compartilhamentos de arquivos grandes da versão GA para o comando criar e atualizar da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-734">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="10322-735">Suporte ao token SAS de delegação de usuário da versão GA</span><span class="sxs-lookup"><span data-stu-id="10322-735">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="10322-736">Novos comandos adicionados `az storage account blob-service-properties show` e `az storage account blob-service-properties update --enable-change-feed` para gerenciar Propriedades do serviço blob para a conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="10322-736">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="10322-737">[PRÓXIMA ALTERAÇÃO DA FALHA] `az storage copy`: `*` não há mais suporte para o caractere de como um curinga na URL, mas novos parâmetros--include-pattern e --exclude-pattern serão adicionados com suporte a curinga `*`.</span><span class="sxs-lookup"><span data-stu-id="10322-737">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="10322-738">Problema corrigido nº 11043: Suporte adicionado para remover contêiner/compartilhamento inteiro no comando `az storage remove`</span><span class="sxs-lookup"><span data-stu-id="10322-738">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="10322-739">26 de novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-739">November 26, 2019</span></span>

<span data-ttu-id="10322-740">Versão 2.0.77</span><span class="sxs-lookup"><span data-stu-id="10322-740">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="10322-741">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-741">ACR</span></span>

* <span data-ttu-id="10322-742">Parâmetro `--branch` preterido da criação/atualização da tarefa ACR</span><span class="sxs-lookup"><span data-stu-id="10322-742">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="10322-743">Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="10322-743">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="10322-744">Sinalizador `--workspace-resource-id` adicionado para permitir a criação do cluster do Red Hat OpenShift no Azure com monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-744">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="10322-745">`monitor_profile` adicionado para criar o cluster do Red Hat OpenShift no Azure com monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-745">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="10322-746">AKS</span><span class="sxs-lookup"><span data-stu-id="10322-746">AKS</span></span>

* <span data-ttu-id="10322-747">Operação de rotação de certificado de cluster de suporte adicionada usando "az aks rotate-certs".</span><span class="sxs-lookup"><span data-stu-id="10322-747">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="10322-748">AppConfig</span><span class="sxs-lookup"><span data-stu-id="10322-748">AppConfig</span></span>

* <span data-ttu-id="10322-749">Suporte adicionado para usar ":" para o separador `as az appconfig kv import`</span><span class="sxs-lookup"><span data-stu-id="10322-749">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="10322-750">Problema corrigido para listar valores de chave com vários rótulos incluindo o rótulo nulo.</span><span class="sxs-lookup"><span data-stu-id="10322-750">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="10322-751">SDK do plano de gerenciamento atualizado, azure-mgmt-appconfiguration, para a versão 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="10322-751">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="10322-752">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-752">AppService</span></span>

* <span data-ttu-id="10322-753">Problema corrigido nº 11100: AttributeError para az webapp up ao criar o plano de serviço</span><span class="sxs-lookup"><span data-stu-id="10322-753">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="10322-754">az webapp up: Forçar a criação ou a implantação em um site para linguagens com suporte, nenhum padrão usado.</span><span class="sxs-lookup"><span data-stu-id="10322-754">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="10322-755">Suporte adicionado para o Ambiente do Serviço de Aplicativo: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="10322-755">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="10322-756">Backup</span><span class="sxs-lookup"><span data-stu-id="10322-756">Backup</span></span>

* <span data-ttu-id="10322-757">Problema corrigido em list-associated-items da política de backup az.</span><span class="sxs-lookup"><span data-stu-id="10322-757">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="10322-758">Parâmetro BackupManagementType opcional adicionado.</span><span class="sxs-lookup"><span data-stu-id="10322-758">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="10322-759">Computação</span><span class="sxs-lookup"><span data-stu-id="10322-759">Compute</span></span>

* <span data-ttu-id="10322-760">Versão de API de computação, discos e instantâneos atualizados para 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="10322-760">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="10322-761">vmss create: melhoria para --orchestration-mode</span><span class="sxs-lookup"><span data-stu-id="10322-761">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="10322-762">sig image-definition create: --os-state adicionado para permitir a especificação se as máquinas virtuais criadas nessa imagem são 'Generalizadas' ou 'Especializadas'</span><span class="sxs-lookup"><span data-stu-id="10322-762">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="10322-763">sig image-definition create: --hyper-v-generation adicionado para permitir a especificação da geração do hipervisor</span><span class="sxs-lookup"><span data-stu-id="10322-763">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="10322-764">sig image-version create: --os-snapshot e --data-snapshots de suporte adicionados</span><span class="sxs-lookup"><span data-stu-id="10322-764">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="10322-765">image create: --data-disk-caching adicionado para permitir a especificação da configuração de cache de discos de dados</span><span class="sxs-lookup"><span data-stu-id="10322-765">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="10322-766">SDK de computação do Python atualizado para 10.0.0</span><span class="sxs-lookup"><span data-stu-id="10322-766">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="10322-767">vm/vmss create: 'Spot' adicionado à propriedade de enumeração 'Priority'</span><span class="sxs-lookup"><span data-stu-id="10322-767">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="10322-768">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro '--max-billing' renomeado para '--max-price', para a VM e o VMSS, a fim de que seja consistente com os cmdlets do Swagger e do PowerShell</span><span class="sxs-lookup"><span data-stu-id="10322-768">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="10322-769">vm monitor log show: suporte adicionado para consultar o log pelo workspace do Log Analytics vinculado.</span><span class="sxs-lookup"><span data-stu-id="10322-769">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="10322-770">IOT</span><span class="sxs-lookup"><span data-stu-id="10322-770">IOT</span></span>

* <span data-ttu-id="10322-771">Correção nº 2531: argumentos de conveniência adicionados para a atualização do hub.</span><span class="sxs-lookup"><span data-stu-id="10322-771">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="10322-772">Correção nº 8323: parâmetros ausentes adicionados para criar o ponto de extremidade personalizado de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="10322-772">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="10322-773">Corrigir bug de regressão: as alterações que substituem o ponto de extremidade de armazenamento padrão foram revertidas.</span><span class="sxs-lookup"><span data-stu-id="10322-773">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="10322-774">Key Vault</span><span class="sxs-lookup"><span data-stu-id="10322-774">Key Vault</span></span>

* <span data-ttu-id="10322-775">Correção nº 11121: ao usar `az keyvault certificate list`, passar `--include-pending` agora não exige um valor de `true` ou `false`</span><span class="sxs-lookup"><span data-stu-id="10322-775">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="10322-776">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="10322-776">NetAppFiles</span></span>

* <span data-ttu-id="10322-777">azure-mgmt-netapp atualizado para 0.7.0 que inclui algumas propriedades de volume adicionais associadas a operações de replicação futuras</span><span class="sxs-lookup"><span data-stu-id="10322-777">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="10322-778">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-778">Network</span></span>

* <span data-ttu-id="10322-779">application-gateway waf-config: preterido</span><span class="sxs-lookup"><span data-stu-id="10322-779">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="10322-780">application-gateway waf-policy: subgrupo managed-rules adicionado para gerenciar os conjuntos de regras e regras de exclusão gerenciados</span><span class="sxs-lookup"><span data-stu-id="10322-780">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="10322-781">application-gateway waf-policy: subgrupo policy-setting adicionado para gerenciar a configuração global de um waf-policy</span><span class="sxs-lookup"><span data-stu-id="10322-781">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="10322-782">[ALTERAÇÃO SIGNIFICATIVA] application-gateway waf-policy: subgrupo rule renomeado para custom-rule</span><span class="sxs-lookup"><span data-stu-id="10322-782">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="10322-783">application-gateway http-listener: --firewall-policy adicionado durante a criação</span><span class="sxs-lookup"><span data-stu-id="10322-783">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="10322-784">application-gateway url-path-map rule: --firewall-policy adicionado durante a criação</span><span class="sxs-lookup"><span data-stu-id="10322-784">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="10322-785">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="10322-785">Packaging</span></span>

* <span data-ttu-id="10322-786">Wrapper az reescrito no Python</span><span class="sxs-lookup"><span data-stu-id="10322-786">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="10322-787">Suporte adicionado para Python 3.8</span><span class="sxs-lookup"><span data-stu-id="10322-787">Added support for Python 3.8</span></span>
* <span data-ttu-id="10322-788">Alterado para Python 3 para o pacote RPM</span><span class="sxs-lookup"><span data-stu-id="10322-788">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="10322-789">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-789">Profile</span></span>

* <span data-ttu-id="10322-790">Erro aperfeiçoado ao executar `az login -u {} -p {}` com a conta Microsoft</span><span class="sxs-lookup"><span data-stu-id="10322-790">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="10322-791">`SSLError` aperfeiçoado ao executar `az login` atrás de um proxy com o certificado raiz autoassinado</span><span class="sxs-lookup"><span data-stu-id="10322-791">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="10322-792">Correção nº 10578: `az login` trava quando mais de uma instância é iniciada ao mesmo tempo no Windows ou WSL</span><span class="sxs-lookup"><span data-stu-id="10322-792">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="10322-793">Correção nº 11059: `az login --allow-no-subscriptions` falhará se houver assinaturas no locatário</span><span class="sxs-lookup"><span data-stu-id="10322-793">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="10322-794">Correção nº 11238: após renomear uma assinatura, fazer logon com a MSI fará a mesma assinatura aparecer duas vezes</span><span class="sxs-lookup"><span data-stu-id="10322-794">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="10322-795">RBAC</span><span class="sxs-lookup"><span data-stu-id="10322-795">RBAC</span></span>

* <span data-ttu-id="10322-796">Correção nº 10996: erro aperfeiçoado para `--force-change-password-next-login` em `az ad user update` quando `--password` não for especificado</span><span class="sxs-lookup"><span data-stu-id="10322-796">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="10322-797">Redis</span><span class="sxs-lookup"><span data-stu-id="10322-797">Redis</span></span>

* <span data-ttu-id="10322-798">Correção nº 2902: evite definir configurações de memória ao atualizar o cache do SKU básico</span><span class="sxs-lookup"><span data-stu-id="10322-798">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="10322-799">Reservas</span><span class="sxs-lookup"><span data-stu-id="10322-799">Reservations</span></span>

* <span data-ttu-id="10322-800">Versão do SDK atualizada para 0.6.0</span><span class="sxs-lookup"><span data-stu-id="10322-800">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="10322-801">Informações de detalhes do plano de cobrança atualizadas após chamar Get-Gatalogs</span><span class="sxs-lookup"><span data-stu-id="10322-801">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="10322-802">Novo comando `az reservations reservation-order calculate` adicionado para calcular o preço de uma reserva</span><span class="sxs-lookup"><span data-stu-id="10322-802">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="10322-803">Novo comando `az reservations reservation-order purchase` adicionado para comprar uma nova reserva</span><span class="sxs-lookup"><span data-stu-id="10322-803">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="10322-804">Rest</span><span class="sxs-lookup"><span data-stu-id="10322-804">Rest</span></span>
* <span data-ttu-id="10322-805">`az rest` alterado para GA</span><span class="sxs-lookup"><span data-stu-id="10322-805">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="10322-806">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-806">SQL</span></span>

* <span data-ttu-id="10322-807">azure-mgmt-sql atualizado para 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="10322-807">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="10322-808">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-808">Storage</span></span>

* <span data-ttu-id="10322-809">storage account create: --enable-hierarchical-namespace adicionado para dar suporte à semântica do sistema de arquivos no serviço Blob.</span><span class="sxs-lookup"><span data-stu-id="10322-809">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="10322-810">Exceção não relacionada removida da mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="10322-810">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="10322-811">Problemas corrigidos com a mensagem de erro incorreta "Você não tem as permissões necessárias para executar essa operação."</span><span class="sxs-lookup"><span data-stu-id="10322-811">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="10322-812">quando bloqueado pelas regras de rede ou AuthenticationFailed.</span><span class="sxs-lookup"><span data-stu-id="10322-812">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="10322-813">4 de novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-813">November 4, 2019</span></span>

<span data-ttu-id="10322-814">Versão 2.0.76</span><span class="sxs-lookup"><span data-stu-id="10322-814">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="10322-815">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-815">ACR</span></span>

* <span data-ttu-id="10322-816">O parâmetro de versão prévia `--pack-image-tag` foi adicionado ao comando `az acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="10322-816">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="10322-817">Suporte adicionado para habilitar a auditoria na criação de um registro</span><span class="sxs-lookup"><span data-stu-id="10322-817">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="10322-818">Suporte adicionado para o RBAC com escopo de repositório</span><span class="sxs-lookup"><span data-stu-id="10322-818">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="10322-819">AKS</span><span class="sxs-lookup"><span data-stu-id="10322-819">AKS</span></span>

* <span data-ttu-id="10322-820">`--enable-cluster-autoscaler`, `--min-count` e `--max-count` foram adicionados ao comando `az aks create`, que habilita o dimensionamento automático do cluster para o pool de nós.</span><span class="sxs-lookup"><span data-stu-id="10322-820">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="10322-821">Foram adicionados os sinalizadores acima, bem como `--update-cluster-autoscaler` e `--disable-cluster-autoscaler` ao comando `az aks update`, permitindo atualizações do cluster de dimensionamento automático.</span><span class="sxs-lookup"><span data-stu-id="10322-821">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="10322-822">AppConfig</span><span class="sxs-lookup"><span data-stu-id="10322-822">AppConfig</span></span>

* <span data-ttu-id="10322-823">O grupo de comandos do recurso AppConfig foi adicionado para gerenciar os sinalizadores de recurso armazenados em uma Configuração de Aplicativos.</span><span class="sxs-lookup"><span data-stu-id="10322-823">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="10322-824">Foi corrigido um bug secundário do comando de exportação para arquivo appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="10322-824">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="10322-825">Foi interrompida a leitura de conteúdo do arquivo de destino durante a exportação.</span><span class="sxs-lookup"><span data-stu-id="10322-825">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-826">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-826">AppService</span></span>

* <span data-ttu-id="10322-827">`az appservice plan create`: Foi adicionado o suporte para definir 'persitecalling' no comando appservice plan create.</span><span class="sxs-lookup"><span data-stu-id="10322-827">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="10322-828">Foi corrigido um problema em que a operação webapp config ssl bind estava removendo as marcas existentes do recurso</span><span class="sxs-lookup"><span data-stu-id="10322-828">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="10322-829">Foi adicionado o sinalizador `--build-remote` para `az functionapp deployment source config-zip` para dar suporte à ação de build remoto durante a implantação do aplicativo de funções.</span><span class="sxs-lookup"><span data-stu-id="10322-829">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="10322-830">Foi alterada a versão do nó padrão em aplicativos de funções para ~10 para Windows</span><span class="sxs-lookup"><span data-stu-id="10322-830">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="10322-831">A propriedade `--runtime-version` foi adicionada a `az functionapp create`</span><span class="sxs-lookup"><span data-stu-id="10322-831">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="10322-832">ARM</span><span class="sxs-lookup"><span data-stu-id="10322-832">ARM</span></span>

* <span data-ttu-id="10322-833">`az deployment/group deployment validate`: Foi adicionado o parâmetro `--handle-extended-json-format` para dar suporte a várias linhas e comentários no modelo JSON durante a implantação.</span><span class="sxs-lookup"><span data-stu-id="10322-833">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="10322-834">O azure-mgmt-resource passou a usar a 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="10322-834">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="10322-835">Backup</span><span class="sxs-lookup"><span data-stu-id="10322-835">Backup</span></span>

* <span data-ttu-id="10322-836">Foi adicionado o suporte de backup aos Arquivos do Azure</span><span class="sxs-lookup"><span data-stu-id="10322-836">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="10322-837">Computação</span><span class="sxs-lookup"><span data-stu-id="10322-837">Compute</span></span>

* <span data-ttu-id="10322-838">`az vm create`: foi adicionado um aviso ao especificar a rede acelerada e um adaptador de rede existente juntos.</span><span class="sxs-lookup"><span data-stu-id="10322-838">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="10322-839">`az vm create`: foi adicionado `--vmss` para especificar um conjunto de dimensionamento de máquinas virtuais existente ao qual a máquina virtual deve ser atribuída.</span><span class="sxs-lookup"><span data-stu-id="10322-839">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="10322-840">`az vm/vmss create`: foi adicionada uma cópia local do arquivo de alias de imagem para que ele possa ser acessado em um ambiente de rede restrita.</span><span class="sxs-lookup"><span data-stu-id="10322-840">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="10322-841">`az vmss create`: foi adicionado `--orchestration-mode` para especificar como as máquinas virtuais são gerenciadas pelo conjunto de dimensionamento.</span><span class="sxs-lookup"><span data-stu-id="10322-841">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="10322-842">`az vm/vmss update`: foi adicionado `--ultra-ssd-enabled` para permitir a atualização da configuração de SSD Ultra.</span><span class="sxs-lookup"><span data-stu-id="10322-842">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="10322-843">[ALTERAÇÃO DA FALHA] `az vm extension set`: foi corrigido o bug em que os usuários não podiam definir uma extensão em uma VM com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="10322-843">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="10322-844">Foram adicionados os novos comandos `az vm image terms accept/cancel/show` para gerenciar os termos de imagem do Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="10322-844">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="10322-845">O VMAccessForLinux foi atualizado para a versão 1.5</span><span class="sxs-lookup"><span data-stu-id="10322-845">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="10322-846">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="10322-846">CosmosDB</span></span>

* <span data-ttu-id="10322-847">[ALTERAÇÃO DA FALHA] `az sql container create`: `--partition-key-path` foi alterado para parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="10322-847">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="10322-848">[ALTERAÇÃO DA FALHA] `az gremlin graph create`: `--partition-key-path` foi alterado para parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="10322-848">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="10322-849">`az sql container create`: Adição de `--unique-key-policy` e `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="10322-849">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="10322-850">`az sql container create/update`: o esquema padrão `--idx` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="10322-850">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="10322-851">`gremlin graph create`: Adicionado `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="10322-851">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="10322-852">`gremlin graph create/update`: o esquema padrão `--idx` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="10322-852">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="10322-853">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="10322-853">Fixed typo in help message</span></span>
* <span data-ttu-id="10322-854">banco de dados: Foram adicionadas informações sobre preteridos</span><span class="sxs-lookup"><span data-stu-id="10322-854">database: Added deprecation information</span></span>
* <span data-ttu-id="10322-855">coleção: Foram adicionadas informações sobre preteridos</span><span class="sxs-lookup"><span data-stu-id="10322-855">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="10322-856">IoT</span><span class="sxs-lookup"><span data-stu-id="10322-856">IoT</span></span>

* <span data-ttu-id="10322-857">Um novo tipo de fonte de roteamento foi adicionado: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="10322-857">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="10322-858">Foi corrigido o erro de recursos ausentes no `az iot hub create`</span><span class="sxs-lookup"><span data-stu-id="10322-858">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="10322-859">Key Vault</span><span class="sxs-lookup"><span data-stu-id="10322-859">Key Vault</span></span>

* <span data-ttu-id="10322-860">Foi corrigido um erro inesperado quando o arquivo de certificado não existe</span><span class="sxs-lookup"><span data-stu-id="10322-860">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="10322-861">Foi corrigido o problema em que o `az keyvault recover/purge` não funcionava</span><span class="sxs-lookup"><span data-stu-id="10322-861">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="10322-862">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="10322-862">NetAppFiles</span></span>

* <span data-ttu-id="10322-863">O azure-mgmt-netapp foi atualizado para 0.6.0 para usar a versão da API 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="10322-863">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="10322-864">Essa nova versão da API inclui:</span><span class="sxs-lookup"><span data-stu-id="10322-864">This new API version includes:</span></span>

    - <span data-ttu-id="10322-865">A criação de volume `--protocol-types` agora aceita "NFSv4.1" não "NFSv4"</span><span class="sxs-lookup"><span data-stu-id="10322-865">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="10322-866">A propriedade da política de exportação de volume agora é chamada 'nfsv41' não 'nfsv4'</span><span class="sxs-lookup"><span data-stu-id="10322-866">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="10322-867">O volume `--creation-token` foi renomeado para `--file-path`</span><span class="sxs-lookup"><span data-stu-id="10322-867">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="10322-868">A data de criação do instantâneo agora é chamada apenas de 'criação'</span><span class="sxs-lookup"><span data-stu-id="10322-868">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="10322-869">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-869">Network</span></span>

* <span data-ttu-id="10322-870">`az network private-dns link vnet create/update`: suporte à vinculação de rede virtual entre locatários.</span><span class="sxs-lookup"><span data-stu-id="10322-870">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="10322-871">[ALTERAÇÃO DA FALHA] `az network vnet subnet list`: `--resource-group` e `--vnet-name` foram alterados para serem obrigatórios agora.</span><span class="sxs-lookup"><span data-stu-id="10322-871">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="10322-872">`az network public-ip prefix create`: Suporte adicionado para especificar a versão do endereço IP (IPv4, IPv6) durante a criação</span><span class="sxs-lookup"><span data-stu-id="10322-872">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="10322-873">O azure-mgmt-network foi atualizado para 7.0.0 e a api-version para 2019-09-01</span><span class="sxs-lookup"><span data-stu-id="10322-873">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="10322-874">`az network vrouter`: Suporte adicionado para o novo roteador virtual de serviço e o emparelhamento do roteador virtual</span><span class="sxs-lookup"><span data-stu-id="10322-874">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="10322-875">`az network express-route gateway connection`: Adicionado o suporte para `--internet-security`</span><span class="sxs-lookup"><span data-stu-id="10322-875">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="10322-876">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-876">Profile</span></span>

* <span data-ttu-id="10322-877">Foi corrigido o problema em que o `az account get-access-token --resource-type ms-graph` não funcionava</span><span class="sxs-lookup"><span data-stu-id="10322-877">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="10322-878">O aviso foi removido de `az login`</span><span class="sxs-lookup"><span data-stu-id="10322-878">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="10322-879">RBAC</span><span class="sxs-lookup"><span data-stu-id="10322-879">RBAC</span></span>

* <span data-ttu-id="10322-880">Foi corrigido o problema em que o `az ad app update --id {} --display-name {}` não funcionava</span><span class="sxs-lookup"><span data-stu-id="10322-880">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="10322-881">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="10322-881">ServiceFabric</span></span>

* <span data-ttu-id="10322-882">`az sf cluster create`: foi corrigido um problema que ocorria ao modificar o VMSS de computação do template.json do Linux e do Windows, do Service Fabric, de discos Standard para discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="10322-882">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="10322-883">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-883">SQL</span></span>

* <span data-ttu-id="10322-884">Os parâmetros `--compute-model`, `--auto-pause-delay` e `--min-capacity` foram adicionados para dar suporte a operações CRUD para a nova oferta de Banco de Dados SQL: Modelo de computação sem servidor.</span><span class="sxs-lookup"><span data-stu-id="10322-884">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="10322-885">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-885">Storage</span></span>

* <span data-ttu-id="10322-886">`az storage account create/update`: Foram adicionados o parâmetro --enable-files-adds e o grupo Argumentos de Propriedades do Azure Active Directory para dar suporte à Autenticação do Serviço de Domínio do Active Directory do Arquivos do Azure</span><span class="sxs-lookup"><span data-stu-id="10322-886">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="10322-887">O `az storage account keys list/renew` foi expandido para dar suporte à listagem ou à regeneração de chaves Kerberos da conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="10322-887">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="10322-888">15 de outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-888">October 15, 2019</span></span>

<span data-ttu-id="10322-889">Versão 2.0.75</span><span class="sxs-lookup"><span data-stu-id="10322-889">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="10322-890">AKS</span><span class="sxs-lookup"><span data-stu-id="10322-890">AKS</span></span>

* <span data-ttu-id="10322-891">Alteração do valor padrão `--load-balancer-sku` para `standard` se for compatível com a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="10322-891">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="10322-892">Alteração do valor padrão `--vm-set-type` para `virtualmachinescalesets` se for compatível com a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="10322-892">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="10322-893">AMS</span><span class="sxs-lookup"><span data-stu-id="10322-893">AMS</span></span>

* <span data-ttu-id="10322-894">[ALTERAÇÃO SIGNIFICATIVA] Alteração do nome de `job start` para `job create`</span><span class="sxs-lookup"><span data-stu-id="10322-894">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="10322-895">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--ask` de `content-key-policy create` para usar uma cadeia de 32 caracteres hexadecimais em vez do UTF8</span><span class="sxs-lookup"><span data-stu-id="10322-895">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-896">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-896">AppService</span></span>

* <span data-ttu-id="10322-897">Adição dos comandos `webapp config access-restriction show|set|add|remove`</span><span class="sxs-lookup"><span data-stu-id="10322-897">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="10322-898">Adição de um melhor tratamento de erro a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="10322-898">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="10322-899">Adição de suporte do SKU `Isolated` para `appservice plan update`</span><span class="sxs-lookup"><span data-stu-id="10322-899">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="10322-900">ARM</span><span class="sxs-lookup"><span data-stu-id="10322-900">ARM</span></span>

* <span data-ttu-id="10322-901">Adição do parâmetro `--handle-extended-json-format``deployment create` para dar suporte a várias linhas e a comentários no modelo json</span><span class="sxs-lookup"><span data-stu-id="10322-901">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="10322-902">Computação</span><span class="sxs-lookup"><span data-stu-id="10322-902">Compute</span></span>

* <span data-ttu-id="10322-903">Parâmetro `--enable-agent` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="10322-903">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="10322-904">Alteração de `vm create` para usar um SKU de IP público padrão automaticamente ao usar zonas</span><span class="sxs-lookup"><span data-stu-id="10322-904">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="10322-905">Alteração de `vm create` para criar automaticamente um nome de computador válido para uma VM, caso nenhum tenha sido fornecido</span><span class="sxs-lookup"><span data-stu-id="10322-905">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="10322-906">Adição do parâmetro `--computer-name-prefix` a `vmss create` para dar suporte ao prefixo de nome de computador personalizado de máquinas virtuais no VMSS</span><span class="sxs-lookup"><span data-stu-id="10322-906">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="10322-907">Adicione o parâmetro `--workspace` a `vm create` para habilitar o workspace de análise de logs automaticamente</span><span class="sxs-lookup"><span data-stu-id="10322-907">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="10322-908">Versão de API de galerias atualizadas para 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="10322-908">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="10322-909">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-909">Core</span></span>

* <span data-ttu-id="10322-910">Adição da verificação de sintaxe para o parâmetro `--set` no comando de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="10322-910">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="10322-911">IoT</span><span class="sxs-lookup"><span data-stu-id="10322-911">IoT</span></span>

* <span data-ttu-id="10322-912">Correção de um problema em que o `iot hub show` retornaria incorretamente um erro com "recurso não encontrado"</span><span class="sxs-lookup"><span data-stu-id="10322-912">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-913">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-913">Monitor</span></span>

* <span data-ttu-id="10322-914">Adição de suporte para CRUD a `monitor log-analytics workspace`</span><span class="sxs-lookup"><span data-stu-id="10322-914">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="10322-915">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-915">Network</span></span>

* <span data-ttu-id="10322-916">Adição de suporte para vinculação virtual entre locatários para `network private-dns link vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-916">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="10322-917">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `network vnet subnet list` para exigir os parâmetros `--resource-group` e `--vnet-name`</span><span class="sxs-lookup"><span data-stu-id="10322-917">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="10322-918">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-918">SQL</span></span>

* <span data-ttu-id="10322-919">Adição de comandos a `sql mi ad-admin` que dão suporte à configuração de um administrador do AAD em instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="10322-919">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="10322-920">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-920">Storage</span></span>

* <span data-ttu-id="10322-921">Adição do parâmetro `--preserve-s2s-access-tier``storage copy` para preservar a camada de acesso durante a cópia do serviço para serviço</span><span class="sxs-lookup"><span data-stu-id="10322-921">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="10322-922">Adição do parâmetro `--enable-large-file-share` a `storage account [create|update]` para dar suporte a compartilhamentos de arquivos grandes para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-922">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="10322-923">24 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-923">September 24, 2019</span></span>

<span data-ttu-id="10322-924">Versão 2.0.74</span><span class="sxs-lookup"><span data-stu-id="10322-924">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="10322-925">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-925">ACR</span></span>

* <span data-ttu-id="10322-926">Inclusão de um parâmetro `--type` obrigatório em `acr config retention update`</span><span class="sxs-lookup"><span data-stu-id="10322-926">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="10322-927">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro renomeado `--name -n` foi alterado para `--registry -r ` para o grupo de comando `acr config`</span><span class="sxs-lookup"><span data-stu-id="10322-927">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="10322-928">AKS</span><span class="sxs-lookup"><span data-stu-id="10322-928">AKS</span></span>

* <span data-ttu-id="10322-929">Inclusão do parâmetro `--load-balancer-sku` no comando `aks create`, o que permite criar um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="10322-929">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="10322-930">Inclusão dos parâmetros `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` e `--load-balancer-outbound-ip-prefixes` nos comandos `aks [create|update]`, o que permite atualizar o perfil do balanceador de carga de um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="10322-930">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="10322-931">Inclusão do parâmetro `--vm-set-type` no comando `aks create`, o que permite especificar os tipos de VM de um cluster do AKS (vmas ou vmss)</span><span class="sxs-lookup"><span data-stu-id="10322-931">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="10322-932">ARM</span><span class="sxs-lookup"><span data-stu-id="10322-932">ARM</span></span>

* <span data-ttu-id="10322-933">Inclusão do parâmetro `--handle-extended-json-format` no comando `group deployment create` para compatibilidade com várias linhas e comentários no modelo JSON</span><span class="sxs-lookup"><span data-stu-id="10322-933">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="10322-934">Computação</span><span class="sxs-lookup"><span data-stu-id="10322-934">Compute</span></span>

* <span data-ttu-id="10322-935">Inclusão do parâmetro `--terminate-notification-time` nos comandos `vmss [create|update]` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="10322-935">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="10322-936">Inclusão do parâmetro `--enable-terminate-notification` no comando `vmss update` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="10322-936">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="10322-937">Inclusão dos parâmetros `--priority,`, `--eviction-policy,` e `--max-billing` nos comandos `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="10322-937">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="10322-938">Alteração de `disk create` para permitir a especificação do tamanho exato do carregamento de disco</span><span class="sxs-lookup"><span data-stu-id="10322-938">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="10322-939">Inclusão de compatibilidade com instantâneos incrementais para discos gerenciados para `snapshot create`</span><span class="sxs-lookup"><span data-stu-id="10322-939">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="10322-940">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="10322-940">Cosmos DB</span></span>

* <span data-ttu-id="10322-941">Inclusão do parâmetro `--type <key-type>` no comando `cosmosdb keys list` para mostrar a chave, as chaves somente leitura ou cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="10322-941">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="10322-942">Adicionado o comando `cosmosdb keys regenerate`</span><span class="sxs-lookup"><span data-stu-id="10322-942">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="10322-943">[PRETERIDO] Comandos `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` e `cosmosdb list-read-only-keys` preteridos</span><span class="sxs-lookup"><span data-stu-id="10322-943">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="10322-944">EventGrid</span><span class="sxs-lookup"><span data-stu-id="10322-944">EventGrid</span></span>

* <span data-ttu-id="10322-945">Correção do texto de ajuda do ponto de extremidade para fazer referência ao parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="10322-945">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="10322-946">Key Vault</span><span class="sxs-lookup"><span data-stu-id="10322-946">Key Vault</span></span>

* <span data-ttu-id="10322-947">Correção do problema em que fazer logon com um locatário (`login -t`) poderia causar uma falha no `keyvault create`</span><span class="sxs-lookup"><span data-stu-id="10322-947">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-948">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-948">Monitor</span></span>

* <span data-ttu-id="10322-949">Correção do problema em que o caractere `:` não era permitido no argumento `--condition` para `monitor metrics alert create`</span><span class="sxs-lookup"><span data-stu-id="10322-949">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="10322-950">Política</span><span class="sxs-lookup"><span data-stu-id="10322-950">Policy</span></span>

* <span data-ttu-id="10322-951">Inclusão de compatibilidade com a API de Política, versão de 01/06/2019</span><span class="sxs-lookup"><span data-stu-id="10322-951">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="10322-952">Inclusão do parâmetro `--enforcement-mode` no comando `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="10322-952">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="10322-953">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-953">Storage</span></span>

* <span data-ttu-id="10322-954">Inclusão do parâmetro `--blob-type` no comando `az storage copy`</span><span class="sxs-lookup"><span data-stu-id="10322-954">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="10322-955">10 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-955">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="10322-956">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-956">ACR</span></span>

* <span data-ttu-id="10322-957">Adição do grupo de comandos `acr config retention` para configurar a política de retenção</span><span class="sxs-lookup"><span data-stu-id="10322-957">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="10322-958">AKS</span><span class="sxs-lookup"><span data-stu-id="10322-958">AKS</span></span>

* <span data-ttu-id="10322-959">Adição de suporte para integração do ACR com os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="10322-959">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="10322-960">Adição do parâmetro `--attach-acr` a `aks [create|update]` para anexar um ACR a um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="10322-960">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="10322-961">Adição do parâmetro `--detach-acr` a `aks update` para desanexar o ACR de um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="10322-961">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="10322-962">ARM</span><span class="sxs-lookup"><span data-stu-id="10322-962">ARM</span></span>

* <span data-ttu-id="10322-963">Atualização para uso da versão de API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="10322-963">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="10322-964">Lote</span><span class="sxs-lookup"><span data-stu-id="10322-964">Batch</span></span>

* <span data-ttu-id="10322-965">Adição de novas definições de configuração JSON de `--json-file` para `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="10322-965">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="10322-966">Adição de `MountConfigurations` para montagens do sistema de arquivos (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="10322-966">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="10322-967">Adição da propriedade opcional `publicIPs` a `NetworkConfiguration` para IPs públicos em pools (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="10322-967">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="10322-968">Adição de suporte para galerias de imagens compartilhadas a `--image`</span><span class="sxs-lookup"><span data-stu-id="10322-968">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="10322-969">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `--start-task-wait-for-success` em `batch pool create` para `true`</span><span class="sxs-lookup"><span data-stu-id="10322-969">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="10322-970">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `Scope` em `AutoUserSpecification` para sempre ser Pool (anteriormente, `Task` em nós do Windows e `Pool` em nós do Linux)</span><span class="sxs-lookup"><span data-stu-id="10322-970">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="10322-971">Esse argumento só pode ser definido em uma configuração JSON com `--json-file`</span><span class="sxs-lookup"><span data-stu-id="10322-971">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="10322-972">HDInsight</span><span class="sxs-lookup"><span data-stu-id="10322-972">HDInsight</span></span>

* <span data-ttu-id="10322-973">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="10322-973">GA release</span></span>
* <span data-ttu-id="10322-974">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--workernode-count/-c` de `az hdinsight resize` para ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10322-974">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="10322-975">Key Vault</span><span class="sxs-lookup"><span data-stu-id="10322-975">Key Vault</span></span>

* <span data-ttu-id="10322-976">Correção do problema em que as sub-redes não podiam ser excluídas das regras da rede</span><span class="sxs-lookup"><span data-stu-id="10322-976">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="10322-977">Correção do problema em que sub-redes e endereços IP duplicados podiam ser adicionados às regras da rede</span><span class="sxs-lookup"><span data-stu-id="10322-977">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="10322-978">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-978">Network</span></span>

* <span data-ttu-id="10322-979">Adição do parâmetro `--interval` a `network watcher flow-log` para definir o valor do intervalo de análise de tráfego</span><span class="sxs-lookup"><span data-stu-id="10322-979">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="10322-980">Adição de `network application-gateway identity` para gerenciar a identidade do gateway</span><span class="sxs-lookup"><span data-stu-id="10322-980">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="10322-981">Adição de suporte para definir a ID do Key Vault como `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="10322-981">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="10322-982">Adicionado `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="10322-982">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="10322-983">Política</span><span class="sxs-lookup"><span data-stu-id="10322-983">Policy</span></span>

* <span data-ttu-id="10322-984">Atualização para uso da versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="10322-984">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="10322-985">27 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-985">August 27, 2019</span></span>

<span data-ttu-id="10322-986">Versão 2.0.72</span><span class="sxs-lookup"><span data-stu-id="10322-986">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="10322-987">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-987">ACR</span></span>

* <span data-ttu-id="10322-988">[ALTERAÇÃO SIGNIFICATIVA] Remoção da compatibilidade com o SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="10322-988">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="10322-989">Gerenciamento de API</span><span class="sxs-lookup"><span data-stu-id="10322-989">API Management</span></span>

* <span data-ttu-id="10322-990">[VERSÃO PRÉVIA] Adição do grupo de comandos `apim`</span><span class="sxs-lookup"><span data-stu-id="10322-990">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-991">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-991">AppService</span></span>

* <span data-ttu-id="10322-992">Correção do problema com o comando `webapp webjob continuous start` ao especificar um slot</span><span class="sxs-lookup"><span data-stu-id="10322-992">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="10322-993">Alteração de `webapp up` para detectar a pasta `env` e removê-la do arquivo usado para implantação</span><span class="sxs-lookup"><span data-stu-id="10322-993">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="10322-994">Keyvault</span><span class="sxs-lookup"><span data-stu-id="10322-994">Keyvault</span></span>

* <span data-ttu-id="10322-995">Correção de um bug no `keyvault secret set` que ignorava o argumento `--expires`</span><span class="sxs-lookup"><span data-stu-id="10322-995">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="10322-996">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-996">Network</span></span>

* <span data-ttu-id="10322-997">Adição de suporte para endereços IPv6 a argumentos `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="10322-997">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="10322-998">Adição de novos comandos `network private-endpoint [create|update|list-types]` para o gerenciamento de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="10322-998">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="10322-999">Adição do grupo de comandos `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="10322-999">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="10322-1000">Adicionados os argumentos `--private-endpoint-network-policies` e `--private-link-service-network-policies` para `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="10322-1000">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="10322-1001">RBAC</span><span class="sxs-lookup"><span data-stu-id="10322-1001">RBAC</span></span>

* <span data-ttu-id="10322-1002">Correção de um problema com `ad app update --homepage` em que a página inicial não era atualizada</span><span class="sxs-lookup"><span data-stu-id="10322-1002">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="10322-1003">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="10322-1003">ServiceFabric</span></span>

* <span data-ttu-id="10322-1004">Adição de suporte para nomes de Key Vault grafados com maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="10322-1004">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="10322-1005">Correção de um problema ao usar certificados no Key Vault</span><span class="sxs-lookup"><span data-stu-id="10322-1005">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="10322-1006">Correção de um problema com o uso de arquivos de certificado PFX</span><span class="sxs-lookup"><span data-stu-id="10322-1006">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="10322-1007">Correção de um problema com `sf cluster certificate add` quando o grupo de recursos do Key Vault não era especificado</span><span class="sxs-lookup"><span data-stu-id="10322-1007">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="10322-1008">Correção de um problema em que `sf cluster set` não funcionava</span><span class="sxs-lookup"><span data-stu-id="10322-1008">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="10322-1009">SignalR</span><span class="sxs-lookup"><span data-stu-id="10322-1009">SignalR</span></span>

* <span data-ttu-id="10322-1010">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="10322-1010">Added new commands:</span></span>
  * <span data-ttu-id="10322-1011">`signalr cors`: gerenciar CORS do SignalR</span><span class="sxs-lookup"><span data-stu-id="10322-1011">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="10322-1012">`signalr restart`: reiniciar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="10322-1012">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="10322-1013">`signalr update`: atualizar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="10322-1013">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="10322-1014">Adicionado o argumento `--service-mode` para `signalr create`</span><span class="sxs-lookup"><span data-stu-id="10322-1014">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="10322-1015">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-1015">Storage</span></span>

* <span data-ttu-id="10322-1016">Adicionado o comando `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="10322-1016">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="10322-1017">13 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-1017">August 13, 2019</span></span>

<span data-ttu-id="10322-1018">Versão 2.0.71</span><span class="sxs-lookup"><span data-stu-id="10322-1018">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-1019">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-1019">AppService</span></span>

* <span data-ttu-id="10322-1020">Um problema de falha de slots com os comandos `webapp webjob continuous` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="10322-1020">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="10322-1021">BotService</span><span class="sxs-lookup"><span data-stu-id="10322-1021">BotService</span></span>

* <span data-ttu-id="10322-1022">[ALTERAÇÃO SIGNIFICATIVA] O suporte para a criação de bots SDK v3 foi removido</span><span class="sxs-lookup"><span data-stu-id="10322-1022">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="10322-1023">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="10322-1023">CognitiveServices</span></span>

* <span data-ttu-id="10322-1024">Adicionados os comandos `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="10322-1024">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="10322-1025">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="10322-1025">Cosmos DB</span></span>

* <span data-ttu-id="10322-1026">Removido o aviso ao atualizar vários locais de gravação</span><span class="sxs-lookup"><span data-stu-id="10322-1026">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="10322-1027">Foram adicionados os comandos CRUD para o CosmosDB SQL, MongoDB, Cassandra, Gremlin e Recursos de tabela e taxa de transferência do recurso</span><span class="sxs-lookup"><span data-stu-id="10322-1027">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="10322-1028">HDInsight</span><span class="sxs-lookup"><span data-stu-id="10322-1028">HDInsight</span></span>

<span data-ttu-id="10322-1029">Esta versão contém um grande número de alterações da falha.</span><span class="sxs-lookup"><span data-stu-id="10322-1029">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="10322-1030">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="10322-1030">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="10322-1031">`--storage-default-container` renomeado para `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="10322-1031">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="10322-1032">`--storage-default-filesystem` renomeado para `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="10322-1032">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="10322-1033">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--name` de `application create` foi alterado para representar o nome do aplicativo em vez do nome do cluster</span><span class="sxs-lookup"><span data-stu-id="10322-1033">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="10322-1034">O argumento `--cluster-name` foi adicionado a `application create` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="10322-1034">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="10322-1035">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `application create`:</span><span class="sxs-lookup"><span data-stu-id="10322-1035">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="10322-1036">`--application-type` renomeado para `--type`</span><span class="sxs-lookup"><span data-stu-id="10322-1036">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="10322-1037">`--marketplace-identifier` renomeado para `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="10322-1037">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="10322-1038">`--https-endpoint-access-mode` renomeado para `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="10322-1038">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="10322-1039">Renomeado de `--https-endpoint-destination-port` para `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="10322-1039">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="10322-1040">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros removidos para `application create`:</span><span class="sxs-lookup"><span data-stu-id="10322-1040">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="10322-1041">[ALTERAÇÃO DA FALHA] Renomeado de `--target-instance-count` para `--workernode-count` para `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="10322-1041">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="10322-1042">[ALTERAÇÃO SIGNIFICATIVA] Todos os comandos no grupo `hdinsight script-action` foram alterados para usar o parâmetro `--name` como o nome da ação de script.</span><span class="sxs-lookup"><span data-stu-id="10322-1042">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="10322-1043">O argumento `--cluster-name` foi adicionado a todos os comandos `hdinsight script-action` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="10322-1043">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="10322-1044">[ALTERAÇÃO SIGNIFICATIVA] Renomeado de `--script-execution-id` para `--execution-id` para todos os comandos `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="10322-1044">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="10322-1045">[ALTERAÇÃO SIGNIFICATIVA]`hdinsight script-action show` renomeado para `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="10322-1045">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="10322-1046">[ALTERAÇÃO DA FALHA] Os parâmetros foram alterados para `hdinsight script-action execute --roles` para serem separados por espaços em vez de separados por vírgula</span><span class="sxs-lookup"><span data-stu-id="10322-1046">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="10322-1047">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro `--persisted` de `hdinsight script-action list` foi removido</span><span class="sxs-lookup"><span data-stu-id="10322-1047">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="10322-1048">O parâmetro `hdinsight create --cluster-configurations` foi alterado para aceitar um caminho para um arquivo JSON local ou uma cadeia de caracteres JSON</span><span class="sxs-lookup"><span data-stu-id="10322-1048">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="10322-1049">Adicionado o comando `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="10322-1049">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="10322-1050">Alterado `hdinsight monitor enable --workspace` para aceitar uma ID do workspace ou nome do workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="10322-1050">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="10322-1051">O argumento `hdinsight monitor enable --primary-key`, que será necessário caso uma ID do workspace seja fornecida como o parâmetro, foi adicionado</span><span class="sxs-lookup"><span data-stu-id="10322-1051">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="10322-1052">Foram adicionados mais exemplos e atualização das descrições das mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="10322-1052">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="10322-1053">Interativo</span><span class="sxs-lookup"><span data-stu-id="10322-1053">Interactive</span></span>

* <span data-ttu-id="10322-1054">Um erro no carregamento foi corrigido</span><span class="sxs-lookup"><span data-stu-id="10322-1054">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="10322-1055">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="10322-1055">Kubernetes</span></span>

* <span data-ttu-id="10322-1056">Alterado para usar `https` se a porta do contêiner do painel estiver usando `https`</span><span class="sxs-lookup"><span data-stu-id="10322-1056">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="10322-1057">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-1057">Network</span></span>

* <span data-ttu-id="10322-1058">O argumento `--yes` foi adicionado a `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="10322-1058">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="10322-1059">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-1059">Profile</span></span>

* <span data-ttu-id="10322-1060">O argumento `--resource-type` foi adicionado a `account get-access-token` para obter tokens de acesso de recurso</span><span class="sxs-lookup"><span data-stu-id="10322-1060">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="10322-1061">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="10322-1061">ServiceFabric</span></span>

* <span data-ttu-id="10322-1062">Todas as versões de sistema operacional com suporte para criação do cluster sf foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="10322-1062">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="10322-1063">Foi corrigido o bug de validação do certificado primário</span><span class="sxs-lookup"><span data-stu-id="10322-1063">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="10322-1064">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-1064">Storage</span></span>

* <span data-ttu-id="10322-1065">Adicionado o comando `storage copy`</span><span class="sxs-lookup"><span data-stu-id="10322-1065">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="10322-1066">30 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-1066">July 30, 2019</span></span>

<span data-ttu-id="10322-1067">Versão 2.0.70</span><span class="sxs-lookup"><span data-stu-id="10322-1067">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="10322-1068">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-1068">ACR</span></span>

* <span data-ttu-id="10322-1069">Corrigido o problema #9952 (uma regressão no comando `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="10322-1069">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="10322-1070">Removido o nome da imagem do construtor padrão em `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="10322-1070">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-1071">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-1071">Appservice</span></span>

* <span data-ttu-id="10322-1072">Alterado `webapp config ssl` para mostrar uma mensagem se um recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="10322-1072">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="10322-1073">Corrigido o problema em que `functionapp create` não aceita o tipo de conta de armazenamento `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="10322-1073">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="10322-1074">Corrigido um problema em que `webapp up` falharia se fosse executado usando versões mais antigas do Python</span><span class="sxs-lookup"><span data-stu-id="10322-1074">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="10322-1075">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-1075">Network</span></span>

* <span data-ttu-id="10322-1076">Removido parâmetro inválido `--ids` de `network nic ip-config add` (corrige o #9861)</span><span class="sxs-lookup"><span data-stu-id="10322-1076">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="10322-1077">Corrige o #9604.</span><span class="sxs-lookup"><span data-stu-id="10322-1077">Fixes #9604.</span></span> <span data-ttu-id="10322-1078">Adicionado o parâmetro `--root-certs` ao `network application-gateway http-settings [create|update]` para dar suporte a certificados raiz confiáveis associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="10322-1078">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="10322-1079">Fixado argumento `--subscription` para `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="10322-1079">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="10322-1080">RBAC</span><span class="sxs-lookup"><span data-stu-id="10322-1080">RBAC</span></span>

* <span data-ttu-id="10322-1081">Adicionado o comando `user update`</span><span class="sxs-lookup"><span data-stu-id="10322-1081">Added `user update` command</span></span>
* <span data-ttu-id="10322-1082">[PRETERIDO] Preterido `--upn-or-object-id` de comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="10322-1082">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="10322-1083">Usar argumento de substituição `--id`</span><span class="sxs-lookup"><span data-stu-id="10322-1083">Use replacement argument `--id`</span></span>
* <span data-ttu-id="10322-1084">Adicionado argumento `--id` para comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="10322-1084">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="10322-1085">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-1085">SQL</span></span>

* <span data-ttu-id="10322-1086">Adicionados comandos de gerenciamento para chaves de instância gerenciada e protetor de TDE</span><span class="sxs-lookup"><span data-stu-id="10322-1086">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="10322-1087">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-1087">Storage</span></span>

* <span data-ttu-id="10322-1088">Adicionado o comando `storage remove`</span><span class="sxs-lookup"><span data-stu-id="10322-1088">Added `storage remove` command</span></span>
* <span data-ttu-id="10322-1089">Corrigido um problema com `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="10322-1089">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="10322-1090">VM</span><span class="sxs-lookup"><span data-stu-id="10322-1090">VM</span></span>

* <span data-ttu-id="10322-1091">Alterado `list-skus` para usar versão de API mais recente a fim de externar detalhes de zona</span><span class="sxs-lookup"><span data-stu-id="10322-1091">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="10322-1092">Alterado o padrão de `--single-placement-group` para `false` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="10322-1092">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="10322-1093">Adicionada a capacidade de selecionar SKUs de armazenamento ZRS para `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="10322-1093">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="10322-1094">Adicionado novo grupo de comandos `vm host` para dar suporte a hosts dedicados</span><span class="sxs-lookup"><span data-stu-id="10322-1094">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="10322-1095">Adicionados parâmetros `--host` e `--host-group` em `vm create` para definir o host dedicado da VM</span><span class="sxs-lookup"><span data-stu-id="10322-1095">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="10322-1096">16 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-1096">July 16, 2019</span></span>

<span data-ttu-id="10322-1097">Versão 2.0.69</span><span class="sxs-lookup"><span data-stu-id="10322-1097">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-1098">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-1098">Appservice</span></span>

* <span data-ttu-id="10322-1099">Os comandos `webapp identity` foram alterados para retornar uma mensagem de erro apropriada se o nome do aplicativo ou ResourceGroupName for inválido</span><span class="sxs-lookup"><span data-stu-id="10322-1099">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="10322-1100">`webapp list` corrigido para retornar o valor correto para numberOfSites se nenhum ResourceGroup foi fornecido</span><span class="sxs-lookup"><span data-stu-id="10322-1100">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="10322-1101">Corrigidos os efeitos colaterais de `appservice plan create` e `webapp create`</span><span class="sxs-lookup"><span data-stu-id="10322-1101">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="10322-1102">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-1102">Core</span></span>

* <span data-ttu-id="10322-1103">Corrigido um problema em que `--subscription` aparecia apesar de não ser aplicável</span><span class="sxs-lookup"><span data-stu-id="10322-1103">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="10322-1104">Lote</span><span class="sxs-lookup"><span data-stu-id="10322-1104">Batch</span></span>

* <span data-ttu-id="10322-1105">[ALTERAÇÃO SIGNIFICATIVA]`batch pool node-agent-skus list` foi substituído por `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="10322-1105">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="10322-1106">Adicionado suporte para regras de segurança bloqueando o acesso de rede a um pool com base na porta de origem do tráfego ao usar a opção `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="10322-1106">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="10322-1107">Suporte adicionado para executar a tarefa no diretório de trabalho de contêiner ou no diretório de trabalho de tarefa em lotes ao usar a opção `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="10322-1107">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="10322-1108">Corrigido o erro na opção `--application-package-references` de `batch pool create` em que ela funcionaria apenas com padrões</span><span class="sxs-lookup"><span data-stu-id="10322-1108">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="10322-1109">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="10322-1109">Eventhubs</span></span>

* <span data-ttu-id="10322-1110">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="10322-1110">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="10322-1111">RDBMS</span><span class="sxs-lookup"><span data-stu-id="10322-1111">RDBMS</span></span>

* <span data-ttu-id="10322-1112">Adicionado um parâmetro opcional para especificar a réplica de SKU para criar o comando de réplica</span><span class="sxs-lookup"><span data-stu-id="10322-1112">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="10322-1113">Corrigido o problema com a falha no teste de CI com a criação de réplica de MySQL</span><span class="sxs-lookup"><span data-stu-id="10322-1113">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="10322-1114">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="10322-1114">Relay</span></span>

* <span data-ttu-id="10322-1115">Corrigido o problema com a conexão híbrida quando a autorização do cliente desabilitava [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="10322-1115">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="10322-1116">Parâmetro `--requires-transport-security` adicionado a `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="10322-1116">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="10322-1117">Barramento de serviço</span><span class="sxs-lookup"><span data-stu-id="10322-1117">Servicebus</span></span>

* <span data-ttu-id="10322-1118">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="10322-1118">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="10322-1119">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-1119">Storage</span></span>

* <span data-ttu-id="10322-1120">Habilitar AADDS de arquivos para atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-1120">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="10322-1121">Problema corrigido `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="10322-1121">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="10322-1122">2 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-1122">July 2, 2019</span></span>

<span data-ttu-id="10322-1123">Versão 2.0.68</span><span class="sxs-lookup"><span data-stu-id="10322-1123">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="10322-1124">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-1124">Core</span></span>

* <span data-ttu-id="10322-1125">Agora, os módulos de comando são consolidados em um único Python distribuível.</span><span class="sxs-lookup"><span data-stu-id="10322-1125">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="10322-1126">Isso substitui o uso direto de muitos pacotes `azure-cli-` no PyPI.</span><span class="sxs-lookup"><span data-stu-id="10322-1126">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="10322-1127">Assim, o tamanho da instalação será reduzido e apenas os usuários que tiverem instalado diretamente por meio do `pip` serão afetados.</span><span class="sxs-lookup"><span data-stu-id="10322-1127">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="10322-1128">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-1128">ACR</span></span>

* <span data-ttu-id="10322-1129">Foi adicionado o suporte para gatilhos de temporizador para tarefa</span><span class="sxs-lookup"><span data-stu-id="10322-1129">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-1130">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-1130">Appservice</span></span>

* <span data-ttu-id="10322-1131">O `functionapp create` foi alterado para habilitar o Application Insights por padrão</span><span class="sxs-lookup"><span data-stu-id="10322-1131">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="10322-1132">[ALTERAÇÃO SIGNIFICATIVA] Foi removido o comando `functionapp devops-build` preterido.</span><span class="sxs-lookup"><span data-stu-id="10322-1132">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="10322-1133">Agora, use o novo comando `az functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="10322-1133">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="10322-1134">Foi adicionado o suporte ao plano de aplicativo de funções Consumo em Linux ao `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="10322-1134">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="10322-1135">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="10322-1135">Cosmos DB</span></span>

* <span data-ttu-id="10322-1136">Foi adicionado o suporte para desabilitar a TTL</span><span class="sxs-lookup"><span data-stu-id="10322-1136">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="10322-1137">DLS</span><span class="sxs-lookup"><span data-stu-id="10322-1137">DLS</span></span>

* <span data-ttu-id="10322-1138">Versão atualizada do ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="10322-1138">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="10322-1139">Comentários</span><span class="sxs-lookup"><span data-stu-id="10322-1139">Feedback</span></span>

* <span data-ttu-id="10322-1140">Ao relatar um comando de extensão com falha, agora, o `az feedback` tenta abrir o navegador na URL do projeto/repositório da extensão por meio do índice</span><span class="sxs-lookup"><span data-stu-id="10322-1140">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="10322-1141">HDInsight</span><span class="sxs-lookup"><span data-stu-id="10322-1141">HDInsight</span></span>

* <span data-ttu-id="10322-1142">[ALTERAÇÃO SIGNIFICATIVA] O nome do grupo de comandos `oms` foi alterado para `monitor`</span><span class="sxs-lookup"><span data-stu-id="10322-1142">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="10322-1143">[ALTERAÇÃO SIGNIFICATIVA]`--http-password/-p` tornou-se um parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="10322-1143">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="10322-1144">Foram adicionados preenchedores para o preenchedor dos parâmetros `--cluster-admin-account` e `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="10322-1144">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="10322-1145">O parâmetro `cluster-users-group-dns` foi alterado para ser obrigatório quando `—esp` estiver presente</span><span class="sxs-lookup"><span data-stu-id="10322-1145">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="10322-1146">Foi adicionado um tempo limite para todos os preenchedores automáticos de argumento existentes</span><span class="sxs-lookup"><span data-stu-id="10322-1146">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="10322-1147">Foi adicionado um tempo limite para transformar o nome do recurso na ID de recurso</span><span class="sxs-lookup"><span data-stu-id="10322-1147">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="10322-1148">Os preenchedores automáticos foram alterados para selecionar recursos de qualquer grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="10322-1148">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="10322-1149">Pode ser um grupo de recursos diferente daquele especificado com `-g`</span><span class="sxs-lookup"><span data-stu-id="10322-1149">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="10322-1150">Foi adicionado o suporte para os parâmetros `--sub-domain-suffix` e `--disable_gateway_auth` no comando `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="10322-1150">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="10322-1151">Serviços gerenciados</span><span class="sxs-lookup"><span data-stu-id="10322-1151">Managed Services</span></span>

* <span data-ttu-id="10322-1152">Introdução ao módulo de comando de serviço gerenciado em versão prévia</span><span class="sxs-lookup"><span data-stu-id="10322-1152">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="10322-1153">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-1153">Profile</span></span>
* <span data-ttu-id="10322-1154">Suprimir o argumento `--subscription` para o comando de logoff</span><span class="sxs-lookup"><span data-stu-id="10322-1154">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="10322-1155">RBAC</span><span class="sxs-lookup"><span data-stu-id="10322-1155">RBAC</span></span>

* <span data-ttu-id="10322-1156">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--password` foi removido de `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="10322-1156">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="10322-1157">Foi adicionado o parâmetro `--assignee-principal-type` ao comando `create` para evitar falhas intermitentes causadas pela latência de replicação do servidor do AAD Graph</span><span class="sxs-lookup"><span data-stu-id="10322-1157">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="10322-1158">Foi corrigida uma falha em `ad signed-in-user` ao listar objetos de propriedade</span><span class="sxs-lookup"><span data-stu-id="10322-1158">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="10322-1159">Foi corrigido um problema em que o `ad sp` não localizava o aplicativo certo de uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="10322-1159">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="10322-1160">RDBMS</span><span class="sxs-lookup"><span data-stu-id="10322-1160">RDBMS</span></span>

* <span data-ttu-id="10322-1161">Foi adicionado o suporte à replicação para o MariaDB</span><span class="sxs-lookup"><span data-stu-id="10322-1161">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="10322-1162">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-1162">SQL</span></span>

* <span data-ttu-id="10322-1163">Valores permitidos documentados para `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="10322-1163">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="10322-1164">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-1164">Storage</span></span>

* <span data-ttu-id="10322-1165">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="10322-1165">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="10322-1166">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="10322-1166">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="10322-1167">VM</span><span class="sxs-lookup"><span data-stu-id="10322-1167">VM</span></span>

* <span data-ttu-id="10322-1168">Foi corrigido o bug em que o `vmss create` retornava uma mensagem de erro quando era executado com `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="10322-1168">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="10322-1169">Foi removida a validação do lado do cliente de `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="10322-1169">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="10322-1170">Não falha quando `--single-placement-group` é definido como `true` e `--instance-count` é maior que 100 ou quando são especificadas zonas de disponibilidade, mas deixa essa validação para o serviço de computação</span><span class="sxs-lookup"><span data-stu-id="10322-1170">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="10322-1171">Foi corrigido o bug em que o `[vm|vmss] extension image list` falhava quando era usado com `--latest`</span><span class="sxs-lookup"><span data-stu-id="10322-1171">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="10322-1172">18 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-1172">June 18, 2019</span></span>

<span data-ttu-id="10322-1173">Versão 2.0.67</span><span class="sxs-lookup"><span data-stu-id="10322-1173">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="10322-1174">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-1174">Core</span></span>

<span data-ttu-id="10322-1175">Esta versão apresenta uma nova marca [Versão prévia] para comunicar com mais clareza aos clientes quando um comando, um grupo de comandos ou um argumento está no status de versão prévia.</span><span class="sxs-lookup"><span data-stu-id="10322-1175">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="10322-1176">Anteriormente, essa informação era transmitida no texto de ajuda ou, implicitamente, pelo número da versão do módulo de comando.</span><span class="sxs-lookup"><span data-stu-id="10322-1176">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="10322-1177">A CLI removerá os números de versão dos pacotes individuais no futuro.</span><span class="sxs-lookup"><span data-stu-id="10322-1177">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="10322-1178">Se um comando estiver em versão prévia, todos os seus argumentos também estarão.</span><span class="sxs-lookup"><span data-stu-id="10322-1178">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="10322-1179">Se um grupo de comandos for rotulado com o status de versão prévia, então todos os seus comandos e argumentos também serão considerados em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="10322-1179">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="10322-1180">Como resultado dessa alteração, diversos grupos de comandos podem parecer surgir "de repente" com o status de versão prévia com esta liberação.</span><span class="sxs-lookup"><span data-stu-id="10322-1180">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="10322-1181">O que realmente aconteceu é que a maioria dos pacotes já estava com status de versão prévia, mas estão sendo consideradas GA com esta liberação</span><span class="sxs-lookup"><span data-stu-id="10322-1181">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="10322-1182">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-1182">ACR</span></span>
* <span data-ttu-id="10322-1183">Adicionado o comando 'acr check-health'</span><span class="sxs-lookup"><span data-stu-id="10322-1183">Added 'acr check-health' command</span></span>
* <span data-ttu-id="10322-1184">Melhorado o tratamento de erro para tokens do AAD e para recuperar comandos externos</span><span class="sxs-lookup"><span data-stu-id="10322-1184">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="10322-1185">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-1185">ACS</span></span>
* <span data-ttu-id="10322-1186">Comandos preteridos do ACS agora ficam ocultos da exibição da ajuda</span><span class="sxs-lookup"><span data-stu-id="10322-1186">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="10322-1187">AMS</span><span class="sxs-lookup"><span data-stu-id="10322-1187">AMS</span></span>
* <span data-ttu-id="10322-1188">[ALTERAÇÃO SIGNIFICATIVA] Alterada para retornar cadeias de caracteres de tempo da ISO 8601 para archive-window-length e key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="10322-1188">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-1189">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-1189">AppService</span></span>
* <span data-ttu-id="10322-1190">Adicionado roteamento com base no local para `webapp deleted list` e `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="10322-1190">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="10322-1191">Corrigido problema em que a URL de destino registrada do webapp ("Não é possível iniciar o aplicativo em...") não era clicável no Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="10322-1191">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="10322-1192">Corrigido um problema em que a criação de aplicativos com algumas SKUs falhava com um erro de AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="10322-1192">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="10322-1193">Adicionada a pré-validação para o `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="10322-1193">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="10322-1194">Corrigido o `[webapp|functionapp] traffic-routing` para usar o actionHostName correto</span><span class="sxs-lookup"><span data-stu-id="10322-1194">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="10322-1195">Adicionado o suporte de slot para comandos `functionapp`</span><span class="sxs-lookup"><span data-stu-id="10322-1195">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="10322-1196">Lote</span><span class="sxs-lookup"><span data-stu-id="10322-1196">Batch</span></span>
* <span data-ttu-id="10322-1197">Corrigida a regressão de autenticação do AAD causada pela geração de relatórios de erros superagressiva para autenticação de chave compartilhada</span><span class="sxs-lookup"><span data-stu-id="10322-1197">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="10322-1198">BatchAI</span><span class="sxs-lookup"><span data-stu-id="10322-1198">BatchAI</span></span>
* <span data-ttu-id="10322-1199">Agora os comandos do BatchAI estão preteridos e ocultos</span><span class="sxs-lookup"><span data-stu-id="10322-1199">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="10322-1200">BotService</span><span class="sxs-lookup"><span data-stu-id="10322-1200">BotService</span></span>
* <span data-ttu-id="10322-1201">Adição das mensagens de aviso "suporte descontinuado"/"modo de manutenção" para os comandos compatíveis com a v3 do SDK</span><span class="sxs-lookup"><span data-stu-id="10322-1201">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="10322-1202">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="10322-1202">CosmosDB</span></span>
* <span data-ttu-id="10322-1203">[PRETERIDO] Preterido o comando `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="10322-1203">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="10322-1204">Adicionado o comando `cosmosdb keys list` – substitui o `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="10322-1204">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="10322-1205">`cosmsodb create/update`: Adicionado novo formato para --location a fim de permitir a configuração da propriedade "isZoneRedundant".</span><span class="sxs-lookup"><span data-stu-id="10322-1205">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="10322-1206">Formato antigo preterido</span><span class="sxs-lookup"><span data-stu-id="10322-1206">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="10322-1207">EventGrid</span><span class="sxs-lookup"><span data-stu-id="10322-1207">EventGrid</span></span>
* <span data-ttu-id="10322-1208">Adicionados comandos do `eventgrid domain` para operações de CRUD no domínio</span><span class="sxs-lookup"><span data-stu-id="10322-1208">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="10322-1209">Adicionados comandos do `eventgrid domain topic` para operações de CRUD nos tópicos do domínio</span><span class="sxs-lookup"><span data-stu-id="10322-1209">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="10322-1210">Adicionado argumento do `--odata-query` ao `eventgrid [topic|event-subscription] list` para filtrar os resultados usando a sintaxe do OData</span><span class="sxs-lookup"><span data-stu-id="10322-1210">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="10322-1211">`event-subscription create/update`: Adicionado o servicebusqueue como novos valores para o parâmetro `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="10322-1211">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="10322-1212">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para `--included-event-types All` com `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1212">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="10322-1213">HDInsight</span><span class="sxs-lookup"><span data-stu-id="10322-1213">HDInsight</span></span>
* <span data-ttu-id="10322-1214">Adicionado suporte para o parâmetro `--ssh-public-key` no comando `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="10322-1214">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="10322-1215">IoT</span><span class="sxs-lookup"><span data-stu-id="10322-1215">IoT</span></span>
* <span data-ttu-id="10322-1216">Adicionado suporte para regenerar as chaves da política de autorização</span><span class="sxs-lookup"><span data-stu-id="10322-1216">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="10322-1217">Adicionados SDK e suporte para o serviço de provisionamento de repositórios do DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="10322-1217">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="10322-1218">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-1218">Network</span></span>
* <span data-ttu-id="10322-1219">Adicionado suporte de zona para o Gateway da NAT</span><span class="sxs-lookup"><span data-stu-id="10322-1219">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="10322-1220">Adicionado o comando `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="10322-1220">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="10322-1221">Corrigido o problema com o `dns zone import` em que os usuários não conseguiam importar registros do curinga A</span><span class="sxs-lookup"><span data-stu-id="10322-1221">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="10322-1222">Corrigido o problema com o `watcher flow-log configure` em que o registro de fluxo não podia ser habilitado em determinadas regiões</span><span class="sxs-lookup"><span data-stu-id="10322-1222">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="10322-1223">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-1223">Resource</span></span>
* <span data-ttu-id="10322-1224">Adicionado o comando do `az rest` para fazer chamadas REST</span><span class="sxs-lookup"><span data-stu-id="10322-1224">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="10322-1225">Corrigido o erro ao usar o `policy assignment list` com um grupo de recursos ou o nível de assinatura `--scope`</span><span class="sxs-lookup"><span data-stu-id="10322-1225">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="10322-1226">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="10322-1226">ServiceBus</span></span>
* <span data-ttu-id="10322-1227">Corrigido o problema com o `servicebus topic create --max-size`[nº9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="10322-1227">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="10322-1228">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-1228">SQL</span></span>
* <span data-ttu-id="10322-1229">Alterado o `--location` para ser opcional para `sql [server|mi] create` – usa o local do grupo de recursos se não especificado</span><span class="sxs-lookup"><span data-stu-id="10322-1229">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="10322-1230">Corrigido o erro "objeto 'NoneType' não é iterável" para `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="10322-1230">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="10322-1231">SQLVm</span><span class="sxs-lookup"><span data-stu-id="10322-1231">SQLVm</span></span>
* <span data-ttu-id="10322-1232">[ALTERAÇÃO DA FALHA] Alterado `sql vm create` para exigir o parâmetro `--license-type`</span><span class="sxs-lookup"><span data-stu-id="10322-1232">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="10322-1233">Alterado para permitir a configuração da SKU da imagem do SQL ao criar ou atualizar uma VM do SQL</span><span class="sxs-lookup"><span data-stu-id="10322-1233">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="10322-1234">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-1234">Storage</span></span>
* <span data-ttu-id="10322-1235">Corrigido o problema com a chave de conta ignorada para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="10322-1235">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="10322-1236">Corrigido o problema com o `storage blob sync` no Linux</span><span class="sxs-lookup"><span data-stu-id="10322-1236">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="10322-1237">VM</span><span class="sxs-lookup"><span data-stu-id="10322-1237">VM</span></span>
* <span data-ttu-id="10322-1238">[VERSÃO PRÉVIA] Adicionados os comandos `vm image template` para criar imagens de VM</span><span class="sxs-lookup"><span data-stu-id="10322-1238">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="10322-1239">4 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-1239">June 4, 2019</span></span>

<span data-ttu-id="10322-1240">Versão 2.0.66</span><span class="sxs-lookup"><span data-stu-id="10322-1240">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="10322-1241">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-1241">Core</span></span>
* <span data-ttu-id="10322-1242">Foi corrigido o bug em que os comandos falhavam quando `--output yaml` era usado com `--query`</span><span class="sxs-lookup"><span data-stu-id="10322-1242">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="10322-1243">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-1243">ACR</span></span>
* <span data-ttu-id="10322-1244">Foi adicionado o grupo de comando 'pack acr' para a criação de Tarefas de build rápida usando Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="10322-1244">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="10322-1245">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-1245">ACS</span></span>
* <span data-ttu-id="10322-1246">Permitir a opção de habilitar/desabilitar o complemento kube-dashboard do AKS</span><span class="sxs-lookup"><span data-stu-id="10322-1246">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="10322-1247">Imprimir uma mensagem amigável quando a assinatura não estiver na lista de permissões para usar o Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="10322-1247">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="10322-1248">Lote</span><span class="sxs-lookup"><span data-stu-id="10322-1248">Batch</span></span>
* <span data-ttu-id="10322-1249">Melhoria no tratamento de erro quando você não está conectado a uma conta \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="10322-1249">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="10322-1250">IoT</span><span class="sxs-lookup"><span data-stu-id="10322-1250">IoT</span></span>
* <span data-ttu-id="10322-1251">Foi adicionado o suporte para failover manual</span><span class="sxs-lookup"><span data-stu-id="10322-1251">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="10322-1252">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-1252">Network</span></span>
* <span data-ttu-id="10322-1253">Foram adicionados os comandos `network application-gateway waf-policy` para oferecer suporte às regras de WAF personalizadas.</span><span class="sxs-lookup"><span data-stu-id="10322-1253">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="10322-1254">Adicionados os argumentos `--waf-policy` e `--max-capacity` para `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1254">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="10322-1255">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-1255">Resource</span></span>
* <span data-ttu-id="10322-1256">Melhoria da mensagem de erro do `deployment create` quando não há nenhum TTY disponível</span><span class="sxs-lookup"><span data-stu-id="10322-1256">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="10322-1257">Função</span><span class="sxs-lookup"><span data-stu-id="10322-1257">Role</span></span>
* <span data-ttu-id="10322-1258">O texto da Ajuda foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="10322-1258">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="10322-1259">Computação</span><span class="sxs-lookup"><span data-stu-id="10322-1259">Compute</span></span>
* <span data-ttu-id="10322-1260">Foi adicionado o suporte para `vm create` para as VMs de uma imagem gerenciada com LUNs de disco de dados que não começam em 0 ou que ignoram números</span><span class="sxs-lookup"><span data-stu-id="10322-1260">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="10322-1261">21 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-1261">May 21, 2019</span></span>

<span data-ttu-id="10322-1262">Versão 2.0.65</span><span class="sxs-lookup"><span data-stu-id="10322-1262">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="10322-1263">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-1263">Core</span></span>
* <span data-ttu-id="10322-1264">Foram adicionados comentários melhores para erros de autenticação</span><span class="sxs-lookup"><span data-stu-id="10322-1264">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="10322-1265">Corrigido um problema em que a CLI carregava extensões que não eram compatíveis com a versão do núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-1265">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="10322-1266">Corrigido um problema com a inicialização quando `clouds.config` está corrompido</span><span class="sxs-lookup"><span data-stu-id="10322-1266">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="10322-1267">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-1267">ACR</span></span>
* <span data-ttu-id="10322-1268">Foi adicionado suporte das Identidades Gerenciadas para Tarefas</span><span class="sxs-lookup"><span data-stu-id="10322-1268">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="10322-1269">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-1269">ACS</span></span>
* <span data-ttu-id="10322-1270">Corrigido o comando `openshift create` quando usado com o cliente AAD do consumidor</span><span class="sxs-lookup"><span data-stu-id="10322-1270">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-1271">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-1271">AppService</span></span>
* <span data-ttu-id="10322-1272">[PRETERIDO] Preterido o comando `functionapp devops-build` – Será removido na próxima versão</span><span class="sxs-lookup"><span data-stu-id="10322-1272">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="10322-1273">`functionapp devops-pipeline` foi alterado para buscar o log de build do Azure DevOps no modo detalhado</span><span class="sxs-lookup"><span data-stu-id="10322-1273">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="10322-1274">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--use_local_settings` foi removido do comando `functionapp devops-pipeline` – não estava operacional</span><span class="sxs-lookup"><span data-stu-id="10322-1274">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="10322-1275">`webapp up` foi alterado para retornar uma saída JSON se `--logs` não for usado</span><span class="sxs-lookup"><span data-stu-id="10322-1275">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="10322-1276">Foi adicionado suporte para escrever recursos padrão para a configuração local de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="10322-1276">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="10322-1277">Foi adicionado suporte para `webapp up` reimplantar um aplicativo sem usar o argumento `--location`</span><span class="sxs-lookup"><span data-stu-id="10322-1277">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="10322-1278">Corrigido um problema em que o valor do SKU gratuito não funcionava na criação do ASP do SKU gratuito do Linux</span><span class="sxs-lookup"><span data-stu-id="10322-1278">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="10322-1279">BotService</span><span class="sxs-lookup"><span data-stu-id="10322-1279">BotService</span></span>
* <span data-ttu-id="10322-1280">Alterado para permitir todas as capitalizações para parâmetros `--lang` em todos os comandos</span><span class="sxs-lookup"><span data-stu-id="10322-1280">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="10322-1281">Descrição atualizada do módulo de comando</span><span class="sxs-lookup"><span data-stu-id="10322-1281">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="10322-1282">Consumo</span><span class="sxs-lookup"><span data-stu-id="10322-1282">Consumption</span></span>
* <span data-ttu-id="10322-1283">O parâmetro obrigatório ausente foi adicionado para executar `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="10322-1283">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="10322-1284">IoT</span><span class="sxs-lookup"><span data-stu-id="10322-1284">IoT</span></span>
* <span data-ttu-id="10322-1285">Suporte adicionado para listar todas as chaves</span><span class="sxs-lookup"><span data-stu-id="10322-1285">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="10322-1286">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-1286">Network</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="10322-1288">O argumento `--nat-gateway` foi adicionado a `network vnet subnet [create|update]` para anexar a um gateway NAT</span><span class="sxs-lookup"><span data-stu-id="10322-1288">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="10322-1289">Corrigido o problema de `dns zone import`, em que os nomes de registro não correspondiam ao tipo de registro</span><span class="sxs-lookup"><span data-stu-id="10322-1289">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="10322-1290">RDBMS</span><span class="sxs-lookup"><span data-stu-id="10322-1290">RDBMS</span></span>
* <span data-ttu-id="10322-1291">Suporte a postgres e mysql adicionado para replicação geográfica</span><span class="sxs-lookup"><span data-stu-id="10322-1291">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="10322-1292">RBAC</span><span class="sxs-lookup"><span data-stu-id="10322-1292">RBAC</span></span>
* <span data-ttu-id="10322-1293">Adição de suporte do escopo de grupo de gerenciamento a `role assignment`</span><span class="sxs-lookup"><span data-stu-id="10322-1293">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="10322-1294">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-1294">Storage</span></span>
* <span data-ttu-id="10322-1295">`storage blob sync`: adicionar um comando de sincronização ao armazenamento de blobs</span><span class="sxs-lookup"><span data-stu-id="10322-1295">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="10322-1296">Computação</span><span class="sxs-lookup"><span data-stu-id="10322-1296">Compute</span></span>
* <span data-ttu-id="10322-1297">`--computer-name` foi adicionado a `vm create` para configurar o nome do computador da VM</span><span class="sxs-lookup"><span data-stu-id="10322-1297">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="10322-1298">`--ssh-key-value` foi renomeado para `--ssh-key-values` para `[vm|vmss] create` – Agora, pode aceitar vários valores de chave pública ou caminhos ssh</span><span class="sxs-lookup"><span data-stu-id="10322-1298">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="10322-1299">__Observação__: Isso **não** é uma alteração da falha – `--ssh-key-value` será analisado corretamente, pois corresponde somente a `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="10322-1299">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="10322-1300">O argumento `--type` de `ppg create` foi alterado para ser opcional</span><span class="sxs-lookup"><span data-stu-id="10322-1300">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="10322-1301">6 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-1301">May 6, 2019</span></span>

<span data-ttu-id="10322-1302">Versão 2.0.64</span><span class="sxs-lookup"><span data-stu-id="10322-1302">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="10322-1303">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-1303">ACS</span></span>
* <span data-ttu-id="10322-1304">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--fqdn` foi removido dos comandos `openshift`</span><span class="sxs-lookup"><span data-stu-id="10322-1304">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="10322-1305">Alterado para usar a versão da API do Red Hat OpenShift no Azure em disponibilidade geral</span><span class="sxs-lookup"><span data-stu-id="10322-1305">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="10322-1306">O sinalizador `customer-admin-group-id` foi adicionado a `openshift create`</span><span class="sxs-lookup"><span data-stu-id="10322-1306">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="10322-1307">[GA] `(PREVIEW)` foi removido da opção `aks create``--network-policy`</span><span class="sxs-lookup"><span data-stu-id="10322-1307">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-1308">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-1308">Appservice</span></span>
* <span data-ttu-id="10322-1309">[PRETERIDO] O comando `functionapp devops-build` foi preterido</span><span class="sxs-lookup"><span data-stu-id="10322-1309">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="10322-1310">Renomeado para `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="10322-1310">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="10322-1311">Corrigido ao obter o nome de usuário correto para cloudshell que estava causando a falha em `webapp up`</span><span class="sxs-lookup"><span data-stu-id="10322-1311">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="10322-1312">Documentação `appservice plan --sku` atualizada para refletir o appserviceplans com suporte</span><span class="sxs-lookup"><span data-stu-id="10322-1312">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="10322-1313">Adicionado argumentos opcionais para o grupo de recursos e plano a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="10322-1313">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="10322-1314">Adicionado suporte a `webapp ssh` para respeitar a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="10322-1314">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="10322-1315">Adicionado suporte `appserviceplan create` para a SKU gratuita do Linux</span><span class="sxs-lookup"><span data-stu-id="10322-1315">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="10322-1316">Alterado `webapp up` para ter uma suspensão de 30 segundos depois de definir appsetting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` para lidar com a inicialização a frio kudu</span><span class="sxs-lookup"><span data-stu-id="10322-1316">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="10322-1317">Adicionado suporte para runtime `powershell` a `functionapp create` no Windows</span><span class="sxs-lookup"><span data-stu-id="10322-1317">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="10322-1318">Adicionado o comando `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="10322-1318">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="10322-1319">Lote</span><span class="sxs-lookup"><span data-stu-id="10322-1319">Batch</span></span>
* <span data-ttu-id="10322-1320">Corrigido o bug no validador para as opções `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="10322-1320">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="10322-1321">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="10322-1321">Botservice</span></span>
* <span data-ttu-id="10322-1322">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para criar um Bot de Aplicativo Web vazio por padrão (ou seja, nenhum bot será implantado no Serviço de Aplicativo)</span><span class="sxs-lookup"><span data-stu-id="10322-1322">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="10322-1323">O sinalizador `--echo` foi adicionado ao `bot create` para usar o comportamento antigo com `-v v4`</span><span class="sxs-lookup"><span data-stu-id="10322-1323">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="10322-1324">[ALTERAÇÃO SIGNIFICATIVA] O valor padrão de `--version` foi alterado para `v4`</span><span class="sxs-lookup"><span data-stu-id="10322-1324">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="10322-1325">__OBSERVAÇÃO:__ `bot prepare-publish` ainda usa o padrão antigo</span><span class="sxs-lookup"><span data-stu-id="10322-1325">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="10322-1326">[ALTERAÇÃO SIGNIFICATIVA]`--lang` foi alterado para não definir mais `Csharp` como padrão.</span><span class="sxs-lookup"><span data-stu-id="10322-1326">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="10322-1327">Se o comando exigir `--lang` e ele não for fornecido, o comando será um erro</span><span class="sxs-lookup"><span data-stu-id="10322-1327">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="10322-1328">[ALTERAÇÃO SIGNIFICATIVA] Os argumentos `--appid` e `--password` foram alterados para `bot create` ser obrigatório e agora podem ser criados por meio de `ad app create`</span><span class="sxs-lookup"><span data-stu-id="10322-1328">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="10322-1329">Foi adicionada validação a `--appid` e `--password`</span><span class="sxs-lookup"><span data-stu-id="10322-1329">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="10322-1330">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4` foi alterado para não criar ou usar uma Conta de Armazenamento ou o Application Insights</span><span class="sxs-lookup"><span data-stu-id="10322-1330">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="10322-1331">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v3` foi alterado para exigir uma região em que o Application Insights está disponível</span><span class="sxs-lookup"><span data-stu-id="10322-1331">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="10322-1332">[ALTERAÇÃO SIGNIFICATIVA] O `bot update` foi alterado para afetar somente as propriedades específicas de um bot</span><span class="sxs-lookup"><span data-stu-id="10322-1332">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="10322-1333">[ALTERAÇÃO SIGNIFICATIVA] Os sinalizadores `--lang` foram alterados para aceitar `Javascript` em vez de `Node`</span><span class="sxs-lookup"><span data-stu-id="10322-1333">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="10322-1334">[ALTERAÇÃO SIGNIFICATIVA] O `Node` foi removido como um valor `--lang` permitido</span><span class="sxs-lookup"><span data-stu-id="10322-1334">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="10322-1335">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para não definir mais `SCM_DO_BUILD_DURING_DEPLOYMENT` como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="10322-1335">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="10322-1336">Todas as implantações por meio do Kudu atuarão de acordo com o comportamento padrão</span><span class="sxs-lookup"><span data-stu-id="10322-1336">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="10322-1337">O `bot download` foi alterado para os bots sem arquivos `.bot` para criar o arquivo de configuração específico a um idioma com os valores das Configurações de Aplicativo do bot</span><span class="sxs-lookup"><span data-stu-id="10322-1337">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="10322-1338">Adicionado o suporte `Typescript` para `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="10322-1338">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="10322-1339">Uma mensagem de aviso foi adicionada a `bot prepare-deploy` para os bots `Javascript` e `Typescript` para quando `--code-dir` não contiver `package.json`</span><span class="sxs-lookup"><span data-stu-id="10322-1339">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="10322-1340">O `bot prepare-deploy` foi alterado para retornar `true`, se bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="10322-1340">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="10322-1341">O log detalhado foi adicionado a `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="10322-1341">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="10322-1342">Mais regiões disponíveis do Application Insights foram adicionadas ao `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="10322-1342">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="10322-1343">Configurar</span><span class="sxs-lookup"><span data-stu-id="10322-1343">Configure</span></span>
* <span data-ttu-id="10322-1344">Adicionado suporte para configurações de valor padrão do argumento baseado em pasta</span><span class="sxs-lookup"><span data-stu-id="10322-1344">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="10322-1345">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="10322-1345">Eventhubs</span></span>
* <span data-ttu-id="10322-1346">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="10322-1346">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="10322-1347">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1347">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="10322-1348">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-1348">Network</span></span>
* <span data-ttu-id="10322-1349">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--cache` foi substituído por `--defer` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1349">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="10322-1350">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="10322-1350">Policy Insights</span></span>
* <span data-ttu-id="10322-1351">Suporte adicionado a `--expand PolicyEvaluationDetails` para detalhes de avaliação de política de consulta no recurso</span><span class="sxs-lookup"><span data-stu-id="10322-1351">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="10322-1352">Função</span><span class="sxs-lookup"><span data-stu-id="10322-1352">Role</span></span>
* <span data-ttu-id="10322-1353">[PRETERIDO] Alterado argumento ocultar '--password' `create-for-rbac` - suporte será removido em maio de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-1353">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="10322-1354">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="10322-1354">Service Bus</span></span>
* <span data-ttu-id="10322-1355">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="10322-1355">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="10322-1356">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1356">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="10322-1357">`topic [create|update]` foi fixado para permitir suporte a `--max-size` para valores de 10, 20, 40 e 80 GB com a SKU Premium</span><span class="sxs-lookup"><span data-stu-id="10322-1357">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="10322-1358">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-1358">SQL</span></span>
* <span data-ttu-id="10322-1359">Adicionados os comandos `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="10322-1359">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="10322-1360">VM</span><span class="sxs-lookup"><span data-stu-id="10322-1360">VM</span></span>
* <span data-ttu-id="10322-1361">O `--protect-from-scale-in` e o `--protect-from-scale-set-actions` foram adicionados a `vmss update` para habilitar atualizações à política de proteção das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="10322-1361">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="10322-1362">Adicionado a `--instance-id` e `vmss update` para habilitar atualização genérica das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="10322-1362">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="10322-1363">`--instance-id` foi adicionado a `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="10322-1363">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="10322-1364">Adição do novo grupo de comandos `ppg` para gerenciar Grupos de Posicionamento de Proximidade</span><span class="sxs-lookup"><span data-stu-id="10322-1364">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="10322-1365">Adicionado a `--ppg`, `[vm|vmss] create` e `vm availability-set create` para gerenciar PPGs</span><span class="sxs-lookup"><span data-stu-id="10322-1365">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="10322-1366">Parâmetro `--hyper-v-generation` adicionado a `image create`</span><span class="sxs-lookup"><span data-stu-id="10322-1366">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="10322-1367">23 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-1367">April 23, 2019</span></span>

<span data-ttu-id="10322-1368">Versão 2.0.63</span><span class="sxs-lookup"><span data-stu-id="10322-1368">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="10322-1369">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-1369">ACS</span></span>
* <span data-ttu-id="10322-1370">Alterado `aks get-credentials` para solicitar substituição dos valores duplicados</span><span class="sxs-lookup"><span data-stu-id="10322-1370">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="10322-1371">Removido `(PREVIEW)` dos comandos de espaços de desenvolvimento "aks use-dev-espaces" e "aks remove-dev-espaces"</span><span class="sxs-lookup"><span data-stu-id="10322-1371">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="10322-1372">AMS</span><span class="sxs-lookup"><span data-stu-id="10322-1372">AMS</span></span>
* <span data-ttu-id="10322-1373">Corrigido o bug com a atualização de filtros de conta e de ativo</span><span class="sxs-lookup"><span data-stu-id="10322-1373">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-1374">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-1374">AppService</span></span>
* <span data-ttu-id="10322-1375">Adicionado suporte para o ASE e o tempo limite para `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="10322-1375">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="10322-1376">Adicionado suporte para o estabelecimento de CI CD em um pipeline do Azure DevOps de um repositório do Github para aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="10322-1376">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="10322-1377">Adicionado argumento `--github-pat` a `functionapp devops-build create` para aceitar o token de acesso pessoal do Github</span><span class="sxs-lookup"><span data-stu-id="10322-1377">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="10322-1378">Adicionado argumento `--github-repository` a `functionapp devops-build create` para aceitar o repositório Github que contém um código-fonte functionapp</span><span class="sxs-lookup"><span data-stu-id="10322-1378">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="10322-1379">Problema corrigido em que `az webapp up --logs` estava falhando com um erro e atualização da versão .NETCORE padrão para 2.1</span><span class="sxs-lookup"><span data-stu-id="10322-1379">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="10322-1380">Configurações de functionapp desnecessárias removidas durante a criação de um aplicativo de funções com plano de consumo</span><span class="sxs-lookup"><span data-stu-id="10322-1380">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="10322-1381">Alterado `webapp up` para que a cadeia de caracteres padrão asp agora acrescente o número no final para criar um novo ASP com base nas opções de SKU</span><span class="sxs-lookup"><span data-stu-id="10322-1381">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="10322-1382">Adicionado `-b` como uma opção a `webapp up` para iniciar o aplicativo no navegador</span><span class="sxs-lookup"><span data-stu-id="10322-1382">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="10322-1383">Alterado `webapp deployment source config zip` para lidar com a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="10322-1383">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="10322-1384">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="10322-1384">Deployment Manager</span></span>
* <span data-ttu-id="10322-1385">[VERSÃO PRÉVIA] Criar e gerenciar artefatos que dão suporte a distribuições</span><span class="sxs-lookup"><span data-stu-id="10322-1385">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="10322-1386">Laboratório</span><span class="sxs-lookup"><span data-stu-id="10322-1386">Lab</span></span>
* <span data-ttu-id="10322-1387">Corrigido o bug que causa uma saída inicial</span><span class="sxs-lookup"><span data-stu-id="10322-1387">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="10322-1388">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-1388">Network</span></span>
* <span data-ttu-id="10322-1389">Adicionada delegação de servidor de nome automática a `dns zone create` no pai durante a criação da zona filho</span><span class="sxs-lookup"><span data-stu-id="10322-1389">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="10322-1390">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-1390">Resource</span></span>
* <span data-ttu-id="10322-1391">[PRETERIDO] Argumentos `--link-id`, `--target-id` e `--filter-string` preteridos de `resource link`</span><span class="sxs-lookup"><span data-stu-id="10322-1391">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="10322-1392">Use os argumentos `--link`, `--target` e `--filter`</span><span class="sxs-lookup"><span data-stu-id="10322-1392">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="10322-1393">Corrigido o problema em que os comandos `resource link [create|update]` não funcionavam</span><span class="sxs-lookup"><span data-stu-id="10322-1393">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="10322-1394">Corrigido um problema em que a exclusão usando uma ID de recurso poderia causar falha no erro</span><span class="sxs-lookup"><span data-stu-id="10322-1394">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="10322-1395">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-1395">SQL</span></span>
* <span data-ttu-id="10322-1396">Adicionado suporte para fuso horário personalizado nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="10322-1396">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="10322-1397">Alterado para permitir que o nome do pool Elástico seja usado com `sql db update`</span><span class="sxs-lookup"><span data-stu-id="10322-1397">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="10322-1398">Adicionado o suporte `--no-wait` para `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1398">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="10322-1399">Adicionado o comando `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="10322-1399">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="10322-1400">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-1400">Storage</span></span>
* <span data-ttu-id="10322-1401">Corrigido o problema com tokens SAS com codificação dupla em `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="10322-1401">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="10322-1402">VM</span><span class="sxs-lookup"><span data-stu-id="10322-1402">VM</span></span>
* <span data-ttu-id="10322-1403">Adicionado sinalizador `--skip-shutdown` a `vm|vmss stop` para desligar as VMs sem o desligamento</span><span class="sxs-lookup"><span data-stu-id="10322-1403">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="10322-1404">Adicionado argumento `--storage-account-type` a `sig image-version create` para definir o tipo de conta do perfil de publicação</span><span class="sxs-lookup"><span data-stu-id="10322-1404">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="10322-1405">Adicionado argumento `--target-regions` a `sig image-version create` para permitir definir os tipos de conta de armazenamento específico da região</span><span class="sxs-lookup"><span data-stu-id="10322-1405">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="10322-1406">9 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-1406">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="10322-1407">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-1407">Core</span></span>
* <span data-ttu-id="10322-1408">Correção do problema em que algumas extensões mostraram uma versão do `Unknown` e não podiam ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="10322-1408">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="10322-1409">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-1409">ACR</span></span>
* <span data-ttu-id="10322-1410">Adição de suporte para execução de uma imagem sem contexto</span><span class="sxs-lookup"><span data-stu-id="10322-1410">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="10322-1411">AMS</span><span class="sxs-lookup"><span data-stu-id="10322-1411">AMS</span></span>
* [PRETERIDO]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [ALTERAÇÃO SIGNIFICATIVA]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="10322-1414">Adição de suporte para novos parâmetros de criptografia em `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="10322-1414">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="10322-1415">Adição de novo parâmetro `--filters` a `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="10322-1415">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-1416">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-1416">AppService</span></span>
* <span data-ttu-id="10322-1417">Adicionado o suporte `--logs` para `webapp up`</span><span class="sxs-lookup"><span data-stu-id="10322-1417">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="10322-1418">Correção de problemas do comando `functionapp devops-build create` de geração de `azure-pipelines.yml`</span><span class="sxs-lookup"><span data-stu-id="10322-1418">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="10322-1419">Melhoria do tratamento de erros e indicadores `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="10322-1419">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="10322-1420">[ALTERAÇÃO SIGNIFICATIVA] Remoção do sinalizador `--local-git` para o comando `devops-build`; a detecção de git local e a manipulação são obrigatórias para a criação de pipelines do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="10322-1420">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="10322-1421">Adição de suporte para a criação de planos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="10322-1421">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="10322-1422">Adição da capacidade de trocar um plano sob um aplicativo de funções usando `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="10322-1422">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="10322-1423">Adição de suporte para configurações de expansão de plano Premium do Azure Functions</span><span class="sxs-lookup"><span data-stu-id="10322-1423">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="10322-1424">CDN</span><span class="sxs-lookup"><span data-stu-id="10322-1424">CDN</span></span>
* <span data-ttu-id="10322-1425">Adição de suporte para `Microsoft_Standard` e `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="10322-1425">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="10322-1426">Comentários</span><span class="sxs-lookup"><span data-stu-id="10322-1426">Feedback</span></span>
* <span data-ttu-id="10322-1427">Alteração de `feedback` para mostrar metadados em comandos executados recentemente</span><span class="sxs-lookup"><span data-stu-id="10322-1427">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="10322-1428">Alteração de `feedback` para solicitar o auxílio do usuário no processo de criação de problema abrindo um navegador e usando um modelo de problema</span><span class="sxs-lookup"><span data-stu-id="10322-1428">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="10322-1429">Alteração do `feedback` para imprimir o corpo do problema ao executar com '--verbose'</span><span class="sxs-lookup"><span data-stu-id="10322-1429">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-1430">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-1430">Monitor</span></span>
* <span data-ttu-id="10322-1431">Correção de um problema em que “count” não era um valor permitido com `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1431">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="10322-1432">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-1432">Network</span></span>
* <span data-ttu-id="10322-1433">Correção do formato de tabela que não estava sendo exibido com `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="10322-1433">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="10322-1434">Adição dos comandos `list-request-headers` e `list-response-headers` para `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="10322-1434">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="10322-1435">Adição do comando `list-server-variables` para `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="10322-1435">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="10322-1436">Correção de um problema em que a atualização do estado do link em uma porta express-route geraria uma exceção de atributo desconhecido `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="10322-1436">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="10322-1437">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="10322-1437">PrivateDNS</span></span>
* <span data-ttu-id="10322-1438">Adição de `network private-dns` para zonas de DNS privado</span><span class="sxs-lookup"><span data-stu-id="10322-1438">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="10322-1439">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-1439">Resource</span></span>
* <span data-ttu-id="10322-1440">Correção do problema com `deployment create` e `group deployment create`, em que um arquivo de parâmetros com um conjunto vazio de parâmetros não funcionaria</span><span class="sxs-lookup"><span data-stu-id="10322-1440">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="10322-1441">Função</span><span class="sxs-lookup"><span data-stu-id="10322-1441">Role</span></span>
* <span data-ttu-id="10322-1442">Correção de `create-for-rbac` para lidar corretamente com `--years`</span><span class="sxs-lookup"><span data-stu-id="10322-1442">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="10322-1443">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `role assignment delete` para solicitar ao excluir todas as atribuições na assinatura incondicionalmente</span><span class="sxs-lookup"><span data-stu-id="10322-1443">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="10322-1444">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-1444">SQL</span></span>
* <span data-ttu-id="10322-1445">Atualização de `sql mi [create|update]` com as propriedades proxyOverride e publicDataEndpointEnabled</span><span class="sxs-lookup"><span data-stu-id="10322-1445">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="10322-1446">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-1446">Storage</span></span>
* <span data-ttu-id="10322-1447">[ALTERAÇÃO SIGNIFICATIVA] Remoção do resultado de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="10322-1447">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="10322-1448">Adição de `--full-uri` a `storage blob generate-sas` para criar o URI completo para o blob com SAS</span><span class="sxs-lookup"><span data-stu-id="10322-1448">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="10322-1449">Adição de `--file-snapshot` a `storage file copy start` para copiar arquivo do instantâneo</span><span class="sxs-lookup"><span data-stu-id="10322-1449">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="10322-1450">Alteração de `storage blob copy cancel` para mostrar apenas o erro em vez da exceção para NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="10322-1450">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="10322-1451">26 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-1451">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="10322-1452">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-1452">Core</span></span>
* <span data-ttu-id="10322-1453">Correção de problemas com incompatibilidade da extensão de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="10322-1453">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="10322-1454">Agora o tratamento de erros encaminha os clientes para a página de problemas</span><span class="sxs-lookup"><span data-stu-id="10322-1454">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="10322-1455">Nuvem</span><span class="sxs-lookup"><span data-stu-id="10322-1455">Cloud</span></span>
* <span data-ttu-id="10322-1456">Erro de “assinatura não encontrada” corrigido em `cloud set`</span><span class="sxs-lookup"><span data-stu-id="10322-1456">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="10322-1457">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-1457">ACR</span></span>
* <span data-ttu-id="10322-1458">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="10322-1458">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="10322-1459">`--auth-mode` adicionado aos comandos `acr build`, `acr run`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="10322-1459">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="10322-1460">Grupo de comandos “acr task credential” adicionado para gerenciar as credenciais de uma Tarefa</span><span class="sxs-lookup"><span data-stu-id="10322-1460">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="10322-1461">“--no-wait” adicionado ao comando `acr build`</span><span class="sxs-lookup"><span data-stu-id="10322-1461">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-1462">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-1462">AppService</span></span>
* <span data-ttu-id="10322-1463">Bug corrigido onde `webapp up` não estava lidando corretamente com a execução do diretório vazio ou do cenário de código desconhecido</span><span class="sxs-lookup"><span data-stu-id="10322-1463">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="10322-1464">Bug corrigido onde os slots não funcionavam para `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="10322-1464">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="10322-1465">Serviço de BOT</span><span class="sxs-lookup"><span data-stu-id="10322-1465">BOT Service</span></span>
* <span data-ttu-id="10322-1466">`bot prepare-deploy` adicionado para se preparar para a implantação de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="10322-1466">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="10322-1467">`bot create --kind registration` alterado para mostrar a senha se ela não for fornecida</span><span class="sxs-lookup"><span data-stu-id="10322-1467">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="10322-1468">[ALTERAÇÃO SIGNIFICATIVA]`--endpoint` alterado em `bot create --kind registration` como padrão para uma cadeia de caracteres vazia, em vez de ser requerido</span><span class="sxs-lookup"><span data-stu-id="10322-1468">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="10322-1469">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="10322-1469">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="10322-1470">CDN</span><span class="sxs-lookup"><span data-stu-id="10322-1470">CDN</span></span>
* <span data-ttu-id="10322-1471">Adicionado o suporte ao `--no-wait` para `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="10322-1471">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [ALTERAÇÃO SIGNIFICATIVA]: `cdn endpoint create` alterado para o comportamento de cache da cadeia de consulta padrão.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="10322-1473">Não há mais padrão para "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="10322-1473">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="10322-1474">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="10322-1474">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="10322-1475">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="10322-1475">Cosmosdb</span></span>
* <span data-ttu-id="10322-1476">Suporte adicionado para `--enable-multiple-write-locations` na atualização da conta</span><span class="sxs-lookup"><span data-stu-id="10322-1476">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="10322-1477">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="10322-1477">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="10322-1478">Interativo</span><span class="sxs-lookup"><span data-stu-id="10322-1478">Interactive</span></span>
* <span data-ttu-id="10322-1479">Incompatibilidade corrigida com a extensão Interativa instalada por meio do azdev</span><span class="sxs-lookup"><span data-stu-id="10322-1479">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-1480">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-1480">Monitor</span></span>
* <span data-ttu-id="10322-1481">Alterado para permitir o valor de dimensão `*` para `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1481">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="10322-1482">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-1482">Network</span></span>
* <span data-ttu-id="10322-1483">Grupo de comandos `rewrite-rule` adicionado em `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="10322-1483">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="10322-1484">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-1484">Profile</span></span>
* <span data-ttu-id="10322-1485">Suporte de conta no nível do locatário para a identidade de serviço gerenciado adicionado em `login`</span><span class="sxs-lookup"><span data-stu-id="10322-1485">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="10322-1486">Postgres</span><span class="sxs-lookup"><span data-stu-id="10322-1486">Postgres</span></span> 
* <span data-ttu-id="10322-1487">Adicionados os comandos postgresql `replica` e `restart server`</span><span class="sxs-lookup"><span data-stu-id="10322-1487">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="10322-1488">Alterado para obter o local padrão do grupo de recursos quando não fornecido para criar servidores e adicionar validação para os dias de retenção</span><span class="sxs-lookup"><span data-stu-id="10322-1488">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="10322-1489">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-1489">Resource</span></span>
* <span data-ttu-id="10322-1490">Saída da tabela aperfeiçoada para `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="10322-1490">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="10322-1491">Corrigido o problema com `deployment [create|validate]` onde o tipo secureObject não era reconhecido</span><span class="sxs-lookup"><span data-stu-id="10322-1491">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="10322-1492">Grafo</span><span class="sxs-lookup"><span data-stu-id="10322-1492">Graph</span></span>
* <span data-ttu-id="10322-1493">Adicionado o suporte ao `--end-date` para `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="10322-1493">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="10322-1494">Suporte adicionado para acrescentar permissões com `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="10322-1494">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="10322-1495">Bug corrigido com `ad app permission list` quando não havia nenhuma permissão</span><span class="sxs-lookup"><span data-stu-id="10322-1495">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="10322-1496">`ad sp delete` alterado para ignorar a exclusão da atribuição de função se a conta atual não tem nenhuma assinatura</span><span class="sxs-lookup"><span data-stu-id="10322-1496">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="10322-1497">`ad app create` alterado para `--identifier-uris` passar para lista vazia como padrão se não fornecido</span><span class="sxs-lookup"><span data-stu-id="10322-1497">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="10322-1498">armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-1498">storage</span></span>
* <span data-ttu-id="10322-1499">`--snapshot` adicionado a `storage file download-batch` para baixar de um instantâneo de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="10322-1499">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="10322-1500">Barra de progresso `storage blob [download-batch|upload-batch]` alterada para ser menos detalhada e indicar o blob atual</span><span class="sxs-lookup"><span data-stu-id="10322-1500">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="10322-1501">Problema corrigido com `storage account update` ao atualizar os parâmetros de criptografia</span><span class="sxs-lookup"><span data-stu-id="10322-1501">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="10322-1502">Problema corrigido onde `storage blob show` falharia ao usar o oauth (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="10322-1502">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="10322-1503">VM</span><span class="sxs-lookup"><span data-stu-id="10322-1503">VM</span></span>
* <span data-ttu-id="10322-1504">Adicionado o comando `image update`</span><span class="sxs-lookup"><span data-stu-id="10322-1504">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="10322-1505">12 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-1505">March 12, 2019</span></span>

<span data-ttu-id="10322-1506">Versão 2.0.60</span><span class="sxs-lookup"><span data-stu-id="10322-1506">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="10322-1507">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-1507">Core</span></span>

* <span data-ttu-id="10322-1508">Foi corrigido um erro incorreto no `cloud set` sobre assinatura não encontrada.</span><span class="sxs-lookup"><span data-stu-id="10322-1508">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="10322-1509">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-1509">ACR</span></span>

* <span data-ttu-id="10322-1510">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="10322-1510">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="10322-1511">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-1511">ACS</span></span>

* <span data-ttu-id="10322-1512">Alteração para ignorar o parâmetro `--listen-address` para `aks browse` se ele não for compatível com kubectl</span><span class="sxs-lookup"><span data-stu-id="10322-1512">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="10322-1513">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-1513">AppService</span></span>

* <span data-ttu-id="10322-1514">Adicionado `[webapp|functionapp] deployment list-publishing-credentials` para obter a URL de publicação do Kudu e suas credenciais.</span><span class="sxs-lookup"><span data-stu-id="10322-1514">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="10322-1515">Removida a instrução de impressão errônea de `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="10322-1515">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="10322-1516">Corrigido `functionapp` para definir a imagem correta do runtime nos planos do Serviço de Aplicativo no Linux.</span><span class="sxs-lookup"><span data-stu-id="10322-1516">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="10322-1517">Removida a marca de versão prévia do `webapp up` e adicionadas melhorias ao comando.</span><span class="sxs-lookup"><span data-stu-id="10322-1517">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="10322-1518">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="10322-1518">Botservice</span></span>

* <span data-ttu-id="10322-1519">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="10322-1519">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="10322-1520">Adicionados `Microsoft-BotFramework-AppId` e `Microsoft-BotFramework-AppPassword` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="10322-1520">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="10322-1521">Removidas as aspas simples da saída de comando `bot publish`, no final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="10322-1521">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="10322-1522">Alterado `bot publish` para que seja assíncrono.</span><span class="sxs-lookup"><span data-stu-id="10322-1522">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="10322-1523">Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-1523">Container</span></span>

* <span data-ttu-id="10322-1524">Adicionado o argumento `--no-wait` para `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="10322-1524">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="10322-1525">EventHub</span><span class="sxs-lookup"><span data-stu-id="10322-1525">EventHub</span></span>

* <span data-ttu-id="10322-1526">Adicionado o sinalizador `--skip-empty-archives` a `eventhub create|update` para dar suporte a arquivos vazios na captura.</span><span class="sxs-lookup"><span data-stu-id="10322-1526">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="10322-1527">Localizar</span><span class="sxs-lookup"><span data-stu-id="10322-1527">Find</span></span>

* <span data-ttu-id="10322-1528">Atualização de funcionalidade principal</span><span class="sxs-lookup"><span data-stu-id="10322-1528">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="10322-1529">HDInsight</span><span class="sxs-lookup"><span data-stu-id="10322-1529">HDInsight</span></span>

* <span data-ttu-id="10322-1530">Adicionado o parâmetro `--storage-account-managed-identity` a `hdinsight create` para oferecer suporte ao MSI do ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="10322-1530">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="10322-1531">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-1531">Network</span></span>

* <span data-ttu-id="10322-1532">Corrigido o problema com `vpn-connection update`, onde a atualização de uma conexão VPN entre gateways em assinaturas diferentes falharia.</span><span class="sxs-lookup"><span data-stu-id="10322-1532">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="10322-1533">Rdbms</span><span class="sxs-lookup"><span data-stu-id="10322-1533">Rdbms</span></span>

* <span data-ttu-id="10322-1534">Correções secundárias para obter a localização padrão do grupo de recursos, quando não fornecida, para criar servidores e adicionar validação nos dias de retenção.</span><span class="sxs-lookup"><span data-stu-id="10322-1534">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="10322-1535">Função</span><span class="sxs-lookup"><span data-stu-id="10322-1535">Role</span></span>

* <span data-ttu-id="10322-1536">Corrigido `role definition update` para usar ID a fim de resolver a definição corretamente.</span><span class="sxs-lookup"><span data-stu-id="10322-1536">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="10322-1537">Alterado `ad app credential reset` para remover a suposição de que a entidade de serviço do aplicativo já existe.</span><span class="sxs-lookup"><span data-stu-id="10322-1537">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="10322-1538">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="10322-1538">Service Fabric</span></span>

* <span data-ttu-id="10322-1539">Corrigido o problema com o fato de `sf cluster list` não ser iterável.</span><span class="sxs-lookup"><span data-stu-id="10322-1539">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="10322-1540">26 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-1540">February 26, 2019</span></span>

<span data-ttu-id="10322-1541">Versão 2.0.59</span><span class="sxs-lookup"><span data-stu-id="10322-1541">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="10322-1542">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-1542">Core</span></span>

* <span data-ttu-id="10322-1543">Corrigido o problema onde algumas instâncias usando `--subscription NAME` produziriam uma exceção</span><span class="sxs-lookup"><span data-stu-id="10322-1543">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="10322-1544">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-1544">ACR</span></span>

* <span data-ttu-id="10322-1545">Parâmetro `--target` adicionado para os comandos `acr build`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="10322-1545">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="10322-1546">Melhor tratamento de erros para os comandos de execução quando não conectado ao Azure</span><span class="sxs-lookup"><span data-stu-id="10322-1546">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="10322-1547">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-1547">ACS</span></span>

* <span data-ttu-id="10322-1548">Opção `--listen-address` adicionada a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="10322-1548">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-1549">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-1549">AppService</span></span>

* <span data-ttu-id="10322-1550">Adicionado o comando `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="10322-1550">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="10322-1551">Lote</span><span class="sxs-lookup"><span data-stu-id="10322-1551">Batch</span></span>
* <span data-ttu-id="10322-1552">[ALTERAÇÃO SIGNIFICATIVA] Comando `batch pool upgrade os` removido</span><span class="sxs-lookup"><span data-stu-id="10322-1552">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="10322-1553">[ALTERAÇÃO SIGNIFICATIVA] Propriedade `Pacakges` removida das respostas `Application`</span><span class="sxs-lookup"><span data-stu-id="10322-1553">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="10322-1554">Comando `batch application package list` adicionado para listar os pacotes de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="10322-1554">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="10322-1555">[ALTERAÇÃO SIGNIFICATIVA]`--application-id` alterado para `--application-name` em todos os comandos `batch application`,</span><span class="sxs-lookup"><span data-stu-id="10322-1555">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="10322-1556">O argumento `--json-file` foi adicionado aos comandos para a solicitação de resposta da API bruta</span><span class="sxs-lookup"><span data-stu-id="10322-1556">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="10322-1557">Validação atualizada para incluir automaticamente `https://` em todos os pontos de extremidade, se ausente</span><span class="sxs-lookup"><span data-stu-id="10322-1557">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="10322-1558">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="10322-1558">CosmosDB</span></span>

* <span data-ttu-id="10322-1559">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="10322-1559">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="10322-1560">Kusto</span><span class="sxs-lookup"><span data-stu-id="10322-1560">Kusto</span></span>

* <span data-ttu-id="10322-1561">[ALTERAÇÃO SIGNIFICATIVA] Os tipos `hot_cache_period` e `soft_delete_period` foram alterados do banco de dados para o formato de duração ISO8601</span><span class="sxs-lookup"><span data-stu-id="10322-1561">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="10322-1562">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-1562">Network</span></span>

* <span data-ttu-id="10322-1563">Adicionado o argumento `--express-route-gateway-bypass` para `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1563">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="10322-1564">Foram adicionados os grupos de comando a partir das extensões `express-route`</span><span class="sxs-lookup"><span data-stu-id="10322-1564">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="10322-1565">Os grupos de comando `express-route gateway` e `express-route port` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="10322-1565">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="10322-1566">Adicionado o argumento `--legacy-mode` para `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1566">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="10322-1567">Os argumentos `--allow-classic-operations` e `--express-route-port` foram adicionados a `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1567">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="10322-1568">Adicionado o argumento `--gateway-default-site` para `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1568">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="10322-1569">Os comandos `ipsec-policy` foram adicionados a `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="10322-1569">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="10322-1570">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-1570">Resource</span></span>

* <span data-ttu-id="10322-1571">Foi corrigido o problema com `deployment create` em que o campo do tipo diferencia letras maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="10322-1571">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="10322-1572">Foi adicionado o suporte para arquivo de parâmetros de URI a `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="10322-1572">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="10322-1573">Foi adicionado o suporte para parâmetros de URI e definições a `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="10322-1573">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="10322-1574">Foi corrigido o tratamento de parâmetros e regras para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="10322-1574">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="10322-1575">Foi corrigido o problema com `resource show/update/delete/tag/invoke-action` em que as IDs de assinatura cruzada não respeitaram corretamente a ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="10322-1575">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="10322-1576">Função</span><span class="sxs-lookup"><span data-stu-id="10322-1576">Role</span></span>

* <span data-ttu-id="10322-1577">Foi adicionado o suporte para as funções do aplicativo a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1577">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="10322-1578">VM</span><span class="sxs-lookup"><span data-stu-id="10322-1578">VM</span></span>

* <span data-ttu-id="10322-1579">Foi corrigido o problema com `vm create where ` – a rede acelerada não foi habilitada por padrão no Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="10322-1579">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="10322-1580">12 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-1580">February 12, 2019</span></span>

<span data-ttu-id="10322-1581">Versão 2.0.58</span><span class="sxs-lookup"><span data-stu-id="10322-1581">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="10322-1582">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-1582">Core</span></span>

* <span data-ttu-id="10322-1583">`az --version` agora exibe uma notificação se você tiver pacotes para atualização</span><span class="sxs-lookup"><span data-stu-id="10322-1583">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="10322-1584">A regressão em que `--ids` não pode ser usado com a saída JSON foi corrigida</span><span class="sxs-lookup"><span data-stu-id="10322-1584">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="10322-1585">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-1585">ACR</span></span>
* <span data-ttu-id="10322-1586">[ALTERAÇÃO SIGNIFICATIVA] O grupo de comandos `acr build-task` foi removido</span><span class="sxs-lookup"><span data-stu-id="10322-1586">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="10322-1587">[ALTERAÇÃO SIGNIFICATIVA] As opções `--tag` e `--manifest` de `acr repository delete` foram removidas</span><span class="sxs-lookup"><span data-stu-id="10322-1587">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="10322-1588">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-1588">ACS</span></span>
* <span data-ttu-id="10322-1589">Suporte adicionado a `aks [enable-addons|disable-addons]` para nomes que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="10322-1589">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="10322-1590">Suporte adicionado para a operação de atualização do Azure Active Directory usando `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="10322-1590">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="10322-1591">Um esclarecimento informando que `--output` é ignorado para `aks get-credentials` foi adicionado</span><span class="sxs-lookup"><span data-stu-id="10322-1591">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="10322-1592">AMS</span><span class="sxs-lookup"><span data-stu-id="10322-1592">AMS</span></span>
* <span data-ttu-id="10322-1593">Adicionados os comandos `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="10322-1593">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="10322-1594">Adicionados os comandos `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="10322-1594">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-1595">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-1595">Appservice</span></span>
* <span data-ttu-id="10322-1596">Foi adicionada a capacidade de criar e configurar funções usando contêineres de ACR</span><span class="sxs-lookup"><span data-stu-id="10322-1596">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="10322-1597">Suporte adicionado para a atualização das configurações de aplicativos Web por meio de JSON</span><span class="sxs-lookup"><span data-stu-id="10322-1597">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="10322-1598">A ajuda foi aprimorada para `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="10322-1598">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="10322-1599">Suporte adicionado para o App Insights para auxiliar na criação de aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="10322-1599">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="10322-1600">Os problemas com o SSH do aplicativo Web foram corrigidos</span><span class="sxs-lookup"><span data-stu-id="10322-1600">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="10322-1601">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="10322-1601">Botservice</span></span>
* <span data-ttu-id="10322-1602">A experiência do usuário para `bot publish` foi aprimorada</span><span class="sxs-lookup"><span data-stu-id="10322-1602">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="10322-1603">Foram adicionados avisos de tempos limite ao executar `npm install` durante `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="10322-1603">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="10322-1604">O caractere inválido `.` de `--name` em `az bot create` foi removido</span><span class="sxs-lookup"><span data-stu-id="10322-1604">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="10322-1605">Alteração para interromper a geração aleatória de nomes de recursos durante a criação do Armazenamento do Azure, Plano do Serviço de Aplicativo, Aplicativo Web/de funções e Application Insights</span><span class="sxs-lookup"><span data-stu-id="10322-1605">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="10322-1606">[PRETERIDO] O argumento `--proj-name` foi preterido em favor de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="10322-1606">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="10322-1607">`az bot publish` foi alterado para remover arquivos de implantação do Node.js do IIS buscados, caso eles já não existissem</span><span class="sxs-lookup"><span data-stu-id="10322-1607">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="10322-1608">Foi adicionado o argumento `--keep-node-modules` para `az bot publish` para não excluir a pasta `node_modules` no Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10322-1608">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="10322-1609">O par chave-valor `"publishCommand"` foi adicionado à saída de `az bot create` durante a criação de uma função do Azure ou bot de aplicativo Web</span><span class="sxs-lookup"><span data-stu-id="10322-1609">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="10322-1610">O valor de `"publishCommand"` é um comando `az bot publish` que é automaticamente preenchido com os parâmetros necessários para publicar o bot recém-criado</span><span class="sxs-lookup"><span data-stu-id="10322-1610">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="10322-1611">O `"WEBSITE_NODE_DEFAULT_VERSION"` foi atualizado no modelo do ARM para que os bots de SDK v4 usem 10.14.1 em vez de 8.9.4</span><span class="sxs-lookup"><span data-stu-id="10322-1611">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="10322-1612">Key Vault</span><span class="sxs-lookup"><span data-stu-id="10322-1612">Key Vault</span></span>
* <span data-ttu-id="10322-1613">Foi corrigido o problema com `keyvault secret backup`, em que alguns usuários recebiam um erro `unexpected_keyword` ao usar `--id`</span><span class="sxs-lookup"><span data-stu-id="10322-1613">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-1614">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-1614">Monitor</span></span>
* <span data-ttu-id="10322-1615">`monitor metrics alert [create|update]` foi alterado para permitir o valor dimensional `*`</span><span class="sxs-lookup"><span data-stu-id="10322-1615">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="10322-1616">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-1616">Network</span></span>
* <span data-ttu-id="10322-1617">`dns zone export` foi alterado para garantir que CNAMEs exportados fossem FQDNs</span><span class="sxs-lookup"><span data-stu-id="10322-1617">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="10322-1618">O parâmetro `--gateway-name` foi adicionado a `nic ip-config address-pool [add|remove]` para dar suporte a pools de endereços de back-end de gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="10322-1618">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="10322-1619">Os argumentos `--traffic-analytics` e `--workspace` foram adicionados a `network watcher flow-log configure` para dar suporte à análise de tráfego por meio de um espaço de trabalho do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="10322-1619">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="10322-1620">`--idle-timeout` e `--floating-ip` foram adicionados a `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1620">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="10322-1621">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="10322-1621">Policy Insights</span></span>
* <span data-ttu-id="10322-1622">Os comandos `policy remediation` foram adicionados para dar suporte a recursos de correção de política de recursos</span><span class="sxs-lookup"><span data-stu-id="10322-1622">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="10322-1623">RDBMS</span><span class="sxs-lookup"><span data-stu-id="10322-1623">RDBMS</span></span>
* <span data-ttu-id="10322-1624">A mensagem e os parâmetros de comando de ajuda foram aprimorados</span><span class="sxs-lookup"><span data-stu-id="10322-1624">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="10322-1625">Redis</span><span class="sxs-lookup"><span data-stu-id="10322-1625">Redis</span></span>
* <span data-ttu-id="10322-1626">Foram adicionados comandos para gerenciar regras de firewall (criar, atualizar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="10322-1626">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="10322-1627">Foram adicionados comandos para gerenciar links do servidor (criar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="10322-1627">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="10322-1628">Foram adicionados comandos para gerenciar o agendamento de patches (criar, atualizar, excluir, mostrar)</span><span class="sxs-lookup"><span data-stu-id="10322-1628">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="10322-1629">Suporte adicionado para Zonas de Disponibilidade e versão mínima de TLS para criar Redis</span><span class="sxs-lookup"><span data-stu-id="10322-1629">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="10322-1630">[ALTERAÇÃO SIGNIFICATIVA] Os comandos `redis update-settings` e `redis list-all` foram removidos</span><span class="sxs-lookup"><span data-stu-id="10322-1630">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="10322-1631">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro para `redis create`: “configurações de locatário” não é aceito no formato chave[=valor]</span><span class="sxs-lookup"><span data-stu-id="10322-1631">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="10322-1632">[PRETERIDO] Uma mensagem de aviso foi adicionada para preterir o comando `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="10322-1632">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="10322-1633">Função</span><span class="sxs-lookup"><span data-stu-id="10322-1633">Role</span></span>
* <span data-ttu-id="10322-1634">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido dos comandos `vm` para esta localização</span><span class="sxs-lookup"><span data-stu-id="10322-1634">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="10322-1635">SQL VM</span><span class="sxs-lookup"><span data-stu-id="10322-1635">SQL VM</span></span>
* <span data-ttu-id="10322-1636">[PRETERIDO] O argumento `--boostrap-acc-pwd` foi preterido devido a um erro de digitação</span><span class="sxs-lookup"><span data-stu-id="10322-1636">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="10322-1637">VM</span><span class="sxs-lookup"><span data-stu-id="10322-1637">VM</span></span>
* <span data-ttu-id="10322-1638">`vm list-skus` foi alterado para permitir o uso de `--all` no lugar de `--all true`</span><span class="sxs-lookup"><span data-stu-id="10322-1638">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="10322-1639">Adicionado `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="10322-1639">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="10322-1640">Foi corrigido o bug em que `vmss encryption enable` falhava se fosse executado anteriormente</span><span class="sxs-lookup"><span data-stu-id="10322-1640">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="10322-1641">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido para os comandos `role`</span><span class="sxs-lookup"><span data-stu-id="10322-1641">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="10322-1642">31 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-1642">January 31, 2019</span></span>

<span data-ttu-id="10322-1643">Versão 2.0.57</span><span class="sxs-lookup"><span data-stu-id="10322-1643">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="10322-1644">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-1644">Core</span></span>

* <span data-ttu-id="10322-1645">Hotfix para o [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="10322-1645">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="10322-1646">28 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-1646">January 28, 2019</span></span>

<span data-ttu-id="10322-1647">Versão 2.0.56</span><span class="sxs-lookup"><span data-stu-id="10322-1647">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="10322-1648">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-1648">ACR</span></span>
* <span data-ttu-id="10322-1649">Suporte adicionado para regras de rede virtual/IP</span><span class="sxs-lookup"><span data-stu-id="10322-1649">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="10322-1650">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-1650">ACS</span></span>
* <span data-ttu-id="10322-1651">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="10322-1651">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="10322-1652">Comandos do OpenShift gerenciado foram adicionados</span><span class="sxs-lookup"><span data-stu-id="10322-1652">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="10322-1653">Suporte adicionado para operações de atualização da entidade de serviço com `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="10322-1653">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="10322-1654">AMS</span><span class="sxs-lookup"><span data-stu-id="10322-1654">AMS</span></span>
* <span data-ttu-id="10322-1655">[ALTERAÇÃO SIGNIFICATIVA]`ams asset get-streaming-locators` renomeado para `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="10322-1655">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="10322-1656">[ALTERAÇÃO SIGNIFICATIVA]`ams streaming-locator get-content-keys` renomeado para `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="10322-1656">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-1657">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-1657">Appservice</span></span>
* <span data-ttu-id="10322-1658">Suporte adicionado para o App Insights no `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="10322-1658">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="10322-1659">Suporte adicionado para a criação do plano de serviço de aplicativo (incluindo Elástico Premium) para Aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="10322-1659">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="10322-1660">Foram corrigidos os problemas com de configuração de aplicativo com os planos Elástico Premium</span><span class="sxs-lookup"><span data-stu-id="10322-1660">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="10322-1661">Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-1661">Container</span></span>
* <span data-ttu-id="10322-1662">Adicionado o comando `container start`</span><span class="sxs-lookup"><span data-stu-id="10322-1662">Added `container start` command</span></span>
* <span data-ttu-id="10322-1663">Alteração para permitir o uso de valores decimais para CPU durante a criação do contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-1663">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="10322-1664">EventGrid</span><span class="sxs-lookup"><span data-stu-id="10322-1664">EventGrid</span></span>
* <span data-ttu-id="10322-1665">Parâmetro `--deadletter-endpoint` adicionado a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1665">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="10322-1666">Storagequeue e hybridconnection foram adicionados como novos valores para 'event-subscription [create|update] --endpoint-type\`</span><span class="sxs-lookup"><span data-stu-id="10322-1666">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="10322-1667">Os parâmetros `--max-delivery-attempts` e `--event-ttl` foram adicionados a `event-subscription create` para especificar a política de repetição para eventos</span><span class="sxs-lookup"><span data-stu-id="10322-1667">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="10322-1668">Uma mensagem de aviso foi adicionada a `event-subscription [create|update]` quando o webhook como destino for usado para uma assinatura de evento</span><span class="sxs-lookup"><span data-stu-id="10322-1668">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="10322-1669">O parâmetro source-resource-id foi adicionado para todos os comandos relacionados a eventos e marcar todos os outros parâmetros relacionados ao recurso de origem como preteridos</span><span class="sxs-lookup"><span data-stu-id="10322-1669">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="10322-1670">HDInsight</span><span class="sxs-lookup"><span data-stu-id="10322-1670">HDInsight</span></span>
* <span data-ttu-id="10322-1671">[ALTERAÇÃO SIGNIFICATIVA] Os parâmetros `--virtual-network` e `--subnet-name` de `hdinsight [application] create` foram removidos</span><span class="sxs-lookup"><span data-stu-id="10322-1671">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="10322-1672">[ALTERAÇÃO SIGNIFICATIVA]`hdinsight create --storage-account` foi alterado para aceitar o nome ou ID da conta de armazenamento, em vez de pontos de extremidade de blob</span><span class="sxs-lookup"><span data-stu-id="10322-1672">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="10322-1673">Parâmetros `--vnet-name` e `--subnet-name` adicionados a `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="10322-1673">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="10322-1674">Suporte adicionado para a criptografia de disco e Enterprise Security Package ao `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="10322-1674">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="10322-1675">Adicionado o comando `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="10322-1675">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="10322-1676">Adicionado o comando `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="10322-1676">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="10322-1677">IoT</span><span class="sxs-lookup"><span data-stu-id="10322-1677">IoT</span></span>
* <span data-ttu-id="10322-1678">O formato de codificação foi adicionado ao comando routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="10322-1678">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="10322-1679">Kusto</span><span class="sxs-lookup"><span data-stu-id="10322-1679">Kusto</span></span>
* <span data-ttu-id="10322-1680">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="10322-1680">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-1681">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-1681">Monitor</span></span>
* <span data-ttu-id="10322-1682">A comparação de ID foi alterada para diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="10322-1682">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="10322-1683">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-1683">Profile</span></span>
* <span data-ttu-id="10322-1684">A conta de nível de locatário foi habilitada para a identidade de serviço gerenciada de `login`</span><span class="sxs-lookup"><span data-stu-id="10322-1684">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="10322-1685">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-1685">Network</span></span>
* <span data-ttu-id="10322-1686">Foi corrigido o problema com `express-route update`: em que o argumento `--bandwidth` era ignorado</span><span class="sxs-lookup"><span data-stu-id="10322-1686">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="10322-1687">Foi corrigido o problema com `ddos-protection update` em que definir a compreensão levava ao rastreamento de pilha</span><span class="sxs-lookup"><span data-stu-id="10322-1687">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="10322-1688">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-1688">Resource</span></span>
* <span data-ttu-id="10322-1689">Suporte adicionado para o arquivo de parâmetros de URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="10322-1689">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="10322-1690">Suporte adicionado para a identidade gerenciada à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="10322-1690">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="10322-1691">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="10322-1691">SQL Virtual Machine</span></span>
* <span data-ttu-id="10322-1692">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="10322-1692">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="10322-1693">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-1693">Storage</span></span>
* <span data-ttu-id="10322-1694">Alteração na correção para atualizar apenas as propriedades que são alteradas no mesmo objeto</span><span class="sxs-lookup"><span data-stu-id="10322-1694">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="10322-1695">#8021 foi corrigido, dados binários são codificados em base 64 quando retornados</span><span class="sxs-lookup"><span data-stu-id="10322-1695">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="10322-1696">VM</span><span class="sxs-lookup"><span data-stu-id="10322-1696">VM</span></span>
* <span data-ttu-id="10322-1697">Alteração de `vm encryption enable` para validar o cofre de chaves de criptografia de disco e se esse cofre de chaves de criptografia de chave existe</span><span class="sxs-lookup"><span data-stu-id="10322-1697">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="10322-1698">O sinalizador `--force` foi adicionado a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="10322-1698">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="10322-1699">15 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="10322-1699">January 15, 2019</span></span>

<span data-ttu-id="10322-1700">Versão 2.0.55</span><span class="sxs-lookup"><span data-stu-id="10322-1700">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="10322-1701">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-1701">ACR</span></span>
* <span data-ttu-id="10322-1702">Alteração para permitir forçar o envio por push de um gráfico Helm que não existe</span><span class="sxs-lookup"><span data-stu-id="10322-1702">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="10322-1703">Alteração para permitir operações de runtime sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="10322-1703">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="10322-1704">[PRETERIDO] O parâmetro `--resource-group` foi preterido nos comandos:</span><span class="sxs-lookup"><span data-stu-id="10322-1704">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="10322-1705">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-1705">ACS</span></span>
* <span data-ttu-id="10322-1706">Suporte adicionado para novas regiões ACI</span><span class="sxs-lookup"><span data-stu-id="10322-1706">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-1707">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-1707">Appservice</span></span>
* <span data-ttu-id="10322-1708">Foi corrigido o problema com o carregamento de certificados para aplicativos que são hospedados em um ASE, em que o RG do ASE e o RG do aplicativo são diferentes</span><span class="sxs-lookup"><span data-stu-id="10322-1708">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="10322-1709">Alteração de `webapp up` para usar a SKU P1V1 como padrão para Linux</span><span class="sxs-lookup"><span data-stu-id="10322-1709">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="10322-1710">`[webapp|functionapp] deployment source config-zip` foi corrigido para mostrar a mensagem de erro adequada quando uma implantação falhar</span><span class="sxs-lookup"><span data-stu-id="10322-1710">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="10322-1711">Adicionado o comando `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="10322-1711">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="10322-1712">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="10322-1712">Botservice</span></span>
* <span data-ttu-id="10322-1713">Atualizações de status de implantação foram adicionadas a `bot create`</span><span class="sxs-lookup"><span data-stu-id="10322-1713">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="10322-1714">Configurar</span><span class="sxs-lookup"><span data-stu-id="10322-1714">Configure</span></span>
* <span data-ttu-id="10322-1715">`none` foi adicionado como um formato de saída configurável</span><span class="sxs-lookup"><span data-stu-id="10322-1715">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="10322-1716">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="10322-1716">CosmosDB</span></span>
* <span data-ttu-id="10322-1717">Suporte adicionado para criar o banco de dados com taxa de transferência compartilhada</span><span class="sxs-lookup"><span data-stu-id="10322-1717">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="10322-1718">HDInsight</span><span class="sxs-lookup"><span data-stu-id="10322-1718">HDInsight</span></span>
* <span data-ttu-id="10322-1719">Foram adicionados comandos para o gerenciamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="10322-1719">Added commands for managing applications</span></span>
* <span data-ttu-id="10322-1720">Foram adicionados comandos para o gerenciamento de ações de script</span><span class="sxs-lookup"><span data-stu-id="10322-1720">Added commands for managing script actions</span></span>
* <span data-ttu-id="10322-1721">Foram adicionados comandos para o gerenciamento do Operations Management Suite (OMS)</span><span class="sxs-lookup"><span data-stu-id="10322-1721">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="10322-1722">Suporte adicionado para listar a utilização regional ao `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="10322-1722">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="10322-1723">[ALTERAÇÃO SIGNIFICATIVA] O tipo de cluster padrão de `hdinsight create` foi removido</span><span class="sxs-lookup"><span data-stu-id="10322-1723">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="10322-1724">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-1724">Network</span></span>
* <span data-ttu-id="10322-1725">Adicionados os argumentos `--custom-headers` e `--status-code-ranges` para `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1725">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="10322-1726">Novos tipos de roteamento foram adicionados: Subrede e múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="10322-1726">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="10322-1727">Adicionados os argumentos `--custom-headers` e `--subnets` para `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1727">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="10322-1728">Foi corrigido o problema no qual fornecer `--vnets ""` a `ddos-protection update` causava um erro</span><span class="sxs-lookup"><span data-stu-id="10322-1728">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="10322-1729">Função</span><span class="sxs-lookup"><span data-stu-id="10322-1729">Role</span></span>
* <span data-ttu-id="10322-1730">[PRETERIDO] O argumento `--password` foi preterido para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="10322-1730">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="10322-1731">Como alternativa, use senhas seguras geradas pela CLI</span><span class="sxs-lookup"><span data-stu-id="10322-1731">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="10322-1732">Segurança</span><span class="sxs-lookup"><span data-stu-id="10322-1732">Security</span></span>
* <span data-ttu-id="10322-1733">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="10322-1733">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="10322-1734">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-1734">Storage</span></span>
* <span data-ttu-id="10322-1735">[ALTERAÇÃO SIGNIFICATIVA] O número padrão de resultados de `storage [blob|file|container|share] list` foi alterado para 5.000.</span><span class="sxs-lookup"><span data-stu-id="10322-1735">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="10322-1736">Use `--num-results *` para o comportamento original de retornar todos os resultados</span><span class="sxs-lookup"><span data-stu-id="10322-1736">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="10322-1737">Parâmetro `--marker` adicionado a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="10322-1737">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="10322-1738">Um marcador de log foi adicionado para a próxima página ao STDERR de `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="10322-1738">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="10322-1739">O comando `storage blob service-properties update` foi adicionado com suporte para sites estáticos</span><span class="sxs-lookup"><span data-stu-id="10322-1739">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="10322-1740">VM</span><span class="sxs-lookup"><span data-stu-id="10322-1740">VM</span></span>
* <span data-ttu-id="10322-1741">`vm [disk|unmanaged-disk]` e `vmss disk` foram alterados para que tenham parâmetros mais consistentes</span><span class="sxs-lookup"><span data-stu-id="10322-1741">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="10322-1742">Suporte adicionado para referência cruzada de imagem de locatário a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="10322-1742">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="10322-1743">O bug de configuração padrão foi corrigido em `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="10322-1743">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="10322-1744">O argumento `--provision-after-extensions` foi adicionado a `vmss extension set` para definir quais extensões deverão ser provisionadas antes da extensão ser definida</span><span class="sxs-lookup"><span data-stu-id="10322-1744">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="10322-1745">O argumento `--replica-count` foi adicionado a `sig image-version update` para definir a contagem de replicação padrão</span><span class="sxs-lookup"><span data-stu-id="10322-1745">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="10322-1746">Foi corrigido o bug com `image create --source` em que o disco do sistema operacional de origem era confundido com uma VM do mesmo nome, mesmo se a ID de recurso completa fosse fornecida</span><span class="sxs-lookup"><span data-stu-id="10322-1746">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="10322-1747">20 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-1747">December 20, 2018</span></span>

<span data-ttu-id="10322-1748">Versão 2.0.54</span><span class="sxs-lookup"><span data-stu-id="10322-1748">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="10322-1749">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-1749">Appservice</span></span>
* <span data-ttu-id="10322-1750">Corrigido o problema que causava falha na reimplantação do `webapp up`</span><span class="sxs-lookup"><span data-stu-id="10322-1750">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="10322-1751">Adicionado suporte para listar e restaurar instantâneos de aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="10322-1751">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="10322-1752">Adicionado suporte para o sinalizador `--runtime` para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="10322-1752">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="10322-1753">IoT Central</span><span class="sxs-lookup"><span data-stu-id="10322-1753">IoTCentral</span></span>
* <span data-ttu-id="10322-1754">Corrigida a chamada à API do comando de atualização</span><span class="sxs-lookup"><span data-stu-id="10322-1754">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="10322-1755">Função</span><span class="sxs-lookup"><span data-stu-id="10322-1755">Role</span></span>
* <span data-ttu-id="10322-1756">[ALTERAÇÃO SIGNIFICATIVA]`ad [app|sp] list` alterado para listar somente os 100 primeiros objetos por padrão</span><span class="sxs-lookup"><span data-stu-id="10322-1756">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="10322-1757">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-1757">SQL</span></span>
* <span data-ttu-id="10322-1758">Adicionado suporte para ordenação personalizada nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="10322-1758">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="10322-1759">VM</span><span class="sxs-lookup"><span data-stu-id="10322-1759">VM</span></span>
* <span data-ttu-id="10322-1760">Parâmetro `---os-type` adicionado a `disk create`</span><span class="sxs-lookup"><span data-stu-id="10322-1760">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="10322-1761">18 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-1761">December 18, 2018</span></span>

<span data-ttu-id="10322-1762">Versão 2.0.53</span><span class="sxs-lookup"><span data-stu-id="10322-1762">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="10322-1763">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-1763">ACR</span></span>
* <span data-ttu-id="10322-1764">Adicionado suporte para importação de imagem de Registros de Contêiner externos</span><span class="sxs-lookup"><span data-stu-id="10322-1764">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="10322-1765">Simplificado o layout da tabela para a lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="10322-1765">Condensed the table layout for task list</span></span>
* <span data-ttu-id="10322-1766">Adicionado suporte para URLs do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="10322-1766">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="10322-1767">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-1767">ACS</span></span>
* <span data-ttu-id="10322-1768">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="10322-1768">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="10322-1769">Removido “(VISUALIZAÇÃO)” de argumentos do AAD para `aks create`</span><span class="sxs-lookup"><span data-stu-id="10322-1769">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="10322-1770">[PRETERIDO] Comandos `az acs` preteridos.</span><span class="sxs-lookup"><span data-stu-id="10322-1770">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="10322-1771">O serviço ACS será desativado em 31 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="10322-1771">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="10322-1772">Adicionado suporte da Política de Rede durante a criação de novos clusters AKS</span><span class="sxs-lookup"><span data-stu-id="10322-1772">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="10322-1773">Removido o requisito do argumento `--nodepool-name` para `aks scale` se houver apenas um pool de nós</span><span class="sxs-lookup"><span data-stu-id="10322-1773">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-1774">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-1774">Appservice</span></span>
* <span data-ttu-id="10322-1775">Corrigido o problema em que `webapp config container` não honra o parâmetro `--slot`</span><span class="sxs-lookup"><span data-stu-id="10322-1775">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="10322-1776">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="10322-1776">Botservice</span></span>
* <span data-ttu-id="10322-1777">Suporte adicionado para análise do arquivo `.bot` ao chamar `bot show`</span><span class="sxs-lookup"><span data-stu-id="10322-1777">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="10322-1778">Corrigido o bug de provisionamento do AppInsights</span><span class="sxs-lookup"><span data-stu-id="10322-1778">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="10322-1779">Corrigido o bug de espaço em branco ao lidar com caminhos de arquivo</span><span class="sxs-lookup"><span data-stu-id="10322-1779">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="10322-1780">Reduzidas as chamadas de rede do Kudu</span><span class="sxs-lookup"><span data-stu-id="10322-1780">Reduced Kudu network calls</span></span>
* <span data-ttu-id="10322-1781">Melhorias de UX para comandos gerais</span><span class="sxs-lookup"><span data-stu-id="10322-1781">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="10322-1782">Consumo</span><span class="sxs-lookup"><span data-stu-id="10322-1782">Consumption</span></span>
* <span data-ttu-id="10322-1783">Corrigidos os bugs da API de orçamento ao mostrar notificações</span><span class="sxs-lookup"><span data-stu-id="10322-1783">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="10322-1784">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="10322-1784">CosmosDB</span></span>
* <span data-ttu-id="10322-1785">Suporte adicionado para atualizar a conta de vários mestres para mestre único</span><span class="sxs-lookup"><span data-stu-id="10322-1785">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="10322-1786">Mapas</span><span class="sxs-lookup"><span data-stu-id="10322-1786">Maps</span></span>
* <span data-ttu-id="10322-1787">Adicionado suporte ao SKU S1 para `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1787">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="10322-1788">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-1788">Network</span></span>
* <span data-ttu-id="10322-1789">Adicionado suporte para `--format` e `--log-version` para `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="10322-1789">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="10322-1790">Corrigido o problema com `dns zone update` em que usar "" para limpar a resolução e o registro de redes virtuais não funcionava</span><span class="sxs-lookup"><span data-stu-id="10322-1790">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="10322-1791">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-1791">Resource</span></span>
* <span data-ttu-id="10322-1792">Corrigido o tratamento do parâmetro de escopo para grupos de gerenciamento do `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1792">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="10322-1793">Adicionado o novo comando `resource wait`</span><span class="sxs-lookup"><span data-stu-id="10322-1793">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="10322-1794">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-1794">Storage</span></span>
*  <span data-ttu-id="10322-1795">Adicionada a capacidade de atualizar a versão do esquema de log para serviços de armazenamento no `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="10322-1795">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="10322-1796">VM</span><span class="sxs-lookup"><span data-stu-id="10322-1796">VM</span></span>
* <span data-ttu-id="10322-1797">Corrigida a falha em `vm identity remove` quando a VM especificada não tem nenhuma identidade de serviço gerenciado atribuída</span><span class="sxs-lookup"><span data-stu-id="10322-1797">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="10322-1798">4 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-1798">December 4, 2018</span></span>

<span data-ttu-id="10322-1799">Versão 2.0.52</span><span class="sxs-lookup"><span data-stu-id="10322-1799">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="10322-1800">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-1800">Core</span></span>
* <span data-ttu-id="10322-1801">Adicionado suporte para provisionamento de recursos de locatários cruzados para a entidade de serviço de multilocatários</span><span class="sxs-lookup"><span data-stu-id="10322-1801">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="10322-1802">Corrigido o bug onde as ids enviadas por pipe de um comando com a saída tsv eram analisados incorretamente</span><span class="sxs-lookup"><span data-stu-id="10322-1802">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-1803">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-1803">Appservice</span></span>
* <span data-ttu-id="10322-1804">[VERSÃO PRÉVIA] Adicionado o comando `webapp up` que ajuda a criar e implantar conteúdo em aplicativo</span><span class="sxs-lookup"><span data-stu-id="10322-1804">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="10322-1805">Corrigido um bug no aplicativo com base em contêiner do Windows devido à alteração de back-end</span><span class="sxs-lookup"><span data-stu-id="10322-1805">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="10322-1806">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-1806">Network</span></span>
* <span data-ttu-id="10322-1807">Adicionado o argumento `--exclusion` a `application-gateway waf-config set` para dar suporte a exclusões de WAF</span><span class="sxs-lookup"><span data-stu-id="10322-1807">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="10322-1808">Função</span><span class="sxs-lookup"><span data-stu-id="10322-1808">Role</span></span>
* <span data-ttu-id="10322-1809">Adicionado suporte para identificadores personalizados para a credencial de senha</span><span class="sxs-lookup"><span data-stu-id="10322-1809">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="10322-1810">VM</span><span class="sxs-lookup"><span data-stu-id="10322-1810">VM</span></span>
* <span data-ttu-id="10322-1811">[PRETERIDO] Parâmetro `vm extension [show|wait] --expand` preterido</span><span class="sxs-lookup"><span data-stu-id="10322-1811">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="10322-1812">Adicionado parâmetro `--force` a `vm restart` para reimplantar as VMs sem resposta</span><span class="sxs-lookup"><span data-stu-id="10322-1812">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="10322-1813">Alterado `[vm|vmss] create --authentication-type` para aceitar "todos" para criar uma VM com senha e autenticação SSH</span><span class="sxs-lookup"><span data-stu-id="10322-1813">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="10322-1814">Adicionado parâmetro `image create --os-disk-caching` para definir o cache de disco do sistema operacional para uma imagem</span><span class="sxs-lookup"><span data-stu-id="10322-1814">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="10322-1815">20 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-1815">November 20, 2018</span></span>

<span data-ttu-id="10322-1816">Versão 2.0.51</span><span class="sxs-lookup"><span data-stu-id="10322-1816">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="10322-1817">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-1817">Core</span></span>
* <span data-ttu-id="10322-1818">Logon do MSI alterado para não reutilizar o nome da assinatura na identidade</span><span class="sxs-lookup"><span data-stu-id="10322-1818">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="10322-1819">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-1819">ACR</span></span>
* <span data-ttu-id="10322-1820">Token de contexto adicionado à etapa da tarefa</span><span class="sxs-lookup"><span data-stu-id="10322-1820">Added context token to task step</span></span>
* <span data-ttu-id="10322-1821">Suporte adicionado para definir segredos na execução do acr para espelhar a tarefa do acr</span><span class="sxs-lookup"><span data-stu-id="10322-1821">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="10322-1822">Suporte aprimorado para `--top` e `--orderby` para os comandos `show-tags` e `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="10322-1822">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-1823">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-1823">Appservice</span></span>
* <span data-ttu-id="10322-1824">Tempo limite padrão para a implantação do zip alterado para sondar o status aumentado para 5 minutos, também adicionando uma propriedade de tempo limite para personalizar esse valor</span><span class="sxs-lookup"><span data-stu-id="10322-1824">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="10322-1825">Padrão `node_version` atualizado.</span><span class="sxs-lookup"><span data-stu-id="10322-1825">Updated the default `node_version`.</span></span> <span data-ttu-id="10322-1826">Redefinir a ação de troca de slots durante uma troca de duas fases preserva todas as configurações do aplicativo e cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="10322-1826">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="10322-1827">Verificação da SKU no lado do cliente removida para o Linux criar o plano do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="10322-1827">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="10322-1828">Erro corrigido ao tentar obter o status de implantação do zip</span><span class="sxs-lookup"><span data-stu-id="10322-1828">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="10322-1829">Iot Central</span><span class="sxs-lookup"><span data-stu-id="10322-1829">IotCentral</span></span>
* <span data-ttu-id="10322-1830">Verificação de disponibilidade do subdomínio adicionada ao criar um aplicativo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="10322-1830">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="10322-1831">KeyVault</span><span class="sxs-lookup"><span data-stu-id="10322-1831">KeyVault</span></span>
* <span data-ttu-id="10322-1832">Bug corrigido em que os erros podem ter sido ignorados</span><span class="sxs-lookup"><span data-stu-id="10322-1832">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="10322-1833">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-1833">Network</span></span>
* <span data-ttu-id="10322-1834">Subcomandos `root-cert` adicionados a `application-gateway` para lidar com os certificados de raiz confiável</span><span class="sxs-lookup"><span data-stu-id="10322-1834">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="10322-1835">Opções `--min-capacity` e `--custom-error-pages` adicionadas a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="10322-1835">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="10322-1836">`--zones` adicionado para suporte da zona de disponibilidade a `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="10322-1836">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="10322-1837">Argumentos `--file-upload-limit`, `--max-request-body-size` e `--request-body-check` a `application-gateway waf-config set` adicionados</span><span class="sxs-lookup"><span data-stu-id="10322-1837">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="10322-1838">Rdbms</span><span class="sxs-lookup"><span data-stu-id="10322-1838">Rdbms</span></span>
* <span data-ttu-id="10322-1839">Comandos vnet do mariadb adicionados</span><span class="sxs-lookup"><span data-stu-id="10322-1839">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="10322-1840">Rbac</span><span class="sxs-lookup"><span data-stu-id="10322-1840">Rbac</span></span>
* <span data-ttu-id="10322-1841">Um problema corrigido ao tentar atualizar credenciais inalteradas em `ad app update`</span><span class="sxs-lookup"><span data-stu-id="10322-1841">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="10322-1842">Avisos de saída adicionados para comunicar alterações de falha em um futuro próximo para `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="10322-1842">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="10322-1843">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-1843">Storage</span></span>
* <span data-ttu-id="10322-1844">Melhor manipulação de casos incomuns para os comandos da cópia de armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-1844">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="10322-1845">Corrigido o problema em que `storage blob copy start-batch` não usava credenciais de logon quando as contas de origem e destino eram iguais</span><span class="sxs-lookup"><span data-stu-id="10322-1845">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="10322-1846">Bug corrigido com `storage [blob|file] url` em que `sas_token` não foi incorporado na URL</span><span class="sxs-lookup"><span data-stu-id="10322-1846">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="10322-1847">Aviso de alteração da falha adicionado a `[blob|container] list`: produzirá apenas os primeiros 5.000 resultados por padrão</span><span class="sxs-lookup"><span data-stu-id="10322-1847">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="10322-1848">VM</span><span class="sxs-lookup"><span data-stu-id="10322-1848">VM</span></span>
* <span data-ttu-id="10322-1849">Suporte adicionado a `[vm|vmss] create --storage-sku` para especificar a SKU da conta de armazenamento para o SO gerenciado e os discos de dados separadamente</span><span class="sxs-lookup"><span data-stu-id="10322-1849">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="10322-1850">Parâmetros do nome da versão alterados de `sig image-version` para `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="10322-1850">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="10322-1851">Argumento `sig image-version` preterido `--image-version-name`, substituído por `--image-version`</span><span class="sxs-lookup"><span data-stu-id="10322-1851">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="10322-1852">Suporte adicionado para usar o disco local do SO a `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="10322-1852">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="10322-1853">Adicionado o suporte ao `--no-wait` para `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="10322-1853">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="10322-1854">Adicionado o comando `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="10322-1854">Added `snapshot wait` command</span></span>
* <span data-ttu-id="10322-1855">Suporte adicionado para usar o nome da instância com `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="10322-1855">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="10322-1856">6 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-1856">November 6, 2018</span></span>

<span data-ttu-id="10322-1857">Versão 2.0.50</span><span class="sxs-lookup"><span data-stu-id="10322-1857">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="10322-1858">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-1858">Core</span></span>
* <span data-ttu-id="10322-1859">Foi adicionado suporte para o serviço principal sn + autenticação do emissor</span><span class="sxs-lookup"><span data-stu-id="10322-1859">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="10322-1860">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-1860">ACR</span></span>
* <span data-ttu-id="10322-1861">Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa</span><span class="sxs-lookup"><span data-stu-id="10322-1861">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="10322-1862">Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação</span><span class="sxs-lookup"><span data-stu-id="10322-1862">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="10322-1863">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-1863">ACS</span></span>
* <span data-ttu-id="10322-1864">[ALTERAÇÃO SIGNIFICATIVA]`enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão</span><span class="sxs-lookup"><span data-stu-id="10322-1864">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="10322-1865">Supervisor</span><span class="sxs-lookup"><span data-stu-id="10322-1865">Advisor</span></span>
* <span data-ttu-id="10322-1866">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="10322-1866">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="10322-1867">AMS</span><span class="sxs-lookup"><span data-stu-id="10322-1867">AMS</span></span>
* <span data-ttu-id="10322-1868">Novos grupos de comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="10322-1868">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="10322-1869">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="10322-1869">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="10322-1870">Adicionados parâmetros de criptografia com suporte para `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="10322-1870">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="10322-1871">O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido</span><span class="sxs-lookup"><span data-stu-id="10322-1871">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="10322-1872">Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="10322-1872">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="10322-1873">Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="10322-1873">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="10322-1874">Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="10322-1874">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="10322-1875">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming locator` foi substituído por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="10322-1875">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="10322-1876">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--content-keys` de `ams streaming locator` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="10322-1876">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="10322-1877">[ALTERAÇÃO SIGNIFICATIVA]`--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="10322-1877">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="10322-1878">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming policy` foi substituído por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="10322-1878">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="10322-1879">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="10322-1879">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="10322-1880">Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="10322-1880">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="10322-1881">Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado</span><span class="sxs-lookup"><span data-stu-id="10322-1881">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="10322-1882">[ALTERAÇÃO SIGNIFICATIVA]`--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="10322-1882">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="10322-1883">Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'.</span><span class="sxs-lookup"><span data-stu-id="10322-1883">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="10322-1884">Um ativo sem rótulo pode ser enviado assim: 'assetName='</span><span class="sxs-lookup"><span data-stu-id="10322-1884">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-1885">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-1885">AppService</span></span>
* <span data-ttu-id="10322-1886">Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido</span><span class="sxs-lookup"><span data-stu-id="10322-1886">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="10322-1887">Configurar</span><span class="sxs-lookup"><span data-stu-id="10322-1887">Configure</span></span>
* <span data-ttu-id="10322-1888">O YAML foi adicionado às opções de formato de saída</span><span class="sxs-lookup"><span data-stu-id="10322-1888">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="10322-1889">Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-1889">Container</span></span>
* <span data-ttu-id="10322-1890">Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml</span><span class="sxs-lookup"><span data-stu-id="10322-1890">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="10322-1891">EventHub</span><span class="sxs-lookup"><span data-stu-id="10322-1891">EventHub</span></span>
* <span data-ttu-id="10322-1892">O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1892">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="10322-1893">Interativo</span><span class="sxs-lookup"><span data-stu-id="10322-1893">Interactive</span></span>
* <span data-ttu-id="10322-1894">O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos</span><span class="sxs-lookup"><span data-stu-id="10322-1894">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-1895">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-1895">Monitor</span></span>
* <span data-ttu-id="10322-1896">Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) para `--condition` em `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-1896">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="10322-1897">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-1897">Network</span></span>
* <span data-ttu-id="10322-1898">Os nomes de comandos `network interface-endpoint` foram preteridos em benefício de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="10322-1898">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="10322-1899">Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID</span><span class="sxs-lookup"><span data-stu-id="10322-1899">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="10322-1900">Foi corrigido um problema onde `--ip-tags` não funcionava corretamente com `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="10322-1900">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="10322-1901">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-1901">Profile</span></span>
* <span data-ttu-id="10322-1902">`--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado</span><span class="sxs-lookup"><span data-stu-id="10322-1902">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="10322-1903">RDBMS</span><span class="sxs-lookup"><span data-stu-id="10322-1903">RDBMS</span></span>
* <span data-ttu-id="10322-1904">Adicionados comandos da réplica mysql</span><span class="sxs-lookup"><span data-stu-id="10322-1904">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="10322-1905">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-1905">Resource</span></span>
* <span data-ttu-id="10322-1906">Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="10322-1906">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="10322-1907">Função</span><span class="sxs-lookup"><span data-stu-id="10322-1907">Role</span></span>
* <span data-ttu-id="10322-1908">Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais</span><span class="sxs-lookup"><span data-stu-id="10322-1908">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="10322-1909">`ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="10322-1909">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="10322-1910">Suporte adicionado para conceder permissões a aplicativos do AAD</span><span class="sxs-lookup"><span data-stu-id="10322-1910">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="10322-1911">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-1911">Storage</span></span>
* <span data-ttu-id="10322-1912">Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="10322-1912">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="10322-1913">VM</span><span class="sxs-lookup"><span data-stu-id="10322-1913">VM</span></span>
* <span data-ttu-id="10322-1914">O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem</span><span class="sxs-lookup"><span data-stu-id="10322-1914">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="10322-1915">O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido</span><span class="sxs-lookup"><span data-stu-id="10322-1915">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="10322-1916">O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado</span><span class="sxs-lookup"><span data-stu-id="10322-1916">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="10322-1917">`vm secret format` foi alterado para exigir a saída json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="10322-1917">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="10322-1918">Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido</span><span class="sxs-lookup"><span data-stu-id="10322-1918">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="10322-1919">Validação de argumento aprimorado para `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="10322-1919">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="10322-1920">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-1920">October 23, 2018</span></span>

<span data-ttu-id="10322-1921">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="10322-1921">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="10322-1922">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-1922">Core</span></span>
* <span data-ttu-id="10322-1923">Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`</span><span class="sxs-lookup"><span data-stu-id="10322-1923">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="10322-1924">Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="10322-1924">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="10322-1925">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-1925">ACR</span></span>
* <span data-ttu-id="10322-1926">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="10322-1926">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="10322-1927">CDN</span><span class="sxs-lookup"><span data-stu-id="10322-1927">CDN</span></span>
* <span data-ttu-id="10322-1928">[ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="10322-1928">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="10322-1929">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="10322-1929">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="10322-1930">Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-1930">Container</span></span>
* <span data-ttu-id="10322-1931">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="10322-1931">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="10322-1932">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="10322-1932">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="10322-1933">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="10322-1933">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="10322-1934">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="10322-1934">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="10322-1935">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="10322-1935">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="10322-1936">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="10322-1936">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="10322-1937">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="10322-1937">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="10322-1938">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="10322-1938">CosmosDB</span></span>
* <span data-ttu-id="10322-1939">Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="10322-1939">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="10322-1940">Interativo</span><span class="sxs-lookup"><span data-stu-id="10322-1940">Interactive</span></span>
* <span data-ttu-id="10322-1941">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="10322-1941">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="10322-1942">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="10322-1942">IoT Central</span></span>
* <span data-ttu-id="10322-1943">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="10322-1943">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="10322-1944">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="10322-1944">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-1945">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-1945">Monitor</span></span>
* <span data-ttu-id="10322-1946">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="10322-1946">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="10322-1947">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="10322-1947">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="10322-1948">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="10322-1948">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="10322-1949">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="10322-1949">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="10322-1950">Adicionado `--namespace` como alias para a opção preterida `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="10322-1950">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="10322-1951">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="10322-1951">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="10322-1952">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="10322-1952">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="10322-1953">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="10322-1953">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="10322-1954">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="10322-1954">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="10322-1955">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="10322-1955">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="10322-1956">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-1956">Network</span></span>
* <span data-ttu-id="10322-1957">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="10322-1957">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="10322-1958">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="10322-1958">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="10322-1959">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="10322-1959">ServiceBus</span></span>
* <span data-ttu-id="10322-1960">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="10322-1960">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="10322-1961">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-1961">SQL</span></span>
* <span data-ttu-id="10322-1962">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="10322-1962">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="10322-1963">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-1963">Storage</span></span>
* <span data-ttu-id="10322-1964">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="10322-1964">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="10322-1965">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="10322-1965">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="10322-1966">VM</span><span class="sxs-lookup"><span data-stu-id="10322-1966">VM</span></span>
* <span data-ttu-id="10322-1967">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="10322-1967">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="10322-1968">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`</span><span class="sxs-lookup"><span data-stu-id="10322-1968">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="10322-1969">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`</span><span class="sxs-lookup"><span data-stu-id="10322-1969">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="10322-1970">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-1970">October 16, 2018</span></span>

<span data-ttu-id="10322-1971">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="10322-1971">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="10322-1972">VM</span><span class="sxs-lookup"><span data-stu-id="10322-1972">VM</span></span>
* <span data-ttu-id="10322-1973">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="10322-1973">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="10322-1974">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-1974">October 9, 2018</span></span>

<span data-ttu-id="10322-1975">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="10322-1975">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="10322-1976">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-1976">Core</span></span>
* <span data-ttu-id="10322-1977">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="10322-1977">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="10322-1978">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-1978">ACR</span></span>
* <span data-ttu-id="10322-1979">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="10322-1979">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="10322-1980">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-1980">ACS</span></span>
* <span data-ttu-id="10322-1981">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="10322-1981">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="10322-1982">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="10322-1982">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="10322-1983">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="10322-1983">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="10322-1984">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="10322-1984">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="10322-1985">Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-1985">Container</span></span>
* <span data-ttu-id="10322-1986">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um runtime específico</span><span class="sxs-lookup"><span data-stu-id="10322-1986">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="10322-1987">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="10322-1987">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="10322-1988">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="10322-1988">Event Hub</span></span>
* <span data-ttu-id="10322-1989">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="10322-1989">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="10322-1990">[ALTERAÇÃO SIGNIFICATIVA]`list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="10322-1990">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="10322-1991">Extensões</span><span class="sxs-lookup"><span data-stu-id="10322-1991">Extensions</span></span>
* <span data-ttu-id="10322-1992">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="10322-1992">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="10322-1993">HDInsight</span><span class="sxs-lookup"><span data-stu-id="10322-1993">HDInsight</span></span>
* <span data-ttu-id="10322-1994">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="10322-1994">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="10322-1995">IoT</span><span class="sxs-lookup"><span data-stu-id="10322-1995">IoT</span></span>
* <span data-ttu-id="10322-1996">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="10322-1996">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="10322-1997">KeyVault</span><span class="sxs-lookup"><span data-stu-id="10322-1997">KeyVault</span></span>
* <span data-ttu-id="10322-1998">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="10322-1998">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="10322-1999">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-1999">Network</span></span>
* <span data-ttu-id="10322-2000">Corrigido `network dns zone create`: O comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="10322-2000">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="10322-2001">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="10322-2001">See #6052</span></span>
* <span data-ttu-id="10322-2002">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="10322-2002">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="10322-2003">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="10322-2003">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="10322-2004">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="10322-2004">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="10322-2005">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="10322-2005">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="10322-2006">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="10322-2006">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="10322-2007">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="10322-2007">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="10322-2008">Função</span><span class="sxs-lookup"><span data-stu-id="10322-2008">Role</span></span>
* <span data-ttu-id="10322-2009">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="10322-2009">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="10322-2010">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="10322-2010">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="10322-2011">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="10322-2011">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="10322-2012">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="10322-2012">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="10322-2013">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="10322-2013">Service Bus</span></span>
* <span data-ttu-id="10322-2014">[ALTERAÇÃO SIGNIFICATIVA]`list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="10322-2014">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="10322-2015">VM</span><span class="sxs-lookup"><span data-stu-id="10322-2015">VM</span></span>
* <span data-ttu-id="10322-2016">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="10322-2016">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="10322-2017">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="10322-2017">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="10322-2018">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="10322-2018">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="10322-2019">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="10322-2019">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="10322-2020">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="10322-2020">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="10322-2021">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="10322-2021">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="10322-2022">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2022">September 21, 2018</span></span>

<span data-ttu-id="10322-2023">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="10322-2023">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="10322-2024">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-2024">ACR</span></span>
* <span data-ttu-id="10322-2025">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="10322-2025">Added ACR Task commands</span></span>
* <span data-ttu-id="10322-2026">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="10322-2026">Added quick run command</span></span>
* <span data-ttu-id="10322-2027">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="10322-2027">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="10322-2028">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="10322-2028">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="10322-2029">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="10322-2029">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="10322-2030">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="10322-2030">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="10322-2031">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-2031">ACS</span></span>
* <span data-ttu-id="10322-2032">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="10322-2032">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="10322-2033">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="10322-2033">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-2034">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-2034">AppService</span></span>

* <span data-ttu-id="10322-2035">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="10322-2035">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="10322-2036">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="10322-2036">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="10322-2037">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="10322-2037">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="10322-2038">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="10322-2038">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="10322-2039">Lote</span><span class="sxs-lookup"><span data-stu-id="10322-2039">Batch</span></span>
* <span data-ttu-id="10322-2040">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="10322-2040">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="10322-2041">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="10322-2041">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="10322-2042">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="10322-2042">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="10322-2043">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="10322-2043">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="10322-2044">Lote AI</span><span class="sxs-lookup"><span data-stu-id="10322-2044">Batch AI</span></span> 
* <span data-ttu-id="10322-2045">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="10322-2045">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="10322-2046">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="10322-2046">Cognitive Services</span></span>
* <span data-ttu-id="10322-2047">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="10322-2047">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="10322-2048">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="10322-2048">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="10322-2049">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="10322-2049">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="10322-2050">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="10322-2050">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="10322-2051">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="10322-2051">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="10322-2052">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="10322-2052">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="10322-2053">Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-2053">Container</span></span>
* <span data-ttu-id="10322-2054">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="10322-2054">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="10322-2055">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="10322-2055">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="10322-2056">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="10322-2056">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="10322-2057">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="10322-2057">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="10322-2058">DataLake</span><span class="sxs-lookup"><span data-stu-id="10322-2058">Datalake</span></span>
* <span data-ttu-id="10322-2059">Comandos adicionados para regras da rede virtual</span><span class="sxs-lookup"><span data-stu-id="10322-2059">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="10322-2060">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="10322-2060">Interactive Shell</span></span>
* <span data-ttu-id="10322-2061">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="10322-2061">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="10322-2062">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="10322-2062">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="10322-2063">IoT</span><span class="sxs-lookup"><span data-stu-id="10322-2063">IoT</span></span>
* <span data-ttu-id="10322-2064">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="10322-2064">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="10322-2065">Key Vault</span><span class="sxs-lookup"><span data-stu-id="10322-2065">Key Vault</span></span>
* <span data-ttu-id="10322-2066">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="10322-2066">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="10322-2067">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-2067">Network</span></span>
* <span data-ttu-id="10322-2068">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="10322-2068">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="10322-2069">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="10322-2069">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="10322-2070">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="10322-2070">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="10322-2071">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="10322-2071">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="10322-2072">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="10322-2072">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="10322-2073">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="10322-2073">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="10322-2074">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="10322-2074">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="10322-2075">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="10322-2075">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="10322-2076">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="10322-2076">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="10322-2077">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="10322-2077">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="10322-2078">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="10322-2078">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="10322-2079">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="10322-2079">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="10322-2080">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="10322-2080">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="10322-2081">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="10322-2081">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="10322-2082">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="10322-2082">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="10322-2083">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="10322-2083">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="10322-2084">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="10322-2084">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="10322-2085">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="10322-2085">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="10322-2086">RDBMS</span><span class="sxs-lookup"><span data-stu-id="10322-2086">RDBMS</span></span>
* <span data-ttu-id="10322-2087">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="10322-2087">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="10322-2088">Reserva</span><span class="sxs-lookup"><span data-stu-id="10322-2088">Reservation</span></span>
* <span data-ttu-id="10322-2089">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="10322-2089">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="10322-2090">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="10322-2090">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="10322-2091">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="10322-2091">Manage App</span></span>
* <span data-ttu-id="10322-2092">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="10322-2092">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="10322-2093">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="10322-2093">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="10322-2094">Função</span><span class="sxs-lookup"><span data-stu-id="10322-2094">Role</span></span>
* <span data-ttu-id="10322-2095">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="10322-2095">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="10322-2096">SignalR</span><span class="sxs-lookup"><span data-stu-id="10322-2096">SignalR</span></span>
* <span data-ttu-id="10322-2097">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="10322-2097">First release</span></span>

### <a name="storage"></a><span data-ttu-id="10322-2098">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-2098">Storage</span></span>
* <span data-ttu-id="10322-2099">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="10322-2099">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="10322-2100">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="10322-2100">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="10322-2101">VM</span><span class="sxs-lookup"><span data-stu-id="10322-2101">VM</span></span>
* <span data-ttu-id="10322-2102">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="10322-2102">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="10322-2103">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="10322-2103">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="10322-2104">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2104">August 28, 2018</span></span>

<span data-ttu-id="10322-2105">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="10322-2105">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="10322-2106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-2106">Core</span></span>

* <span data-ttu-id="10322-2107">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="10322-2107">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="10322-2108">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="10322-2108">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="10322-2109">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-2109">ACR</span></span>

* <span data-ttu-id="10322-2110">Adicionada uma solução alternativa para operações de runtime sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="10322-2110">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="10322-2111">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="10322-2111">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="10322-2112">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-2112">ACS</span></span>

* <span data-ttu-id="10322-2113">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="10322-2113">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="10322-2114">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="10322-2114">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-2115">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-2115">AppService</span></span>

* <span data-ttu-id="10322-2116">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="10322-2116">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="10322-2117">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="10322-2117">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="10322-2118">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="10322-2118">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="10322-2119">Backup</span><span class="sxs-lookup"><span data-stu-id="10322-2119">Backup</span></span>

* <span data-ttu-id="10322-2120">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="10322-2120">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="10322-2121">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="10322-2121">Bot Service</span></span>

* <span data-ttu-id="10322-2122">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="10322-2122">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="10322-2123">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="10322-2123">Cognitive Services</span></span>

* <span data-ttu-id="10322-2124">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="10322-2124">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="10322-2125">IoT</span><span class="sxs-lookup"><span data-stu-id="10322-2125">IoT</span></span>

* <span data-ttu-id="10322-2126">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="10322-2126">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-2127">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-2127">Monitor</span></span>

* <span data-ttu-id="10322-2128">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="10322-2128">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="10322-2129">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="10322-2129">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="10322-2130">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-2130">Network</span></span>

* <span data-ttu-id="10322-2131">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="10322-2131">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="10322-2132">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-2132">Resource</span></span>

* <span data-ttu-id="10322-2133">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="10322-2133">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="10322-2134">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-2134">Storage</span></span>

* <span data-ttu-id="10322-2135">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="10322-2135">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="10322-2136">VM</span><span class="sxs-lookup"><span data-stu-id="10322-2136">VM</span></span>

* <span data-ttu-id="10322-2137">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="10322-2137">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="10322-2138">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="10322-2138">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="10322-2139">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2139">Auguest 14, 2018</span></span>

<span data-ttu-id="10322-2140">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="10322-2140">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="10322-2141">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-2141">Core</span></span>

* <span data-ttu-id="10322-2142">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="10322-2142">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="10322-2143">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="10322-2143">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="10322-2144">Telemetria</span><span class="sxs-lookup"><span data-stu-id="10322-2144">Telemetry</span></span>

* <span data-ttu-id="10322-2145">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="10322-2145">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="10322-2146">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-2146">ACR</span></span>

* <span data-ttu-id="10322-2147">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="10322-2147">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="10322-2148">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="10322-2148">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="10322-2149">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-2149">ACS</span></span>

* <span data-ttu-id="10322-2150">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="10322-2150">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="10322-2151">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="10322-2151">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="10322-2152">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="10322-2152">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="10322-2153">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="10322-2153">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="10322-2154">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="10322-2154">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="10322-2155">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-2155">AppService</span></span>

* <span data-ttu-id="10322-2156">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="10322-2156">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="10322-2157">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="10322-2157">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="10322-2158">BatchAI</span><span class="sxs-lookup"><span data-stu-id="10322-2158">BatchAI</span></span>

* <span data-ttu-id="10322-2159">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="10322-2159">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="10322-2160">Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-2160">Container</span></span>

* <span data-ttu-id="10322-2161">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-2161">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="10322-2162">IoT</span><span class="sxs-lookup"><span data-stu-id="10322-2162">IoT</span></span>

* <span data-ttu-id="10322-2163">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="10322-2163">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="10322-2164">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="10322-2164">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="10322-2165">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="10322-2165">Iot Central</span></span>

* <span data-ttu-id="10322-2166">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="10322-2166">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="10322-2167">KeyVault</span><span class="sxs-lookup"><span data-stu-id="10322-2167">KeyVault</span></span>


* <span data-ttu-id="10322-2168">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="10322-2168">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="10322-2169">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="10322-2169">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="10322-2170">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="10322-2170">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="10322-2171">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="10322-2171">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="10322-2172">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="10322-2172">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="10322-2173">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="10322-2173">Relay</span></span>

* <span data-ttu-id="10322-2174">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="10322-2174">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="10322-2175">Sql</span><span class="sxs-lookup"><span data-stu-id="10322-2175">Sql</span></span>

* <span data-ttu-id="10322-2176">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="10322-2176">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="10322-2177">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-2177">Storage</span></span>

* <span data-ttu-id="10322-2178">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="10322-2178">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="10322-2179">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="10322-2179">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="10322-2180">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="10322-2180">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="10322-2181">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="10322-2181">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="10322-2182">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-2182">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="10322-2183">VM</span><span class="sxs-lookup"><span data-stu-id="10322-2183">VM</span></span>

* <span data-ttu-id="10322-2184">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="10322-2184">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="10322-2185">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2185">July 31, 2018</span></span>

<span data-ttu-id="10322-2186">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="10322-2186">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="10322-2187">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-2187">ACR</span></span>

* <span data-ttu-id="10322-2188">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="10322-2188">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="10322-2189">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="10322-2189">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="10322-2190">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-2190">ACS</span></span>

* <span data-ttu-id="10322-2191">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="10322-2191">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="10322-2192">Lote</span><span class="sxs-lookup"><span data-stu-id="10322-2192">Batch</span></span>

* <span data-ttu-id="10322-2193">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="10322-2193">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="10322-2194">Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-2194">Container</span></span>

* <span data-ttu-id="10322-2195">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="10322-2195">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="10322-2196">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-2196">Network</span></span>

* <span data-ttu-id="10322-2197">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="10322-2197">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="10322-2198">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-2198">Resource</span></span>

* <span data-ttu-id="10322-2199">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="10322-2199">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="10322-2200">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="10322-2200">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="10322-2201">Função</span><span class="sxs-lookup"><span data-stu-id="10322-2201">Role</span></span>

* <span data-ttu-id="10322-2202">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="10322-2202">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="10322-2203">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="10322-2203">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="10322-2204">Search</span><span class="sxs-lookup"><span data-stu-id="10322-2204">Search</span></span>

* <span data-ttu-id="10322-2205">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="10322-2205">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="10322-2206">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="10322-2206">Service Bus</span></span>

* <span data-ttu-id="10322-2207">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="10322-2207">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="10322-2208">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="10322-2208">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="10322-2209">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="10322-2209">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="10322-2210">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="10322-2210">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="10322-2211">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-2211">Storage</span></span>

* <span data-ttu-id="10322-2212">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="10322-2212">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="10322-2213">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="10322-2213">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="10322-2214">VM</span><span class="sxs-lookup"><span data-stu-id="10322-2214">VM</span></span>

* <span data-ttu-id="10322-2215">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="10322-2215">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="10322-2216">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="10322-2216">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="10322-2217">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="10322-2217">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="10322-2218">[ALTERAÇÃO SIGNIFICATIVA]`[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="10322-2218">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="10322-2219">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2219">July 18, 2018</span></span>

<span data-ttu-id="10322-2220">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="10322-2220">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="10322-2221">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-2221">Core</span></span>

* <span data-ttu-id="10322-2222">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="10322-2222">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="10322-2223">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="10322-2223">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="10322-2224">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="10322-2224">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="10322-2225">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-2225">ACR</span></span>

* <span data-ttu-id="10322-2226">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="10322-2226">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="10322-2227">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="10322-2227">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="10322-2228">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="10322-2228">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="10322-2229">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="10322-2229">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="10322-2230">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-2230">ACS</span></span>

* <span data-ttu-id="10322-2231">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="10322-2231">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-2232">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-2232">AppService</span></span>

* <span data-ttu-id="10322-2233">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="10322-2233">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="10322-2234">Lote</span><span class="sxs-lookup"><span data-stu-id="10322-2234">Batch</span></span>

* <span data-ttu-id="10322-2235">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="10322-2235">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="10322-2236">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="10322-2236">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="10322-2237">Lote AI</span><span class="sxs-lookup"><span data-stu-id="10322-2237">Batch AI</span></span>

* <span data-ttu-id="10322-2238">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="10322-2238">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="10322-2239">Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-2239">Container</span></span>

* <span data-ttu-id="10322-2240">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="10322-2240">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="10322-2241">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="10322-2241">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="10322-2242">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-2242">Network</span></span>

* <span data-ttu-id="10322-2243">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="10322-2243">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="10322-2244">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="10322-2244">Added `network nic wait`</span></span>
* <span data-ttu-id="10322-2245">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="10322-2245">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="10322-2246">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="10322-2246">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="10322-2247">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-2247">Resource</span></span>

* <span data-ttu-id="10322-2248">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="10322-2248">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="10322-2249">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="10322-2249">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="10322-2250">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="10322-2250">Added `deployment wait` command</span></span>
* <span data-ttu-id="10322-2251">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="10322-2251">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="10322-2252">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-2252">SQL</span></span>

* <span data-ttu-id="10322-2253">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="10322-2253">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="10322-2254">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="10322-2254">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="10322-2255">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="10322-2255">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="10322-2256">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-2256">Storage</span></span>

* <span data-ttu-id="10322-2257">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="10322-2257">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="10322-2258">VM</span><span class="sxs-lookup"><span data-stu-id="10322-2258">VM</span></span>

* <span data-ttu-id="10322-2259">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="10322-2259">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="10322-2260">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="10322-2260">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="10322-2261">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="10322-2261">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="10322-2262">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2262">July 3, 2018</span></span>

<span data-ttu-id="10322-2263">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="10322-2263">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="10322-2264">AKS</span><span class="sxs-lookup"><span data-stu-id="10322-2264">AKS</span></span>

* <span data-ttu-id="10322-2265">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="10322-2265">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="10322-2266">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2266">July 3, 2018</span></span>

<span data-ttu-id="10322-2267">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="10322-2267">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="10322-2268">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-2268">Core</span></span>

* <span data-ttu-id="10322-2269">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="10322-2269">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="10322-2270">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-2270">ACR</span></span>

* <span data-ttu-id="10322-2271">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="10322-2271">Added polling build status</span></span>
* <span data-ttu-id="10322-2272">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="10322-2272">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="10322-2273">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="10322-2273">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="10322-2274">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-2274">ACS</span></span>

* <span data-ttu-id="10322-2275">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="10322-2275">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="10322-2276">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="10322-2276">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="10322-2277">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="10322-2277">Updated options for `aks browse` command.</span></span> <span data-ttu-id="10322-2278">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="10322-2278">Added `--listen-port` support</span></span>
* <span data-ttu-id="10322-2279">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="10322-2279">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="10322-2280">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="10322-2280">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="10322-2281">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="10322-2281">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-2282">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-2282">AppService</span></span>

* <span data-ttu-id="10322-2283">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="10322-2283">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="10322-2284">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="10322-2284">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="10322-2285">Backup</span><span class="sxs-lookup"><span data-stu-id="10322-2285">Backup</span></span>

* <span data-ttu-id="10322-2286">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="10322-2286">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="10322-2287">BatchAI</span><span class="sxs-lookup"><span data-stu-id="10322-2287">BatchAI</span></span>

* <span data-ttu-id="10322-2288">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="10322-2288">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="10322-2289">Nuvem</span><span class="sxs-lookup"><span data-stu-id="10322-2289">Cloud</span></span>

* <span data-ttu-id="10322-2290">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="10322-2290">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="10322-2291">Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-2291">Container</span></span>

* <span data-ttu-id="10322-2292">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="10322-2292">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="10322-2293">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="10322-2293">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="10322-2294">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="10322-2294">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="10322-2295">Extensão</span><span class="sxs-lookup"><span data-stu-id="10322-2295">Extension</span></span>

* <span data-ttu-id="10322-2296">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="10322-2296">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="10322-2297">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-2297">Network</span></span>

* <span data-ttu-id="10322-2298">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="10322-2298">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="10322-2299">Rdbms</span><span class="sxs-lookup"><span data-stu-id="10322-2299">Rdbms</span></span>

* <span data-ttu-id="10322-2300">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="10322-2300">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="10322-2301">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-2301">Resource</span></span>

* <span data-ttu-id="10322-2302">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="10322-2302">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="10322-2303">VM</span><span class="sxs-lookup"><span data-stu-id="10322-2303">VM</span></span>

* <span data-ttu-id="10322-2304">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="10322-2304">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="10322-2305">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2305">June 25, 2018</span></span>

<span data-ttu-id="10322-2306">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="10322-2306">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="10322-2307">CLI</span><span class="sxs-lookup"><span data-stu-id="10322-2307">CLI</span></span>

* <span data-ttu-id="10322-2308">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="10322-2308">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="10322-2309">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2309">June 19, 2018</span></span>

<span data-ttu-id="10322-2310">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="10322-2310">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="10322-2311">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-2311">Core</span></span>

* <span data-ttu-id="10322-2312">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="10322-2312">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="10322-2313">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-2313">ACR</span></span>

* <span data-ttu-id="10322-2314">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="10322-2314">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="10322-2315">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="10322-2315">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="10322-2316">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-2316">ACS</span></span>

* <span data-ttu-id="10322-2317">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="10322-2317">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="10322-2318">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="10322-2318">Added `--update` support</span></span>
* <span data-ttu-id="10322-2319">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="10322-2319">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="10322-2320">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="10322-2320">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="10322-2321">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="10322-2321">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="10322-2322">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="10322-2322">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="10322-2323">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="10322-2323">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="10322-2324">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="10322-2324">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-2325">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-2325">AppService</span></span>

* <span data-ttu-id="10322-2326">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="10322-2326">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="10322-2327">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="10322-2327">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="10322-2328">Lote</span><span class="sxs-lookup"><span data-stu-id="10322-2328">Batch</span></span>

* <span data-ttu-id="10322-2329">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="10322-2329">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="10322-2330">Lote AI</span><span class="sxs-lookup"><span data-stu-id="10322-2330">Batch AI</span></span>

* <span data-ttu-id="10322-2331">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="10322-2331">Added support for workspaces.</span></span> <span data-ttu-id="10322-2332">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="10322-2332">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="10322-2333">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="10322-2333">Added support for experiments.</span></span> <span data-ttu-id="10322-2334">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="10322-2334">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="10322-2335">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="10322-2335">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="10322-2336">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="10322-2336">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="10322-2337">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="10322-2337">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="10322-2338">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="10322-2338">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="10322-2339">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="10322-2339">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="10322-2340">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="10322-2340">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="10322-2341">[ALTERAÇÃO SIGNIFICATIVA]`--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="10322-2341">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="10322-2342">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="10322-2342">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="10322-2343">[ALTERAÇÃO SIGNIFICATIVA]`--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="10322-2343">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="10322-2344">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="10322-2344">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="10322-2345">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="10322-2345">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="10322-2346">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="10322-2346">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="10322-2347">[ALTERAÇÃO SIGNIFICATIVA]`--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="10322-2347">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="10322-2348">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="10322-2348">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="10322-2349">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="10322-2349">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="10322-2350">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="10322-2350">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="10322-2351">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="10322-2351">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="10322-2352">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="10322-2352">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="10322-2353">Mapas</span><span class="sxs-lookup"><span data-stu-id="10322-2353">Maps</span></span>

* <span data-ttu-id="10322-2354">[ALTERAÇÃO SIGNIFICATIVA]`maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="10322-2354">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="10322-2355">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-2355">Network</span></span>

* <span data-ttu-id="10322-2356">Suporte adicionado para `https` a `network lb probe create` [nº6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="10322-2356">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="10322-2357">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="10322-2357">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="10322-2358">#6502</span><span class="sxs-lookup"><span data-stu-id="10322-2358">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="10322-2359">Reservas</span><span class="sxs-lookup"><span data-stu-id="10322-2359">Reservations</span></span>

* <span data-ttu-id="10322-2360">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="10322-2360">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="10322-2361">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="10322-2361">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="10322-2362">[ALTERAÇÃO SIGNIFICATIVA]`kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="10322-2362">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="10322-2363">[ALTERAÇÃO SIGNIFICATIVA]`capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="10322-2363">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="10322-2364">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="10322-2364">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="10322-2365">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="10322-2365">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="10322-2366">Função</span><span class="sxs-lookup"><span data-stu-id="10322-2366">Role</span></span>

* <span data-ttu-id="10322-2367">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="10322-2367">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="10322-2368">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-2368">SQL</span></span>

* <span data-ttu-id="10322-2369">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="10322-2369">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="10322-2370">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-2370">Storage</span></span>

* <span data-ttu-id="10322-2371">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="10322-2371">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="10322-2372">VM</span><span class="sxs-lookup"><span data-stu-id="10322-2372">VM</span></span>

* <span data-ttu-id="10322-2373">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="10322-2373">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="10322-2374">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="10322-2374">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="10322-2375">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="10322-2375">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="10322-2376">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2376">June 13, 2018</span></span>

<span data-ttu-id="10322-2377">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="10322-2377">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="10322-2378">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-2378">Core</span></span>

* <span data-ttu-id="10322-2379">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="10322-2379">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="10322-2380">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2380">June 13, 2018</span></span>

<span data-ttu-id="10322-2381">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="10322-2381">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="10322-2382">AKS</span><span class="sxs-lookup"><span data-stu-id="10322-2382">AKS</span></span>

* <span data-ttu-id="10322-2383">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="10322-2383">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="10322-2384">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="10322-2384">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="10322-2385">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="10322-2385">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="10322-2386">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="10322-2386">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="10322-2387">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="10322-2387">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-2388">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-2388">AppService</span></span>

* <span data-ttu-id="10322-2389">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="10322-2389">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="10322-2390">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2390">June 5, 2018</span></span>

<span data-ttu-id="10322-2391">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="10322-2391">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="10322-2392">Interativo</span><span class="sxs-lookup"><span data-stu-id="10322-2392">Interactive</span></span>

* <span data-ttu-id="10322-2393">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="10322-2393">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="10322-2394">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2394">June 5, 2018</span></span>

<span data-ttu-id="10322-2395">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="10322-2395">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="10322-2396">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-2396">Core</span></span>

* <span data-ttu-id="10322-2397">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="10322-2397">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="10322-2398">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="10322-2398">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="10322-2399">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-2399">ACR</span></span>

* <span data-ttu-id="10322-2400">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="10322-2400">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="10322-2401">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="10322-2401">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="10322-2402">AKS</span><span class="sxs-lookup"><span data-stu-id="10322-2402">AKS</span></span>

* <span data-ttu-id="10322-2403">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="10322-2403">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="10322-2404">Lote</span><span class="sxs-lookup"><span data-stu-id="10322-2404">Batch</span></span>

* <span data-ttu-id="10322-2405">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="10322-2405">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="10322-2406">IOT</span><span class="sxs-lookup"><span data-stu-id="10322-2406">IOT</span></span>

* <span data-ttu-id="10322-2407">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="10322-2407">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="10322-2408">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-2408">Network</span></span>

* <span data-ttu-id="10322-2409">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="10322-2409">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="10322-2410">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="10322-2410">Policy Insights</span></span>

* <span data-ttu-id="10322-2411">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="10322-2411">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="10322-2412">ARM</span><span class="sxs-lookup"><span data-stu-id="10322-2412">ARM</span></span>

* <span data-ttu-id="10322-2413">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="10322-2413">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="10322-2414">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-2414">SQL</span></span>

* <span data-ttu-id="10322-2415">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="10322-2415">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="10322-2416">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="10322-2416">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="10322-2417">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-2417">Storage</span></span>

* <span data-ttu-id="10322-2418">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="10322-2418">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="10322-2419">VM</span><span class="sxs-lookup"><span data-stu-id="10322-2419">VM</span></span>

* <span data-ttu-id="10322-2420">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="10322-2420">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="10322-2421">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="10322-2421">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="10322-2422">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="10322-2422">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="10322-2423">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2423">May 22, 2018</span></span>

<span data-ttu-id="10322-2424">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="10322-2424">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="10322-2425">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-2425">Core</span></span>

* <span data-ttu-id="10322-2426">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="10322-2426">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="10322-2427">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-2427">ACS</span></span>

* <span data-ttu-id="10322-2428">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="10322-2428">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="10322-2429">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="10322-2429">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-2430">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-2430">AppService</span></span>

* <span data-ttu-id="10322-2431">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="10322-2431">Improved generic update commands</span></span>
* <span data-ttu-id="10322-2432">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="10322-2432">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="10322-2433">Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-2433">Container</span></span>

* <span data-ttu-id="10322-2434">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="10322-2434">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="10322-2435">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-2435">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="10322-2436">Extensão</span><span class="sxs-lookup"><span data-stu-id="10322-2436">Extension</span></span>

* <span data-ttu-id="10322-2437">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="10322-2437">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="10322-2438">Interativo</span><span class="sxs-lookup"><span data-stu-id="10322-2438">Interactive</span></span>

* <span data-ttu-id="10322-2439">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="10322-2439">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="10322-2440">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="10322-2440">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="10322-2441">KeyVault</span><span class="sxs-lookup"><span data-stu-id="10322-2441">KeyVault</span></span>

* <span data-ttu-id="10322-2442">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="10322-2442">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="10322-2443">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-2443">Network</span></span>

* <span data-ttu-id="10322-2444">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="10322-2444">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="10322-2445">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="10322-2445">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="10322-2446">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-2446">SQL</span></span>

* <span data-ttu-id="10322-2447">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="10322-2447">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="10322-2448">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="10322-2448">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="10322-2449">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="10322-2449">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="10322-2450">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10322-2450">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="10322-2451">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="10322-2451">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="10322-2452">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="10322-2452">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="10322-2453">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="10322-2453">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="10322-2454">`edition`.</span><span class="sxs-lookup"><span data-stu-id="10322-2454">`edition`.</span></span> <span data-ttu-id="10322-2455">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="10322-2455">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="10322-2456">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="10322-2456">`elasticPoolName`.</span></span> <span data-ttu-id="10322-2457">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="10322-2457">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="10322-2458">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="10322-2458">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="10322-2459">`edition`.</span><span class="sxs-lookup"><span data-stu-id="10322-2459">`edition`.</span></span> <span data-ttu-id="10322-2460">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="10322-2460">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="10322-2461">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="10322-2461">`dtu`.</span></span> <span data-ttu-id="10322-2462">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="10322-2462">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="10322-2463">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="10322-2463">`databaseDtuMin`.</span></span> <span data-ttu-id="10322-2464">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="10322-2464">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="10322-2465">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="10322-2465">`databaseDtuMax`.</span></span> <span data-ttu-id="10322-2466">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="10322-2466">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="10322-2467">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="10322-2467">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="10322-2468">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="10322-2468">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="10322-2469">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-2469">Storage</span></span>

* <span data-ttu-id="10322-2470">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="10322-2470">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="10322-2471">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="10322-2471">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="10322-2472">VM</span><span class="sxs-lookup"><span data-stu-id="10322-2472">VM</span></span>

* <span data-ttu-id="10322-2473">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="10322-2473">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="10322-2474">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="10322-2474">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="10322-2475">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="10322-2475">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="10322-2476">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="10322-2476">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="10322-2477">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="10322-2477">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="10322-2478">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2478">May 7, 2018</span></span>

<span data-ttu-id="10322-2479">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="10322-2479">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="10322-2480">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-2480">Core</span></span>

* <span data-ttu-id="10322-2481">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="10322-2481">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="10322-2482">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="10322-2482">Added limited support for positional arguments</span></span>
* <span data-ttu-id="10322-2483">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="10322-2483">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="10322-2484">#5591</span><span class="sxs-lookup"><span data-stu-id="10322-2484">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="10322-2485">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="10322-2485">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="10322-2486">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="10322-2486">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="10322-2487">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="10322-2487">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="10322-2488">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="10322-2488">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="10322-2489">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="10322-2489">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="10322-2490">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-2490">ACR</span></span>

* <span data-ttu-id="10322-2491">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="10322-2491">Added ACR Build commands</span></span>
* <span data-ttu-id="10322-2492">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="10322-2492">Improved resource not found error messages</span></span>
* <span data-ttu-id="10322-2493">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="10322-2493">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="10322-2494">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="10322-2494">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="10322-2495">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="10322-2495">Improved repository commands error messages</span></span>
* <span data-ttu-id="10322-2496">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="10322-2496">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="10322-2497">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-2497">ACS</span></span>

* <span data-ttu-id="10322-2498">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="10322-2498">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="10322-2499">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="10322-2499">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="10322-2500">AMS</span><span class="sxs-lookup"><span data-stu-id="10322-2500">AMS</span></span>

* <span data-ttu-id="10322-2501">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="10322-2501">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-2502">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-2502">Appservice</span></span>

* <span data-ttu-id="10322-2503">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="10322-2503">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="10322-2504">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="10322-2504">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="10322-2505">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="10322-2505">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="10322-2506">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="10322-2506">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="10322-2507">Lote AI</span><span class="sxs-lookup"><span data-stu-id="10322-2507">Batch AI</span></span>

* <span data-ttu-id="10322-2508">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="10322-2508">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="10322-2509">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="10322-2509">Cognitive Services</span></span>

* <span data-ttu-id="10322-2510">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create`[#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="10322-2510">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="10322-2511">Consumo</span><span class="sxs-lookup"><span data-stu-id="10322-2511">Consumption</span></span>

* <span data-ttu-id="10322-2512">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="10322-2512">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="10322-2513">Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-2513">Container</span></span>

* <span data-ttu-id="10322-2514">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="10322-2514">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="10322-2515">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="10322-2515">Cosmos DB</span></span>

* <span data-ttu-id="10322-2516">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="10322-2516">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="10322-2517">DMS</span><span class="sxs-lookup"><span data-stu-id="10322-2517">DMS</span></span>

* <span data-ttu-id="10322-2518">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="10322-2518">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="10322-2519">Extensão</span><span class="sxs-lookup"><span data-stu-id="10322-2519">Extension</span></span>

* <span data-ttu-id="10322-2520">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="10322-2520">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="10322-2521">Interativo</span><span class="sxs-lookup"><span data-stu-id="10322-2521">Interactive</span></span>

* <span data-ttu-id="10322-2522">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="10322-2522">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="10322-2523">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="10322-2523">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="10322-2524">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="10322-2524">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="10322-2525">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="10322-2525">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="10322-2526">Laboratório</span><span class="sxs-lookup"><span data-stu-id="10322-2526">Lab</span></span>

* <span data-ttu-id="10322-2527">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="10322-2527">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="10322-2528">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-2528">Network</span></span>

* <span data-ttu-id="10322-2529">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="10322-2529">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="10322-2530">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-2530">Profile</span></span>

* <span data-ttu-id="10322-2531">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="10322-2531">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="10322-2532">[ALTERAÇÃO SIGNIFICATIVA]`--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="10322-2532">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="10322-2533">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="10322-2533">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="10322-2534">Redis</span><span class="sxs-lookup"><span data-stu-id="10322-2534">Redis</span></span>

* <span data-ttu-id="10322-2535">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="10322-2535">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="10322-2536">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="10322-2536">Deprecated `redis list-all`.</span></span> <span data-ttu-id="10322-2537">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="10322-2537">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="10322-2538">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="10322-2538">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="10322-2539">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="10322-2539">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="10322-2540">Função</span><span class="sxs-lookup"><span data-stu-id="10322-2540">Role</span></span>

* <span data-ttu-id="10322-2541">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="10322-2541">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="10322-2542">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-2542">Storage</span></span>

* <span data-ttu-id="10322-2543">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="10322-2543">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="10322-2544">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="10322-2544">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="10322-2545">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="10322-2545">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="10322-2546">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="10322-2546">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="10322-2547">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="10322-2547">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="10322-2548">VM</span><span class="sxs-lookup"><span data-stu-id="10322-2548">VM</span></span>

* <span data-ttu-id="10322-2549">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="10322-2549">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="10322-2550">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="10322-2550">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="10322-2551">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="10322-2551">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="10322-2552">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="10322-2552">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="10322-2553">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="10322-2553">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="10322-2554">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="10322-2554">Added write accelerator support</span></span>
* <span data-ttu-id="10322-2555">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="10322-2555">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="10322-2556">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="10322-2556">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="10322-2557">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="10322-2557">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="10322-2558">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2558">April 10, 2018</span></span>

<span data-ttu-id="10322-2559">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="10322-2559">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="10322-2560">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-2560">ACR</span></span>

* <span data-ttu-id="10322-2561">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="10322-2561">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="10322-2562">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-2562">ACS</span></span>

* <span data-ttu-id="10322-2563">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="10322-2563">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-2564">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-2564">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="10322-2566">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="10322-2566">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="10322-2567">BatchAI</span><span class="sxs-lookup"><span data-stu-id="10322-2567">BatchAI</span></span>

* <span data-ttu-id="10322-2568">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="10322-2568">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="10322-2569">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="10322-2569">Job level mounting</span></span>
  - <span data-ttu-id="10322-2570">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="10322-2570">Environment variables with secret values</span></span>
  - <span data-ttu-id="10322-2571">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="10322-2571">Performance counters settings</span></span>
  - <span data-ttu-id="10322-2572">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="10322-2572">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="10322-2573">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="10322-2573">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="10322-2574">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="10322-2574">Usage and limits reporting</span></span>
  - <span data-ttu-id="10322-2575">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="10322-2575">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="10322-2576">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="10322-2576">Support for custom images</span></span>
  - <span data-ttu-id="10322-2577">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="10322-2577">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="10322-2578">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="10322-2578">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="10322-2579">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="10322-2579">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="10322-2580">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="10322-2580">National clouds are supported</span></span>
* <span data-ttu-id="10322-2581">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="10322-2581">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="10322-2582">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="10322-2582">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="10322-2583">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="10322-2583">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="10322-2584">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="10322-2584">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="10322-2585">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="10322-2585">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="10322-2586">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="10322-2586">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="10322-2587">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="10322-2587">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="10322-2588">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="10322-2588">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="10322-2589">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="10322-2589">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="10322-2590">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="10322-2590">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="10322-2591">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="10322-2591">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="10322-2592">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="10322-2592">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="10322-2593">[ALTERAÇÃO SIGNIFICATIVA]`--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="10322-2593">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="10322-2594">Cobrança</span><span class="sxs-lookup"><span data-stu-id="10322-2594">Billing</span></span>

* <span data-ttu-id="10322-2595">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="10322-2595">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="10322-2596">Consumo</span><span class="sxs-lookup"><span data-stu-id="10322-2596">Consumption</span></span>

* <span data-ttu-id="10322-2597">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="10322-2597">Added `marketplace` commands</span></span>
* <span data-ttu-id="10322-2598">[ALTERAÇÃO SIGNIFICATIVA]`reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="10322-2598">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="10322-2599">[ALTERAÇÃO SIGNIFICATIVA]`reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="10322-2599">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="10322-2600">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="10322-2600">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="10322-2601">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="10322-2601">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="10322-2602">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="10322-2602">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="10322-2603">Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-2603">Container</span></span>

* <span data-ttu-id="10322-2604">Adição dos parâmetros de montagem de volume do Repositório Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="10322-2604">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="10322-2605">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="10322-2605">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="10322-2606">Extensão</span><span class="sxs-lookup"><span data-stu-id="10322-2606">Extension</span></span>

* <span data-ttu-id="10322-2607">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="10322-2607">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="10322-2608">Interativo</span><span class="sxs-lookup"><span data-stu-id="10322-2608">Interactive</span></span>

* <span data-ttu-id="10322-2609">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="10322-2609">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="10322-2610">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="10322-2610">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="10322-2611">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="10322-2611">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="10322-2612">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-2612">Network</span></span>

* <span data-ttu-id="10322-2613">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="10322-2613">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="10322-2614">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="10322-2614">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="10322-2615">#4910</span><span class="sxs-lookup"><span data-stu-id="10322-2615">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="10322-2616">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="10322-2616">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="10322-2617">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="10322-2617">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="10322-2618">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-2618">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="10322-2619">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-2619">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="10322-2620">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="10322-2620">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="10322-2621">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-2621">Profile</span></span>

* <span data-ttu-id="10322-2622">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="10322-2622">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="10322-2623">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="10322-2623">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="10322-2624">RDBMS</span><span class="sxs-lookup"><span data-stu-id="10322-2624">RDBMS</span></span>

* <span data-ttu-id="10322-2625">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="10322-2625">Added `georestore` command</span></span>
* <span data-ttu-id="10322-2626">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="10322-2626">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="10322-2627">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-2627">Resource</span></span>

* <span data-ttu-id="10322-2628">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="10322-2628">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="10322-2629">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="10322-2629">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="10322-2630">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-2630">SQL</span></span>

* <span data-ttu-id="10322-2631">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="10322-2631">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="10322-2632">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-2632">Storage</span></span>

* <span data-ttu-id="10322-2633">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="10322-2633">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="10322-2634">VM</span><span class="sxs-lookup"><span data-stu-id="10322-2634">VM</span></span>

* <span data-ttu-id="10322-2635">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="10322-2635">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="10322-2636">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="10322-2636">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="10322-2638">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="10322-2638">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="10322-2639">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="10322-2639">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="10322-2640">#5718</span><span class="sxs-lookup"><span data-stu-id="10322-2640">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="10322-2641">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="10322-2641">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="10322-2642">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2642">March 27, 2018</span></span>

<span data-ttu-id="10322-2643">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="10322-2643">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="10322-2644">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-2644">Core</span></span>

* <span data-ttu-id="10322-2645">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="10322-2645">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="10322-2646">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-2646">ACS</span></span>

* <span data-ttu-id="10322-2647">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="10322-2647">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-2648">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-2648">Appservice</span></span>

* <span data-ttu-id="10322-2649">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="10322-2649">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="10322-2650">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="10322-2650">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="10322-2651">Backup</span><span class="sxs-lookup"><span data-stu-id="10322-2651">Backup</span></span>

* <span data-ttu-id="10322-2652">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="10322-2652">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="10322-2653">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="10322-2653">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="10322-2654">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="10322-2654">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="10322-2655">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="10322-2655">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="10322-2656">Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-2656">Container</span></span>

* <span data-ttu-id="10322-2657">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="10322-2657">Added `container exec` command.</span></span> <span data-ttu-id="10322-2658">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="10322-2658">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="10322-2659">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-2659">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="10322-2660">Extensão</span><span class="sxs-lookup"><span data-stu-id="10322-2660">Extension</span></span>

* <span data-ttu-id="10322-2661">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="10322-2661">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="10322-2662">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="10322-2662">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="10322-2663">[ALTERAÇÃO SIGNIFICATIVA]`extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="10322-2663">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="10322-2664">Interativo</span><span class="sxs-lookup"><span data-stu-id="10322-2664">Interactive</span></span>

* <span data-ttu-id="10322-2665">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="10322-2665">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="10322-2666">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="10322-2666">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="10322-2667">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="10322-2667">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="10322-2668">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="10322-2668">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="10322-2669">Laboratório</span><span class="sxs-lookup"><span data-stu-id="10322-2669">Lab</span></span>

* <span data-ttu-id="10322-2670">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="10322-2670">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-2671">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-2671">Monitor</span></span>

* <span data-ttu-id="10322-2672">Adicionado suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [nº5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="10322-2672">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="10322-2673">Corrigido [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="10322-2673">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="10322-2674">Suporte adicionado para `--namespace` a `metrics list-definitions` [nº5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="10322-2674">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="10322-2675">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-2675">Network</span></span>

* <span data-ttu-id="10322-2676">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="10322-2676">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="10322-2677">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-2677">Profile</span></span>

* <span data-ttu-id="10322-2678">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="10322-2678">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="10322-2679">RDBMS</span><span class="sxs-lookup"><span data-stu-id="10322-2679">RDBMS</span></span>

* <span data-ttu-id="10322-2680">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="10322-2680">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="10322-2681">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-2681">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="10322-2683">Função</span><span class="sxs-lookup"><span data-stu-id="10322-2683">Role</span></span>

* <span data-ttu-id="10322-2684">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="10322-2684">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="10322-2685">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="10322-2685">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="10322-2686">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="10322-2686">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="10322-2687">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="10322-2687">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="10322-2688">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="10322-2688">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="10322-2689">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-2689">Storage</span></span>

* <span data-ttu-id="10322-2690">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="10322-2690">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="10322-2691">Corrigido [#4049](https://github.com/Azure/azure-cli/issues/4049): problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="10322-2691">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="10322-2692">VM</span><span class="sxs-lookup"><span data-stu-id="10322-2692">VM</span></span>

* <span data-ttu-id="10322-2693">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="10322-2693">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="10322-2694">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="10322-2694">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="10322-2695">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="10322-2695">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="10322-2696">[ALTERAÇÃO SIGNIFICATIVA]`vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="10322-2696">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="10322-2697">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2697">March 13, 2018</span></span>

<span data-ttu-id="10322-2698">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="10322-2698">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="10322-2699">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-2699">ACR</span></span>

* <span data-ttu-id="10322-2700">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="10322-2700">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="10322-2701">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="10322-2701">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="10322-2702">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="10322-2702">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="10322-2703">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-2703">ACS</span></span>

* <span data-ttu-id="10322-2704">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="10322-2704">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="10322-2705">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="10322-2705">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="10322-2706">Supervisor</span><span class="sxs-lookup"><span data-stu-id="10322-2706">Advisor</span></span>

* <span data-ttu-id="10322-2707">[ALTERAÇÃO SIGNIFICATIVA]`advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="10322-2707">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="10322-2708">[ALTERAÇÃO SIGNIFICATIVA]`advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="10322-2708">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="10322-2709">[ALTERAÇÃO SIGNIFICATIVA]`advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="10322-2709">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="10322-2710">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="10322-2710">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="10322-2711">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="10322-2711">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-2712">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-2712">Appservice</span></span>

* <span data-ttu-id="10322-2713">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="10322-2713">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="10322-2714">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="10322-2714">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="10322-2715">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="10322-2715">Eventhubs</span></span>

* <span data-ttu-id="10322-2716">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="10322-2716">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="10322-2717">Extensão</span><span class="sxs-lookup"><span data-stu-id="10322-2717">Extension</span></span>

* <span data-ttu-id="10322-2718">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="10322-2718">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="10322-2719">Interativo</span><span class="sxs-lookup"><span data-stu-id="10322-2719">Interactive</span></span>

* <span data-ttu-id="10322-2720">Corrigido [#5625](https://github.com/Azure/azure-cli/issues/5625): manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="10322-2720">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="10322-2721">Corrigido [#3016](https://github.com/Azure/azure-cli/issues/3016): histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="10322-2721">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="10322-2722">Corrigido [#5688](https://github.com/Azure/azure-cli/issues/5688): as conclusões não aparecerão se o carregamento da tabela de comando encontrar uma exceção</span><span class="sxs-lookup"><span data-stu-id="10322-2722">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="10322-2723">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="10322-2723">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-2724">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-2724">Monitor</span></span>

* <span data-ttu-id="10322-2725">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="10322-2725">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="10322-2726">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="10322-2726">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="10322-2727">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="10322-2727">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="10322-2728">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="10322-2728">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="10322-2729">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-2729">Network</span></span>

* <span data-ttu-id="10322-2730">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="10322-2730">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="10322-2731">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="10322-2731">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="10322-2732">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="10322-2732">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="10322-2733">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="10322-2733">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="10322-2734">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-2734">Profile</span></span>

* <span data-ttu-id="10322-2735">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="10322-2735">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="10322-2736">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="10322-2736">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="10322-2737">RDBMS</span><span class="sxs-lookup"><span data-stu-id="10322-2737">RDBMS</span></span>

* <span data-ttu-id="10322-2738">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="10322-2738">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="10322-2739">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="10322-2739">Service Bus</span></span>

* <span data-ttu-id="10322-2740">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="10322-2740">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="10322-2741">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-2741">Storage</span></span>

* <span data-ttu-id="10322-2742">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="10322-2742">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="10322-2743">Corrigido [#5286](https://github.com/Azure/azure-cli/issues/5286): os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="10322-2743">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="10322-2744">VM</span><span class="sxs-lookup"><span data-stu-id="10322-2744">VM</span></span>

* <span data-ttu-id="10322-2745">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="10322-2745">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="10322-2746">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="10322-2746">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="10322-2747">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="10322-2747">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="10322-2748">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="10322-2748">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="10322-2749">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2749">February 27, 2018</span></span>

<span data-ttu-id="10322-2750">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="10322-2750">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="10322-2751">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-2751">Core</span></span>

* <span data-ttu-id="10322-2752">Corrigido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="10322-2752">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="10322-2753">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="10322-2753">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="10322-2754">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="10322-2754">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="10322-2755">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-2755">ACS</span></span>

* <span data-ttu-id="10322-2756">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="10322-2756">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="10322-2757">Problema corrigido: permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="10322-2757">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="10322-2758">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="10322-2758">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="10322-2759">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="10322-2759">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-2760">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-2760">Appservice</span></span>

* <span data-ttu-id="10322-2761">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="10322-2761">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="10322-2762">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="10322-2762">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="10322-2763">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="10322-2763">Cognitive Services</span></span>

* <span data-ttu-id="10322-2764">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="10322-2764">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="10322-2765">Consumo</span><span class="sxs-lookup"><span data-stu-id="10322-2765">Consumption</span></span>

* <span data-ttu-id="10322-2766">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="10322-2766">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="10322-2767">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="10322-2767">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="10322-2768">Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-2768">Container</span></span>

* <span data-ttu-id="10322-2769">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="10322-2769">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="10322-2770">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-2770">Network</span></span>

* <span data-ttu-id="10322-2771">Corrigido [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="10322-2771">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="10322-2772">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-2772">Resource</span></span>

* <span data-ttu-id="10322-2773">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="10322-2773">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="10322-2774">Função</span><span class="sxs-lookup"><span data-stu-id="10322-2774">Role</span></span>

* <span data-ttu-id="10322-2775">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="10322-2775">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="10322-2776">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-2776">SQL</span></span>

* <span data-ttu-id="10322-2777">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="10322-2777">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="10322-2778">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-2778">Storage</span></span>

* <span data-ttu-id="10322-2779">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="10322-2779">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="10322-2780">VM</span><span class="sxs-lookup"><span data-stu-id="10322-2780">VM</span></span>

* <span data-ttu-id="10322-2781">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="10322-2781">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="10322-2782">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2782">February 13, 2018</span></span>

<span data-ttu-id="10322-2783">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="10322-2783">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="10322-2784">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-2784">Core</span></span>

* <span data-ttu-id="10322-2785">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="10322-2785">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="10322-2786">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-2786">ACS</span></span>

* <span data-ttu-id="10322-2787">[ALTERAÇÃO SIGNIFICATIVA]`aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="10322-2787">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="10322-2788">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="10322-2788">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="10322-2789">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="10322-2789">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="10322-2790">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="10322-2790">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="10322-2791">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="10322-2791">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="10322-2792">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="10322-2792">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="10322-2793">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="10322-2793">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="10322-2794">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="10322-2794">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-2795">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-2795">Appservice</span></span>

* <span data-ttu-id="10322-2796">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="10322-2796">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="10322-2797">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="10322-2797">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="10322-2798">CDN</span><span class="sxs-lookup"><span data-stu-id="10322-2798">CDN</span></span>

* <span data-ttu-id="10322-2799">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="10322-2799">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="10322-2800">Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-2800">Container</span></span>

* <span data-ttu-id="10322-2801">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="10322-2801">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="10322-2802">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-2802">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="10322-2803">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="10322-2803">CosmosDB</span></span>

* <span data-ttu-id="10322-2804">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="10322-2804">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="10322-2805">Extensão</span><span class="sxs-lookup"><span data-stu-id="10322-2805">Extension</span></span>

* <span data-ttu-id="10322-2806">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-2806">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="10322-2807">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-2807">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="10322-2808">Comentários</span><span class="sxs-lookup"><span data-stu-id="10322-2808">Feedback</span></span>

* <span data-ttu-id="10322-2809">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="10322-2809">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="10322-2810">Interativo</span><span class="sxs-lookup"><span data-stu-id="10322-2810">Interactive</span></span>

* <span data-ttu-id="10322-2811">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="10322-2811">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="10322-2812">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="10322-2812">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="10322-2813">IoT</span><span class="sxs-lookup"><span data-stu-id="10322-2813">IoT</span></span>

* <span data-ttu-id="10322-2814">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="10322-2814">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="10322-2815">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="10322-2815">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="10322-2816">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-2816">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="10322-2817">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="10322-2817">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-2818">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-2818">Monitor</span></span>

* <span data-ttu-id="10322-2819">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="10322-2819">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="10322-2820">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-2820">Network</span></span>

* <span data-ttu-id="10322-2821">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="10322-2821">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="10322-2822">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-2822">Profile</span></span>

* <span data-ttu-id="10322-2823">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="10322-2823">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="10322-2824">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-2824">Resource</span></span>

* <span data-ttu-id="10322-2825">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="10322-2825">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="10322-2826">Função</span><span class="sxs-lookup"><span data-stu-id="10322-2826">Role</span></span>

* <span data-ttu-id="10322-2827">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="10322-2827">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="10322-2828">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-2828">SQL</span></span>

* <span data-ttu-id="10322-2829">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="10322-2829">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="10322-2830">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="10322-2830">Added `sql db rename`</span></span>
* <span data-ttu-id="10322-2831">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="10322-2831">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="10322-2832">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-2832">Storage</span></span>

* <span data-ttu-id="10322-2833">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="10322-2833">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="10322-2834">VM</span><span class="sxs-lookup"><span data-stu-id="10322-2834">VM</span></span>

* <span data-ttu-id="10322-2835">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="10322-2835">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="10322-2836">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="10322-2836">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="10322-2837">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="10322-2837">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="10322-2838">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2838">January 31, 2018</span></span>

<span data-ttu-id="10322-2839">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="10322-2839">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="10322-2840">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-2840">Core</span></span>

* <span data-ttu-id="10322-2841">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="10322-2841">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="10322-2842">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="10322-2842">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="10322-2843">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="10322-2843">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="10322-2844">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="10322-2844">Use `--verbose` to see</span></span>
* <span data-ttu-id="10322-2845">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="10322-2845">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="10322-2846">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-2846">ACS</span></span>

* <span data-ttu-id="10322-2847">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="10322-2847">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="10322-2848">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="10322-2848">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-2849">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-2849">Appservice</span></span>

* <span data-ttu-id="10322-2850">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="10322-2850">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="10322-2851">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="10322-2851">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="10322-2852">CDN</span><span class="sxs-lookup"><span data-stu-id="10322-2852">CDN</span></span>

* <span data-ttu-id="10322-2853">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="10322-2853">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="10322-2854">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="10322-2854">CosmosDB</span></span>

* <span data-ttu-id="10322-2855">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="10322-2855">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="10322-2856">Interativo</span><span class="sxs-lookup"><span data-stu-id="10322-2856">Interactive</span></span>

* <span data-ttu-id="10322-2857">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="10322-2857">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="10322-2858">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-2858">Network</span></span>

* <span data-ttu-id="10322-2859">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="10322-2859">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="10322-2860">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="10322-2860">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="10322-2861">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="10322-2861">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="10322-2862">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="10322-2862">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="10322-2863">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="10322-2863">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="10322-2864">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="10322-2864">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="10322-2865">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="10322-2865">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="10322-2866">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="10322-2866">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="10322-2867">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="10322-2867">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="10322-2868">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="10322-2868">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="10322-2869">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-2869">Profile</span></span>

* <span data-ttu-id="10322-2870">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="10322-2870">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="10322-2871">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-2871">Resource</span></span>

* <span data-ttu-id="10322-2872">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="10322-2872">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="10322-2873">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-2873">Storage</span></span>

* <span data-ttu-id="10322-2874">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="10322-2874">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="10322-2875">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="10322-2875">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="10322-2876">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="10322-2876">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="10322-2877">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="10322-2877">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="10322-2878">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="10322-2878">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="10322-2879">VM</span><span class="sxs-lookup"><span data-stu-id="10322-2879">VM</span></span>

* <span data-ttu-id="10322-2880">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="10322-2880">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="10322-2881">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="10322-2881">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="10322-2882">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="10322-2882">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="10322-2883">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="10322-2883">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="10322-2884">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="10322-2884">January 17, 2018</span></span>

<span data-ttu-id="10322-2885">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="10322-2885">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="10322-2886">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-2886">ACR</span></span>

* <span data-ttu-id="10322-2887">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="10322-2887">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="10322-2888">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="10322-2888">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="10322-2889">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-2889">ACS</span></span>

* <span data-ttu-id="10322-2890">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="10322-2890">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="10322-2891">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="10322-2891">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-2892">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-2892">Appservice</span></span>

* <span data-ttu-id="10322-2893">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="10322-2893">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="10322-2894">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="10322-2894">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="10322-2895">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="10322-2895">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="10322-2896">Backup</span><span class="sxs-lookup"><span data-stu-id="10322-2896">Backup</span></span>

* <span data-ttu-id="10322-2897">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="10322-2897">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="10322-2898">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="10322-2898">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="10322-2899">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="10322-2899">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="10322-2900">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="10322-2900">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="10322-2901">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="10322-2901">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="10322-2902">Lote</span><span class="sxs-lookup"><span data-stu-id="10322-2902">Batch</span></span>

* <span data-ttu-id="10322-2903">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="10322-2903">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="10322-2904">Nuvem</span><span class="sxs-lookup"><span data-stu-id="10322-2904">Cloud</span></span>

* <span data-ttu-id="10322-2905">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="10322-2905">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="10322-2906">Consumo</span><span class="sxs-lookup"><span data-stu-id="10322-2906">Consumption</span></span>

* <span data-ttu-id="10322-2907">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="10322-2907">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="10322-2908">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="10322-2908">Event Grid</span></span>

* <span data-ttu-id="10322-2909">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="10322-2909">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="10322-2910">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="10322-2910">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="10322-2911">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="10322-2911">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="10322-2912">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="10322-2912">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="10322-2913">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="10322-2913">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="10322-2914">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="10322-2914">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="10322-2915">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="10322-2915">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="10322-2916">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="10322-2916">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="10322-2917">Interativo</span><span class="sxs-lookup"><span data-stu-id="10322-2917">Interactive</span></span>

* <span data-ttu-id="10322-2918">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="10322-2918">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="10322-2919">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="10322-2919">Fixed errors on startup</span></span>
* <span data-ttu-id="10322-2920">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="10322-2920">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="10322-2921">IoT</span><span class="sxs-lookup"><span data-stu-id="10322-2921">IoT</span></span>

* <span data-ttu-id="10322-2922">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="10322-2922">Added support for device provisioning service</span></span>
* <span data-ttu-id="10322-2923">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="10322-2923">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="10322-2924">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="10322-2924">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-2925">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-2925">Monitor</span></span>

* <span data-ttu-id="10322-2926">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="10322-2926">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="10322-2927">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="10322-2927">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="10322-2928">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="10322-2928">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="10322-2929">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-2929">Network</span></span>

* <span data-ttu-id="10322-2930">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="10322-2930">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="10322-2931">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-2931">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="10322-2932">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-2932">Profile</span></span>

* <span data-ttu-id="10322-2933">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="10322-2933">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="10322-2934">Função</span><span class="sxs-lookup"><span data-stu-id="10322-2934">Role</span></span>

* <span data-ttu-id="10322-2935">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="10322-2935">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="10322-2936">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="10322-2936">Service Fabric</span></span>

* <span data-ttu-id="10322-2937">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="10322-2937">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="10322-2938">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="10322-2938">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="10322-2939">VM</span><span class="sxs-lookup"><span data-stu-id="10322-2939">VM</span></span>

* <span data-ttu-id="10322-2940">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="10322-2940">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="10322-2941">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="10322-2941">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="10322-2942">[ALTERAÇÃO SIGNIFICATIVA]`externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="10322-2942">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="10322-2943">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="10322-2943">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="10322-2944">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="10322-2944">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="10322-2945">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="10322-2945">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="10322-2946">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="10322-2946">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="10322-2947">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="10322-2947">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="10322-2948">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="10322-2948">December 19, 2017</span></span>

<span data-ttu-id="10322-2949">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="10322-2949">Version 2.0.23</span></span>

* <span data-ttu-id="10322-2950">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="10322-2950">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="10322-2951">Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-2951">Container</span></span>

* <span data-ttu-id="10322-2952">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-2952">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="10322-2953">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-2953">Network</span></span>

* <span data-ttu-id="10322-2954">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-2954">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="10322-2955">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-2955">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="10322-2956">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-2956">Storage</span></span>

* <span data-ttu-id="10322-2957">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="10322-2957">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="10322-2958">VM</span><span class="sxs-lookup"><span data-stu-id="10322-2958">VM</span></span>

* <span data-ttu-id="10322-2959">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="10322-2959">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="10322-2960">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="10322-2960">December 5, 2017</span></span>

<span data-ttu-id="10322-2961">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="10322-2961">Version 2.0.22</span></span>

* <span data-ttu-id="10322-2962">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="10322-2962">Removed `az component` commands.</span></span> <span data-ttu-id="10322-2963">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="10322-2963">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="10322-2964">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-2964">Core</span></span>
* <span data-ttu-id="10322-2965">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="10322-2965">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="10322-2966">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="10322-2966">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="10322-2967">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-2967">ACS</span></span>

* <span data-ttu-id="10322-2968">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="10322-2968">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="10322-2969">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="10322-2969">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="10322-2970">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="10322-2970">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="10322-2971">Supervisor</span><span class="sxs-lookup"><span data-stu-id="10322-2971">Advisor</span></span>

* <span data-ttu-id="10322-2972">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="10322-2972">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-2973">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-2973">Appservice</span></span>

* <span data-ttu-id="10322-2974">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="10322-2974">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="10322-2975">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="10322-2975">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="10322-2976">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="10322-2976">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="10322-2977">Consumo</span><span class="sxs-lookup"><span data-stu-id="10322-2977">Consumption</span></span>

* <span data-ttu-id="10322-2978">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="10322-2978">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="10322-2979">Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-2979">Container</span></span>

* <span data-ttu-id="10322-2980">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="10322-2980">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-2981">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-2981">Monitor</span></span>

* <span data-ttu-id="10322-2982">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="10322-2982">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="10322-2983">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-2983">Resource</span></span>

* <span data-ttu-id="10322-2984">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="10322-2984">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="10322-2985">Função</span><span class="sxs-lookup"><span data-stu-id="10322-2985">Role</span></span>

* <span data-ttu-id="10322-2986">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="10322-2986">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="10322-2987">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="10322-2987">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="10322-2988">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="10322-2988">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="10322-2989">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-2989">SQL</span></span>

* <span data-ttu-id="10322-2990">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="10322-2990">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="10322-2991">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="10322-2991">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="10322-2992">VM</span><span class="sxs-lookup"><span data-stu-id="10322-2992">VM</span></span>

* <span data-ttu-id="10322-2993">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="10322-2993">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="10322-2994">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="10322-2994">November 14, 2017</span></span>

<span data-ttu-id="10322-2995">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="10322-2995">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="10322-2996">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-2996">ACR</span></span>

* <span data-ttu-id="10322-2997">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="10322-2997">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="10322-2998">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-2998">ACS</span></span>

* <span data-ttu-id="10322-2999">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="10322-2999">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="10322-3000">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="10322-3000">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="10322-3001">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="10322-3001">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="10322-3002">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="10322-3002">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="10322-3003">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="10322-3003">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-3004">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-3004">Appservice</span></span>

* <span data-ttu-id="10322-3005">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="10322-3005">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="10322-3006">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="10322-3006">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="10322-3007">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="10322-3007">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="10322-3008">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="10322-3008">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="10322-3009">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="10322-3009">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="10322-3010">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="10322-3010">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="10322-3011">Lote</span><span class="sxs-lookup"><span data-stu-id="10322-3011">Batch</span></span>

* <span data-ttu-id="10322-3012">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="10322-3012">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="10322-3013">Batchai</span><span class="sxs-lookup"><span data-stu-id="10322-3013">Batchai</span></span>

* <span data-ttu-id="10322-3014">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="10322-3014">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="10322-3015">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="10322-3015">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="10322-3016">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="10322-3016">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="10322-3017">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="10322-3017">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="10322-3018">Nuvem</span><span class="sxs-lookup"><span data-stu-id="10322-3018">Cloud</span></span>

* <span data-ttu-id="10322-3019">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="10322-3019">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="10322-3020">Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-3020">Container</span></span>

* <span data-ttu-id="10322-3021">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="10322-3021">Added support to open multiple ports</span></span>
* <span data-ttu-id="10322-3022">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="10322-3022">Added container group restart policy</span></span>
* <span data-ttu-id="10322-3023">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="10322-3023">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="10322-3024">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="10322-3024">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="10322-3025">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="10322-3025">Data Lake Analytics</span></span>

* <span data-ttu-id="10322-3026">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="10322-3026">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="10322-3027">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="10322-3027">Data Lake Store</span></span>

* <span data-ttu-id="10322-3028">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="10322-3028">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="10322-3029">Extensão</span><span class="sxs-lookup"><span data-stu-id="10322-3029">Extension</span></span>

* <span data-ttu-id="10322-3030">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="10322-3030">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="10322-3031">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="10322-3031">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="10322-3032">IoT</span><span class="sxs-lookup"><span data-stu-id="10322-3032">IoT</span></span>

* <span data-ttu-id="10322-3033">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="10322-3033">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-3034">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-3034">Monitor</span></span>

* <span data-ttu-id="10322-3035">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="10322-3035">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="10322-3036">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-3036">Network</span></span>

* <span data-ttu-id="10322-3037">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="10322-3037">Added support for CAA DNS records</span></span>
* <span data-ttu-id="10322-3038">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="10322-3038">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="10322-3039">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="10322-3039">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="10322-3040">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="10322-3040">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="10322-3041">Reservas</span><span class="sxs-lookup"><span data-stu-id="10322-3041">Reservations</span></span>

* <span data-ttu-id="10322-3042">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="10322-3042">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="10322-3043">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-3043">Resource</span></span>

* <span data-ttu-id="10322-3044">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="10322-3044">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="10322-3045">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-3045">SQL</span></span>

* <span data-ttu-id="10322-3046">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-3046">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="10322-3047">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-3047">Storage</span></span>

* <span data-ttu-id="10322-3048">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="10322-3048">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="10322-3049">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="10322-3049">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="10322-3050">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="10322-3050">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="10322-3051">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="10322-3051">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="10322-3052">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="10322-3052">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="10322-3053">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="10322-3053">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="10322-3054">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-3054">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="10322-3055">VM</span><span class="sxs-lookup"><span data-stu-id="10322-3055">VM</span></span>

* <span data-ttu-id="10322-3056">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="10322-3056">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="10322-3057">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="10322-3057">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="10322-3058">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="10322-3058">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="10322-3059">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="10322-3059">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="10322-3060">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="10322-3060">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="10322-3061">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="10322-3061">October 24, 2017</span></span>

<span data-ttu-id="10322-3062">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="10322-3062">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="10322-3063">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-3063">Core</span></span>

* <span data-ttu-id="10322-3064">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="10322-3064">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="10322-3065">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-3065">ACR</span></span>

* <span data-ttu-id="10322-3066">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="10322-3066">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="10322-3067">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="10322-3067">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="10322-3068">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="10322-3068">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="10322-3069">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-3069">ACS</span></span>

* <span data-ttu-id="10322-3070">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="10322-3070">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="10322-3071">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="10322-3071">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-3072">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-3072">Appservice</span></span>

* <span data-ttu-id="10322-3073">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="10322-3073">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="10322-3074">Componente</span><span class="sxs-lookup"><span data-stu-id="10322-3074">Component</span></span>

* <span data-ttu-id="10322-3075">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="10322-3075">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-3076">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-3076">Monitor</span></span>

* <span data-ttu-id="10322-3077">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="10322-3077">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="10322-3078">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-3078">Resource</span></span>

* <span data-ttu-id="10322-3079">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="10322-3079">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="10322-3080">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="10322-3080">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="10322-3081">VM</span><span class="sxs-lookup"><span data-stu-id="10322-3081">VM</span></span>

* <span data-ttu-id="10322-3082">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="10322-3082">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="10322-3083">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="10322-3083">October 9, 2017</span></span>

<span data-ttu-id="10322-3084">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="10322-3084">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="10322-3085">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-3085">Core</span></span>

* <span data-ttu-id="10322-3086">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="10322-3086">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-3087">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-3087">Appservice</span></span>

* <span data-ttu-id="10322-3088">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="10322-3088">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="10322-3089">Lote</span><span class="sxs-lookup"><span data-stu-id="10322-3089">Batch</span></span>

* <span data-ttu-id="10322-3090">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="10322-3090">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="10322-3091">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="10322-3091">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="10322-3092">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="10322-3092">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="10322-3093">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="10322-3093">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="10322-3094">Batchai</span><span class="sxs-lookup"><span data-stu-id="10322-3094">Batchai</span></span>

* <span data-ttu-id="10322-3095">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="10322-3095">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="10322-3096">Keyvault</span><span class="sxs-lookup"><span data-stu-id="10322-3096">Keyvault</span></span>

* <span data-ttu-id="10322-3097">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="10322-3097">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="10322-3098">(#4448)</span><span class="sxs-lookup"><span data-stu-id="10322-3098">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="10322-3099">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-3099">Network</span></span>

* <span data-ttu-id="10322-3100">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="10322-3100">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="10322-3101">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="10322-3101">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="10322-3102">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-3102">Resource</span></span>

* <span data-ttu-id="10322-3103">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="10322-3103">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="10322-3104">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="10322-3104">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="10322-3105">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="10322-3105">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="10322-3106">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="10322-3106">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="10322-3107">Sql</span><span class="sxs-lookup"><span data-stu-id="10322-3107">Sql</span></span>

* <span data-ttu-id="10322-3108">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="10322-3108">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="10322-3109">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="10322-3109">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="10322-3110">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="10322-3110">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="10322-3111">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-3111">Storage</span></span>

* <span data-ttu-id="10322-3112">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="10322-3112">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="10322-3113">VM</span><span class="sxs-lookup"><span data-stu-id="10322-3113">Vm</span></span>

* <span data-ttu-id="10322-3114">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="10322-3114">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="10322-3115">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="10322-3115">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="10322-3116">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="10322-3116">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="10322-3117">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="10322-3117">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="10322-3118">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="10322-3118">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="10322-3119">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="10322-3119">September 22, 2017</span></span>

<span data-ttu-id="10322-3120">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="10322-3120">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="10322-3121">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-3121">Resource</span></span>

* <span data-ttu-id="10322-3122">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="10322-3122">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="10322-3123">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="10322-3123">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="10322-3124">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="10322-3124">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="10322-3125">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="10322-3125">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="10322-3126">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-3126">Network</span></span>

* <span data-ttu-id="10322-3127">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="10322-3127">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="10322-3128">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="10322-3128">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="10322-3129">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="10322-3129">Added `asg` application security group commands</span></span>
* <span data-ttu-id="10322-3130">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="10322-3130">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="10322-3131">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-3131">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="10322-3132">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-3132">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="10322-3133">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="10322-3133">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="10322-3134">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-3134">Storage</span></span>

* <span data-ttu-id="10322-3135">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="10322-3135">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="10322-3136">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="10322-3136">Eventgrid</span></span>

* <span data-ttu-id="10322-3137">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="10322-3137">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="10322-3138">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-3138">SQL</span></span>

* <span data-ttu-id="10322-3139">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="10322-3139">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="10322-3140">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="10322-3140">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="10322-3141">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-3141">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="10322-3142">Keyvault</span><span class="sxs-lookup"><span data-stu-id="10322-3142">Keyvault</span></span>

* <span data-ttu-id="10322-3143">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="10322-3143">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="10322-3144">VM</span><span class="sxs-lookup"><span data-stu-id="10322-3144">VM</span></span>

* <span data-ttu-id="10322-3145">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="10322-3145">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="10322-3146">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="10322-3146">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="10322-3147">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="10322-3147">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="10322-3148">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="10322-3148">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="10322-3149">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="10322-3149">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="10322-3150">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="10322-3150">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="10322-3151">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-3151">ACS</span></span>

* <span data-ttu-id="10322-3152">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="10322-3152">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-3153">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-3153">Appservice</span></span>

* <span data-ttu-id="10322-3154">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="10322-3154">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="10322-3155">Backup</span><span class="sxs-lookup"><span data-stu-id="10322-3155">Backup</span></span>

* <span data-ttu-id="10322-3156">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="10322-3156">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="10322-3157">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="10322-3157">September 11, 2017</span></span>

<span data-ttu-id="10322-3158">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="10322-3158">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="10322-3159">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-3159">Core</span></span>

* <span data-ttu-id="10322-3160">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="10322-3160">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="10322-3161">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="10322-3161">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="10322-3162">Acs</span><span class="sxs-lookup"><span data-stu-id="10322-3162">Acs</span></span>

* <span data-ttu-id="10322-3163">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="10322-3163">Added `acs list-locations` command</span></span>
* <span data-ttu-id="10322-3164">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="10322-3164">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-3165">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-3165">Appservice</span></span>

* <span data-ttu-id="10322-3166">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="10322-3166">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="10322-3167">CDN</span><span class="sxs-lookup"><span data-stu-id="10322-3167">CDN</span></span>

* <span data-ttu-id="10322-3168">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="10322-3168">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="10322-3169">Extensão</span><span class="sxs-lookup"><span data-stu-id="10322-3169">Extension</span></span>

* <span data-ttu-id="10322-3170">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="10322-3170">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="10322-3171">Keyvault</span><span class="sxs-lookup"><span data-stu-id="10322-3171">Keyvault</span></span>

* <span data-ttu-id="10322-3172">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="10322-3172">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="10322-3173">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-3173">Network</span></span>

* <span data-ttu-id="10322-3174">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="10322-3174">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="10322-3175">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="10322-3175">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="10322-3176">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="10322-3176">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="10322-3177">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="10322-3177">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="10322-3178">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="10322-3178">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="10322-3179">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-3179">Resource</span></span>

* <span data-ttu-id="10322-3180">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="10322-3180">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="10322-3181">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="10322-3181">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="10322-3182">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="10322-3182">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="10322-3183">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="10322-3183">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="10322-3184">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-3184">SQL</span></span>

* <span data-ttu-id="10322-3185">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="10322-3185">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="10322-3186">VM</span><span class="sxs-lookup"><span data-stu-id="10322-3186">VM</span></span>

* <span data-ttu-id="10322-3187">Corrigido: não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="10322-3187">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="10322-3188">Corrigido: usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="10322-3188">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="10322-3189">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="10322-3189">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="10322-3190">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="10322-3190">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="10322-3191">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="10322-3191">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="10322-3192">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="10322-3192">August 31, 2017</span></span>

<span data-ttu-id="10322-3193">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="10322-3193">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="10322-3194">Keyvault</span><span class="sxs-lookup"><span data-stu-id="10322-3194">Keyvault</span></span>

* <span data-ttu-id="10322-3195">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="10322-3195">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="10322-3196">Sf</span><span class="sxs-lookup"><span data-stu-id="10322-3196">Sf</span></span>

* <span data-ttu-id="10322-3197">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="10322-3197">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="10322-3198">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-3198">Storage</span></span>

* <span data-ttu-id="10322-3199">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="10322-3199">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="10322-3200">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="10322-3200">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="10322-3201">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="10322-3201">August 28, 2017</span></span>

<span data-ttu-id="10322-3202">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="10322-3202">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="10322-3203">CLI</span><span class="sxs-lookup"><span data-stu-id="10322-3203">CLI</span></span>

* <span data-ttu-id="10322-3204">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="10322-3204">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="10322-3205">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-3205">ACS</span></span>

* <span data-ttu-id="10322-3206">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="10322-3206">Corrected preview regions</span></span>
* <span data-ttu-id="10322-3207">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="10322-3207">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="10322-3208">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="10322-3208">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-3209">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-3209">Appservice</span></span>

* <span data-ttu-id="10322-3210">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="10322-3210">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="10322-3211">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="10322-3211">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="10322-3212">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="10322-3212">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="10322-3213">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="10322-3213">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="10322-3214">Corrigido: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="10322-3214">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="10322-3215">IoT</span><span class="sxs-lookup"><span data-stu-id="10322-3215">IoT</span></span>

* <span data-ttu-id="10322-3216">Corrigido #3934: a criação de uma política não limpa mais as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="10322-3216">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="10322-3217">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-3217">Network</span></span>

* <span data-ttu-id="10322-3218">[ALTERAÇÃO SIGNIFICATIVA]`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="10322-3218">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="10322-3219">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-3219">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="10322-3220">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="10322-3220">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="10322-3221">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="10322-3221">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="10322-3222">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="10322-3222">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="10322-3223">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-3223">Profile</span></span>

* <span data-ttu-id="10322-3224">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="10322-3224">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="10322-3225">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="10322-3225">Service Fabric</span></span>

* <span data-ttu-id="10322-3226">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="10322-3226">Preview release</span></span>
* <span data-ttu-id="10322-3227">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="10322-3227">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="10322-3228">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="10322-3228">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="10322-3229">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="10322-3229">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="10322-3230">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-3230">Storage</span></span>

* <span data-ttu-id="10322-3231">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="10322-3231">Enabled setting blob tier</span></span>
* <span data-ttu-id="10322-3232">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="10322-3232">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="10322-3233">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="10322-3233">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="10322-3234">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="10322-3234">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="10322-3235">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="10322-3235">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="10322-3236">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="10322-3236">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="10322-3237">VM</span><span class="sxs-lookup"><span data-stu-id="10322-3237">VM</span></span>

* <span data-ttu-id="10322-3238">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="10322-3238">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="10322-3239">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="10322-3239">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="10322-3240">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="10322-3240">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="10322-3241">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="10322-3241">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="10322-3242">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="10322-3242">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="10322-3243">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="10322-3243">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="10322-3244">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="10322-3244">August 15, 2017</span></span>

<span data-ttu-id="10322-3245">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="10322-3245">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="10322-3246">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-3246">ACS</span></span>

* <span data-ttu-id="10322-3247">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="10322-3247">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-3248">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-3248">Appservice</span></span>

* <span data-ttu-id="10322-3249">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="10322-3249">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="10322-3250">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="10322-3250">Event Grid</span></span>

* <span data-ttu-id="10322-3251">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="10322-3251">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="10322-3252">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="10322-3252">August 11, 2017</span></span>

<span data-ttu-id="10322-3253">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="10322-3253">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="10322-3254">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-3254">ACS</span></span>

* <span data-ttu-id="10322-3255">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="10322-3255">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="10322-3256">Lote</span><span class="sxs-lookup"><span data-stu-id="10322-3256">Batch</span></span>

* <span data-ttu-id="10322-3257">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="10322-3257">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="10322-3258">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="10322-3258">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="10322-3259">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="10322-3259">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="10322-3260">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://”</span><span class="sxs-lookup"><span data-stu-id="10322-3260">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="10322-3261">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="10322-3261">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="10322-3262">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="10322-3262">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="10322-3263">Componente</span><span class="sxs-lookup"><span data-stu-id="10322-3263">Component</span></span>

* <span data-ttu-id="10322-3264">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="10322-3264">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="10322-3265">Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-3265">Container</span></span>

* <span data-ttu-id="10322-3266">`create`: corrigido o problema em que o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="10322-3266">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="10322-3267">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="10322-3267">Data Lake Store</span></span>

* <span data-ttu-id="10322-3268">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="10322-3268">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="10322-3269">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="10322-3269">Event Grid</span></span>

* <span data-ttu-id="10322-3270">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="10322-3270">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="10322-3271">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-3271">Network</span></span>

* <span data-ttu-id="10322-3272">`lb`: corrigido o problema em que os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="10322-3272">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="10322-3273">`application-gateway {subresource} delete`: corrigido o problema em que `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="10322-3273">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="10322-3274">`application-gateway http-settings update`: corrigido o problema em que `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="10322-3274">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="10322-3275">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="10322-3275">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="10322-3276">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-3276">Profile</span></span>

* <span data-ttu-id="10322-3277">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="10322-3277">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="10322-3278">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-3278">Storage</span></span>

* <span data-ttu-id="10322-3279">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="10322-3279">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="10322-3280">VM</span><span class="sxs-lookup"><span data-stu-id="10322-3280">VM</span></span>

* <span data-ttu-id="10322-3281">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="10322-3281">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="10322-3282">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="10322-3282">Exposed `list-skus` command</span></span>
* <span data-ttu-id="10322-3283">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="10322-3283">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="10322-3284">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="10322-3284">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="10322-3285">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="10322-3285">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="10322-3286">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="10322-3286">July 28, 2017</span></span>

<span data-ttu-id="10322-3287">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="10322-3287">Version 2.0.12</span></span>

* <span data-ttu-id="10322-3288">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-3288">Added container commands</span></span>
* <span data-ttu-id="10322-3289">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="10322-3289">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="10322-3290">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-3290">Core</span></span>

* <span data-ttu-id="10322-3291">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="10322-3291">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="10322-3292">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="10322-3292">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="10322-3293">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="10322-3293">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="10322-3294">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="10322-3294">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="10322-3295">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="10322-3295">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="10322-3296">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="10322-3296">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="10322-3297">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="10322-3297">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="10322-3298">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="10322-3298">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="10322-3299">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="10322-3299">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="10322-3300">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="10322-3300">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="10322-3301">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="10322-3301">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="10322-3302">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="10322-3302">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="10322-3303">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="10322-3303">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="10322-3304">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="10322-3304">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="10322-3305">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="10322-3305">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="10322-3306">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="10322-3306">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="10322-3307">ACR</span><span class="sxs-lookup"><span data-stu-id="10322-3307">ACR</span></span>

* <span data-ttu-id="10322-3308">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="10322-3308">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="10322-3309">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="10322-3309">Support SKU update for managed registries</span></span>
* <span data-ttu-id="10322-3310">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="10322-3310">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="10322-3311">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="10322-3311">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="10322-3312">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="10322-3312">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="10322-3313">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="10322-3313">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="10322-3314">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-3314">ACS</span></span>

* <span data-ttu-id="10322-3315">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="10322-3315">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-3316">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-3316">Appservice</span></span>

* <span data-ttu-id="10322-3317">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="10322-3317">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="10322-3318">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="10322-3318">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="10322-3319">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="10322-3319">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="10322-3320">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="10322-3320">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="10322-3321">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="10322-3321">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="10322-3322">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="10322-3322">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="10322-3323">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="10322-3323">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="10322-3324">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="10322-3324">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="10322-3325">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="10322-3325">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="10322-3326">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="10322-3326">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="10322-3327">Lote</span><span class="sxs-lookup"><span data-stu-id="10322-3327">Batch</span></span>

* <span data-ttu-id="10322-3328">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="10322-3328">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="10322-3329">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="10322-3329">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="10322-3330">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="10322-3330">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="10322-3331">CDN</span><span class="sxs-lookup"><span data-stu-id="10322-3331">CDN</span></span>

* <span data-ttu-id="10322-3332">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="10322-3332">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="10322-3333">Nuvem</span><span class="sxs-lookup"><span data-stu-id="10322-3333">Cloud</span></span>

* <span data-ttu-id="10322-3334">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="10322-3334">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="10322-3335">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="10322-3335">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="10322-3336">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="10322-3336">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="10322-3337">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="10322-3337">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="10322-3338">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="10322-3338">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="10322-3339">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="10322-3339">CosmosDB</span></span>

* <span data-ttu-id="10322-3340">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="10322-3340">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="10322-3341">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="10322-3341">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="10322-3342">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="10322-3342">Data Lake Analytics</span></span>

* <span data-ttu-id="10322-3343">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="10322-3343">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="10322-3344">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="10322-3344">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="10322-3345">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="10322-3345">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="10322-3346">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="10322-3346">Data Lake Store</span></span>

* <span data-ttu-id="10322-3347">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="10322-3347">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="10322-3348">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="10322-3348">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="10322-3349">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="10322-3349">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="10322-3350">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="10322-3350">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="10322-3351">Interativo</span><span class="sxs-lookup"><span data-stu-id="10322-3351">Interactive</span></span>

* <span data-ttu-id="10322-3352">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="10322-3352">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="10322-3353">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="10322-3353">Increased test coverage</span></span>
* <span data-ttu-id="10322-3354">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="10322-3354">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="10322-3355">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="10322-3355">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="10322-3356">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="10322-3356">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="10322-3357">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="10322-3357">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="10322-3358">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="10322-3358">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="10322-3359">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="10322-3359">Added `--progress` flag</span></span>
* <span data-ttu-id="10322-3360">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="10322-3360">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="10322-3361">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="10322-3361">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="10322-3362">IoT</span><span class="sxs-lookup"><span data-stu-id="10322-3362">IoT</span></span>

* <span data-ttu-id="10322-3363">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="10322-3363">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="10322-3364">(#3934)</span><span class="sxs-lookup"><span data-stu-id="10322-3364">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="10322-3365">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="10322-3365">Key vault</span></span>

* <span data-ttu-id="10322-3366">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="10322-3366">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="10322-3367">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="10322-3367">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="10322-3368">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="10322-3368">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="10322-3369">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="10322-3369">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="10322-3370">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="10322-3370">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="10322-3371">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="10322-3371">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="10322-3372">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="10322-3372">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="10322-3373">(#3307)</span><span class="sxs-lookup"><span data-stu-id="10322-3373">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="10322-3374">Laboratório</span><span class="sxs-lookup"><span data-stu-id="10322-3374">Lab</span></span>

* <span data-ttu-id="10322-3375">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="10322-3375">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="10322-3376">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="10322-3376">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-3377">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-3377">Monitor</span></span>

* <span data-ttu-id="10322-3378">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="10322-3378">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="10322-3379">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="10322-3379">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="10322-3380">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="10322-3380">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="10322-3381">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="10322-3381">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="10322-3382">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="10322-3382">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="10322-3383">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="10322-3383">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="10322-3384">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="10322-3384">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="10322-3385">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="10322-3385">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="10322-3386">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="10322-3386">`location` no longer required</span></span>
  * <span data-ttu-id="10322-3387">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="10322-3387">Add name and ID support for target</span></span>
  * <span data-ttu-id="10322-3388">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="10322-3388">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="10322-3389">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="10322-3389">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="10322-3390">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="10322-3390">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="10322-3391">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="10322-3391">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="10322-3392">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="10322-3392">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="10322-3393">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="10322-3393">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="10322-3394">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-3394">Network</span></span>

* <span data-ttu-id="10322-3395">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="10322-3395">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="10322-3396">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="10322-3396">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="10322-3397">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="10322-3397">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="10322-3398">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="10322-3398">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="10322-3399">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="10322-3399">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="10322-3400">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="10322-3400">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="10322-3401">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="10322-3401">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="10322-3402">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="10322-3402">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="10322-3403">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="10322-3403">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="10322-3404">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="10322-3404">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="10322-3405">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="10322-3405">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="10322-3406">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="10322-3406">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="10322-3407">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="10322-3407">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="10322-3408">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="10322-3408">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="10322-3409">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="10322-3409">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="10322-3410">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="10322-3410">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="10322-3411">Adicionado o suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para --dns-servers</span><span class="sxs-lookup"><span data-stu-id="10322-3411">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="10322-3412">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="10322-3412">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="10322-3413">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="10322-3413">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="10322-3414">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="10322-3414">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="10322-3415">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="10322-3415">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="10322-3416">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="10322-3416">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="10322-3417">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="10322-3417">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="10322-3418">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="10322-3418">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="10322-3419">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="10322-3419">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="10322-3420">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="10322-3420">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="10322-3421">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="10322-3421">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="10322-3422">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-3422">Profile</span></span>

* <span data-ttu-id="10322-3423">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="10322-3423">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="10322-3424">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="10322-3424">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="10322-3425">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="10322-3425">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="10322-3426">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="10322-3426">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="10322-3427">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="10322-3427">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="10322-3428">RDBMS</span><span class="sxs-lookup"><span data-stu-id="10322-3428">RDBMS</span></span>

* <span data-ttu-id="10322-3429">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="10322-3429">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="10322-3430">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="10322-3430">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="10322-3431">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="10322-3431">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="10322-3432">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="10322-3432">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="10322-3433">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-3433">Resource</span></span>

* <span data-ttu-id="10322-3434">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="10322-3434">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="10322-3435">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="10322-3435">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="10322-3436">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="10322-3436">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="10322-3437">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="10322-3437">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="10322-3438">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="10322-3438">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="10322-3439">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="10322-3439">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="10322-3440">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="10322-3440">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="10322-3441">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="10322-3441">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="10322-3442">Função</span><span class="sxs-lookup"><span data-stu-id="10322-3442">Role</span></span>

* <span data-ttu-id="10322-3443">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="10322-3443">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="10322-3444">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="10322-3444">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="10322-3445">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="10322-3445">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="10322-3446">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="10322-3446">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="10322-3447">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="10322-3447">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="10322-3448">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="10322-3448">Service Fabric</span></span>
* <span data-ttu-id="10322-3449">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="10322-3449">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="10322-3450">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="10322-3450">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="10322-3451">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="10322-3451">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="10322-3452">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-3452">SQL</span></span>

* <span data-ttu-id="10322-3453">Removido o parâmetro `sql server create` `--identity` desfeito</span><span class="sxs-lookup"><span data-stu-id="10322-3453">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="10322-3454">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="10322-3454">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="10322-3455">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="10322-3455">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="10322-3456">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-3456">Storage</span></span>

* <span data-ttu-id="10322-3457">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="10322-3457">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="10322-3458">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="10322-3458">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="10322-3459">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="10322-3459">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="10322-3460">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="10322-3460">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="10322-3461">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="10322-3461">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="10322-3462">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="10322-3462">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="10322-3463">VM</span><span class="sxs-lookup"><span data-stu-id="10322-3463">VM</span></span>

* <span data-ttu-id="10322-3464">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="10322-3464">Support configuring nsg</span></span>
* <span data-ttu-id="10322-3465">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="10322-3465">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="10322-3466">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="10322-3466">Support managed service identities</span></span>
* <span data-ttu-id="10322-3467">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="10322-3467">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="10322-3468">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="10322-3468">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="10322-3469">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="10322-3469">May 10, 2017</span></span>

<span data-ttu-id="10322-3470">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="10322-3470">Version 2.0.6</span></span>

* <span data-ttu-id="10322-3471">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="10322-3471">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="10322-3472">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="10322-3472">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="10322-3473">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="10322-3473">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="10322-3474">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="10322-3474">Include Cognitive Services module</span></span>
* <span data-ttu-id="10322-3475">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="10322-3475">Include Service Fabric module</span></span>
* <span data-ttu-id="10322-3476">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="10322-3476">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="10322-3477">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="10322-3477">Add support for CDN commands</span></span>
* <span data-ttu-id="10322-3478">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="10322-3478">Remove Container module</span></span>
* <span data-ttu-id="10322-3479">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="10322-3479">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="10322-3480">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="10322-3480">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="10322-3481">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-3481">Core</span></span>

* <span data-ttu-id="10322-3482">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="10322-3482">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="10322-3483">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="10322-3483">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="10322-3484">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="10322-3484">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="10322-3485">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="10322-3485">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="10322-3486">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="10322-3486">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="10322-3487">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="10322-3487">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="10322-3488">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="10322-3488">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="10322-3489">núcleo: permitir que o caminho do arquivo accessTokens.json seja configurável por meio de uma variável de ambiente ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="10322-3489">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="10322-3490">núcleo: permitir que padrões configurados sejam aplicados em argumentos opcionais ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="10322-3490">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="10322-3491">núcleo: desempenho aprimorado</span><span class="sxs-lookup"><span data-stu-id="10322-3491">core: Improved performance</span></span>
* <span data-ttu-id="10322-3492">núcleo: certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="10322-3492">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="10322-3493">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="10322-3493">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="10322-3494">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-3494">ACS</span></span>

* <span data-ttu-id="10322-3495">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10322-3495">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="10322-3496">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="10322-3496">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="10322-3497">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="10322-3497">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="10322-3498">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="10322-3498">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-3499">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-3499">AppService</span></span>

* <span data-ttu-id="10322-3500">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="10322-3500">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="10322-3501">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="10322-3501">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="10322-3502">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="10322-3502">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="10322-3503">Exposição de argumentos para configurar a implantação e as “pilhas em runtime” em webapp create</span><span class="sxs-lookup"><span data-stu-id="10322-3503">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="10322-3504">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="10322-3504">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="10322-3505">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="10322-3505">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="10322-3506">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="10322-3506">support slot swap with preview</span></span>
* <span data-ttu-id="10322-3507">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="10322-3507">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="10322-3508">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="10322-3508">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="10322-3509">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="10322-3509">CosmosDB</span></span>

* <span data-ttu-id="10322-3510">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="10322-3510">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="10322-3511">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="10322-3511">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="10322-3512">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="10322-3512">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="10322-3513">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="10322-3513">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="10322-3514">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="10322-3514">Data Lake Analytics</span></span>

* <span data-ttu-id="10322-3515">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="10322-3515">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="10322-3516">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="10322-3516">Add support for new catalog item type: package.</span></span> <span data-ttu-id="10322-3517">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="10322-3517">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="10322-3518">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="10322-3518">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="10322-3519">Tabela</span><span class="sxs-lookup"><span data-stu-id="10322-3519">Table</span></span>
  * <span data-ttu-id="10322-3520">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="10322-3520">Table valued function</span></span>
  * <span data-ttu-id="10322-3521">Visualizar</span><span class="sxs-lookup"><span data-stu-id="10322-3521">View</span></span>
  * <span data-ttu-id="10322-3522">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="10322-3522">Table Statistics.</span></span> <span data-ttu-id="10322-3523">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="10322-3523">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="10322-3524">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="10322-3524">Data Lake Store</span></span>

* <span data-ttu-id="10322-3525">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="10322-3525">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="10322-3526">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="10322-3526">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="10322-3527">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="10322-3527">missed help for access show.</span></span> <span data-ttu-id="10322-3528">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="10322-3528">adding it.</span></span> <span data-ttu-id="10322-3529">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="10322-3529">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="10322-3530">Localizar</span><span class="sxs-lookup"><span data-stu-id="10322-3530">Find</span></span>

* <span data-ttu-id="10322-3531">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="10322-3531">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="10322-3532">KeyVault</span><span class="sxs-lookup"><span data-stu-id="10322-3532">KeyVault</span></span>

* <span data-ttu-id="10322-3533">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="10322-3533">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="10322-3534">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois estes parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="10322-3534">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="10322-3535">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="10322-3535">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="10322-3536">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="10322-3536">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="10322-3537">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="10322-3537">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="10322-3538">Laboratório</span><span class="sxs-lookup"><span data-stu-id="10322-3538">Lab</span></span>

* <span data-ttu-id="10322-3539">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="10322-3539">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="10322-3540">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="10322-3540">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="10322-3541">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="10322-3541">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="10322-3542">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="10322-3542">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="10322-3543">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="10322-3543">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="10322-3544">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="10322-3544">Monitor</span></span>

* <span data-ttu-id="10322-3545">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="10322-3545">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="10322-3546">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="10322-3546">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="10322-3547">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-3547">Network</span></span>

* <span data-ttu-id="10322-3548">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="10322-3548">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="10322-3549">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="10322-3549">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="10322-3550">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10322-3550">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="10322-3551">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10322-3551">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="10322-3552">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="10322-3552">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="10322-3553">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="10322-3553">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="10322-3554">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="10322-3554">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="10322-3555">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="10322-3555">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="10322-3556">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="10322-3556">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="10322-3557">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="10322-3557">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="10322-3558">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="10322-3558">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="10322-3559">BC: corrigido um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="10322-3559">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="10322-3560">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="10322-3560">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="10322-3561">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="10322-3561">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="10322-3562">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="10322-3562">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="10322-3563">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="10322-3563">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="10322-3564">Perfil</span><span class="sxs-lookup"><span data-stu-id="10322-3564">Profile</span></span>

* <span data-ttu-id="10322-3565">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="10322-3565">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="10322-3566">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="10322-3566">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="10322-3567">Redis</span><span class="sxs-lookup"><span data-stu-id="10322-3567">Redis</span></span>

* <span data-ttu-id="10322-3568">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="10322-3568">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="10322-3569">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="10322-3569">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="10322-3570">Recurso</span><span class="sxs-lookup"><span data-stu-id="10322-3570">Resource</span></span>

* <span data-ttu-id="10322-3571">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="10322-3571">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="10322-3572">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="10322-3572">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="10322-3573">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="10322-3573">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="10322-3574">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="10322-3574">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="10322-3575">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="10322-3575">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="10322-3576">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="10322-3576">Add docs for az lock update.</span></span> <span data-ttu-id="10322-3577">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="10322-3577">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="10322-3578">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="10322-3578">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="10322-3579">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="10322-3579">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="10322-3580">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="10322-3580">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="10322-3581">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="10322-3581">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="10322-3582">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="10322-3582">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="10322-3583">Função</span><span class="sxs-lookup"><span data-stu-id="10322-3583">Role</span></span>

* <span data-ttu-id="10322-3584">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="10322-3584">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="10322-3585">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="10322-3585">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="10322-3586">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="10322-3586">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="10322-3587">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="10322-3587">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="10322-3588">SQL</span><span class="sxs-lookup"><span data-stu-id="10322-3588">SQL</span></span>

* <span data-ttu-id="10322-3589">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="10322-3589">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="10322-3590">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="10322-3590">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="10322-3591">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-3591">Storage</span></span>

* <span data-ttu-id="10322-3592">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="10322-3592">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="10322-3593">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="10322-3593">Add support for incremental blob copy</span></span>
* <span data-ttu-id="10322-3594">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="10322-3594">Add support for large block blob upload</span></span>
* <span data-ttu-id="10322-3595">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="10322-3595">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="10322-3596">VM</span><span class="sxs-lookup"><span data-stu-id="10322-3596">VM</span></span>

* <span data-ttu-id="10322-3597">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="10322-3597">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="10322-3598">observação: em comandos da VM em nuvens soberanas, evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="10322-3598">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="10322-3599">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="10322-3599">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="10322-3600">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="10322-3600">az vm/vmss disk</span></span>
  3. <span data-ttu-id="10322-3601">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="10322-3601">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="10322-3602">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="10322-3602">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="10322-3603">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="10322-3603">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="10322-3604">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="10322-3604">April 3, 2017</span></span>

<span data-ttu-id="10322-3605">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="10322-3605">Version 2.0.2</span></span>

<span data-ttu-id="10322-3606">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="10322-3606">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="10322-3607">Núcleo</span><span class="sxs-lookup"><span data-stu-id="10322-3607">Core</span></span>

* <span data-ttu-id="10322-3608">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="10322-3608">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="10322-3609">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="10322-3609">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="10322-3610">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="10322-3610">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="10322-3611">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="10322-3611">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="10322-3612">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="10322-3612">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="10322-3613">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="10322-3613">Add prompting for missing template parameters.</span></span> <span data-ttu-id="10322-3614">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="10322-3614">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="10322-3615">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="10322-3615">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="10322-3616">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="10322-3616">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="10322-3617">ACS</span><span class="sxs-lookup"><span data-stu-id="10322-3617">ACS</span></span>

* <span data-ttu-id="10322-3618">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="10322-3618">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="10322-3619">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="10322-3619">Add support for ssh key password prompting.</span></span> <span data-ttu-id="10322-3620">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="10322-3620">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="10322-3621">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="10322-3621">Add support for windows clusters.</span></span> <span data-ttu-id="10322-3622">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="10322-3622">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="10322-3623">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="10322-3623">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="10322-3624">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="10322-3624">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="10322-3625">AppService</span><span class="sxs-lookup"><span data-stu-id="10322-3625">AppService</span></span>

* <span data-ttu-id="10322-3626">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="10322-3626">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="10322-3627">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="10322-3627">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="10322-3628">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="10322-3628">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="10322-3629">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="10322-3629">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="10322-3630">DataLake</span><span class="sxs-lookup"><span data-stu-id="10322-3630">DataLake</span></span>

* <span data-ttu-id="10322-3631">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="10322-3631">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="10322-3632">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="10322-3632">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="10322-3633">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="10322-3633">DocuemntDB</span></span>

* <span data-ttu-id="10322-3634">DocumentDB: adicionado suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="10322-3634">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="10322-3635">VM</span><span class="sxs-lookup"><span data-stu-id="10322-3635">VM</span></span>

* <span data-ttu-id="10322-3636">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="10322-3636">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="10322-3637">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="10322-3637">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="10322-3638">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="10322-3638">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="10322-3639">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="10322-3639">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="10322-3640">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="10322-3640">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="10322-3641">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="10322-3641">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="10322-3642">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="10322-3642">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="10322-3643">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="10322-3643">February 27, 2017</span></span>

<span data-ttu-id="10322-3644">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="10322-3644">Version 2.0.0</span></span>

<span data-ttu-id="10322-3645">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="10322-3645">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="10322-3646">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="10322-3646">Container Service (acs)</span></span>
- <span data-ttu-id="10322-3647">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="10322-3647">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="10322-3648">Rede</span><span class="sxs-lookup"><span data-stu-id="10322-3648">Networking</span></span>
- <span data-ttu-id="10322-3649">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="10322-3649">Storage</span></span>

<span data-ttu-id="10322-3650">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="10322-3650">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="10322-3651">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="10322-3651">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="10322-3652">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="10322-3652">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="10322-3653">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="10322-3653">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="10322-3654">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="10322-3654">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="10322-3655">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="10322-3655">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="10322-3656">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="10322-3656">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="10322-3657">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="10322-3657">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="10322-3658">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="10322-3658">Provide feedback from the command line with the `az feedback` command</span></span>
