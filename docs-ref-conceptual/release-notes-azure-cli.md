---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 04/01/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: cca6f42f29467126553c6e8a332907b1ad1ebc74
ms.sourcegitcommit: 712c8ca6457552b6b7a8866c1370a6ec51d07f2c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2020
ms.locfileid: "80525254"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="1dfd6-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="1dfd6-103">Azure CLI release notes</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="1dfd6-104">1º de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="1dfd6-104">April 01, 2020</span></span>

<span data-ttu-id="1dfd6-105">Versão 2.3.1</span><span class="sxs-lookup"><span data-stu-id="1dfd6-105">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-106">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-106">ACR</span></span>

* <span data-ttu-id="1dfd6-107">Corrigir a versão errada do azure-mgmt-containerregistry para Linux</span><span class="sxs-lookup"><span data-stu-id="1dfd6-107">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="1dfd6-108">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-108">Profile</span></span>

* <span data-ttu-id="1dfd6-109">az login: Corrigir falha de logon com perfis de nuvem diferentes de `latest`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-109">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="1dfd6-110">31 de março de 2020</span><span class="sxs-lookup"><span data-stu-id="1dfd6-110">March 31, 2020</span></span>

<span data-ttu-id="1dfd6-111">Versão 2.3.0</span><span class="sxs-lookup"><span data-stu-id="1dfd6-111">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-112">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-112">ACR</span></span>

* <span data-ttu-id="1dfd6-113">'az acr task update': exceção de ponteiro nulo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-113">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="1dfd6-114">`az acr import`: Modificar a mensagem de ajuda e de erro para esclarecer o uso de --source e --registry</span><span class="sxs-lookup"><span data-stu-id="1dfd6-114">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="1dfd6-115">Adicionar um validador para o argumento 'registry_name'</span><span class="sxs-lookup"><span data-stu-id="1dfd6-115">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="1dfd6-116">`az acr login`: remover o sinalizador de visualização em '--expose-token'</span><span class="sxs-lookup"><span data-stu-id="1dfd6-116">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="1dfd6-117">O parâmetro de branch 'az acr task create/update' de [ALTERAÇÃO SIGNIFICATIVA] foi removido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-117">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="1dfd6-118">O cliente 'az acr task update' agora pode atualizar o contexto, o token do git e/ou os gatilhos individualmente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-118">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="1dfd6-119">'az acr agentpool': novo recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-119">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="1dfd6-120">AKS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-120">AKS</span></span>

* <span data-ttu-id="1dfd6-121">Corrigir apiServerAccessProfile ao atualizar --api-server-authorized-ip-ranges</span><span class="sxs-lookup"><span data-stu-id="1dfd6-121">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="1dfd6-122">aks update: Substituir IPs de saída por valores de entrada ao atualizar</span><span class="sxs-lookup"><span data-stu-id="1dfd6-122">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="1dfd6-123">Não criar SPN para clusters MSI e dar suporte à anexação de ACR a clusters MSI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-123">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="1dfd6-124">AMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-124">AMS</span></span>

* <span data-ttu-id="1dfd6-125">Correção nº. 12469: a adição da política de chave de conteúdo Fairplay falha devido a problemas com o parâmetro 'ask'</span><span class="sxs-lookup"><span data-stu-id="1dfd6-125">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="1dfd6-126">AppConfig</span><span class="sxs-lookup"><span data-stu-id="1dfd6-126">AppConfig</span></span>

* <span data-ttu-id="1dfd6-127">Adicionar --skip-keyvault a kv export</span><span class="sxs-lookup"><span data-stu-id="1dfd6-127">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-128">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-128">AppService</span></span>

* <span data-ttu-id="1dfd6-129">Correção nº 12509: remover a marca para az webapp up por padrão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-129">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="1dfd6-130">az functionapp create: o menu de ajuda de --runtime-version foi atualizado e um aviso foi adicionado quando o usuário especifica --runtime-version para dotnet</span><span class="sxs-lookup"><span data-stu-id="1dfd6-130">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="1dfd6-131">az functionapp create: atualizado o modo como o javaVersion estava sendo definido para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="1dfd6-131">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="1dfd6-132">ARM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-132">ARM</span></span>

* <span data-ttu-id="1dfd6-133">az deployment create/validate: usar --handle-extended-json-format por padrão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-133">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="1dfd6-134">az lock create: adicionar exemplos de criação de subrecurso na documentação da ajuda</span><span class="sxs-lookup"><span data-stu-id="1dfd6-134">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="1dfd6-135">az deployment {group/mg/sub/tenant} list: dar suporte à filtragem de provisioningState</span><span class="sxs-lookup"><span data-stu-id="1dfd6-135">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="1dfd6-136">az deployment: corrigir o bug de análise para o comentário no último argumento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-136">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="1dfd6-137">Backup</span><span class="sxs-lookup"><span data-stu-id="1dfd6-137">Backup</span></span>

* <span data-ttu-id="1dfd6-138">Adicionadas várias funcionalidades de restauração de arquivo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-138">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="1dfd6-139">Adicionado suporte para backup somente de discos do SO</span><span class="sxs-lookup"><span data-stu-id="1dfd6-139">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="1dfd6-140">Adicionado o parâmetro restore-as-unmanaged-disk para especificar a restauração não gerenciada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-140">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="1dfd6-141">Computação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-141">Compute</span></span>

* <span data-ttu-id="1dfd6-142">az vm create: adicionar opção NONE de --nsg-rule</span><span class="sxs-lookup"><span data-stu-id="1dfd6-142">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="1dfd6-143">az vmss create/update: remover a marca de visualização de reparos automáticos do vmss</span><span class="sxs-lookup"><span data-stu-id="1dfd6-143">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="1dfd6-144">az vm update: dar suporte a --workspace</span><span class="sxs-lookup"><span data-stu-id="1dfd6-144">az vm update: Support --workspace</span></span>
* <span data-ttu-id="1dfd6-145">Corrigir um bug no código de inicialização de VirtualMachineScaleSetExtension</span><span class="sxs-lookup"><span data-stu-id="1dfd6-145">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="1dfd6-146">Atualizar a versão do VMAccessAgent para 2.4</span><span class="sxs-lookup"><span data-stu-id="1dfd6-146">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="1dfd6-147">az vmss set-orchestration-service-state: dar suporte para o estado de definição do serviço de orquestração do vmss</span><span class="sxs-lookup"><span data-stu-id="1dfd6-147">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="1dfd6-148">Atualizar a API do disco para a versão 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="1dfd6-148">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="1dfd6-149">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span><span class="sxs-lookup"><span data-stu-id="1dfd6-149">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="1dfd6-150">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-150">Cosmos DB</span></span>

* <span data-ttu-id="1dfd6-151">Corrigir a ausência da opção --type para redirecionamentos de preterimento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-151">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="1dfd6-152">Docker</span><span class="sxs-lookup"><span data-stu-id="1dfd6-152">Docker</span></span>

* <span data-ttu-id="1dfd6-153">Atualizar para Alpine 3.11 e Python 3.6.10</span><span class="sxs-lookup"><span data-stu-id="1dfd6-153">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="1dfd6-154">Extensão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-154">Extension</span></span>

* <span data-ttu-id="1dfd6-155">Permitir carregar extensões no caminho do sistema por meio de pacotes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-155">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1dfd6-156">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1dfd6-156">HDInsight</span></span>

* <span data-ttu-id="1dfd6-157">(az hdinsight create:) dar suporte à especificação da versão de TLS mínima pelos clientes usando o parâmetro `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-157">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="1dfd6-158">O valor permitido é 1.0,1.1,1.2</span><span class="sxs-lookup"><span data-stu-id="1dfd6-158">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="1dfd6-159">IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-159">IoT</span></span>

* <span data-ttu-id="1dfd6-160">Adicionar codeowner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-160">Add codeowner</span></span>
* <span data-ttu-id="1dfd6-161">az iot hub create : alterar o SKU padrão de F1 para S1</span><span class="sxs-lookup"><span data-stu-id="1dfd6-161">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="1dfd6-162">iot hub: dar suporte a IotHub no perfil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="1dfd6-162">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="1dfd6-163">IoT Central</span><span class="sxs-lookup"><span data-stu-id="1dfd6-163">IoTCentral</span></span>

* <span data-ttu-id="1dfd6-164">Atualizar detalhes do erro, atualizar modelo de aplicativo padrão e a mensagem de aviso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-164">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="1dfd6-165">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-165">KeyVault</span></span>

* <span data-ttu-id="1dfd6-166">Suporte para backup/restauração de certificado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-166">Support certificate backup/restore</span></span>
* <span data-ttu-id="1dfd6-167">keyvault create/update: Suporte a --retention-days</span><span class="sxs-lookup"><span data-stu-id="1dfd6-167">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="1dfd6-168">Não exibir mais chaves/segredos gerenciados durante a listagem</span><span class="sxs-lookup"><span data-stu-id="1dfd6-168">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="1dfd6-169">az keyvault create: suporte a `--network-acls`, `--network-acls-ips` e `--network-acls-vnets` para especificar regras de rede ao criar o cofre</span><span class="sxs-lookup"><span data-stu-id="1dfd6-169">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="1dfd6-170">Bloqueio</span><span class="sxs-lookup"><span data-stu-id="1dfd6-170">Lock</span></span>

* <span data-ttu-id="1dfd6-171">az lock delete fix bug: az lock delete não funciona no Microsoft.DocumentDB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-171">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="1dfd6-172">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-172">Monitor</span></span>

* <span data-ttu-id="1dfd6-173">az monitor clone: suporte a regras de métrica de clone de um recurso para outro</span><span class="sxs-lookup"><span data-stu-id="1dfd6-173">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="1dfd6-174">Corrigir IcM179210086: não é possível criar um alerta de métrica personalizado para a métrica de Application Insights</span><span class="sxs-lookup"><span data-stu-id="1dfd6-174">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="1dfd6-175">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="1dfd6-175">NetAppFiles</span></span>

* <span data-ttu-id="1dfd6-176">az volume create: permitir volumes de proteção de dados adicionando operações de replicação: approve, suspend, resume, status, remove</span><span class="sxs-lookup"><span data-stu-id="1dfd6-176">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-177">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-177">Network</span></span>

* <span data-ttu-id="1dfd6-178">az network application-gateway waf-policy managed-rule rule-set add: dar suporte a Microsoft_BotManagerRuleSet</span><span class="sxs-lookup"><span data-stu-id="1dfd6-178">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="1dfd6-179">network watcher flow-log show: corrigir informações erradas em preterimento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-179">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="1dfd6-180">dar suporte a nomes de host no ouvinte do gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-180">support host names in application gateway listener</span></span>
* <span data-ttu-id="1dfd6-181">az network nat gateway: dar suporte para criar um recurso vazio sem IP público nem prefixo de IP público</span><span class="sxs-lookup"><span data-stu-id="1dfd6-181">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="1dfd6-182">Dar suporte à geração de gateway de VPN</span><span class="sxs-lookup"><span data-stu-id="1dfd6-182">Support vpn gateway generation</span></span>
* <span data-ttu-id="1dfd6-183">Dar suporte a `--if-none-match` em `az network dns record-set {} add-record`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-183">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="1dfd6-184">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-184">Packaging</span></span>

* <span data-ttu-id="1dfd6-185">Remover o suporte ao Python 3.5</span><span class="sxs-lookup"><span data-stu-id="1dfd6-185">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="1dfd6-186">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-186">Profile</span></span>

* <span data-ttu-id="1dfd6-187">az login: Mostrar aviso para erro de MFA</span><span class="sxs-lookup"><span data-stu-id="1dfd6-187">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="1dfd6-188">RDBMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-188">RDBMS</span></span>

* <span data-ttu-id="1dfd6-189">Adicionar comandos de gerenciamento de chaves de criptografia de dados do servidor para PostgreSQL e MySQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-189">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="1dfd6-190">10 de março de 2020</span><span class="sxs-lookup"><span data-stu-id="1dfd6-190">March 10, 2020</span></span>

<span data-ttu-id="1dfd6-191">Versão 2.2.0</span><span class="sxs-lookup"><span data-stu-id="1dfd6-191">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-192">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-192">ACR</span></span>

* <span data-ttu-id="1dfd6-193">Correção: `az acr login` gerava erro incorretamente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-193">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="1dfd6-194">Adicionou o novo comando `az acr helm install-cli`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-194">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="1dfd6-195">Adicionou link privado e suporte do CMK</span><span class="sxs-lookup"><span data-stu-id="1dfd6-195">Add private link and CMK support</span></span>
* <span data-ttu-id="1dfd6-196">Adicionou o comando 'private-link-resource list'</span><span class="sxs-lookup"><span data-stu-id="1dfd6-196">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="1dfd6-197">AKS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-197">AKS</span></span>

* <span data-ttu-id="1dfd6-198">correção da busca do AKS no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="1dfd6-198">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="1dfd6-199">az aks: correção dos erros de complemento de monitoramento e de agentpool NoneType</span><span class="sxs-lookup"><span data-stu-id="1dfd6-199">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="1dfd6-200">Adicionou --nodepool-tags ao pool de nós ao criar o cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="1dfd6-200">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="1dfd6-201">Adicionou --tags ao adicionar ou atualizar um pool de nós para o cluster</span><span class="sxs-lookup"><span data-stu-id="1dfd6-201">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="1dfd6-202">AKS create: adicionou `--enable-private-cluster`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-202">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="1dfd6-203">Adicionou --nodepool-labels ao criar o cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="1dfd6-203">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="1dfd6-204">Adicionou --labels ao adicionar um novo pool de nós ao cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="1dfd6-204">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="1dfd6-205">Adicionou / ausente na URL do painel</span><span class="sxs-lookup"><span data-stu-id="1dfd6-205">add missing / in the dashboard url</span></span>
* <span data-ttu-id="1dfd6-206">Suporte para criar clusters do AKS habilitando identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-206">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="1dfd6-207">az aks: validou o plug-in de rede como "Azure" ou "Kubenet"</span><span class="sxs-lookup"><span data-stu-id="1dfd6-207">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="1dfd6-208">az aks: adicionou suporte da chave da sessão do AAD</span><span class="sxs-lookup"><span data-stu-id="1dfd6-208">az aks: Add aad session key support</span></span>
* <span data-ttu-id="1dfd6-209">[ALTERAÇÃO SIGNIFICATIVA] AZ AKS: suporte para alterações de MSI para GF e BF para omsagent (Monitoramento de contêiner) (#1)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-209">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="1dfd6-210">az aks use-dev-spaces: adicionou a opção de tipo de ponto de extremidade ao comando use-dev-spaces para personalizar o ponto de extremidade criado em um controlador Azure Dev Spaces</span><span class="sxs-lookup"><span data-stu-id="1dfd6-210">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="1dfd6-211">AppConfig</span><span class="sxs-lookup"><span data-stu-id="1dfd6-211">AppConfig</span></span>

* <span data-ttu-id="1dfd6-212">Desbloqueou usando "KV set" para adicionar o recurso e a referência do keyvault...</span><span class="sxs-lookup"><span data-stu-id="1dfd6-212">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-213">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-213">AppService</span></span>

* <span data-ttu-id="1dfd6-214">az webapp create: correção do problema ao executar o comando com --runtime</span><span class="sxs-lookup"><span data-stu-id="1dfd6-214">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="1dfd6-215">az functionapp deployment source config-zip: adicionou uma mensagem de erro se o grupo de recursos ou o nome da função forem inválidos/não existirem</span><span class="sxs-lookup"><span data-stu-id="1dfd6-215">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="1dfd6-216">functionapp create: correção da mensagem de aviso que aparece com `functionapp create` hoje, que cita um sinalizador de `--functions_version`, mas usa erroneamente `_` em vez de `-` no nome do sinalizador</span><span class="sxs-lookup"><span data-stu-id="1dfd6-216">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="1dfd6-217">az functionapp create: atualizou o modo como linuxFxVersion e o nome da imagem de contêiner eram definidos para aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="1dfd6-217">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="1dfd6-218">az functionapp deployment source config-zip: correção de um problema causado pelas configurações do aplicativo que alterava a condição de corrida durante a implantação do zip, provocando erros 5xx durante a implantação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-218">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="1dfd6-219">Correção #5720946: AZ WebApp backup falha ao definir o nome</span><span class="sxs-lookup"><span data-stu-id="1dfd6-219">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="1dfd6-220">ARM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-220">ARM</span></span>

* <span data-ttu-id="1dfd6-221">az resource: aprimorou os exemplos do módulo de recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-221">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="1dfd6-222">az policy assignment list: suporte à listagem de atribuições de política no escopo do Grupo de Gerenciamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-222">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="1dfd6-223">Adicionou `az deployment group` e `az deployment operation group` para a implantação de modelos nos grupos de recursos.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-223">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="1dfd6-224">Esta é uma duplicata de `az group deployment` e `az group deployment operation`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-224">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="1dfd6-225">Adicionou `az deployment sub` e `az deployment operation sub` para a implantação de modelos no escopo da assinatura.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-225">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="1dfd6-226">Esta é uma duplicata de `az deployment` e `az deployment operation`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-226">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="1dfd6-227">Adicionou `az deployment mg` e `az deployment operation mg` para implantação de modelos nos grupos de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-227">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="1dfd6-228">Adicionou `az deployment tenant` e `az deployment operation tenant` para implantação de modelos no escopo do locatário.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-228">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="1dfd6-229">az policy assignment create: adicionou descrição ao parâmetro `--location`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-229">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="1dfd6-230">az group deployment create: adicionou o parâmetro `--aux-tenants` para dar suporte a locatários cruzados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-230">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="1dfd6-231">CDN</span><span class="sxs-lookup"><span data-stu-id="1dfd6-231">CDN</span></span>

* <span data-ttu-id="1dfd6-232">Adicionou comandos do WAF da CDN</span><span class="sxs-lookup"><span data-stu-id="1dfd6-232">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="1dfd6-233">Computação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-233">Compute</span></span>

* <span data-ttu-id="1dfd6-234">az sig image-version: adicionar --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="1dfd6-234">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="1dfd6-235">AZ PPG show: adicionou --outlocation-status para habilitar a busca do status de colocalização de todos os recursos no grupo de posicionamento por proximidade</span><span class="sxs-lookup"><span data-stu-id="1dfd6-235">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="1dfd6-236">az vmss create/update: suporte a reparos automáticos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-236">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="1dfd6-237">[ALTERAÇÃO SIGNIFICATIVA] modelo de imagem AZ: renomear modelo para builder</span><span class="sxs-lookup"><span data-stu-id="1dfd6-237">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="1dfd6-238">AZ Image Builder Create: adicionou --Image-template</span><span class="sxs-lookup"><span data-stu-id="1dfd6-238">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="1dfd6-239">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-239">Cosmos DB</span></span>

* <span data-ttu-id="1dfd6-240">Adicionou procedimento armazenado do SQL, UDF e disparar cmdlets</span><span class="sxs-lookup"><span data-stu-id="1dfd6-240">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="1dfd6-241">az cosmosdb create: adicionou --key-uri para dar suporte à adição de informações de criptografia do cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="1dfd6-241">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="1dfd6-242">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-242">KeyVault</span></span>

* <span data-ttu-id="1dfd6-243">keyvault create: habilitou a exclusão reversível por padrão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-243">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="1dfd6-244">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-244">Monitor</span></span>

* <span data-ttu-id="1dfd6-245">az monitor metrics alert create: suporte a `~` em `--condition`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-245">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-246">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-246">Network</span></span>

* <span data-ttu-id="1dfd6-247">az network application-gateway rewrite-rule create: suporte à configuração de URL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-247">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="1dfd6-248">az network dns zone import: --zone-name não diferenciará maiúsculas de minúsculas no futuro</span><span class="sxs-lookup"><span data-stu-id="1dfd6-248">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="1dfd6-249">az network private-endpoint/private-link-service: removeu rótulo de visualização</span><span class="sxs-lookup"><span data-stu-id="1dfd6-249">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="1dfd6-250">az network bastion: suporte a bastions</span><span class="sxs-lookup"><span data-stu-id="1dfd6-250">az network bastion: support bastion</span></span>
* <span data-ttu-id="1dfd6-251">az network vnet list-available-ips: dar suporte à lista de IPs disponíveis em uma vnet</span><span class="sxs-lookup"><span data-stu-id="1dfd6-251">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="1dfd6-252">az network watcher flow-log create/list/delete/update: adicionou novos comandos para gerenciar o log de fluxo do Inspetor e expor o --local para identificá-lo explicitamente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-252">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="1dfd6-253">az network watcher flow-log configure: preterido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-253">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="1dfd6-254">az network watcher flow-log show: dá suporte a --location e --name para obter o resultado formatado por ARM, saída formatada antiga preterida</span><span class="sxs-lookup"><span data-stu-id="1dfd6-254">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="1dfd6-255">Política</span><span class="sxs-lookup"><span data-stu-id="1dfd6-255">Policy</span></span>

* <span data-ttu-id="1dfd6-256">az policy assignment create: correção do bug que gerou automaticamente o nome da atribuição de política, que excede o limite</span><span class="sxs-lookup"><span data-stu-id="1dfd6-256">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="1dfd6-257">RBAC</span><span class="sxs-lookup"><span data-stu-id="1dfd6-257">RBAC</span></span>

* <span data-ttu-id="1dfd6-258">az ad group show: correção do valor --group, que é tratado como um problema de regex</span><span class="sxs-lookup"><span data-stu-id="1dfd6-258">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="1dfd6-259">RDBMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-259">RDBMS</span></span>

* <span data-ttu-id="1dfd6-260">Trocou a versão do zure-mgmt-rdbms SDK para 2.0.0</span><span class="sxs-lookup"><span data-stu-id="1dfd6-260">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="1dfd6-261">az postgres private-endpoint-connection: gerenciou conexões de ponto de extremidade privado do Postgres</span><span class="sxs-lookup"><span data-stu-id="1dfd6-261">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="1dfd6-262">az postgres private-link-resource: gerenciou recursos de link privado do Postgres</span><span class="sxs-lookup"><span data-stu-id="1dfd6-262">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="1dfd6-263">az mysql private-endpoint-connection: gerenciar conexões de ponto de extremidade privado do MySQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-263">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="1dfd6-264">az mysql private-link-resource: gerenciou recursos de link privado do MySQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-264">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="1dfd6-265">az mariadb private-endpoint-connection: gerenciou conexões de ponto de extremidade privado do MariaDB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-265">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="1dfd6-266">az mariadb private-link-resource: gerenciou recursos de link privado do MariaDB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-266">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="1dfd6-267">Atualizando testes de ponto de extremidade privado do RDBMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-267">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-268">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-268">SQL</span></span>

* <span data-ttu-id="1dfd6-269">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span><span class="sxs-lookup"><span data-stu-id="1dfd6-269">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="1dfd6-270">(sql server create:) adicionou o sinalizador ' habilitar '/' desabilitar ' opcional public-network-access ao SQL Server create</span><span class="sxs-lookup"><span data-stu-id="1dfd6-270">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="1dfd6-271">(sql server update:) fez algumas alterações voltadas para o cliente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-271">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="1dfd6-272">adicionou a propriedade minimal_tls_version para o banco de BD de MI e SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-272">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-273">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-273">Storage</span></span>

* <span data-ttu-id="1dfd6-274">az storage blob delete-batch: sinalizador `--dryrun` de comportamento inadequado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-274">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="1dfd6-275">az storage account network-rule add (correção de bug): a operação de adição deve ser idempotente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-275">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="1dfd6-276">az storage account create/update: Adicionou suporte de preferência de roteamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-276">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="1dfd6-277">Atualizou a versão do azure-mgmt-storage para 8.0.0</span><span class="sxs-lookup"><span data-stu-id="1dfd6-277">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="1dfd6-278">az storage container immutability create: adicionou o parâmetro --allow-protected-append-write</span><span class="sxs-lookup"><span data-stu-id="1dfd6-278">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="1dfd6-279">az storage account private-link-resource list: Adicionou suporte para lista de recursos de link privado para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-279">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="1dfd6-280">az storage account private-endpoint-connection approve/reject/show/delete: Suporte para gerenciar conexões de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-280">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="1dfd6-281">az storage account blob-service-properties update: adicionou --enable-restore-policy e --restore-days</span><span class="sxs-lookup"><span data-stu-id="1dfd6-281">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="1dfd6-282">az storage blob restore: adicionou suporte para restaurar intervalos de blob</span><span class="sxs-lookup"><span data-stu-id="1dfd6-282">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="1dfd6-283">18 de fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="1dfd6-283">February 18, 2020</span></span>

<span data-ttu-id="1dfd6-284">Versão 2.1.0</span><span class="sxs-lookup"><span data-stu-id="1dfd6-284">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-285">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-285">ACR</span></span>

* <span data-ttu-id="1dfd6-286">Adicionar um novo argumento `--expose-token` a `az acr login`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-286">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="1dfd6-287">Corrigir a saída incorreta de `az acr task identity show -n Name -r Registry -o table`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-287">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="1dfd6-288">az acr login: Gerar CLIError se erros forem retornados pelo comando docker</span><span class="sxs-lookup"><span data-stu-id="1dfd6-288">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-289">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-289">ACS</span></span>

* <span data-ttu-id="1dfd6-290">aks create/update: adicionar a validação `--vnet-subnet-id`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-290">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="1dfd6-291">Aladdin</span><span class="sxs-lookup"><span data-stu-id="1dfd6-291">Aladdin</span></span>

* <span data-ttu-id="1dfd6-292">Analisar os exemplos gerados no _help.py do comando</span><span class="sxs-lookup"><span data-stu-id="1dfd6-292">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="1dfd6-293">AMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-293">AMS</span></span>

* <span data-ttu-id="1dfd6-294">az ams já está em GA</span><span class="sxs-lookup"><span data-stu-id="1dfd6-294">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="1dfd6-295">AppConfig</span><span class="sxs-lookup"><span data-stu-id="1dfd6-295">AppConfig</span></span>

* <span data-ttu-id="1dfd6-296">Revisar a mensagem de ajuda para excluir o filtro de chave/rótulo não compatível</span><span class="sxs-lookup"><span data-stu-id="1dfd6-296">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="1dfd6-297">Remover a marca de versão prévia da maioria dos comandos que excluem a identidade gerenciada e têm sinalizadores</span><span class="sxs-lookup"><span data-stu-id="1dfd6-297">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="1dfd6-298">Adicionar a chave gerenciada do cliente ao atualizar os repositórios</span><span class="sxs-lookup"><span data-stu-id="1dfd6-298">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-299">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-299">AppService</span></span>

* <span data-ttu-id="1dfd6-300">az webapp list-runtimes: Corrigir o bug de list-runtimes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-300">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="1dfd6-301">Adicionar az webapp|functionapp config ssl create</span><span class="sxs-lookup"><span data-stu-id="1dfd6-301">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="1dfd6-302">Adicionar compatibilidade com aplicativos de funções v3 e nó 12</span><span class="sxs-lookup"><span data-stu-id="1dfd6-302">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="1dfd6-303">ARM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-303">ARM</span></span>

* <span data-ttu-id="1dfd6-304">az policy assignment create: Corrigir a mensagem de erro quando o parâmetro `--policy` for inválido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-304">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="1dfd6-305">az group deployment create: Corrigir o erro "stat: o caminho é muito longo para o Windows" ao usar o arquivo grande parameters.json</span><span class="sxs-lookup"><span data-stu-id="1dfd6-305">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="1dfd6-306">Backup</span><span class="sxs-lookup"><span data-stu-id="1dfd6-306">Backup</span></span>

* <span data-ttu-id="1dfd6-307">Corrigir o fluxo de recuperação de nível de item no OLR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-307">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="1dfd6-308">Adicionar compatibilidade com restauração como arquivo aos bancos de dados SQL e SAP</span><span class="sxs-lookup"><span data-stu-id="1dfd6-308">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="1dfd6-309">Computação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-309">Compute</span></span>

* <span data-ttu-id="1dfd6-310">vm/vmss/availability-set update: adicionar --ppg para permitir a atualização de ProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="1dfd6-310">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="1dfd6-311">vmss create: adicionar --data-disk-iops e --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="1dfd6-311">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="1dfd6-312">az vm host: remover a marca de versão prévia de `vm host` e `vm host group`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-312">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="1dfd6-313">[ALTERAÇÃO SIGNIFICATIVA] Correção nº 10.728: `az vm create`: criar uma sub-rede automaticamente quando a vnet for especificada e não houver uma sub-rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-313">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="1dfd6-314">Aumentar a robustez da lista de imagens de VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-314">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="1dfd6-315">Eventhub</span><span class="sxs-lookup"><span data-stu-id="1dfd6-315">Eventhub</span></span>

* <span data-ttu-id="1dfd6-316">Compatibilidade com o Azure Stack para o perfil 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="1dfd6-316">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="1dfd6-317">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-317">KeyVault</span></span>

* <span data-ttu-id="1dfd6-318">az keyvault key create: adicionar um novo valor `import` ao parâmetro `--ops`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-318">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="1dfd6-319">az keyvault key list-versions: compatibilidade com o parâmetro `--id` para especificar chaves</span><span class="sxs-lookup"><span data-stu-id="1dfd6-319">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="1dfd6-320">Compatibilidade com conexões de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-320">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-321">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-321">Network</span></span>

* <span data-ttu-id="1dfd6-322">Avançar para azure-mgmt-network 9.0.0</span><span class="sxs-lookup"><span data-stu-id="1dfd6-322">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="1dfd6-323">az network private-link-service update/create: dá suporte a --enable-proxy-protocol</span><span class="sxs-lookup"><span data-stu-id="1dfd6-323">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="1dfd6-324">Adicionar o recurso de Monitor de conexão V2</span><span class="sxs-lookup"><span data-stu-id="1dfd6-324">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="1dfd6-325">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-325">Packaging</span></span>

* <span data-ttu-id="1dfd6-326">[ALTERAÇÃO SIGNIFICATIVA] Fim da compatibilidade com o Python 2.7</span><span class="sxs-lookup"><span data-stu-id="1dfd6-326">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="1dfd6-327">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-327">Profile</span></span>

* <span data-ttu-id="1dfd6-328">Visualização: Adicionar novos atributos `homeTenantId` e `managedByTenants` às contas de assinatura.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-328">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="1dfd6-329">Executar `az login` novamente para as alterações entrarem em vigor</span><span class="sxs-lookup"><span data-stu-id="1dfd6-329">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="1dfd6-330">az login: Mostrar um aviso quando uma assinatura estiver listada de mais de um locatário e definir a primeira como padrão.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-330">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="1dfd6-331">Para selecionar um locatário específico ao acessar essa assinatura, inclua `--tenant` em `az login`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-331">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-332">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-332">Role</span></span>

* <span data-ttu-id="1dfd6-333">az role assignment create: Corrigir o erro em que atribuir uma função a uma entidade de serviço pelo nome de exibição gera um HTTP 400</span><span class="sxs-lookup"><span data-stu-id="1dfd6-333">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-334">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-334">SQL</span></span>

* <span data-ttu-id="1dfd6-335">Atualizar o cmdlet da Instância Gerenciada do SQL `az sql mi update` com dois novos parâmetros: nível e família</span><span class="sxs-lookup"><span data-stu-id="1dfd6-335">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-336">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-336">Storage</span></span>

* <span data-ttu-id="1dfd6-337">[ALTERAÇÃO DA FALHA] `az storage account create`: Alterar o tipo de conta de armazenamento padrão para StorageV2</span><span class="sxs-lookup"><span data-stu-id="1dfd6-337">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="1dfd6-338">4 de fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="1dfd6-338">February 04, 2020</span></span>

<span data-ttu-id="1dfd6-339">Versão 2.0.81</span><span class="sxs-lookup"><span data-stu-id="1dfd6-339">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-340">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-340">ACS</span></span>

* <span data-ttu-id="1dfd6-341">Adicionar suporte para definir portas alocadas de saída e tempos limite ociosos no balanceador de carga standard</span><span class="sxs-lookup"><span data-stu-id="1dfd6-341">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="1dfd6-342">Atualizar para a versão da API 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="1dfd6-342">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-343">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-343">ACR</span></span>

* <span data-ttu-id="1dfd6-344">A [ALTERAÇÃO DA FALHA] `az acr delete` será exibida</span><span class="sxs-lookup"><span data-stu-id="1dfd6-344">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="1dfd6-345">A [ALTERAÇÃO SIGNIFICATIVA] 'az acr task delete’ será exibida</span><span class="sxs-lookup"><span data-stu-id="1dfd6-345">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="1dfd6-346">Adicionar um novo grupo de comandos ‘az acr taskrun show/list/delete’ para o gerenciamento de taskrun</span><span class="sxs-lookup"><span data-stu-id="1dfd6-346">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="1dfd6-347">AKS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-347">AKS</span></span>

* <span data-ttu-id="1dfd6-348">Cada cluster obtém uma entidade de serviço separada para aprimorar o isolamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-348">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="1dfd6-349">AppConfig</span><span class="sxs-lookup"><span data-stu-id="1dfd6-349">AppConfig</span></span>

* <span data-ttu-id="1dfd6-350">Dar suporte à importação/exportação de referências keyvault de/a appservice</span><span class="sxs-lookup"><span data-stu-id="1dfd6-350">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="1dfd6-351">Dar suporte à importação/exportação de todos os rótulos de appconfig para appconfig</span><span class="sxs-lookup"><span data-stu-id="1dfd6-351">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="1dfd6-352">Validar nomes de chave e recursos antes de configurar e importar</span><span class="sxs-lookup"><span data-stu-id="1dfd6-352">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="1dfd6-353">Exponha a modificação do sku para o repositório de configurações.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-353">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="1dfd6-354">Adicione o grupo de comandos à identidade gerenciada.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-354">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-355">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-355">AppService</span></span>

* <span data-ttu-id="1dfd6-356">Azure Stack: comandos de superfície no perfil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="1dfd6-356">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="1dfd6-357">functionapp: adicionar a capacidade de criar aplicativos de funções Java no Linux</span><span class="sxs-lookup"><span data-stu-id="1dfd6-357">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="1dfd6-358">ARM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-358">ARM</span></span>

* <span data-ttu-id="1dfd6-359">Correção de problema nº 10246: `az resource tag` falha quando o parâmetro `--ids` passado é a ID do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-359">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="1dfd6-360">Correção de problema nº 11658: o comando `az group export` não é compatível com os parâmetros `--query` e `--output`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-360">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="1dfd6-361">Correção de problema nº 10279: O código de saída `az group deployment validate` é 0 quando a verificação falha</span><span class="sxs-lookup"><span data-stu-id="1dfd6-361">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="1dfd6-362">Correção de problema nº 9916: aprimorar a mensagem de erro do conflito entre a marca e outras condições de filtro para o comando `az resource list`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-362">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="1dfd6-363">Adicionar novo parâmetro `--managed-by` para dar suporte à adição de informações managedBy para o comando `az group create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-363">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="1dfd6-364">Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="1dfd6-364">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="1dfd6-365">Adicionar o subgrupo `monitor` para gerenciar o monitoramento do Log Analytics no cluster do Red Hat OpensShift no Azure</span><span class="sxs-lookup"><span data-stu-id="1dfd6-365">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="1dfd6-366">BotService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-366">BotService</span></span>

* <span data-ttu-id="1dfd6-367">Correção de problema nº 11697: `az bot create` não é idempotente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-367">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="1dfd6-368">Alterar testes de correção de nomes para serem executados somente em modo Ao vivo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-368">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="1dfd6-369">CDN</span><span class="sxs-lookup"><span data-stu-id="1dfd6-369">CDN</span></span>

* <span data-ttu-id="1dfd6-370">Adicionar suporte ao recurso rulesEngine</span><span class="sxs-lookup"><span data-stu-id="1dfd6-370">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="1dfd6-371">Adicionar o novo grupo de comandos ‘cdn endpoint rule’ para gerenciar regras</span><span class="sxs-lookup"><span data-stu-id="1dfd6-371">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="1dfd6-372">Atualizar a versão azure-mgmt-cdn para a 4.0.0 para usar a versão da API 2019-04-15</span><span class="sxs-lookup"><span data-stu-id="1dfd6-372">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="1dfd6-373">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-373">Deployment Manager</span></span>

* <span data-ttu-id="1dfd6-374">Adicione a operação de lista para todos os recursos.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-374">Add list operation for all resources.</span></span>
* <span data-ttu-id="1dfd6-375">Aprimore o recurso de etapa do novo tipo de etapa.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-375">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="1dfd6-376">Atualize o pacote azure-mgmt-deploymentmanager para usar a versão 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-376">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="1dfd6-377">IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-377">IoT</span></span>

* <span data-ttu-id="1dfd6-378">Substitua os comandos ‘IoT hub Job’.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-378">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="1dfd6-379">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-379">IoT Central</span></span>

* <span data-ttu-id="1dfd6-380">Dê suporte à atualização/criação de aplicativos com o novo nome do SKU ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-380">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="1dfd6-381">Key Vault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-381">Key Vault</span></span>

* <span data-ttu-id="1dfd6-382">Adicione um novo comando `az keyvault key download` para baixar chaves.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-382">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="1dfd6-383">Diversos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-383">Misc</span></span>

* <span data-ttu-id="1dfd6-384">Correção nº 6371: dar suporte à conclusão da variável de nome de arquivo e de ambiente em Bash</span><span class="sxs-lookup"><span data-stu-id="1dfd6-384">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-385">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-385">Network</span></span>

* <span data-ttu-id="1dfd6-386">Correção nº 2092: az network dns record-set add/remove: adicione um aviso quando record-set não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-386">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="1dfd6-387">No futuro, haverá suporte para um argumento extra para confirmar essa criação automática.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-387">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="1dfd6-388">Política</span><span class="sxs-lookup"><span data-stu-id="1dfd6-388">Policy</span></span>

* <span data-ttu-id="1dfd6-389">Adicionar o novo comando `az policy metadata` para recuperar recursos avançados de metadados de política</span><span class="sxs-lookup"><span data-stu-id="1dfd6-389">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="1dfd6-390">`az policy remediation create`: Especifique se a conformidade deve ser reavaliada antes da correção com o parâmetro `--resource-discovery-mode`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-390">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="1dfd6-391">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-391">Profile</span></span>

* <span data-ttu-id="1dfd6-392">`az account get-access-token`: Adicionar parâmetro `--tenant` para adquirir o token do locatário diretamente, sem a necessidade de especificar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="1dfd6-392">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="1dfd6-393">RBAC</span><span class="sxs-lookup"><span data-stu-id="1dfd6-393">RBAC</span></span>

* <span data-ttu-id="1dfd6-394">[ALTERAÇÃO SIGNIFICATIVA] Correção nº 11883: `az role assignment create`: o escopo vazio exibirá erro</span><span class="sxs-lookup"><span data-stu-id="1dfd6-394">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="1dfd6-395">Segurança</span><span class="sxs-lookup"><span data-stu-id="1dfd6-395">Security</span></span>

* <span data-ttu-id="1dfd6-396">Adicione novos comandos `az atp show` e `az atp update` para exibir e gerenciar configurações avançadas de proteção contra ameaças para contas de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-396">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-397">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-397">SQL</span></span>

* <span data-ttu-id="1dfd6-398">`sql dw create`: substitua os parâmetros `--zone-redundant` e `--read-replica-count`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-398">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="1dfd6-399">Esses parâmetros não se aplicam ao DataWarehouse.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-399">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="1dfd6-400">[ALTERAÇÃO DA FALHA] `az sql db create`: Remova "WideWorldImportersStd" e "WideWorldImportersFull" como valores permitidos documentados para "az sql db create --sample-name".</span><span class="sxs-lookup"><span data-stu-id="1dfd6-400">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="1dfd6-401">Esses bancos de dados de exemplo sempre farão a criação falhar.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-401">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="1dfd6-402">Adicione os novos comandos `sql db classification show/list/update/delete` e `sql db classification recommendation list/enable/disable` para gerenciar classificações de confidencialidade para bancos de dados SQL.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-402">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="1dfd6-403">`az sql db audit-policy`: Correção para ações e grupos de auditoria vazios</span><span class="sxs-lookup"><span data-stu-id="1dfd6-403">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-404">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-404">Storage</span></span>

* <span data-ttu-id="1dfd6-405">Adicione um novo grupo de comandos `az storage share-rm` para usar o provedor de recursos Microsoft.Storage para operações de gerenciamento de compartilhamento de arquivo do Azure.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-405">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="1dfd6-406">Correção de problema nº 11415: erro de permissão para `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-406">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="1dfd6-407">Integre Azcopy 10.3.3 e dê suporte a Win32.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-407">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="1dfd6-408">`az storage copy`: Adicione os parâmetros `--include-path`, `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-408">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="1dfd6-409">`az storage remove`: Altere os parâmetros `--inlcude` e `--exclude` para os parâmetros `--include-path`, `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-409">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="1dfd6-410">`az storage sync`: Adicione os parâmetros `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-410">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="1dfd6-411">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1dfd6-411">ServiceFabric</span></span>

* <span data-ttu-id="1dfd6-412">Adicione novos comandos para gerenciar o aplicativo e os serviços.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-412">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="1dfd6-413">13 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="1dfd6-413">January 13, 2020</span></span>

<span data-ttu-id="1dfd6-414">Versão 2.0.80</span><span class="sxs-lookup"><span data-stu-id="1dfd6-414">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="1dfd6-415">Computação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-415">Compute</span></span>

* <span data-ttu-id="1dfd6-416">atualização do disco: Adicionar --disk-encryption-set e --encryption-type</span><span class="sxs-lookup"><span data-stu-id="1dfd6-416">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="1dfd6-417">criação/atualização do instantâneo: Adicionar --disk-encryption-set e --encryption-type</span><span class="sxs-lookup"><span data-stu-id="1dfd6-417">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-418">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-418">Storage</span></span>

* <span data-ttu-id="1dfd6-419">Atualizar a versão do azure-mgmt-storage para 7.1.0</span><span class="sxs-lookup"><span data-stu-id="1dfd6-419">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="1dfd6-420">`az storage account create`: Adicionar `--encryption-key-type-for-table` e `--encryption-key-type-for-queue` para dar suporte ao Serviço de Criptografia de Tabela e de Fila</span><span class="sxs-lookup"><span data-stu-id="1dfd6-420">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="1dfd6-421">07 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="1dfd6-421">January 07, 2020</span></span>

<span data-ttu-id="1dfd6-422">Versão 2.0.79</span><span class="sxs-lookup"><span data-stu-id="1dfd6-422">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-423">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-423">ACR</span></span>

* <span data-ttu-id="1dfd6-424">[ALTERAÇÃO SIGNIFICATIVA] Remover o parâmetro '--os' para 'acr build', 'acr task create/update', 'acr run' e 'acr pack'.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-424">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="1dfd6-425">Em vez disso, use '--platform'.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-425">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="1dfd6-426">AppConfig</span><span class="sxs-lookup"><span data-stu-id="1dfd6-426">AppConfig</span></span>

* <span data-ttu-id="1dfd6-427">Adicionar suporte para importar/exportar sinalizadores de recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-427">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="1dfd6-428">Adicione o novo comando 'az appconfig kv set-keyvault' para criar a referência do keyvault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-428">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="1dfd6-429">Suporte a várias convenções de nomenclatura ao exportar os sinalizadores de recurso para o arquivo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-429">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-430">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-430">AppService</span></span>

* <span data-ttu-id="1dfd6-431">Corrigir o problema #7154: Atualizar a documentação para o comando <> para usar acentos grave em vez de aspas simples</span><span class="sxs-lookup"><span data-stu-id="1dfd6-431">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="1dfd6-432">Corrigir o problema #11287: webapp up: Por padrão, faça o aplicativo criado usando 'should be 'SSL enabled'</span><span class="sxs-lookup"><span data-stu-id="1dfd6-432">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="1dfd6-433">Corrigir o problema #11592: Adicionar o sinalizador az webapp up para sites HTML estáticos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-433">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="1dfd6-434">ARM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-434">ARM</span></span>

* <span data-ttu-id="1dfd6-435">Corrigir `az resource tag`: As marcas do Cofre dos Serviços de Recuperação não podem ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-435">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="1dfd6-436">Backup</span><span class="sxs-lookup"><span data-stu-id="1dfd6-436">Backup</span></span>

* <span data-ttu-id="1dfd6-437">Novo comando 'backup protection undelete' adicionado para habilitar o recurso de exclusão reversível para carga de trabalho IaasVM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-437">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="1dfd6-438">Novo parâmetro '--soft-delete-feature-state' adicionado para definir o comando propriedades do backup</span><span class="sxs-lookup"><span data-stu-id="1dfd6-438">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="1dfd6-439">Suporte de exclusão de disco adicionado para carga de trabalho IaasVM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-439">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="1dfd6-440">Computação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-440">Compute</span></span>

* <span data-ttu-id="1dfd6-441">Corrigir a falha `vm create` no perfil do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-441">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="1dfd6-442">parte final/listar definições de métricas de monitor de vm: suporte a métricas de consulta e definições de lista para uma vm.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-442">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="1dfd6-443">Adicionar nova ação de comando de reaplicação para az vm</span><span class="sxs-lookup"><span data-stu-id="1dfd6-443">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1dfd6-444">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1dfd6-444">HDInsight</span></span>

* <span data-ttu-id="1dfd6-445">Suporte para criar um cluster Kafka com o Proxy REST do Kafka</span><span class="sxs-lookup"><span data-stu-id="1dfd6-445">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="1dfd6-446">Atualizar azure-mgmt-hdinsight para 1.3.0</span><span class="sxs-lookup"><span data-stu-id="1dfd6-446">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="1dfd6-447">Diversos.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-447">Misc.</span></span>

* <span data-ttu-id="1dfd6-448">Adicionar comando de visualização `az version show` para mostrar as versões dos módulos e das extensões da CLI do Azure no formato JSON por padrão ou no formato configurado por --output</span><span class="sxs-lookup"><span data-stu-id="1dfd6-448">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="1dfd6-449">Hubs de Eventos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-449">Event Hubs</span></span>

* <span data-ttu-id="1dfd6-450">[ALTERAÇÃO SIGNIFICATIVA] Remover a opção de status 'ReceiveDisabled' do comando 'az eventhubs eventhub update' e 'az eventhubs eventhub create'.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-450">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="1dfd6-451">Essa opção não é válida para entidades do Hub de Eventos.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-451">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="1dfd6-452">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="1dfd6-452">Service Bus</span></span>

* <span data-ttu-id="1dfd6-453">[ALTERAÇÃO SIGNIFICATIVA] Remover a opção de status 'ReceiveDisabled' do comando 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create' e 'az servicebus queue update'.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-453">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="1dfd6-454">Essa opção não é válida para tópicos e filas do Barramento de Serviço.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-454">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="1dfd6-455">RBAC</span><span class="sxs-lookup"><span data-stu-id="1dfd6-455">RBAC</span></span>

* <span data-ttu-id="1dfd6-456">Correção #11712: `az ad app/sp show` não devolve o código de saída 3 quando o aplicativo ou a entidade de serviço não existir</span><span class="sxs-lookup"><span data-stu-id="1dfd6-456">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-457">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-457">Storage</span></span>

* <span data-ttu-id="1dfd6-458">`az storage account create`: Remover o sinalizador de visualização do parâmetro --enable-hierarchical-namespace</span><span class="sxs-lookup"><span data-stu-id="1dfd6-458">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="1dfd6-459">Atualizar a versão azure-mgmt-storage para 7.0.0 para usar a versão de API 2019-06-01</span><span class="sxs-lookup"><span data-stu-id="1dfd6-459">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="1dfd6-460">Adicionar novos parâmetros `--enable-delete-retention` e `--delete-retention-days` para dar suporte ao gerenciamento da política de retenção de exclusão para a conta de armazenamento blob-service-properties.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-460">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="1dfd6-461">17 de dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-461">December 17, 2019</span></span>

<span data-ttu-id="1dfd6-462">2.0.78</span><span class="sxs-lookup"><span data-stu-id="1dfd6-462">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-463">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-463">ACR</span></span>

* <span data-ttu-id="1dfd6-464">Contexto local de suporte adicionado na execução da tarefa acr</span><span class="sxs-lookup"><span data-stu-id="1dfd6-464">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-465">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-465">ACS</span></span>

* <span data-ttu-id="1dfd6-466">[ALTERAÇÃO SIGNIFICATIVA]criar az openshift: renomear `--workspace-resource-id` para `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-466">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="1dfd6-467">AMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-467">AMS</span></span>

* <span data-ttu-id="1dfd6-468">Comandos de exibição atualizados para devolver 3 quando o recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-468">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="1dfd6-469">AppConfig</span><span class="sxs-lookup"><span data-stu-id="1dfd6-469">AppConfig</span></span>

* <span data-ttu-id="1dfd6-470">Bug corrigido ao acrescentar a versão de API à URL de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-470">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="1dfd6-471">A solução existente não funciona com a paginação.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-471">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="1dfd6-472">Suporte adicionado para a exibição de idiomas além do inglês, pois nosso serviço de back-end é compatível com unicode para globalização.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-472">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-473">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-473">AppService</span></span>

* <span data-ttu-id="1dfd6-474">Problema corrigido nº 11217: webapp: o upload ssl de configuração do az webapp deve ser compatível com o parâmetro do slot</span><span class="sxs-lookup"><span data-stu-id="1dfd6-474">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="1dfd6-475">Problema corrigido nº 10965: Erro: O nome não pode estar vazio.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-475">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="1dfd6-476">Permitir remoção por ip_address e sub-rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-476">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="1dfd6-477">Suporte adicionado para importar certificados do Key Vault `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-477">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="1dfd6-478">ARM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-478">ARM</span></span>

* <span data-ttu-id="1dfd6-479">Pacote azure-mgmt-resource atualizado para usar 6.0.0</span><span class="sxs-lookup"><span data-stu-id="1dfd6-479">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="1dfd6-480">Suporte entre locatários para o comando `az group deployment create` adicionando o novo parâmetro `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-480">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="1dfd6-481">Novo parâmetro `--metadata` adicionado para dar suporte à adição de informações de metadados para definições de conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-481">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="1dfd6-482">Backup</span><span class="sxs-lookup"><span data-stu-id="1dfd6-482">Backup</span></span>

* <span data-ttu-id="1dfd6-483">Suporte de backup adicionado para carga de trabalho SQL e SAP Hana.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-483">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="1dfd6-484">BotService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-484">BotService</span></span>

* <span data-ttu-id="1dfd6-485">[ALTERAÇÃO SIGNIFICATIVA] Remover o sinalizador '--version ' do comando de visualização 'az bot create'.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-485">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="1dfd6-486">Somente os bots do SDK v4 são compatíveis.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-486">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="1dfd6-487">Verificação de disponibilidade de nome adicionada para 'az bot create'.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-487">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="1dfd6-488">Suporte adicionado para atualizar a URL do ícone para um bot por meio de 'az bot update'.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-488">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="1dfd6-489">Suporte adicionado para atualizar um canal Direct Line por meio de 'az bot directline update'.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-489">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="1dfd6-490">Suporte ao sinalizador '--enable-enhanced-auth' adicionado para 'az bot directline create'.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-490">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="1dfd6-491">Os seguintes grupos de comandos estão em GA e não estão em versão prévia: 'az bot authsetting'.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-491">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="1dfd6-492">Os seguintes comandos em 'az bot' estão em GA e não na versão prévia: 'criar', 'preparar-implantar', 'mostrar', 'excluir', 'atualizar'.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-492">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="1dfd6-493">Correção do valor 'az bot prepare-deploy' alterando '--proj-file-path ' para letras minúsculas (por exemplo, "Test. csproj" para "Test. csproj").</span><span class="sxs-lookup"><span data-stu-id="1dfd6-493">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="1dfd6-494">Computação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-494">Compute</span></span>

* <span data-ttu-id="1dfd6-495">Criar/atualizar vmss: --scale-in-policy adicionado, que decide quais máquinas virtuais são escolhidas para remoção quando um VMSS é dimensionado.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-495">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="1dfd6-496">atualização de vm/vmss: --priority adicionado.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-496">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="1dfd6-497">atualização de vm/vmss: --max-price adicionado.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-497">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="1dfd6-498">Grupo de comandos do conjunto de criptografia de disco adicionado (criar, mostrar, atualizar, excluir e listar).</span><span class="sxs-lookup"><span data-stu-id="1dfd6-498">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="1dfd6-499">criação de disco: --encryption-type e --disk-encryption-set adicionados.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-499">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="1dfd6-500">vm/vmss create: --os-disk-encryption-set e --data-disk-encryption-sets adicionados.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-500">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-501">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-501">Core</span></span>

* <span data-ttu-id="1dfd6-502">Suporte para Python 3.4 removido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-502">Removed support for Python 3.4</span></span>
* <span data-ttu-id="1dfd6-503">Pesquisa de funções de plug-in em vários comandos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-503">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="1dfd6-504">DLS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-504">DLS</span></span>

* <span data-ttu-id="1dfd6-505">Versão atualizada do SDK do ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="1dfd6-505">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="1dfd6-506">Instalar</span><span class="sxs-lookup"><span data-stu-id="1dfd6-506">Install</span></span>

* <span data-ttu-id="1dfd6-507">Instalar suporte de script Python 3.8</span><span class="sxs-lookup"><span data-stu-id="1dfd6-507">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="1dfd6-508">IOT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-508">IOT</span></span>

* <span data-ttu-id="1dfd6-509">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro--failover-region removido de failover manual.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-509">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="1dfd6-510">Agora ele fará failover para a região secundária emparelhada atribuída geograficamente.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-510">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="1dfd6-511">Key Vault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-511">Key Vault</span></span>

* <span data-ttu-id="1dfd6-512">Nº 8095 corrigido: `az keyvault storage remove`: melhorar a mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="1dfd6-512">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="1dfd6-513">Nº 8921 corrigido: `az keyvault key/secret/certificate list/list-deleted/list-versions`: corrigir o bug de validação no parâmetro `--maxresults`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-513">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="1dfd6-514">Nº 10512 corrigido: `az keyvault set-policy`: melhorar a mensagem de erro quando nenhuma das `--object-id`, `--spn` ou `--upn` for especificada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-514">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="1dfd6-515">Nº 10846 corrigido: `az keyvault secret show-deleted`: quando `--id` for especificado, `--name/-n` não será necessário</span><span class="sxs-lookup"><span data-stu-id="1dfd6-515">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="1dfd6-516">Nº 11084 corrigido: `az keyvault secret download`: melhorar a mensagem de ajuda do parâmetro `--encoding`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-516">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-517">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-517">Network</span></span>

* <span data-ttu-id="1dfd6-518">Investigação de gateway de aplicativo de rede az: Suporte --port option adicionado para especificar uma porta para sondar servidores de back-end ao criar e atualizar</span><span class="sxs-lookup"><span data-stu-id="1dfd6-518">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="1dfd6-519">az network application-gateway url-path-map create/update: correção de bug para `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-519">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="1dfd6-520">az network application-gateway: Suporte `--rewrite-rule-set` adicionado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-520">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="1dfd6-521">az network list-service-aliases: Foram adicionados aliases de serviço da lista de suporte que podem ser usados para políticas de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="1dfd6-521">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="1dfd6-522">importar zona dns da rede az: Suporte adicionado. @ no nome do registro</span><span class="sxs-lookup"><span data-stu-id="1dfd6-522">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="1dfd6-523">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-523">Packaging</span></span>

* <span data-ttu-id="1dfd6-524">Compilações de back edge adicionadas para instalação de pip</span><span class="sxs-lookup"><span data-stu-id="1dfd6-524">Added back edge builds for pip install</span></span>
* <span data-ttu-id="1dfd6-525">Pacote eoan do Ubuntu adicionado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-525">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="1dfd6-526">Política</span><span class="sxs-lookup"><span data-stu-id="1dfd6-526">Policy</span></span>

* <span data-ttu-id="1dfd6-527">Inclusão de compatibilidade com a API de Política, versão de 01/09/2019.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-527">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="1dfd6-528">az policy set-definition: Agrupamento de suporte adicionado nas definições do conjunto de políticas com `--definition-groups` parâmetro</span><span class="sxs-lookup"><span data-stu-id="1dfd6-528">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="1dfd6-529">Redis</span><span class="sxs-lookup"><span data-stu-id="1dfd6-529">Redis</span></span>

* <span data-ttu-id="1dfd6-530">Adicionado o parâmetro de visualização `--replicas-per-master` ao comando `az redis create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-530">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="1dfd6-531">Azure-MGMT-Redis adicionado do 6.0.0 para o 7.0.0rc1</span><span class="sxs-lookup"><span data-stu-id="1dfd6-531">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="1dfd6-532">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1dfd6-532">ServiceFabric</span></span>

* <span data-ttu-id="1dfd6-533">Corrigido em nó-tipo adicionar lógica, incluindo #10963: A adição do novo tipo de nó com nível de durabilidade Gold sempre gerará erro da CLI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-533">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="1dfd6-534">Versão do ServiceFabricNodeVmExt atualizada para 1.1 no modelo de criação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-534">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-535">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-535">SQL</span></span>

* <span data-ttu-id="1dfd6-536">Adicionados os parâmetros "--read-scale" e "--read-replicas" aos comandos criar e atualizar do BD SQL para dar suporte ao gerenciamento de escala de leitura.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-536">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-537">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-537">Storage</span></span>

* <span data-ttu-id="1dfd6-538">Propriedade de compartilhamentos de arquivos grandes da versão GA para o comando criar e atualizar da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-538">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="1dfd6-539">Suporte ao token SAS de delegação de usuário da versão GA</span><span class="sxs-lookup"><span data-stu-id="1dfd6-539">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="1dfd6-540">Novos comandos adicionados `az storage account blob-service-properties show` e `az storage account blob-service-properties update --enable-change-feed` para gerenciar Propriedades do serviço blob para a conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-540">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="1dfd6-541">[PRÓXIMA ALTERAÇÃO DA FALHA] `az storage copy`: `*` não há mais suporte para o caractere de como um curinga na URL, mas novos parâmetros--include-pattern e --exclude-pattern serão adicionados com suporte a curinga `*`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-541">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="1dfd6-542">Problema corrigido nº 11043: Suporte adicionado para remover contêiner/compartilhamento inteiro no comando `az storage remove`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-542">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="1dfd6-543">26 de novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-543">November 26, 2019</span></span>

<span data-ttu-id="1dfd6-544">Versão 2.0.77</span><span class="sxs-lookup"><span data-stu-id="1dfd6-544">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-545">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-545">ACR</span></span>

* <span data-ttu-id="1dfd6-546">Parâmetro `--branch` preterido da criação/atualização da tarefa ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-546">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="1dfd6-547">Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="1dfd6-547">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="1dfd6-548">Sinalizador `--workspace-resource-id` adicionado para permitir a criação do cluster do Red Hat OpenShift no Azure com monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-548">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="1dfd6-549">`monitor_profile` adicionado para criar o cluster do Red Hat OpenShift no Azure com monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-549">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="1dfd6-550">AKS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-550">AKS</span></span>

* <span data-ttu-id="1dfd6-551">Operação de rotação de certificado de cluster de suporte adicionada usando "az aks rotate-certs".</span><span class="sxs-lookup"><span data-stu-id="1dfd6-551">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="1dfd6-552">AppConfig</span><span class="sxs-lookup"><span data-stu-id="1dfd6-552">AppConfig</span></span>

* <span data-ttu-id="1dfd6-553">Suporte adicionado para usar ":" para o separador `as az appconfig kv import`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-553">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="1dfd6-554">Problema corrigido para listar valores de chave com vários rótulos incluindo o rótulo nulo.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-554">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="1dfd6-555">SDK do plano de gerenciamento atualizado, azure-mgmt-appconfiguration, para a versão 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-555">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="1dfd6-556">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-556">AppService</span></span>

* <span data-ttu-id="1dfd6-557">Problema corrigido nº 11100: AttributeError para az webapp up ao criar o plano de serviço</span><span class="sxs-lookup"><span data-stu-id="1dfd6-557">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="1dfd6-558">az webapp up: Forçar a criação ou a implantação em um site para linguagens com suporte, nenhum padrão usado.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-558">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="1dfd6-559">Suporte adicionado para o Ambiente do Serviço de Aplicativo: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="1dfd6-559">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="1dfd6-560">Backup</span><span class="sxs-lookup"><span data-stu-id="1dfd6-560">Backup</span></span>

* <span data-ttu-id="1dfd6-561">Problema corrigido em list-associated-items da política de backup az.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-561">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="1dfd6-562">Parâmetro BackupManagementType opcional adicionado.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-562">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="1dfd6-563">Computação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-563">Compute</span></span>

* <span data-ttu-id="1dfd6-564">Versão de API de computação, discos e instantâneos atualizados para 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="1dfd6-564">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="1dfd6-565">vmss create: melhoria para --orchestration-mode</span><span class="sxs-lookup"><span data-stu-id="1dfd6-565">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="1dfd6-566">sig image-definition create: --os-state adicionado para permitir a especificação se as máquinas virtuais criadas nessa imagem são 'Generalizadas' ou 'Especializadas'</span><span class="sxs-lookup"><span data-stu-id="1dfd6-566">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="1dfd6-567">sig image-definition create: --hyper-v-generation adicionado para permitir a especificação da geração do hipervisor</span><span class="sxs-lookup"><span data-stu-id="1dfd6-567">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="1dfd6-568">sig image-version create: --os-snapshot e --data-snapshots de suporte adicionados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-568">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="1dfd6-569">image create: --data-disk-caching adicionado para permitir a especificação da configuração de cache de discos de dados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-569">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="1dfd6-570">SDK de computação do Python atualizado para 10.0.0</span><span class="sxs-lookup"><span data-stu-id="1dfd6-570">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="1dfd6-571">vm/vmss create: 'Spot' adicionado à propriedade de enumeração 'Priority'</span><span class="sxs-lookup"><span data-stu-id="1dfd6-571">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="1dfd6-572">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro '--max-billing' renomeado para '--max-price', para a VM e o VMSS, a fim de que seja consistente com os cmdlets do Swagger e do PowerShell</span><span class="sxs-lookup"><span data-stu-id="1dfd6-572">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="1dfd6-573">vm monitor log show: suporte adicionado para consultar o log pelo workspace do Log Analytics vinculado.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-573">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="1dfd6-574">IOT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-574">IOT</span></span>

* <span data-ttu-id="1dfd6-575">Correção nº 2531: argumentos de conveniência adicionados para a atualização do hub.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-575">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="1dfd6-576">Correção nº 8323: parâmetros ausentes adicionados para criar o ponto de extremidade personalizado de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-576">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="1dfd6-577">Corrigir bug de regressão: as alterações que substituem o ponto de extremidade de armazenamento padrão foram revertidas.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-577">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="1dfd6-578">Key Vault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-578">Key Vault</span></span>

* <span data-ttu-id="1dfd6-579">Correção nº 11121: ao usar `az keyvault certificate list`, passar `--include-pending` agora não exige um valor de `true` ou `false`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-579">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="1dfd6-580">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="1dfd6-580">NetAppFiles</span></span>

* <span data-ttu-id="1dfd6-581">azure-mgmt-netapp atualizado para 0.7.0 que inclui algumas propriedades de volume adicionais associadas a operações de replicação futuras</span><span class="sxs-lookup"><span data-stu-id="1dfd6-581">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-582">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-582">Network</span></span>

* <span data-ttu-id="1dfd6-583">application-gateway waf-config: preterido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-583">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="1dfd6-584">application-gateway waf-policy: subgrupo managed-rules adicionado para gerenciar os conjuntos de regras e regras de exclusão gerenciados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-584">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="1dfd6-585">application-gateway waf-policy: subgrupo policy-setting adicionado para gerenciar a configuração global de um waf-policy</span><span class="sxs-lookup"><span data-stu-id="1dfd6-585">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="1dfd6-586">[ALTERAÇÃO SIGNIFICATIVA] application-gateway waf-policy: subgrupo rule renomeado para custom-rule</span><span class="sxs-lookup"><span data-stu-id="1dfd6-586">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="1dfd6-587">application-gateway http-listener: --firewall-policy adicionado durante a criação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-587">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="1dfd6-588">application-gateway url-path-map rule: --firewall-policy adicionado durante a criação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-588">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="1dfd6-589">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-589">Packaging</span></span>

* <span data-ttu-id="1dfd6-590">Wrapper az reescrito no Python</span><span class="sxs-lookup"><span data-stu-id="1dfd6-590">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="1dfd6-591">Suporte adicionado para Python 3.8</span><span class="sxs-lookup"><span data-stu-id="1dfd6-591">Added support for Python 3.8</span></span>
* <span data-ttu-id="1dfd6-592">Alterado para Python 3 para o pacote RPM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-592">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="1dfd6-593">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-593">Profile</span></span>

* <span data-ttu-id="1dfd6-594">Erro aperfeiçoado ao executar `az login -u {} -p {}` com a conta Microsoft</span><span class="sxs-lookup"><span data-stu-id="1dfd6-594">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="1dfd6-595">`SSLError` aperfeiçoado ao executar `az login` atrás de um proxy com o certificado raiz autoassinado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-595">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="1dfd6-596">Correção nº 10578: `az login` trava quando mais de uma instância é iniciada ao mesmo tempo no Windows ou WSL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-596">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="1dfd6-597">Correção nº 11059: `az login --allow-no-subscriptions` falhará se houver assinaturas no locatário</span><span class="sxs-lookup"><span data-stu-id="1dfd6-597">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="1dfd6-598">Correção nº 11238: após renomear uma assinatura, fazer logon com a MSI fará a mesma assinatura aparecer duas vezes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-598">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="1dfd6-599">RBAC</span><span class="sxs-lookup"><span data-stu-id="1dfd6-599">RBAC</span></span>

* <span data-ttu-id="1dfd6-600">Correção nº 10996: erro aperfeiçoado para `--force-change-password-next-login` em `az ad user update` quando `--password` não for especificado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-600">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="1dfd6-601">Redis</span><span class="sxs-lookup"><span data-stu-id="1dfd6-601">Redis</span></span>

* <span data-ttu-id="1dfd6-602">Correção nº 2902: evite definir configurações de memória ao atualizar o cache do SKU básico</span><span class="sxs-lookup"><span data-stu-id="1dfd6-602">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="1dfd6-603">Reservas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-603">Reservations</span></span>

* <span data-ttu-id="1dfd6-604">Versão do SDK atualizada para 0.6.0</span><span class="sxs-lookup"><span data-stu-id="1dfd6-604">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="1dfd6-605">Informações de detalhes do plano de cobrança atualizadas após chamar Get-Gatalogs</span><span class="sxs-lookup"><span data-stu-id="1dfd6-605">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="1dfd6-606">Novo comando `az reservations reservation-order calculate` adicionado para calcular o preço de uma reserva</span><span class="sxs-lookup"><span data-stu-id="1dfd6-606">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="1dfd6-607">Novo comando `az reservations reservation-order purchase` adicionado para comprar uma nova reserva</span><span class="sxs-lookup"><span data-stu-id="1dfd6-607">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="1dfd6-608">Rest</span><span class="sxs-lookup"><span data-stu-id="1dfd6-608">Rest</span></span>
* <span data-ttu-id="1dfd6-609">`az rest` alterado para GA</span><span class="sxs-lookup"><span data-stu-id="1dfd6-609">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-610">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-610">SQL</span></span>

* <span data-ttu-id="1dfd6-611">azure-mgmt-sql atualizado para 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-611">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-612">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-612">Storage</span></span>

* <span data-ttu-id="1dfd6-613">storage account create: --enable-hierarchical-namespace adicionado para dar suporte à semântica do sistema de arquivos no serviço Blob.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-613">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="1dfd6-614">Exceção não relacionada removida da mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="1dfd6-614">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="1dfd6-615">Problemas corrigidos com a mensagem de erro incorreta "Você não tem as permissões necessárias para executar essa operação."</span><span class="sxs-lookup"><span data-stu-id="1dfd6-615">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="1dfd6-616">quando bloqueado pelas regras de rede ou AuthenticationFailed.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-616">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="1dfd6-617">4 de novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-617">November 4, 2019</span></span>

<span data-ttu-id="1dfd6-618">Versão 2.0.76</span><span class="sxs-lookup"><span data-stu-id="1dfd6-618">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-619">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-619">ACR</span></span>

* <span data-ttu-id="1dfd6-620">O parâmetro de versão prévia `--pack-image-tag` foi adicionado ao comando `az acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-620">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="1dfd6-621">Suporte adicionado para habilitar a auditoria na criação de um registro</span><span class="sxs-lookup"><span data-stu-id="1dfd6-621">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="1dfd6-622">Suporte adicionado para o RBAC com escopo de repositório</span><span class="sxs-lookup"><span data-stu-id="1dfd6-622">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="1dfd6-623">AKS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-623">AKS</span></span>

* <span data-ttu-id="1dfd6-624">`--enable-cluster-autoscaler`, `--min-count` e `--max-count` foram adicionados ao comando `az aks create`, que habilita o dimensionamento automático do cluster para o pool de nós.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-624">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="1dfd6-625">Foram adicionados os sinalizadores acima, bem como `--update-cluster-autoscaler` e `--disable-cluster-autoscaler` ao comando `az aks update`, permitindo atualizações do cluster de dimensionamento automático.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-625">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="1dfd6-626">AppConfig</span><span class="sxs-lookup"><span data-stu-id="1dfd6-626">AppConfig</span></span>

* <span data-ttu-id="1dfd6-627">O grupo de comandos do recurso AppConfig foi adicionado para gerenciar os sinalizadores de recurso armazenados em uma Configuração de Aplicativos.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-627">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="1dfd6-628">Foi corrigido um bug secundário do comando de exportação para arquivo appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-628">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="1dfd6-629">Foi interrompida a leitura de conteúdo do arquivo de destino durante a exportação.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-629">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-630">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-630">AppService</span></span>

* <span data-ttu-id="1dfd6-631">`az appservice plan create`: Foi adicionado o suporte para definir 'persitecalling' no comando appservice plan create.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-631">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="1dfd6-632">Foi corrigido um problema em que a operação webapp config ssl bind estava removendo as marcas existentes do recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-632">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="1dfd6-633">Foi adicionado o sinalizador `--build-remote` para `az functionapp deployment source config-zip` para dar suporte à ação de build remoto durante a implantação do aplicativo de funções.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-633">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="1dfd6-634">Foi alterada a versão do nó padrão em aplicativos de funções para ~10 para Windows</span><span class="sxs-lookup"><span data-stu-id="1dfd6-634">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="1dfd6-635">A propriedade `--runtime-version` foi adicionada a `az functionapp create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-635">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="1dfd6-636">ARM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-636">ARM</span></span>

* <span data-ttu-id="1dfd6-637">`az deployment/group deployment validate`: Foi adicionado o parâmetro `--handle-extended-json-format` para dar suporte a várias linhas e comentários no modelo JSON durante a implantação.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-637">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="1dfd6-638">O azure-mgmt-resource passou a usar a 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="1dfd6-638">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="1dfd6-639">Backup</span><span class="sxs-lookup"><span data-stu-id="1dfd6-639">Backup</span></span>

* <span data-ttu-id="1dfd6-640">Foi adicionado o suporte de backup aos Arquivos do Azure</span><span class="sxs-lookup"><span data-stu-id="1dfd6-640">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="1dfd6-641">Computação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-641">Compute</span></span>

* <span data-ttu-id="1dfd6-642">`az vm create`: foi adicionado um aviso ao especificar a rede acelerada e um adaptador de rede existente juntos.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-642">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="1dfd6-643">`az vm create`: foi adicionado `--vmss` para especificar um conjunto de dimensionamento de máquinas virtuais existente ao qual a máquina virtual deve ser atribuída.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-643">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="1dfd6-644">`az vm/vmss create`: foi adicionada uma cópia local do arquivo de alias de imagem para que ele possa ser acessado em um ambiente de rede restrita.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-644">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="1dfd6-645">`az vmss create`: foi adicionado `--orchestration-mode` para especificar como as máquinas virtuais são gerenciadas pelo conjunto de dimensionamento.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-645">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="1dfd6-646">`az vm/vmss update`: foi adicionado `--ultra-ssd-enabled` para permitir a atualização da configuração de SSD Ultra.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-646">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="1dfd6-647">[ALTERAÇÃO DA FALHA] `az vm extension set`: foi corrigido o bug em que os usuários não podiam definir uma extensão em uma VM com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-647">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="1dfd6-648">Foram adicionados os novos comandos `az vm image terms accept/cancel/show` para gerenciar os termos de imagem do Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-648">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="1dfd6-649">O VMAccessForLinux foi atualizado para a versão 1.5</span><span class="sxs-lookup"><span data-stu-id="1dfd6-649">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1dfd6-650">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-650">CosmosDB</span></span>

* <span data-ttu-id="1dfd6-651">[ALTERAÇÃO DA FALHA] `az sql container create`: `--partition-key-path` foi alterado para parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="1dfd6-651">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="1dfd6-652">[ALTERAÇÃO DA FALHA] `az gremlin graph create`: `--partition-key-path` foi alterado para parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="1dfd6-652">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="1dfd6-653">`az sql container create`: Adição de `--unique-key-policy` e `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-653">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="1dfd6-654">`az sql container create/update`: o esquema padrão `--idx` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-654">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="1dfd6-655">`gremlin graph create`: Adicionado `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-655">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="1dfd6-656">`gremlin graph create/update`: o esquema padrão `--idx` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-656">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="1dfd6-657">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="1dfd6-657">Fixed typo in help message</span></span>
* <span data-ttu-id="1dfd6-658">banco de dados: Foram adicionadas informações sobre preteridos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-658">database: Added deprecation information</span></span>
* <span data-ttu-id="1dfd6-659">coleção: Foram adicionadas informações sobre preteridos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-659">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="1dfd6-660">IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-660">IoT</span></span>

* <span data-ttu-id="1dfd6-661">Um novo tipo de fonte de roteamento foi adicionado: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="1dfd6-661">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="1dfd6-662">Foi corrigido o erro de recursos ausentes no `az iot hub create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-662">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="1dfd6-663">Key Vault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-663">Key Vault</span></span>

* <span data-ttu-id="1dfd6-664">Foi corrigido um erro inesperado quando o arquivo de certificado não existe</span><span class="sxs-lookup"><span data-stu-id="1dfd6-664">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="1dfd6-665">Foi corrigido o problema em que o `az keyvault recover/purge` não funcionava</span><span class="sxs-lookup"><span data-stu-id="1dfd6-665">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="1dfd6-666">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="1dfd6-666">NetAppFiles</span></span>

* <span data-ttu-id="1dfd6-667">O azure-mgmt-netapp foi atualizado para 0.6.0 para usar a versão da API 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-667">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="1dfd6-668">Essa nova versão da API inclui:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-668">This new API version includes:</span></span>

    - <span data-ttu-id="1dfd6-669">A criação de volume `--protocol-types` agora aceita "NFSv4.1" não "NFSv4"</span><span class="sxs-lookup"><span data-stu-id="1dfd6-669">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="1dfd6-670">A propriedade da política de exportação de volume agora é chamada 'nfsv41' não 'nfsv4'</span><span class="sxs-lookup"><span data-stu-id="1dfd6-670">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="1dfd6-671">O volume `--creation-token` foi renomeado para `--file-path`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-671">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="1dfd6-672">A data de criação do instantâneo agora é chamada apenas de 'criação'</span><span class="sxs-lookup"><span data-stu-id="1dfd6-672">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-673">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-673">Network</span></span>

* <span data-ttu-id="1dfd6-674">`az network private-dns link vnet create/update`: suporte à vinculação de rede virtual entre locatários.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-674">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="1dfd6-675">[ALTERAÇÃO DA FALHA] `az network vnet subnet list`: `--resource-group` e `--vnet-name` foram alterados para serem obrigatórios agora.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-675">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="1dfd6-676">`az network public-ip prefix create`: Suporte adicionado para especificar a versão do endereço IP (IPv4, IPv6) durante a criação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-676">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="1dfd6-677">O azure-mgmt-network foi atualizado para 7.0.0 e a api-version para 2019-09-01</span><span class="sxs-lookup"><span data-stu-id="1dfd6-677">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="1dfd6-678">`az network vrouter`: Suporte adicionado para o novo roteador virtual de serviço e o emparelhamento do roteador virtual</span><span class="sxs-lookup"><span data-stu-id="1dfd6-678">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="1dfd6-679">`az network express-route gateway connection`: Adicionado o suporte para `--internet-security`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-679">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="1dfd6-680">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-680">Profile</span></span>

* <span data-ttu-id="1dfd6-681">Foi corrigido o problema em que o `az account get-access-token --resource-type ms-graph` não funcionava</span><span class="sxs-lookup"><span data-stu-id="1dfd6-681">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="1dfd6-682">O aviso foi removido de `az login`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-682">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="1dfd6-683">RBAC</span><span class="sxs-lookup"><span data-stu-id="1dfd6-683">RBAC</span></span>

* <span data-ttu-id="1dfd6-684">Foi corrigido o problema em que o `az ad app update --id {} --display-name {}` não funcionava</span><span class="sxs-lookup"><span data-stu-id="1dfd6-684">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="1dfd6-685">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1dfd6-685">ServiceFabric</span></span>

* <span data-ttu-id="1dfd6-686">`az sf cluster create`: foi corrigido um problema que ocorria ao modificar o VMSS de computação do template.json do Linux e do Windows, do Service Fabric, de discos Standard para discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-686">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-687">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-687">SQL</span></span>

* <span data-ttu-id="1dfd6-688">Os parâmetros `--compute-model`, `--auto-pause-delay` e `--min-capacity` foram adicionados para dar suporte a operações CRUD para a nova oferta de Banco de Dados SQL: Modelo de computação sem servidor.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-688">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-689">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-689">Storage</span></span>

* <span data-ttu-id="1dfd6-690">`az storage account create/update`: Foram adicionados o parâmetro --enable-files-adds e o grupo Argumentos de Propriedades do Azure Active Directory para dar suporte à Autenticação do Serviço de Domínio do Active Directory do Arquivos do Azure</span><span class="sxs-lookup"><span data-stu-id="1dfd6-690">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="1dfd6-691">O `az storage account keys list/renew` foi expandido para dar suporte à listagem ou à regeneração de chaves Kerberos da conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-691">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="1dfd6-692">15 de outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-692">October 15, 2019</span></span>

<span data-ttu-id="1dfd6-693">Versão 2.0.75</span><span class="sxs-lookup"><span data-stu-id="1dfd6-693">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="1dfd6-694">AKS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-694">AKS</span></span>

* <span data-ttu-id="1dfd6-695">Alteração do valor padrão `--load-balancer-sku` para `standard` se for compatível com a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-695">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="1dfd6-696">Alteração do valor padrão `--vm-set-type` para `virtualmachinescalesets` se for compatível com a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-696">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="1dfd6-697">AMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-697">AMS</span></span>

* <span data-ttu-id="1dfd6-698">[ALTERAÇÃO SIGNIFICATIVA] Alteração do nome de `job start` para `job create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-698">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="1dfd6-699">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--ask` de `content-key-policy create` para usar uma cadeia de 32 caracteres hexadecimais em vez do UTF8</span><span class="sxs-lookup"><span data-stu-id="1dfd6-699">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-700">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-700">AppService</span></span>

* <span data-ttu-id="1dfd6-701">Adição dos comandos `webapp config access-restriction show|set|add|remove`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-701">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="1dfd6-702">Adição de um melhor tratamento de erro a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-702">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="1dfd6-703">Adição de suporte do SKU `Isolated` para `appservice plan update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-703">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="1dfd6-704">ARM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-704">ARM</span></span>

* <span data-ttu-id="1dfd6-705">Adição do parâmetro `--handle-extended-json-format``deployment create` para dar suporte a várias linhas e a comentários no modelo json</span><span class="sxs-lookup"><span data-stu-id="1dfd6-705">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="1dfd6-706">Computação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-706">Compute</span></span>

* <span data-ttu-id="1dfd6-707">Parâmetro `--enable-agent` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-707">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="1dfd6-708">Alteração de `vm create` para usar um SKU de IP público padrão automaticamente ao usar zonas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-708">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="1dfd6-709">Alteração de `vm create` para criar automaticamente um nome de computador válido para uma VM, caso nenhum tenha sido fornecido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-709">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="1dfd6-710">Adição do parâmetro `--computer-name-prefix` a `vmss create` para dar suporte ao prefixo de nome de computador personalizado de máquinas virtuais no VMSS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-710">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="1dfd6-711">Adicione o parâmetro `--workspace` a `vm create` para habilitar o workspace de análise de logs automaticamente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-711">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="1dfd6-712">Versão de API de galerias atualizadas para 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="1dfd6-712">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-713">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-713">Core</span></span>

* <span data-ttu-id="1dfd6-714">Adição da verificação de sintaxe para o parâmetro `--set` no comando de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="1dfd6-714">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="1dfd6-715">IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-715">IoT</span></span>

* <span data-ttu-id="1dfd6-716">Correção de um problema em que o `iot hub show` retornaria incorretamente um erro com "recurso não encontrado"</span><span class="sxs-lookup"><span data-stu-id="1dfd6-716">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="1dfd6-717">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-717">Monitor</span></span>

* <span data-ttu-id="1dfd6-718">Adição de suporte para CRUD a `monitor log-analytics workspace`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-718">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-719">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-719">Network</span></span>

* <span data-ttu-id="1dfd6-720">Adição de suporte para vinculação virtual entre locatários para `network private-dns link vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-720">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="1dfd6-721">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `network vnet subnet list` para exigir os parâmetros `--resource-group` e `--vnet-name`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-721">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-722">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-722">SQL</span></span>

* <span data-ttu-id="1dfd6-723">Adição de comandos a `sql mi ad-admin` que dão suporte à configuração de um administrador do AAD em instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-723">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-724">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-724">Storage</span></span>

* <span data-ttu-id="1dfd6-725">Adição do parâmetro `--preserve-s2s-access-tier``storage copy` para preservar a camada de acesso durante a cópia do serviço para serviço</span><span class="sxs-lookup"><span data-stu-id="1dfd6-725">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="1dfd6-726">Adição do parâmetro `--enable-large-file-share` a `storage account [create|update]` para dar suporte a compartilhamentos de arquivos grandes para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-726">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="1dfd6-727">24 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-727">September 24, 2019</span></span>

<span data-ttu-id="1dfd6-728">Versão 2.0.74</span><span class="sxs-lookup"><span data-stu-id="1dfd6-728">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-729">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-729">ACR</span></span>

* <span data-ttu-id="1dfd6-730">Inclusão de um parâmetro `--type` obrigatório em `acr config retention update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-730">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="1dfd6-731">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro renomeado `--name -n` foi alterado para `--registry -r ` para o grupo de comando `acr config`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-731">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="1dfd6-732">AKS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-732">AKS</span></span>

* <span data-ttu-id="1dfd6-733">Inclusão do parâmetro `--load-balancer-sku` no comando `aks create`, o que permite criar um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-733">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="1dfd6-734">Inclusão dos parâmetros `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` e `--load-balancer-outbound-ip-prefixes` nos comandos `aks [create|update]`, o que permite atualizar o perfil do balanceador de carga de um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-734">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="1dfd6-735">Inclusão do parâmetro `--vm-set-type` no comando `aks create`, o que permite especificar os tipos de VM de um cluster do AKS (vmas ou vmss)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-735">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="1dfd6-736">ARM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-736">ARM</span></span>

* <span data-ttu-id="1dfd6-737">Inclusão do parâmetro `--handle-extended-json-format` no comando `group deployment create` para compatibilidade com várias linhas e comentários no modelo JSON</span><span class="sxs-lookup"><span data-stu-id="1dfd6-737">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="1dfd6-738">Computação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-738">Compute</span></span>

* <span data-ttu-id="1dfd6-739">Inclusão do parâmetro `--terminate-notification-time` nos comandos `vmss [create|update]` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-739">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="1dfd6-740">Inclusão do parâmetro `--enable-terminate-notification` no comando `vmss update` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-740">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="1dfd6-741">Inclusão dos parâmetros `--priority,`, `--eviction-policy,` e `--max-billing` nos comandos `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-741">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="1dfd6-742">Alteração de `disk create` para permitir a especificação do tamanho exato do carregamento de disco</span><span class="sxs-lookup"><span data-stu-id="1dfd6-742">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="1dfd6-743">Inclusão de compatibilidade com instantâneos incrementais para discos gerenciados para `snapshot create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-743">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="1dfd6-744">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-744">Cosmos DB</span></span>

* <span data-ttu-id="1dfd6-745">Inclusão do parâmetro `--type <key-type>` no comando `cosmosdb keys list` para mostrar a chave, as chaves somente leitura ou cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-745">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="1dfd6-746">Adicionado o comando `cosmosdb keys regenerate`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-746">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="1dfd6-747">[PRETERIDO] Comandos `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` e `cosmosdb list-read-only-keys` preteridos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-747">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="1dfd6-748">EventGrid</span><span class="sxs-lookup"><span data-stu-id="1dfd6-748">EventGrid</span></span>

* <span data-ttu-id="1dfd6-749">Correção do texto de ajuda do ponto de extremidade para fazer referência ao parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="1dfd6-749">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="1dfd6-750">Key Vault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-750">Key Vault</span></span>

* <span data-ttu-id="1dfd6-751">Correção do problema em que fazer logon com um locatário (`login -t`) poderia causar uma falha no `keyvault create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-751">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="1dfd6-752">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-752">Monitor</span></span>

* <span data-ttu-id="1dfd6-753">Correção do problema em que o caractere `:` não era permitido no argumento `--condition` para `monitor metrics alert create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-753">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="1dfd6-754">Política</span><span class="sxs-lookup"><span data-stu-id="1dfd6-754">Policy</span></span>

* <span data-ttu-id="1dfd6-755">Inclusão de compatibilidade com a API de Política, versão de 01/06/2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-755">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="1dfd6-756">Inclusão do parâmetro `--enforcement-mode` no comando `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-756">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-757">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-757">Storage</span></span>

* <span data-ttu-id="1dfd6-758">Inclusão do parâmetro `--blob-type` no comando `az storage copy`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-758">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="1dfd6-759">10 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-759">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-760">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-760">ACR</span></span>

* <span data-ttu-id="1dfd6-761">Adição do grupo de comandos `acr config retention` para configurar a política de retenção</span><span class="sxs-lookup"><span data-stu-id="1dfd6-761">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="1dfd6-762">AKS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-762">AKS</span></span>

* <span data-ttu-id="1dfd6-763">Adição de suporte para integração do ACR com os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-763">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="1dfd6-764">Adição do parâmetro `--attach-acr` a `aks [create|update]` para anexar um ACR a um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-764">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="1dfd6-765">Adição do parâmetro `--detach-acr` a `aks update` para desanexar o ACR de um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-765">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="1dfd6-766">ARM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-766">ARM</span></span>

* <span data-ttu-id="1dfd6-767">Atualização para uso da versão de API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="1dfd6-767">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="1dfd6-768">Lote</span><span class="sxs-lookup"><span data-stu-id="1dfd6-768">Batch</span></span>

* <span data-ttu-id="1dfd6-769">Adição de novas definições de configuração JSON de `--json-file` para `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-769">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="1dfd6-770">Adição de `MountConfigurations` para montagens do sistema de arquivos (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-770">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="1dfd6-771">Adição da propriedade opcional `publicIPs` a `NetworkConfiguration` para IPs públicos em pools (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-771">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="1dfd6-772">Adição de suporte para galerias de imagens compartilhadas a `--image`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-772">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="1dfd6-773">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `--start-task-wait-for-success` em `batch pool create` para `true`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-773">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="1dfd6-774">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `Scope` em `AutoUserSpecification` para sempre ser Pool (anteriormente, `Task` em nós do Windows e `Pool` em nós do Linux)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-774">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="1dfd6-775">Esse argumento só pode ser definido em uma configuração JSON com `--json-file`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-775">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1dfd6-776">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1dfd6-776">HDInsight</span></span>

* <span data-ttu-id="1dfd6-777">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="1dfd6-777">GA release</span></span>
* <span data-ttu-id="1dfd6-778">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--workernode-count/-c` de `az hdinsight resize` para ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-778">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="1dfd6-779">Key Vault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-779">Key Vault</span></span>

* <span data-ttu-id="1dfd6-780">Correção do problema em que as sub-redes não podiam ser excluídas das regras da rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-780">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="1dfd6-781">Correção do problema em que sub-redes e endereços IP duplicados podiam ser adicionados às regras da rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-781">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-782">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-782">Network</span></span>

* <span data-ttu-id="1dfd6-783">Adição do parâmetro `--interval` a `network watcher flow-log` para definir o valor do intervalo de análise de tráfego</span><span class="sxs-lookup"><span data-stu-id="1dfd6-783">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="1dfd6-784">Adição de `network application-gateway identity` para gerenciar a identidade do gateway</span><span class="sxs-lookup"><span data-stu-id="1dfd6-784">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="1dfd6-785">Adição de suporte para definir a ID do Key Vault como `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-785">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="1dfd6-786">Adicionado `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-786">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="1dfd6-787">Política</span><span class="sxs-lookup"><span data-stu-id="1dfd6-787">Policy</span></span>

* <span data-ttu-id="1dfd6-788">Atualização para uso da versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="1dfd6-788">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="1dfd6-789">27 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-789">August 27, 2019</span></span>

<span data-ttu-id="1dfd6-790">Versão 2.0.72</span><span class="sxs-lookup"><span data-stu-id="1dfd6-790">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-791">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-791">ACR</span></span>

* <span data-ttu-id="1dfd6-792">[ALTERAÇÃO SIGNIFICATIVA] Remoção da compatibilidade com o SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-792">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="1dfd6-793">Gerenciamento de API</span><span class="sxs-lookup"><span data-stu-id="1dfd6-793">API Management</span></span>

* <span data-ttu-id="1dfd6-794">[VERSÃO PRÉVIA] Adição do grupo de comandos `apim`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-794">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-795">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-795">AppService</span></span>

* <span data-ttu-id="1dfd6-796">Correção do problema com o comando `webapp webjob continuous start` ao especificar um slot</span><span class="sxs-lookup"><span data-stu-id="1dfd6-796">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="1dfd6-797">Alteração de `webapp up` para detectar a pasta `env` e removê-la do arquivo usado para implantação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-797">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="1dfd6-798">Keyvault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-798">Keyvault</span></span>

* <span data-ttu-id="1dfd6-799">Correção de um bug no `keyvault secret set` que ignorava o argumento `--expires`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-799">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-800">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-800">Network</span></span>

* <span data-ttu-id="1dfd6-801">Adição de suporte para endereços IPv6 a argumentos `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-801">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="1dfd6-802">Adição de novos comandos `network private-endpoint [create|update|list-types]` para o gerenciamento de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-802">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="1dfd6-803">Adição do grupo de comandos `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-803">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="1dfd6-804">Adicionados os argumentos `--private-endpoint-network-policies` e `--private-link-service-network-policies` para `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-804">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="1dfd6-805">RBAC</span><span class="sxs-lookup"><span data-stu-id="1dfd6-805">RBAC</span></span>

* <span data-ttu-id="1dfd6-806">Correção de um problema com `ad app update --homepage` em que a página inicial não era atualizada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-806">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="1dfd6-807">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1dfd6-807">ServiceFabric</span></span>

* <span data-ttu-id="1dfd6-808">Adição de suporte para nomes de Key Vault grafados com maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-808">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="1dfd6-809">Correção de um problema ao usar certificados no Key Vault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-809">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="1dfd6-810">Correção de um problema com o uso de arquivos de certificado PFX</span><span class="sxs-lookup"><span data-stu-id="1dfd6-810">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="1dfd6-811">Correção de um problema com `sf cluster certificate add` quando o grupo de recursos do Key Vault não era especificado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-811">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="1dfd6-812">Correção de um problema em que `sf cluster set` não funcionava</span><span class="sxs-lookup"><span data-stu-id="1dfd6-812">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="1dfd6-813">SignalR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-813">SignalR</span></span>

* <span data-ttu-id="1dfd6-814">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-814">Added new commands:</span></span>
  * <span data-ttu-id="1dfd6-815">`signalr cors`: gerenciar CORS do SignalR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-815">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="1dfd6-816">`signalr restart`: reiniciar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-816">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="1dfd6-817">`signalr update`: atualizar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-817">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="1dfd6-818">Adicionado o argumento `--service-mode` para `signalr create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-818">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-819">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-819">Storage</span></span>

* <span data-ttu-id="1dfd6-820">Adicionado o comando `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-820">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="1dfd6-821">13 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-821">August 13, 2019</span></span>

<span data-ttu-id="1dfd6-822">Versão 2.0.71</span><span class="sxs-lookup"><span data-stu-id="1dfd6-822">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-823">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-823">AppService</span></span>

* <span data-ttu-id="1dfd6-824">Um problema de falha de slots com os comandos `webapp webjob continuous` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-824">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="1dfd6-825">BotService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-825">BotService</span></span>

* <span data-ttu-id="1dfd6-826">[ALTERAÇÃO SIGNIFICATIVA] O suporte para a criação de bots SDK v3 foi removido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-826">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="1dfd6-827">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1dfd6-827">CognitiveServices</span></span>

* <span data-ttu-id="1dfd6-828">Adicionados os comandos `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-828">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="1dfd6-829">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-829">Cosmos DB</span></span>

* <span data-ttu-id="1dfd6-830">Removido o aviso ao atualizar vários locais de gravação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-830">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="1dfd6-831">Foram adicionados os comandos CRUD para o CosmosDB SQL, MongoDB, Cassandra, Gremlin e Recursos de tabela e taxa de transferência do recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-831">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1dfd6-832">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1dfd6-832">HDInsight</span></span>

<span data-ttu-id="1dfd6-833">Esta versão contém um grande número de alterações da falha.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-833">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="1dfd6-834">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-834">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="1dfd6-835">`--storage-default-container` renomeado para `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-835">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="1dfd6-836">`--storage-default-filesystem` renomeado para `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-836">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="1dfd6-837">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--name` de `application create` foi alterado para representar o nome do aplicativo em vez do nome do cluster</span><span class="sxs-lookup"><span data-stu-id="1dfd6-837">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="1dfd6-838">O argumento `--cluster-name` foi adicionado a `application create` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="1dfd6-838">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="1dfd6-839">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `application create`:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-839">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="1dfd6-840">`--application-type` renomeado para `--type`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-840">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="1dfd6-841">`--marketplace-identifier` renomeado para `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-841">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="1dfd6-842">`--https-endpoint-access-mode` renomeado para `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-842">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="1dfd6-843">Renomeado de `--https-endpoint-destination-port` para `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-843">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="1dfd6-844">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros removidos para `application create`:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-844">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="1dfd6-845">[ALTERAÇÃO DA FALHA] Renomeado de `--target-instance-count` para `--workernode-count` para `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-845">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="1dfd6-846">[ALTERAÇÃO SIGNIFICATIVA] Todos os comandos no grupo `hdinsight script-action` foram alterados para usar o parâmetro `--name` como o nome da ação de script.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-846">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="1dfd6-847">O argumento `--cluster-name` foi adicionado a todos os comandos `hdinsight script-action` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="1dfd6-847">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="1dfd6-848">[ALTERAÇÃO SIGNIFICATIVA] Renomeado de `--script-execution-id` para `--execution-id` para todos os comandos `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-848">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="1dfd6-849">[ALTERAÇÃO SIGNIFICATIVA]`hdinsight script-action show` renomeado para `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-849">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="1dfd6-850">[ALTERAÇÃO DA FALHA] Os parâmetros foram alterados para `hdinsight script-action execute --roles` para serem separados por espaços em vez de separados por vírgula</span><span class="sxs-lookup"><span data-stu-id="1dfd6-850">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="1dfd6-851">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro `--persisted` de `hdinsight script-action list` foi removido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-851">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="1dfd6-852">O parâmetro `hdinsight create --cluster-configurations` foi alterado para aceitar um caminho para um arquivo JSON local ou uma cadeia de caracteres JSON</span><span class="sxs-lookup"><span data-stu-id="1dfd6-852">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="1dfd6-853">Adicionado o comando `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-853">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="1dfd6-854">Alterado `hdinsight monitor enable --workspace` para aceitar uma ID do workspace ou nome do workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="1dfd6-854">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="1dfd6-855">O argumento `hdinsight monitor enable --primary-key`, que será necessário caso uma ID do workspace seja fornecida como o parâmetro, foi adicionado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-855">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="1dfd6-856">Foram adicionados mais exemplos e atualização das descrições das mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="1dfd6-856">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="1dfd6-857">Interativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-857">Interactive</span></span>

* <span data-ttu-id="1dfd6-858">Um erro no carregamento foi corrigido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-858">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="1dfd6-859">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-859">Kubernetes</span></span>

* <span data-ttu-id="1dfd6-860">Alterado para usar `https` se a porta do contêiner do painel estiver usando `https`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-860">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-861">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-861">Network</span></span>

* <span data-ttu-id="1dfd6-862">O argumento `--yes` foi adicionado a `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-862">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="1dfd6-863">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-863">Profile</span></span>

* <span data-ttu-id="1dfd6-864">O argumento `--resource-type` foi adicionado a `account get-access-token` para obter tokens de acesso de recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-864">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="1dfd6-865">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1dfd6-865">ServiceFabric</span></span>

* <span data-ttu-id="1dfd6-866">Todas as versões de sistema operacional com suporte para criação do cluster sf foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-866">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="1dfd6-867">Foi corrigido o bug de validação do certificado primário</span><span class="sxs-lookup"><span data-stu-id="1dfd6-867">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-868">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-868">Storage</span></span>

* <span data-ttu-id="1dfd6-869">Adicionado o comando `storage copy`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-869">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="1dfd6-870">30 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-870">July 30, 2019</span></span>

<span data-ttu-id="1dfd6-871">Versão 2.0.70</span><span class="sxs-lookup"><span data-stu-id="1dfd6-871">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-872">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-872">ACR</span></span>

* <span data-ttu-id="1dfd6-873">Corrigido o problema #9952 (uma regressão no comando `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-873">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="1dfd6-874">Removido o nome da imagem do construtor padrão em `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-874">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-875">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-875">Appservice</span></span>

* <span data-ttu-id="1dfd6-876">Alterado `webapp config ssl` para mostrar uma mensagem se um recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-876">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="1dfd6-877">Corrigido o problema em que `functionapp create` não aceita o tipo de conta de armazenamento `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-877">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="1dfd6-878">Corrigido um problema em que `webapp up` falharia se fosse executado usando versões mais antigas do Python</span><span class="sxs-lookup"><span data-stu-id="1dfd6-878">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-879">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-879">Network</span></span>

* <span data-ttu-id="1dfd6-880">Removido parâmetro inválido `--ids` de `network nic ip-config add` (corrige o #9861)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-880">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="1dfd6-881">Corrige o #9604.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-881">Fixes #9604.</span></span> <span data-ttu-id="1dfd6-882">Adicionado o parâmetro `--root-certs` ao `network application-gateway http-settings [create|update]` para dar suporte a certificados raiz confiáveis associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-882">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="1dfd6-883">Fixado argumento `--subscription` para `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-883">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="1dfd6-884">RBAC</span><span class="sxs-lookup"><span data-stu-id="1dfd6-884">RBAC</span></span>

* <span data-ttu-id="1dfd6-885">Adicionado o comando `user update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-885">Added `user update` command</span></span>
* <span data-ttu-id="1dfd6-886">[PRETERIDO] Preterido `--upn-or-object-id` de comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="1dfd6-886">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="1dfd6-887">Usar argumento de substituição `--id`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-887">Use replacement argument `--id`</span></span>
* <span data-ttu-id="1dfd6-888">Adicionado argumento `--id` para comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="1dfd6-888">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-889">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-889">SQL</span></span>

* <span data-ttu-id="1dfd6-890">Adicionados comandos de gerenciamento para chaves de instância gerenciada e protetor de TDE</span><span class="sxs-lookup"><span data-stu-id="1dfd6-890">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-891">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-891">Storage</span></span>

* <span data-ttu-id="1dfd6-892">Adicionado o comando `storage remove`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-892">Added `storage remove` command</span></span>
* <span data-ttu-id="1dfd6-893">Corrigido um problema com `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-893">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-894">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-894">VM</span></span>

* <span data-ttu-id="1dfd6-895">Alterado `list-skus` para usar versão de API mais recente a fim de externar detalhes de zona</span><span class="sxs-lookup"><span data-stu-id="1dfd6-895">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="1dfd6-896">Alterado o padrão de `--single-placement-group` para `false` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-896">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="1dfd6-897">Adicionada a capacidade de selecionar SKUs de armazenamento ZRS para `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-897">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="1dfd6-898">Adicionado novo grupo de comandos `vm host` para dar suporte a hosts dedicados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-898">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="1dfd6-899">Adicionados parâmetros `--host` e `--host-group` em `vm create` para definir o host dedicado da VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-899">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="1dfd6-900">16 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-900">July 16, 2019</span></span>

<span data-ttu-id="1dfd6-901">Versão 2.0.69</span><span class="sxs-lookup"><span data-stu-id="1dfd6-901">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-902">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-902">Appservice</span></span>

* <span data-ttu-id="1dfd6-903">Os comandos `webapp identity` foram alterados para retornar uma mensagem de erro apropriada se o nome do aplicativo ou ResourceGroupName for inválido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-903">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="1dfd6-904">`webapp list` corrigido para retornar o valor correto para numberOfSites se nenhum ResourceGroup foi fornecido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-904">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="1dfd6-905">Corrigidos os efeitos colaterais de `appservice plan create` e `webapp create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-905">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-906">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-906">Core</span></span>

* <span data-ttu-id="1dfd6-907">Corrigido um problema em que `--subscription` aparecia apesar de não ser aplicável</span><span class="sxs-lookup"><span data-stu-id="1dfd6-907">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="1dfd6-908">Lote</span><span class="sxs-lookup"><span data-stu-id="1dfd6-908">Batch</span></span>

* <span data-ttu-id="1dfd6-909">[ALTERAÇÃO SIGNIFICATIVA]`batch pool node-agent-skus list` foi substituído por `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-909">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="1dfd6-910">Adicionado suporte para regras de segurança bloqueando o acesso de rede a um pool com base na porta de origem do tráfego ao usar a opção `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-910">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="1dfd6-911">Suporte adicionado para executar a tarefa no diretório de trabalho de contêiner ou no diretório de trabalho de tarefa em lotes ao usar a opção `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-911">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="1dfd6-912">Corrigido o erro na opção `--application-package-references` de `batch pool create` em que ela funcionaria apenas com padrões</span><span class="sxs-lookup"><span data-stu-id="1dfd6-912">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="1dfd6-913">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-913">Eventhubs</span></span>

* <span data-ttu-id="1dfd6-914">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-914">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="1dfd6-915">RDBMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-915">RDBMS</span></span>

* <span data-ttu-id="1dfd6-916">Adicionado um parâmetro opcional para especificar a réplica de SKU para criar o comando de réplica</span><span class="sxs-lookup"><span data-stu-id="1dfd6-916">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="1dfd6-917">Corrigido o problema com a falha no teste de CI com a criação de réplica de MySQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-917">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="1dfd6-918">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-918">Relay</span></span>

* <span data-ttu-id="1dfd6-919">Corrigido o problema com a conexão híbrida quando a autorização do cliente desabilitava [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-919">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="1dfd6-920">Parâmetro `--requires-transport-security` adicionado a `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-920">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="1dfd6-921">Barramento de serviço</span><span class="sxs-lookup"><span data-stu-id="1dfd6-921">Servicebus</span></span>

* <span data-ttu-id="1dfd6-922">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-922">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-923">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-923">Storage</span></span>

* <span data-ttu-id="1dfd6-924">Habilitar AADDS de arquivos para atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-924">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="1dfd6-925">Problema corrigido `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-925">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="1dfd6-926">2 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-926">July 2, 2019</span></span>

<span data-ttu-id="1dfd6-927">Versão 2.0.68</span><span class="sxs-lookup"><span data-stu-id="1dfd6-927">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-928">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-928">Core</span></span>

* <span data-ttu-id="1dfd6-929">Agora, os módulos de comando são consolidados em um único Python distribuível.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-929">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="1dfd6-930">Isso substitui o uso direto de muitos pacotes `azure-cli-` no PyPI.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-930">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="1dfd6-931">Assim, o tamanho da instalação será reduzido e apenas os usuários que tiverem instalado diretamente por meio do `pip` serão afetados.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-931">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-932">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-932">ACR</span></span>

* <span data-ttu-id="1dfd6-933">Foi adicionado o suporte para gatilhos de temporizador para tarefa</span><span class="sxs-lookup"><span data-stu-id="1dfd6-933">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-934">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-934">Appservice</span></span>

* <span data-ttu-id="1dfd6-935">O `functionapp create` foi alterado para habilitar o Application Insights por padrão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-935">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="1dfd6-936">[ALTERAÇÃO SIGNIFICATIVA] Foi removido o comando `functionapp devops-build` preterido.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-936">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="1dfd6-937">Agora, use o novo comando `az functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-937">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="1dfd6-938">Foi adicionado o suporte ao plano de aplicativo de funções Consumo em Linux ao `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-938">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="1dfd6-939">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-939">Cosmos DB</span></span>

* <span data-ttu-id="1dfd6-940">Foi adicionado o suporte para desabilitar a TTL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-940">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="1dfd6-941">DLS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-941">DLS</span></span>

* <span data-ttu-id="1dfd6-942">Versão atualizada do ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-942">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="1dfd6-943">Comentários</span><span class="sxs-lookup"><span data-stu-id="1dfd6-943">Feedback</span></span>

* <span data-ttu-id="1dfd6-944">Ao relatar um comando de extensão com falha, agora, o `az feedback` tenta abrir o navegador na URL do projeto/repositório da extensão por meio do índice</span><span class="sxs-lookup"><span data-stu-id="1dfd6-944">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1dfd6-945">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1dfd6-945">HDInsight</span></span>

* <span data-ttu-id="1dfd6-946">[ALTERAÇÃO SIGNIFICATIVA] O nome do grupo de comandos `oms` foi alterado para `monitor`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-946">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="1dfd6-947">[ALTERAÇÃO SIGNIFICATIVA]`--http-password/-p` tornou-se um parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="1dfd6-947">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="1dfd6-948">Foram adicionados preenchedores para o preenchedor dos parâmetros `--cluster-admin-account` e `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-948">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="1dfd6-949">O parâmetro `cluster-users-group-dns` foi alterado para ser obrigatório quando `—esp` estiver presente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-949">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="1dfd6-950">Foi adicionado um tempo limite para todos os preenchedores automáticos de argumento existentes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-950">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="1dfd6-951">Foi adicionado um tempo limite para transformar o nome do recurso na ID de recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-951">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="1dfd6-952">Os preenchedores automáticos foram alterados para selecionar recursos de qualquer grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-952">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="1dfd6-953">Pode ser um grupo de recursos diferente daquele especificado com `-g`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-953">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="1dfd6-954">Foi adicionado o suporte para os parâmetros `--sub-domain-suffix` e `--disable_gateway_auth` no comando `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-954">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="1dfd6-955">Serviços gerenciados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-955">Managed Services</span></span>

* <span data-ttu-id="1dfd6-956">Introdução ao módulo de comando de serviço gerenciado em versão prévia</span><span class="sxs-lookup"><span data-stu-id="1dfd6-956">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="1dfd6-957">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-957">Profile</span></span>
* <span data-ttu-id="1dfd6-958">Suprimir o argumento `--subscription` para o comando de logoff</span><span class="sxs-lookup"><span data-stu-id="1dfd6-958">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="1dfd6-959">RBAC</span><span class="sxs-lookup"><span data-stu-id="1dfd6-959">RBAC</span></span>

* <span data-ttu-id="1dfd6-960">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--password` foi removido de `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-960">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="1dfd6-961">Foi adicionado o parâmetro `--assignee-principal-type` ao comando `create` para evitar falhas intermitentes causadas pela latência de replicação do servidor do AAD Graph</span><span class="sxs-lookup"><span data-stu-id="1dfd6-961">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="1dfd6-962">Foi corrigida uma falha em `ad signed-in-user` ao listar objetos de propriedade</span><span class="sxs-lookup"><span data-stu-id="1dfd6-962">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="1dfd6-963">Foi corrigido um problema em que o `ad sp` não localizava o aplicativo certo de uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="1dfd6-963">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="1dfd6-964">RDBMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-964">RDBMS</span></span>

* <span data-ttu-id="1dfd6-965">Foi adicionado o suporte à replicação para o MariaDB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-965">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-966">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-966">SQL</span></span>

* <span data-ttu-id="1dfd6-967">Valores permitidos documentados para `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-967">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-968">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-968">Storage</span></span>

* <span data-ttu-id="1dfd6-969">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-969">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="1dfd6-970">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-970">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="1dfd6-971">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-971">VM</span></span>

* <span data-ttu-id="1dfd6-972">Foi corrigido o bug em que o `vmss create` retornava uma mensagem de erro quando era executado com `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-972">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="1dfd6-973">Foi removida a validação do lado do cliente de `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-973">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="1dfd6-974">Não falha quando `--single-placement-group` é definido como `true` e `--instance-count` é maior que 100 ou quando são especificadas zonas de disponibilidade, mas deixa essa validação para o serviço de computação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-974">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="1dfd6-975">Foi corrigido o bug em que o `[vm|vmss] extension image list` falhava quando era usado com `--latest`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-975">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="1dfd6-976">18 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-976">June 18, 2019</span></span>

<span data-ttu-id="1dfd6-977">Versão 2.0.67</span><span class="sxs-lookup"><span data-stu-id="1dfd6-977">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-978">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-978">Core</span></span>

<span data-ttu-id="1dfd6-979">Esta versão apresenta uma nova marca [Versão prévia] para comunicar com mais clareza aos clientes quando um comando, um grupo de comandos ou um argumento está no status de versão prévia.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-979">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="1dfd6-980">Anteriormente, essa informação era transmitida no texto de ajuda ou, implicitamente, pelo número da versão do módulo de comando.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-980">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="1dfd6-981">A CLI removerá os números de versão dos pacotes individuais no futuro.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-981">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="1dfd6-982">Se um comando estiver em versão prévia, todos os seus argumentos também estarão.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-982">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="1dfd6-983">Se um grupo de comandos for rotulado com o status de versão prévia, então todos os seus comandos e argumentos também serão considerados em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-983">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="1dfd6-984">Como resultado dessa alteração, diversos grupos de comandos podem parecer surgir "de repente" com o status de versão prévia com esta liberação.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-984">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="1dfd6-985">O que realmente aconteceu é que a maioria dos pacotes já estava com status de versão prévia, mas estão sendo consideradas GA com esta liberação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-985">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-986">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-986">ACR</span></span>
* <span data-ttu-id="1dfd6-987">Adicionado o comando 'acr check-health'</span><span class="sxs-lookup"><span data-stu-id="1dfd6-987">Added 'acr check-health' command</span></span>
* <span data-ttu-id="1dfd6-988">Melhorado o tratamento de erro para tokens do AAD e para recuperar comandos externos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-988">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-989">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-989">ACS</span></span>
* <span data-ttu-id="1dfd6-990">Comandos preteridos do ACS agora ficam ocultos da exibição da ajuda</span><span class="sxs-lookup"><span data-stu-id="1dfd6-990">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="1dfd6-991">AMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-991">AMS</span></span>
* <span data-ttu-id="1dfd6-992">[ALTERAÇÃO SIGNIFICATIVA] Alterada para retornar cadeias de caracteres de tempo da ISO 8601 para archive-window-length e key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="1dfd6-992">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-993">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-993">AppService</span></span>
* <span data-ttu-id="1dfd6-994">Adicionado roteamento com base no local para `webapp deleted list` e `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-994">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="1dfd6-995">Corrigido problema em que a URL de destino registrada do webapp ("Não é possível iniciar o aplicativo em...") não era clicável no Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="1dfd6-995">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="1dfd6-996">Corrigido um problema em que a criação de aplicativos com algumas SKUs falhava com um erro de AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="1dfd6-996">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="1dfd6-997">Adicionada a pré-validação para o `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-997">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="1dfd6-998">Corrigido o `[webapp|functionapp] traffic-routing` para usar o actionHostName correto</span><span class="sxs-lookup"><span data-stu-id="1dfd6-998">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="1dfd6-999">Adicionado o suporte de slot para comandos `functionapp`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-999">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="1dfd6-1000">Lote</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1000">Batch</span></span>
* <span data-ttu-id="1dfd6-1001">Corrigida a regressão de autenticação do AAD causada pela geração de relatórios de erros superagressiva para autenticação de chave compartilhada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1001">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="1dfd6-1002">BatchAI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1002">BatchAI</span></span>
* <span data-ttu-id="1dfd6-1003">Agora os comandos do BatchAI estão preteridos e ocultos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1003">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="1dfd6-1004">BotService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1004">BotService</span></span>
* <span data-ttu-id="1dfd6-1005">Adição das mensagens de aviso "suporte descontinuado"/"modo de manutenção" para os comandos compatíveis com a v3 do SDK</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1005">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1dfd6-1006">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1006">CosmosDB</span></span>
* <span data-ttu-id="1dfd6-1007">[PRETERIDO] Preterido o comando `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1007">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="1dfd6-1008">Adicionado o comando `cosmosdb keys list` – substitui o `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1008">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="1dfd6-1009">`cosmsodb create/update`: Adicionado novo formato para --location a fim de permitir a configuração da propriedade "isZoneRedundant".</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1009">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="1dfd6-1010">Formato antigo preterido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1010">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="1dfd6-1011">EventGrid</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1011">EventGrid</span></span>
* <span data-ttu-id="1dfd6-1012">Adicionados comandos do `eventgrid domain` para operações de CRUD no domínio</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1012">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="1dfd6-1013">Adicionados comandos do `eventgrid domain topic` para operações de CRUD nos tópicos do domínio</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1013">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="1dfd6-1014">Adicionado argumento do `--odata-query` ao `eventgrid [topic|event-subscription] list` para filtrar os resultados usando a sintaxe do OData</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1014">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="1dfd6-1015">`event-subscription create/update`: Adicionado o servicebusqueue como novos valores para o parâmetro `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1015">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="1dfd6-1016">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para `--included-event-types All` com `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1016">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1dfd6-1017">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1017">HDInsight</span></span>
* <span data-ttu-id="1dfd6-1018">Adicionado suporte para o parâmetro `--ssh-public-key` no comando `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1018">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="1dfd6-1019">IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1019">IoT</span></span>
* <span data-ttu-id="1dfd6-1020">Adicionado suporte para regenerar as chaves da política de autorização</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1020">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="1dfd6-1021">Adicionados SDK e suporte para o serviço de provisionamento de repositórios do DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1021">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-1022">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1022">Network</span></span>
* <span data-ttu-id="1dfd6-1023">Adicionado suporte de zona para o Gateway da NAT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1023">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="1dfd6-1024">Adicionado o comando `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1024">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="1dfd6-1025">Corrigido o problema com o `dns zone import` em que os usuários não conseguiam importar registros do curinga A</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1025">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="1dfd6-1026">Corrigido o problema com o `watcher flow-log configure` em que o registro de fluxo não podia ser habilitado em determinadas regiões</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1026">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-1027">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1027">Resource</span></span>
* <span data-ttu-id="1dfd6-1028">Adicionado o comando do `az rest` para fazer chamadas REST</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1028">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="1dfd6-1029">Corrigido o erro ao usar o `policy assignment list` com um grupo de recursos ou o nível de assinatura `--scope`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1029">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="1dfd6-1030">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1030">ServiceBus</span></span>
* <span data-ttu-id="1dfd6-1031">Corrigido o problema com o `servicebus topic create --max-size`[nº9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1031">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-1032">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1032">SQL</span></span>
* <span data-ttu-id="1dfd6-1033">Alterado o `--location` para ser opcional para `sql [server|mi] create` – usa o local do grupo de recursos se não especificado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1033">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="1dfd6-1034">Corrigido o erro "objeto 'NoneType' não é iterável" para `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1034">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="1dfd6-1035">SQLVm</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1035">SQLVm</span></span>
* <span data-ttu-id="1dfd6-1036">[ALTERAÇÃO DA FALHA] Alterado `sql vm create` para exigir o parâmetro `--license-type`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1036">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="1dfd6-1037">Alterado para permitir a configuração da SKU da imagem do SQL ao criar ou atualizar uma VM do SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1037">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-1038">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1038">Storage</span></span>
* <span data-ttu-id="1dfd6-1039">Corrigido o problema com a chave de conta ignorada para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1039">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="1dfd6-1040">Corrigido o problema com o `storage blob sync` no Linux</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1040">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-1041">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1041">VM</span></span>
* <span data-ttu-id="1dfd6-1042">[VERSÃO PRÉVIA] Adicionados os comandos `vm image template` para criar imagens de VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1042">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="1dfd6-1043">4 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1043">June 4, 2019</span></span>

<span data-ttu-id="1dfd6-1044">Versão 2.0.66</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1044">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-1045">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1045">Core</span></span>
* <span data-ttu-id="1dfd6-1046">Foi corrigido o bug em que os comandos falhavam quando `--output yaml` era usado com `--query`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1046">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-1047">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1047">ACR</span></span>
* <span data-ttu-id="1dfd6-1048">Foi adicionado o grupo de comando 'pack acr' para a criação de Tarefas de build rápida usando Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1048">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-1049">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1049">ACS</span></span>
* <span data-ttu-id="1dfd6-1050">Permitir a opção de habilitar/desabilitar o complemento kube-dashboard do AKS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1050">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="1dfd6-1051">Imprimir uma mensagem amigável quando a assinatura não estiver na lista de permissões para usar o Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1051">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="1dfd6-1052">Lote</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1052">Batch</span></span>
* <span data-ttu-id="1dfd6-1053">Melhoria no tratamento de erro quando você não está conectado a uma conta \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1053">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="1dfd6-1054">IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1054">IoT</span></span>
* <span data-ttu-id="1dfd6-1055">Foi adicionado o suporte para failover manual</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1055">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-1056">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1056">Network</span></span>
* <span data-ttu-id="1dfd6-1057">Foram adicionados os comandos `network application-gateway waf-policy` para oferecer suporte às regras de WAF personalizadas.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1057">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="1dfd6-1058">Adicionados os argumentos `--waf-policy` e `--max-capacity` para `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1058">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="1dfd6-1059">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1059">Resource</span></span>
* <span data-ttu-id="1dfd6-1060">Melhoria da mensagem de erro do `deployment create` quando não há nenhum TTY disponível</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1060">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-1061">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1061">Role</span></span>
* <span data-ttu-id="1dfd6-1062">O texto da Ajuda foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1062">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="1dfd6-1063">Computação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1063">Compute</span></span>
* <span data-ttu-id="1dfd6-1064">Foi adicionado o suporte para `vm create` para as VMs de uma imagem gerenciada com LUNs de disco de dados que não começam em 0 ou que ignoram números</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1064">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="1dfd6-1065">21 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1065">May 21, 2019</span></span>

<span data-ttu-id="1dfd6-1066">Versão 2.0.65</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1066">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-1067">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1067">Core</span></span>
* <span data-ttu-id="1dfd6-1068">Foram adicionados comentários melhores para erros de autenticação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1068">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="1dfd6-1069">Corrigido um problema em que a CLI carregava extensões que não eram compatíveis com a versão do núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1069">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="1dfd6-1070">Corrigido um problema com a inicialização quando `clouds.config` está corrompido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1070">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-1071">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1071">ACR</span></span>
* <span data-ttu-id="1dfd6-1072">Foi adicionado suporte das Identidades Gerenciadas para Tarefas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1072">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-1073">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1073">ACS</span></span>
* <span data-ttu-id="1dfd6-1074">Corrigido o comando `openshift create` quando usado com o cliente AAD do consumidor</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1074">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-1075">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1075">AppService</span></span>
* <span data-ttu-id="1dfd6-1076">[PRETERIDO] Preterido o comando `functionapp devops-build` – Será removido na próxima versão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1076">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="1dfd6-1077">`functionapp devops-pipeline` foi alterado para buscar o log de build do Azure DevOps no modo detalhado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1077">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="1dfd6-1078">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--use_local_settings` foi removido do comando `functionapp devops-pipeline` – não estava operacional</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1078">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="1dfd6-1079">`webapp up` foi alterado para retornar uma saída JSON se `--logs` não for usado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1079">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="1dfd6-1080">Foi adicionado suporte para escrever recursos padrão para a configuração local de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1080">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="1dfd6-1081">Foi adicionado suporte para `webapp up` reimplantar um aplicativo sem usar o argumento `--location`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1081">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="1dfd6-1082">Corrigido um problema em que o valor do SKU gratuito não funcionava na criação do ASP do SKU gratuito do Linux</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1082">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="1dfd6-1083">BotService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1083">BotService</span></span>
* <span data-ttu-id="1dfd6-1084">Alterado para permitir todas as capitalizações para parâmetros `--lang` em todos os comandos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1084">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="1dfd6-1085">Descrição atualizada do módulo de comando</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1085">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="1dfd6-1086">Consumo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1086">Consumption</span></span>
* <span data-ttu-id="1dfd6-1087">O parâmetro obrigatório ausente foi adicionado para executar `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1087">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="1dfd6-1088">IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1088">IoT</span></span>
* <span data-ttu-id="1dfd6-1089">Suporte adicionado para listar todas as chaves</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1089">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-1090">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1090">Network</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="1dfd6-1092">O argumento `--nat-gateway` foi adicionado a `network vnet subnet [create|update]` para anexar a um gateway NAT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1092">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="1dfd6-1093">Corrigido o problema de `dns zone import`, em que os nomes de registro não correspondiam ao tipo de registro</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1093">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="1dfd6-1094">RDBMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1094">RDBMS</span></span>
* <span data-ttu-id="1dfd6-1095">Suporte a postgres e mysql adicionado para replicação geográfica</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1095">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="1dfd6-1096">RBAC</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1096">RBAC</span></span>
* <span data-ttu-id="1dfd6-1097">Adição de suporte do escopo de grupo de gerenciamento a `role assignment`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1097">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-1098">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1098">Storage</span></span>
* <span data-ttu-id="1dfd6-1099">`storage blob sync`: adicionar um comando de sincronização ao armazenamento de blobs</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1099">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="1dfd6-1100">Computação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1100">Compute</span></span>
* <span data-ttu-id="1dfd6-1101">`--computer-name` foi adicionado a `vm create` para configurar o nome do computador da VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1101">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="1dfd6-1102">`--ssh-key-value` foi renomeado para `--ssh-key-values` para `[vm|vmss] create` – Agora, pode aceitar vários valores de chave pública ou caminhos ssh</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1102">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="1dfd6-1103">__Observação__: Isso **não** é uma alteração da falha – `--ssh-key-value` será analisado corretamente, pois corresponde somente a `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1103">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="1dfd6-1104">O argumento `--type` de `ppg create` foi alterado para ser opcional</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1104">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="1dfd6-1105">6 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1105">May 6, 2019</span></span>

<span data-ttu-id="1dfd6-1106">Versão 2.0.64</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1106">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-1107">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1107">ACS</span></span>
* <span data-ttu-id="1dfd6-1108">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--fqdn` foi removido dos comandos `openshift`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1108">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="1dfd6-1109">Alterado para usar a versão da API do Red Hat OpenShift no Azure em disponibilidade geral</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1109">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="1dfd6-1110">O sinalizador `customer-admin-group-id` foi adicionado a `openshift create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1110">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="1dfd6-1111">[GA] `(PREVIEW)` foi removido da opção `aks create``--network-policy`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1111">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-1112">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1112">Appservice</span></span>
* <span data-ttu-id="1dfd6-1113">[PRETERIDO] O comando `functionapp devops-build` foi preterido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1113">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="1dfd6-1114">Renomeado para `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1114">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="1dfd6-1115">Corrigido ao obter o nome de usuário correto para cloudshell que estava causando a falha em `webapp up`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1115">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="1dfd6-1116">Documentação `appservice plan --sku` atualizada para refletir o appserviceplans com suporte</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1116">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="1dfd6-1117">Adicionado argumentos opcionais para o grupo de recursos e plano a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1117">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="1dfd6-1118">Adicionado suporte a `webapp ssh` para respeitar a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1118">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="1dfd6-1119">Adicionado suporte `appserviceplan create` para a SKU gratuita do Linux</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1119">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="1dfd6-1120">Alterado `webapp up` para ter uma suspensão de 30 segundos depois de definir appsetting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` para lidar com a inicialização a frio kudu</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1120">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="1dfd6-1121">Adicionado suporte para runtime `powershell` a `functionapp create` no Windows</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1121">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="1dfd6-1122">Adicionado o comando `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1122">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="1dfd6-1123">Lote</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1123">Batch</span></span>
* <span data-ttu-id="1dfd6-1124">Corrigido o bug no validador para as opções `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1124">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="1dfd6-1125">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1125">Botservice</span></span>
* <span data-ttu-id="1dfd6-1126">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para criar um Bot de Aplicativo Web vazio por padrão (ou seja, nenhum bot será implantado no Serviço de Aplicativo)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1126">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="1dfd6-1127">O sinalizador `--echo` foi adicionado ao `bot create` para usar o comportamento antigo com `-v v4`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1127">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="1dfd6-1128">[ALTERAÇÃO SIGNIFICATIVA] O valor padrão de `--version` foi alterado para `v4`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1128">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="1dfd6-1129">__OBSERVAÇÃO:__ `bot prepare-publish` ainda usa o padrão antigo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1129">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="1dfd6-1130">[ALTERAÇÃO SIGNIFICATIVA]`--lang` foi alterado para não definir mais `Csharp` como padrão.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1130">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="1dfd6-1131">Se o comando exigir `--lang` e ele não for fornecido, o comando será um erro</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1131">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="1dfd6-1132">[ALTERAÇÃO SIGNIFICATIVA] Os argumentos `--appid` e `--password` foram alterados para `bot create` ser obrigatório e agora podem ser criados por meio de `ad app create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1132">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="1dfd6-1133">Foi adicionada validação a `--appid` e `--password`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1133">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="1dfd6-1134">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4` foi alterado para não criar ou usar uma Conta de Armazenamento ou o Application Insights</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1134">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="1dfd6-1135">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v3` foi alterado para exigir uma região em que o Application Insights está disponível</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1135">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="1dfd6-1136">[ALTERAÇÃO SIGNIFICATIVA] O `bot update` foi alterado para afetar somente as propriedades específicas de um bot</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1136">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="1dfd6-1137">[ALTERAÇÃO SIGNIFICATIVA] Os sinalizadores `--lang` foram alterados para aceitar `Javascript` em vez de `Node`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1137">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="1dfd6-1138">[ALTERAÇÃO SIGNIFICATIVA] O `Node` foi removido como um valor `--lang` permitido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1138">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="1dfd6-1139">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para não definir mais `SCM_DO_BUILD_DURING_DEPLOYMENT` como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1139">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="1dfd6-1140">Todas as implantações por meio do Kudu atuarão de acordo com o comportamento padrão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1140">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="1dfd6-1141">O `bot download` foi alterado para os bots sem arquivos `.bot` para criar o arquivo de configuração específico a um idioma com os valores das Configurações de Aplicativo do bot</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1141">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="1dfd6-1142">Adicionado o suporte `Typescript` para `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1142">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="1dfd6-1143">Uma mensagem de aviso foi adicionada a `bot prepare-deploy` para os bots `Javascript` e `Typescript` para quando `--code-dir` não contiver `package.json`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1143">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="1dfd6-1144">O `bot prepare-deploy` foi alterado para retornar `true`, se bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1144">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="1dfd6-1145">O log detalhado foi adicionado a `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1145">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="1dfd6-1146">Mais regiões disponíveis do Application Insights foram adicionadas ao `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1146">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="1dfd6-1147">Configurar</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1147">Configure</span></span>
* <span data-ttu-id="1dfd6-1148">Adicionado suporte para configurações de valor padrão do argumento baseado em pasta</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1148">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="1dfd6-1149">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1149">Eventhubs</span></span>
* <span data-ttu-id="1dfd6-1150">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1150">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="1dfd6-1151">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1151">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-1152">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1152">Network</span></span>
* <span data-ttu-id="1dfd6-1153">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--cache` foi substituído por `--defer` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1153">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="1dfd6-1154">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1154">Policy Insights</span></span>
* <span data-ttu-id="1dfd6-1155">Suporte adicionado a `--expand PolicyEvaluationDetails` para detalhes de avaliação de política de consulta no recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1155">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-1156">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1156">Role</span></span>
* <span data-ttu-id="1dfd6-1157">[PRETERIDO] Alterado argumento ocultar '--password' `create-for-rbac` - suporte será removido em maio de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1157">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="1dfd6-1158">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1158">Service Bus</span></span>
* <span data-ttu-id="1dfd6-1159">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1159">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="1dfd6-1160">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1160">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="1dfd6-1161">`topic [create|update]` foi fixado para permitir suporte a `--max-size` para valores de 10, 20, 40 e 80 GB com a SKU Premium</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1161">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-1162">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1162">SQL</span></span>
* <span data-ttu-id="1dfd6-1163">Adicionados os comandos `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1163">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-1164">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1164">VM</span></span>
* <span data-ttu-id="1dfd6-1165">O `--protect-from-scale-in` e o `--protect-from-scale-set-actions` foram adicionados a `vmss update` para habilitar atualizações à política de proteção das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1165">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="1dfd6-1166">Adicionado a `--instance-id` e `vmss update` para habilitar atualização genérica das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1166">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="1dfd6-1167">`--instance-id` foi adicionado a `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1167">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="1dfd6-1168">Adição do novo grupo de comandos `ppg` para gerenciar Grupos de Posicionamento de Proximidade</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1168">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="1dfd6-1169">Adicionado a `--ppg`, `[vm|vmss] create` e `vm availability-set create` para gerenciar PPGs</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1169">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="1dfd6-1170">Parâmetro `--hyper-v-generation` adicionado a `image create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1170">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="1dfd6-1171">23 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1171">April 23, 2019</span></span>

<span data-ttu-id="1dfd6-1172">Versão 2.0.63</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1172">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-1173">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1173">ACS</span></span>
* <span data-ttu-id="1dfd6-1174">Alterado `aks get-credentials` para solicitar substituição dos valores duplicados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1174">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="1dfd6-1175">Removido `(PREVIEW)` dos comandos de espaços de desenvolvimento "aks use-dev-espaces" e "aks remove-dev-espaces"</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1175">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="1dfd6-1176">AMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1176">AMS</span></span>
* <span data-ttu-id="1dfd6-1177">Corrigido o bug com a atualização de filtros de conta e de ativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1177">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-1178">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1178">AppService</span></span>
* <span data-ttu-id="1dfd6-1179">Adicionado suporte para o ASE e o tempo limite para `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1179">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="1dfd6-1180">Adicionado suporte para o estabelecimento de CI CD em um pipeline do Azure DevOps de um repositório do Github para aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1180">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="1dfd6-1181">Adicionado argumento `--github-pat` a `functionapp devops-build create` para aceitar o token de acesso pessoal do Github</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1181">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="1dfd6-1182">Adicionado argumento `--github-repository` a `functionapp devops-build create` para aceitar o repositório Github que contém um código-fonte functionapp</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1182">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="1dfd6-1183">Problema corrigido em que `az webapp up --logs` estava falhando com um erro e atualização da versão .NETCORE padrão para 2.1</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1183">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="1dfd6-1184">Configurações de functionapp desnecessárias removidas durante a criação de um aplicativo de funções com plano de consumo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1184">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="1dfd6-1185">Alterado `webapp up` para que a cadeia de caracteres padrão asp agora acrescente o número no final para criar um novo ASP com base nas opções de SKU</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1185">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="1dfd6-1186">Adicionado `-b` como uma opção a `webapp up` para iniciar o aplicativo no navegador</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1186">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="1dfd6-1187">Alterado `webapp deployment source config zip` para lidar com a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1187">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="1dfd6-1188">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1188">Deployment Manager</span></span>
* <span data-ttu-id="1dfd6-1189">[VERSÃO PRÉVIA] Criar e gerenciar artefatos que dão suporte a distribuições</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1189">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="1dfd6-1190">Laboratório</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1190">Lab</span></span>
* <span data-ttu-id="1dfd6-1191">Corrigido o bug que causa uma saída inicial</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1191">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-1192">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1192">Network</span></span>
* <span data-ttu-id="1dfd6-1193">Adicionada delegação de servidor de nome automática a `dns zone create` no pai durante a criação da zona filho</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1193">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-1194">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1194">Resource</span></span>
* <span data-ttu-id="1dfd6-1195">[PRETERIDO] Argumentos `--link-id`, `--target-id` e `--filter-string` preteridos de `resource link`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1195">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="1dfd6-1196">Use os argumentos `--link`, `--target` e `--filter`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1196">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="1dfd6-1197">Corrigido o problema em que os comandos `resource link [create|update]` não funcionavam</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1197">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="1dfd6-1198">Corrigido um problema em que a exclusão usando uma ID de recurso poderia causar falha no erro</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1198">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-1199">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1199">SQL</span></span>
* <span data-ttu-id="1dfd6-1200">Adicionado suporte para fuso horário personalizado nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1200">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="1dfd6-1201">Alterado para permitir que o nome do pool Elástico seja usado com `sql db update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1201">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="1dfd6-1202">Adicionado o suporte `--no-wait` para `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1202">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="1dfd6-1203">Adicionado o comando `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1203">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-1204">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1204">Storage</span></span>
* <span data-ttu-id="1dfd6-1205">Corrigido o problema com tokens SAS com codificação dupla em `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1205">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-1206">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1206">VM</span></span>
* <span data-ttu-id="1dfd6-1207">Adicionado sinalizador `--skip-shutdown` a `vm|vmss stop` para desligar as VMs sem o desligamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1207">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="1dfd6-1208">Adicionado argumento `--storage-account-type` a `sig image-version create` para definir o tipo de conta do perfil de publicação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1208">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="1dfd6-1209">Adicionado argumento `--target-regions` a `sig image-version create` para permitir definir os tipos de conta de armazenamento específico da região</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1209">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="1dfd6-1210">9 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1210">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-1211">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1211">Core</span></span>
* <span data-ttu-id="1dfd6-1212">Correção do problema em que algumas extensões mostraram uma versão do `Unknown` e não podiam ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1212">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-1213">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1213">ACR</span></span>
* <span data-ttu-id="1dfd6-1214">Adição de suporte para execução de uma imagem sem contexto</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1214">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="1dfd6-1215">AMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1215">AMS</span></span>
* [PRETERIDO]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [ALTERAÇÃO SIGNIFICATIVA]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="1dfd6-1218">Adição de suporte para novos parâmetros de criptografia em `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1218">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="1dfd6-1219">Adição de novo parâmetro `--filters` a `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1219">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-1220">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1220">AppService</span></span>
* <span data-ttu-id="1dfd6-1221">Adicionado o suporte `--logs` para `webapp up`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1221">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="1dfd6-1222">Correção de problemas do comando `functionapp devops-build create` de geração de `azure-pipelines.yml`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1222">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="1dfd6-1223">Melhoria do tratamento de erros e indicadores `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1223">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="1dfd6-1224">[ALTERAÇÃO SIGNIFICATIVA] Remoção do sinalizador `--local-git` para o comando `devops-build`; a detecção de git local e a manipulação são obrigatórias para a criação de pipelines do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1224">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="1dfd6-1225">Adição de suporte para a criação de planos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1225">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="1dfd6-1226">Adição da capacidade de trocar um plano sob um aplicativo de funções usando `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1226">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="1dfd6-1227">Adição de suporte para configurações de expansão de plano Premium do Azure Functions</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1227">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="1dfd6-1228">CDN</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1228">CDN</span></span>
* <span data-ttu-id="1dfd6-1229">Adição de suporte para `Microsoft_Standard` e `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1229">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="1dfd6-1230">Comentários</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1230">Feedback</span></span>
* <span data-ttu-id="1dfd6-1231">Alteração de `feedback` para mostrar metadados em comandos executados recentemente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1231">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="1dfd6-1232">Alteração de `feedback` para solicitar o auxílio do usuário no processo de criação de problema abrindo um navegador e usando um modelo de problema</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1232">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="1dfd6-1233">Alteração do `feedback` para imprimir o corpo do problema ao executar com '--verbose'</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1233">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="1dfd6-1234">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1234">Monitor</span></span>
* <span data-ttu-id="1dfd6-1235">Correção de um problema em que “count” não era um valor permitido com `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1235">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="1dfd6-1236">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1236">Network</span></span>
* <span data-ttu-id="1dfd6-1237">Correção do formato de tabela que não estava sendo exibido com `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1237">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="1dfd6-1238">Adição dos comandos `list-request-headers` e `list-response-headers` para `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1238">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="1dfd6-1239">Adição do comando `list-server-variables` para `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1239">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="1dfd6-1240">Correção de um problema em que a atualização do estado do link em uma porta express-route geraria uma exceção de atributo desconhecido `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1240">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="1dfd6-1241">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1241">PrivateDNS</span></span>
* <span data-ttu-id="1dfd6-1242">Adição de `network private-dns` para zonas de DNS privado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1242">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-1243">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1243">Resource</span></span>
* <span data-ttu-id="1dfd6-1244">Correção do problema com `deployment create` e `group deployment create`, em que um arquivo de parâmetros com um conjunto vazio de parâmetros não funcionaria</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1244">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-1245">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1245">Role</span></span>
* <span data-ttu-id="1dfd6-1246">Correção de `create-for-rbac` para lidar corretamente com `--years`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1246">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="1dfd6-1247">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `role assignment delete` para solicitar ao excluir todas as atribuições na assinatura incondicionalmente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1247">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-1248">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1248">SQL</span></span>
* <span data-ttu-id="1dfd6-1249">Atualização de `sql mi [create|update]` com as propriedades proxyOverride e publicDataEndpointEnabled</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1249">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-1250">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1250">Storage</span></span>
* <span data-ttu-id="1dfd6-1251">[ALTERAÇÃO SIGNIFICATIVA] Remoção do resultado de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1251">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="1dfd6-1252">Adição de `--full-uri` a `storage blob generate-sas` para criar o URI completo para o blob com SAS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1252">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="1dfd6-1253">Adição de `--file-snapshot` a `storage file copy start` para copiar arquivo do instantâneo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1253">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="1dfd6-1254">Alteração de `storage blob copy cancel` para mostrar apenas o erro em vez da exceção para NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1254">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="1dfd6-1255">26 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1255">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="1dfd6-1256">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1256">Core</span></span>
* <span data-ttu-id="1dfd6-1257">Correção de problemas com incompatibilidade da extensão de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1257">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="1dfd6-1258">Agora o tratamento de erros encaminha os clientes para a página de problemas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1258">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="1dfd6-1259">Nuvem</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1259">Cloud</span></span>
* <span data-ttu-id="1dfd6-1260">Erro de “assinatura não encontrada” corrigido em `cloud set`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1260">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-1261">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1261">ACR</span></span>
* <span data-ttu-id="1dfd6-1262">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1262">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="1dfd6-1263">`--auth-mode` adicionado aos comandos `acr build`, `acr run`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1263">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="1dfd6-1264">Grupo de comandos “acr task credential” adicionado para gerenciar as credenciais de uma Tarefa</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1264">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="1dfd6-1265">“--no-wait” adicionado ao comando `acr build`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1265">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-1266">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1266">AppService</span></span>
* <span data-ttu-id="1dfd6-1267">Bug corrigido onde `webapp up` não estava lidando corretamente com a execução do diretório vazio ou do cenário de código desconhecido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1267">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="1dfd6-1268">Bug corrigido onde os slots não funcionavam para `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1268">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="1dfd6-1269">Serviço de BOT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1269">BOT Service</span></span>
* <span data-ttu-id="1dfd6-1270">`bot prepare-deploy` adicionado para se preparar para a implantação de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1270">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="1dfd6-1271">`bot create --kind registration` alterado para mostrar a senha se ela não for fornecida</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1271">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="1dfd6-1272">[ALTERAÇÃO SIGNIFICATIVA]`--endpoint` alterado em `bot create --kind registration` como padrão para uma cadeia de caracteres vazia, em vez de ser requerido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1272">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="1dfd6-1273">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1273">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="1dfd6-1274">CDN</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1274">CDN</span></span>
* <span data-ttu-id="1dfd6-1275">Adicionado o suporte ao `--no-wait` para `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1275">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [ALTERAÇÃO SIGNIFICATIVA]: `cdn endpoint create` alterado para o comportamento de cache da cadeia de consulta padrão.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="1dfd6-1277">Não há mais padrão para "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1277">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="1dfd6-1278">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1278">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1dfd6-1279">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1279">Cosmosdb</span></span>
* <span data-ttu-id="1dfd6-1280">Suporte adicionado para `--enable-multiple-write-locations` na atualização da conta</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1280">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="1dfd6-1281">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1281">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="1dfd6-1282">Interativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1282">Interactive</span></span>
* <span data-ttu-id="1dfd6-1283">Incompatibilidade corrigida com a extensão Interativa instalada por meio do azdev</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1283">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="1dfd6-1284">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1284">Monitor</span></span>
* <span data-ttu-id="1dfd6-1285">Alterado para permitir o valor de dimensão `*` para `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1285">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-1286">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1286">Network</span></span>
* <span data-ttu-id="1dfd6-1287">Grupo de comandos `rewrite-rule` adicionado em `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1287">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="1dfd6-1288">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1288">Profile</span></span>
* <span data-ttu-id="1dfd6-1289">Suporte de conta no nível do locatário para a identidade de serviço gerenciado adicionado em `login`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1289">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="1dfd6-1290">Postgres</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1290">Postgres</span></span> 
* <span data-ttu-id="1dfd6-1291">Adicionados os comandos postgresql `replica` e `restart server`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1291">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="1dfd6-1292">Alterado para obter o local padrão do grupo de recursos quando não fornecido para criar servidores e adicionar validação para os dias de retenção</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1292">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-1293">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1293">Resource</span></span>
* <span data-ttu-id="1dfd6-1294">Saída da tabela aperfeiçoada para `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1294">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="1dfd6-1295">Corrigido o problema com `deployment [create|validate]` onde o tipo secureObject não era reconhecido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1295">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="1dfd6-1296">Grafo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1296">Graph</span></span>
* <span data-ttu-id="1dfd6-1297">Adicionado o suporte ao `--end-date` para `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1297">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="1dfd6-1298">Suporte adicionado para acrescentar permissões com `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1298">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="1dfd6-1299">Bug corrigido com `ad app permission list` quando não havia nenhuma permissão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1299">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="1dfd6-1300">`ad sp delete` alterado para ignorar a exclusão da atribuição de função se a conta atual não tem nenhuma assinatura</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1300">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="1dfd6-1301">`ad app create` alterado para `--identifier-uris` passar para lista vazia como padrão se não fornecido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1301">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-1302">armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1302">storage</span></span>
* <span data-ttu-id="1dfd6-1303">`--snapshot` adicionado a `storage file download-batch` para baixar de um instantâneo de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1303">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="1dfd6-1304">Barra de progresso `storage blob [download-batch|upload-batch]` alterada para ser menos detalhada e indicar o blob atual</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1304">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="1dfd6-1305">Problema corrigido com `storage account update` ao atualizar os parâmetros de criptografia</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1305">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="1dfd6-1306">Problema corrigido onde `storage blob show` falharia ao usar o oauth (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1306">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-1307">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1307">VM</span></span>
* <span data-ttu-id="1dfd6-1308">Adicionado o comando `image update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1308">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="1dfd6-1309">12 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1309">March 12, 2019</span></span>

<span data-ttu-id="1dfd6-1310">Versão 2.0.60</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1310">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-1311">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1311">Core</span></span>

* <span data-ttu-id="1dfd6-1312">Foi corrigido um erro incorreto no `cloud set` sobre assinatura não encontrada.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1312">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-1313">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1313">ACR</span></span>

* <span data-ttu-id="1dfd6-1314">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1314">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-1315">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1315">ACS</span></span>

* <span data-ttu-id="1dfd6-1316">Alteração para ignorar o parâmetro `--listen-address` para `aks browse` se ele não for compatível com kubectl</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1316">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="1dfd6-1317">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1317">AppService</span></span>

* <span data-ttu-id="1dfd6-1318">Adicionado `[webapp|functionapp] deployment list-publishing-credentials` para obter a URL de publicação do Kudu e suas credenciais.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1318">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="1dfd6-1319">Removida a instrução de impressão errônea de `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1319">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="1dfd6-1320">Corrigido `functionapp` para definir a imagem correta do runtime nos planos do Serviço de Aplicativo no Linux.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1320">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="1dfd6-1321">Removida a marca de versão prévia do `webapp up` e adicionadas melhorias ao comando.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1321">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="1dfd6-1322">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1322">Botservice</span></span>

* <span data-ttu-id="1dfd6-1323">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1323">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="1dfd6-1324">Adicionados `Microsoft-BotFramework-AppId` e `Microsoft-BotFramework-AppPassword` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1324">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="1dfd6-1325">Removidas as aspas simples da saída de comando `bot publish`, no final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1325">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="1dfd6-1326">Alterado `bot publish` para que seja assíncrono.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1326">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="1dfd6-1327">Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1327">Container</span></span>

* <span data-ttu-id="1dfd6-1328">Adicionado o argumento `--no-wait` para `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1328">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="1dfd6-1329">EventHub</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1329">EventHub</span></span>

* <span data-ttu-id="1dfd6-1330">Adicionado o sinalizador `--skip-empty-archives` a `eventhub create|update` para dar suporte a arquivos vazios na captura.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1330">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="1dfd6-1331">Localizar</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1331">Find</span></span>

* <span data-ttu-id="1dfd6-1332">Atualização de funcionalidade principal</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1332">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1dfd6-1333">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1333">HDInsight</span></span>

* <span data-ttu-id="1dfd6-1334">Adicionado o parâmetro `--storage-account-managed-identity` a `hdinsight create` para oferecer suporte ao MSI do ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1334">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-1335">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1335">Network</span></span>

* <span data-ttu-id="1dfd6-1336">Corrigido o problema com `vpn-connection update`, onde a atualização de uma conexão VPN entre gateways em assinaturas diferentes falharia.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1336">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="1dfd6-1337">Rdbms</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1337">Rdbms</span></span>

* <span data-ttu-id="1dfd6-1338">Correções secundárias para obter a localização padrão do grupo de recursos, quando não fornecida, para criar servidores e adicionar validação nos dias de retenção.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1338">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-1339">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1339">Role</span></span>

* <span data-ttu-id="1dfd6-1340">Corrigido `role definition update` para usar ID a fim de resolver a definição corretamente.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1340">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="1dfd6-1341">Alterado `ad app credential reset` para remover a suposição de que a entidade de serviço do aplicativo já existe.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1341">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="1dfd6-1342">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1342">Service Fabric</span></span>

* <span data-ttu-id="1dfd6-1343">Corrigido o problema com o fato de `sf cluster list` não ser iterável.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1343">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="1dfd6-1344">26 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1344">February 26, 2019</span></span>

<span data-ttu-id="1dfd6-1345">Versão 2.0.59</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1345">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-1346">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1346">Core</span></span>

* <span data-ttu-id="1dfd6-1347">Corrigido o problema onde algumas instâncias usando `--subscription NAME` produziriam uma exceção</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1347">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-1348">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1348">ACR</span></span>

* <span data-ttu-id="1dfd6-1349">Parâmetro `--target` adicionado para os comandos `acr build`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1349">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="1dfd6-1350">Melhor tratamento de erros para os comandos de execução quando não conectado ao Azure</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1350">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-1351">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1351">ACS</span></span>

* <span data-ttu-id="1dfd6-1352">Opção `--listen-address` adicionada a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1352">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-1353">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1353">AppService</span></span>

* <span data-ttu-id="1dfd6-1354">Adicionado o comando `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1354">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="1dfd6-1355">Lote</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1355">Batch</span></span>
* <span data-ttu-id="1dfd6-1356">[ALTERAÇÃO SIGNIFICATIVA] Comando `batch pool upgrade os` removido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1356">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="1dfd6-1357">[ALTERAÇÃO SIGNIFICATIVA] Propriedade `Pacakges` removida das respostas `Application`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1357">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="1dfd6-1358">Comando `batch application package list` adicionado para listar os pacotes de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1358">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="1dfd6-1359">[ALTERAÇÃO SIGNIFICATIVA]`--application-id` alterado para `--application-name` em todos os comandos `batch application`,</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1359">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="1dfd6-1360">O argumento `--json-file` foi adicionado aos comandos para a solicitação de resposta da API bruta</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1360">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="1dfd6-1361">Validação atualizada para incluir automaticamente `https://` em todos os pontos de extremidade, se ausente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1361">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1dfd6-1362">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1362">CosmosDB</span></span>

* <span data-ttu-id="1dfd6-1363">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1363">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="1dfd6-1364">Kusto</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1364">Kusto</span></span>

* <span data-ttu-id="1dfd6-1365">[ALTERAÇÃO SIGNIFICATIVA] Os tipos `hot_cache_period` e `soft_delete_period` foram alterados do banco de dados para o formato de duração ISO8601</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1365">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-1366">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1366">Network</span></span>

* <span data-ttu-id="1dfd6-1367">Adicionado o argumento `--express-route-gateway-bypass` para `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1367">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="1dfd6-1368">Foram adicionados os grupos de comando a partir das extensões `express-route`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1368">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="1dfd6-1369">Os grupos de comando `express-route gateway` e `express-route port` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1369">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="1dfd6-1370">Adicionado o argumento `--legacy-mode` para `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1370">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="1dfd6-1371">Os argumentos `--allow-classic-operations` e `--express-route-port` foram adicionados a `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1371">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="1dfd6-1372">Adicionado o argumento `--gateway-default-site` para `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1372">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="1dfd6-1373">Os comandos `ipsec-policy` foram adicionados a `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1373">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-1374">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1374">Resource</span></span>

* <span data-ttu-id="1dfd6-1375">Foi corrigido o problema com `deployment create` em que o campo do tipo diferencia letras maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1375">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="1dfd6-1376">Foi adicionado o suporte para arquivo de parâmetros de URI a `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1376">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="1dfd6-1377">Foi adicionado o suporte para parâmetros de URI e definições a `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1377">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="1dfd6-1378">Foi corrigido o tratamento de parâmetros e regras para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1378">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="1dfd6-1379">Foi corrigido o problema com `resource show/update/delete/tag/invoke-action` em que as IDs de assinatura cruzada não respeitaram corretamente a ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1379">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-1380">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1380">Role</span></span>

* <span data-ttu-id="1dfd6-1381">Foi adicionado o suporte para as funções do aplicativo a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1381">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-1382">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1382">VM</span></span>

* <span data-ttu-id="1dfd6-1383">Foi corrigido o problema com `vm create where ` – a rede acelerada não foi habilitada por padrão no Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1383">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="1dfd6-1384">12 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1384">February 12, 2019</span></span>

<span data-ttu-id="1dfd6-1385">Versão 2.0.58</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1385">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-1386">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1386">Core</span></span>

* <span data-ttu-id="1dfd6-1387">`az --version` agora exibe uma notificação se você tiver pacotes para atualização</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1387">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="1dfd6-1388">A regressão em que `--ids` não pode ser usado com a saída JSON foi corrigida</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1388">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-1389">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1389">ACR</span></span>
* <span data-ttu-id="1dfd6-1390">[ALTERAÇÃO SIGNIFICATIVA] O grupo de comandos `acr build-task` foi removido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1390">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="1dfd6-1391">[ALTERAÇÃO SIGNIFICATIVA] As opções `--tag` e `--manifest` de `acr repository delete` foram removidas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1391">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-1392">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1392">ACS</span></span>
* <span data-ttu-id="1dfd6-1393">Suporte adicionado a `aks [enable-addons|disable-addons]` para nomes que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1393">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="1dfd6-1394">Suporte adicionado para a operação de atualização do Azure Active Directory usando `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1394">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="1dfd6-1395">Um esclarecimento informando que `--output` é ignorado para `aks get-credentials` foi adicionado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1395">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="1dfd6-1396">AMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1396">AMS</span></span>
* <span data-ttu-id="1dfd6-1397">Adicionados os comandos `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1397">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="1dfd6-1398">Adicionados os comandos `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1398">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-1399">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1399">Appservice</span></span>
* <span data-ttu-id="1dfd6-1400">Foi adicionada a capacidade de criar e configurar funções usando contêineres de ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1400">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="1dfd6-1401">Suporte adicionado para a atualização das configurações de aplicativos Web por meio de JSON</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1401">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="1dfd6-1402">A ajuda foi aprimorada para `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1402">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="1dfd6-1403">Suporte adicionado para o App Insights para auxiliar na criação de aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1403">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="1dfd6-1404">Os problemas com o SSH do aplicativo Web foram corrigidos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1404">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="1dfd6-1405">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1405">Botservice</span></span>
* <span data-ttu-id="1dfd6-1406">A experiência do usuário para `bot publish` foi aprimorada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1406">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="1dfd6-1407">Foram adicionados avisos de tempos limite ao executar `npm install` durante `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1407">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="1dfd6-1408">O caractere inválido `.` de `--name` em `az bot create` foi removido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1408">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="1dfd6-1409">Alteração para interromper a geração aleatória de nomes de recursos durante a criação do Armazenamento do Azure, Plano do Serviço de Aplicativo, Aplicativo Web/de funções e Application Insights</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1409">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="1dfd6-1410">[PRETERIDO] O argumento `--proj-name` foi preterido em favor de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1410">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="1dfd6-1411">`az bot publish` foi alterado para remover arquivos de implantação do Node.js do IIS buscados, caso eles já não existissem</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1411">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="1dfd6-1412">Foi adicionado o argumento `--keep-node-modules` para `az bot publish` para não excluir a pasta `node_modules` no Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1412">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="1dfd6-1413">O par chave-valor `"publishCommand"` foi adicionado à saída de `az bot create` durante a criação de uma função do Azure ou bot de aplicativo Web</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1413">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="1dfd6-1414">O valor de `"publishCommand"` é um comando `az bot publish` que é automaticamente preenchido com os parâmetros necessários para publicar o bot recém-criado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1414">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="1dfd6-1415">O `"WEBSITE_NODE_DEFAULT_VERSION"` foi atualizado no modelo do ARM para que os bots de SDK v4 usem 10.14.1 em vez de 8.9.4</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1415">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="1dfd6-1416">Key Vault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1416">Key Vault</span></span>
* <span data-ttu-id="1dfd6-1417">Foi corrigido o problema com `keyvault secret backup`, em que alguns usuários recebiam um erro `unexpected_keyword` ao usar `--id`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1417">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="1dfd6-1418">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1418">Monitor</span></span>
* <span data-ttu-id="1dfd6-1419">`monitor metrics alert [create|update]` foi alterado para permitir o valor dimensional `*`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1419">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-1420">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1420">Network</span></span>
* <span data-ttu-id="1dfd6-1421">`dns zone export` foi alterado para garantir que CNAMEs exportados fossem FQDNs</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1421">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="1dfd6-1422">O parâmetro `--gateway-name` foi adicionado a `nic ip-config address-pool [add|remove]` para dar suporte a pools de endereços de back-end de gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1422">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="1dfd6-1423">Os argumentos `--traffic-analytics` e `--workspace` foram adicionados a `network watcher flow-log configure` para dar suporte à análise de tráfego por meio de um espaço de trabalho do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1423">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="1dfd6-1424">`--idle-timeout` e `--floating-ip` foram adicionados a `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1424">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="1dfd6-1425">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1425">Policy Insights</span></span>
* <span data-ttu-id="1dfd6-1426">Os comandos `policy remediation` foram adicionados para dar suporte a recursos de correção de política de recursos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1426">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="1dfd6-1427">RDBMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1427">RDBMS</span></span>
* <span data-ttu-id="1dfd6-1428">A mensagem e os parâmetros de comando de ajuda foram aprimorados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1428">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="1dfd6-1429">Redis</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1429">Redis</span></span>
* <span data-ttu-id="1dfd6-1430">Foram adicionados comandos para gerenciar regras de firewall (criar, atualizar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1430">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="1dfd6-1431">Foram adicionados comandos para gerenciar links do servidor (criar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1431">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="1dfd6-1432">Foram adicionados comandos para gerenciar o agendamento de patches (criar, atualizar, excluir, mostrar)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1432">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="1dfd6-1433">Suporte adicionado para Zonas de Disponibilidade e versão mínima de TLS para criar Redis</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1433">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="1dfd6-1434">[ALTERAÇÃO SIGNIFICATIVA] Os comandos `redis update-settings` e `redis list-all` foram removidos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1434">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="1dfd6-1435">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro para `redis create`: “configurações de locatário” não é aceito no formato chave[=valor]</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1435">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="1dfd6-1436">[PRETERIDO] Uma mensagem de aviso foi adicionada para preterir o comando `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1436">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-1437">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1437">Role</span></span>
* <span data-ttu-id="1dfd6-1438">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido dos comandos `vm` para esta localização</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1438">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="1dfd6-1439">SQL VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1439">SQL VM</span></span>
* <span data-ttu-id="1dfd6-1440">[PRETERIDO] O argumento `--boostrap-acc-pwd` foi preterido devido a um erro de digitação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1440">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-1441">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1441">VM</span></span>
* <span data-ttu-id="1dfd6-1442">`vm list-skus` foi alterado para permitir o uso de `--all` no lugar de `--all true`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1442">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="1dfd6-1443">Adicionado `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1443">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="1dfd6-1444">Foi corrigido o bug em que `vmss encryption enable` falhava se fosse executado anteriormente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1444">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="1dfd6-1445">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido para os comandos `role`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1445">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="1dfd6-1446">31 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1446">January 31, 2019</span></span>

<span data-ttu-id="1dfd6-1447">Versão 2.0.57</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1447">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-1448">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1448">Core</span></span>

* <span data-ttu-id="1dfd6-1449">Hotfix para o [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1449">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="1dfd6-1450">28 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1450">January 28, 2019</span></span>

<span data-ttu-id="1dfd6-1451">Versão 2.0.56</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1451">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-1452">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1452">ACR</span></span>
* <span data-ttu-id="1dfd6-1453">Suporte adicionado para regras de rede virtual/IP</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1453">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-1454">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1454">ACS</span></span>
* <span data-ttu-id="1dfd6-1455">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1455">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="1dfd6-1456">Comandos do OpenShift gerenciado foram adicionados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1456">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="1dfd6-1457">Suporte adicionado para operações de atualização da entidade de serviço com `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1457">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="1dfd6-1458">AMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1458">AMS</span></span>
* <span data-ttu-id="1dfd6-1459">[ALTERAÇÃO SIGNIFICATIVA]`ams asset get-streaming-locators` renomeado para `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1459">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="1dfd6-1460">[ALTERAÇÃO SIGNIFICATIVA]`ams streaming-locator get-content-keys` renomeado para `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1460">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-1461">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1461">Appservice</span></span>
* <span data-ttu-id="1dfd6-1462">Suporte adicionado para o App Insights no `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1462">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="1dfd6-1463">Suporte adicionado para a criação do plano de serviço de aplicativo (incluindo Elástico Premium) para Aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1463">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="1dfd6-1464">Foram corrigidos os problemas com de configuração de aplicativo com os planos Elástico Premium</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1464">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="1dfd6-1465">Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1465">Container</span></span>
* <span data-ttu-id="1dfd6-1466">Adicionado o comando `container start`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1466">Added `container start` command</span></span>
* <span data-ttu-id="1dfd6-1467">Alteração para permitir o uso de valores decimais para CPU durante a criação do contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1467">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="1dfd6-1468">EventGrid</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1468">EventGrid</span></span>
* <span data-ttu-id="1dfd6-1469">Parâmetro `--deadletter-endpoint` adicionado a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1469">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="1dfd6-1470">Storagequeue e hybridconnection foram adicionados como novos valores para 'event-subscription [create|update] --endpoint-type\`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1470">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="1dfd6-1471">Os parâmetros `--max-delivery-attempts` e `--event-ttl` foram adicionados a `event-subscription create` para especificar a política de repetição para eventos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1471">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="1dfd6-1472">Uma mensagem de aviso foi adicionada a `event-subscription [create|update]` quando o webhook como destino for usado para uma assinatura de evento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1472">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="1dfd6-1473">O parâmetro source-resource-id foi adicionado para todos os comandos relacionados a eventos e marcar todos os outros parâmetros relacionados ao recurso de origem como preteridos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1473">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1dfd6-1474">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1474">HDInsight</span></span>
* <span data-ttu-id="1dfd6-1475">[ALTERAÇÃO SIGNIFICATIVA] Os parâmetros `--virtual-network` e `--subnet-name` de `hdinsight [application] create` foram removidos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1475">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="1dfd6-1476">[ALTERAÇÃO SIGNIFICATIVA]`hdinsight create --storage-account` foi alterado para aceitar o nome ou ID da conta de armazenamento, em vez de pontos de extremidade de blob</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1476">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="1dfd6-1477">Parâmetros `--vnet-name` e `--subnet-name` adicionados a `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1477">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="1dfd6-1478">Suporte adicionado para a criptografia de disco e Enterprise Security Package ao `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1478">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="1dfd6-1479">Adicionado o comando `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1479">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="1dfd6-1480">Adicionado o comando `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1480">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="1dfd6-1481">IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1481">IoT</span></span>
* <span data-ttu-id="1dfd6-1482">O formato de codificação foi adicionado ao comando routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1482">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="1dfd6-1483">Kusto</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1483">Kusto</span></span>
* <span data-ttu-id="1dfd6-1484">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1484">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="1dfd6-1485">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1485">Monitor</span></span>
* <span data-ttu-id="1dfd6-1486">A comparação de ID foi alterada para diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1486">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="1dfd6-1487">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1487">Profile</span></span>
* <span data-ttu-id="1dfd6-1488">A conta de nível de locatário foi habilitada para a identidade de serviço gerenciada de `login`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1488">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-1489">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1489">Network</span></span>
* <span data-ttu-id="1dfd6-1490">Foi corrigido o problema com `express-route update`: em que o argumento `--bandwidth` era ignorado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1490">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="1dfd6-1491">Foi corrigido o problema com `ddos-protection update` em que definir a compreensão levava ao rastreamento de pilha</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1491">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-1492">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1492">Resource</span></span>
* <span data-ttu-id="1dfd6-1493">Suporte adicionado para o arquivo de parâmetros de URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1493">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="1dfd6-1494">Suporte adicionado para a identidade gerenciada à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1494">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="1dfd6-1495">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1495">SQL Virtual Machine</span></span>
* <span data-ttu-id="1dfd6-1496">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1496">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-1497">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1497">Storage</span></span>
* <span data-ttu-id="1dfd6-1498">Alteração na correção para atualizar apenas as propriedades que são alteradas no mesmo objeto</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1498">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="1dfd6-1499">#8021 foi corrigido, dados binários são codificados em base 64 quando retornados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1499">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-1500">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1500">VM</span></span>
* <span data-ttu-id="1dfd6-1501">Alteração de `vm encryption enable` para validar o cofre de chaves de criptografia de disco e se esse cofre de chaves de criptografia de chave existe</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1501">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="1dfd6-1502">O sinalizador `--force` foi adicionado a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1502">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="1dfd6-1503">15 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1503">January 15, 2019</span></span>

<span data-ttu-id="1dfd6-1504">Versão 2.0.55</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1504">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-1505">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1505">ACR</span></span>
* <span data-ttu-id="1dfd6-1506">Alteração para permitir forçar o envio por push de um gráfico Helm que não existe</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1506">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="1dfd6-1507">Alteração para permitir operações de runtime sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1507">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="1dfd6-1508">[PRETERIDO] O parâmetro `--resource-group` foi preterido nos comandos:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1508">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="1dfd6-1509">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1509">ACS</span></span>
* <span data-ttu-id="1dfd6-1510">Suporte adicionado para novas regiões ACI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1510">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-1511">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1511">Appservice</span></span>
* <span data-ttu-id="1dfd6-1512">Foi corrigido o problema com o carregamento de certificados para aplicativos que são hospedados em um ASE, em que o RG do ASE e o RG do aplicativo são diferentes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1512">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="1dfd6-1513">Alteração de `webapp up` para usar a SKU P1V1 como padrão para Linux</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1513">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="1dfd6-1514">`[webapp|functionapp] deployment source config-zip` foi corrigido para mostrar a mensagem de erro adequada quando uma implantação falhar</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1514">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="1dfd6-1515">Adicionado o comando `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1515">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="1dfd6-1516">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1516">Botservice</span></span>
* <span data-ttu-id="1dfd6-1517">Atualizações de status de implantação foram adicionadas a `bot create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1517">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="1dfd6-1518">Configurar</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1518">Configure</span></span>
* <span data-ttu-id="1dfd6-1519">`none` foi adicionado como um formato de saída configurável</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1519">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1dfd6-1520">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1520">CosmosDB</span></span>
* <span data-ttu-id="1dfd6-1521">Suporte adicionado para criar o banco de dados com taxa de transferência compartilhada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1521">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1dfd6-1522">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1522">HDInsight</span></span>
* <span data-ttu-id="1dfd6-1523">Foram adicionados comandos para o gerenciamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1523">Added commands for managing applications</span></span>
* <span data-ttu-id="1dfd6-1524">Foram adicionados comandos para o gerenciamento de ações de script</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1524">Added commands for managing script actions</span></span>
* <span data-ttu-id="1dfd6-1525">Foram adicionados comandos para o gerenciamento do Operations Management Suite (OMS)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1525">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="1dfd6-1526">Suporte adicionado para listar a utilização regional ao `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1526">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="1dfd6-1527">[ALTERAÇÃO SIGNIFICATIVA] O tipo de cluster padrão de `hdinsight create` foi removido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1527">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-1528">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1528">Network</span></span>
* <span data-ttu-id="1dfd6-1529">Adicionados os argumentos `--custom-headers` e `--status-code-ranges` para `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1529">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="1dfd6-1530">Novos tipos de roteamento foram adicionados: Subrede e múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1530">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="1dfd6-1531">Adicionados os argumentos `--custom-headers` e `--subnets` para `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1531">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="1dfd6-1532">Foi corrigido o problema no qual fornecer `--vnets ""` a `ddos-protection update` causava um erro</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1532">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-1533">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1533">Role</span></span>
* <span data-ttu-id="1dfd6-1534">[PRETERIDO] O argumento `--password` foi preterido para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1534">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="1dfd6-1535">Como alternativa, use senhas seguras geradas pela CLI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1535">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="1dfd6-1536">Segurança</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1536">Security</span></span>
* <span data-ttu-id="1dfd6-1537">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1537">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-1538">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1538">Storage</span></span>
* <span data-ttu-id="1dfd6-1539">[ALTERAÇÃO SIGNIFICATIVA] O número padrão de resultados de `storage [blob|file|container|share] list` foi alterado para 5.000.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1539">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="1dfd6-1540">Use `--num-results *` para o comportamento original de retornar todos os resultados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1540">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="1dfd6-1541">Parâmetro `--marker` adicionado a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1541">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="1dfd6-1542">Um marcador de log foi adicionado para a próxima página ao STDERR de `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1542">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="1dfd6-1543">O comando `storage blob service-properties update` foi adicionado com suporte para sites estáticos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1543">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-1544">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1544">VM</span></span>
* <span data-ttu-id="1dfd6-1545">`vm [disk|unmanaged-disk]` e `vmss disk` foram alterados para que tenham parâmetros mais consistentes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1545">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="1dfd6-1546">Suporte adicionado para referência cruzada de imagem de locatário a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1546">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="1dfd6-1547">O bug de configuração padrão foi corrigido em `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1547">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="1dfd6-1548">O argumento `--provision-after-extensions` foi adicionado a `vmss extension set` para definir quais extensões deverão ser provisionadas antes da extensão ser definida</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1548">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="1dfd6-1549">O argumento `--replica-count` foi adicionado a `sig image-version update` para definir a contagem de replicação padrão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1549">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="1dfd6-1550">Foi corrigido o bug com `image create --source` em que o disco do sistema operacional de origem era confundido com uma VM do mesmo nome, mesmo se a ID de recurso completa fosse fornecida</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1550">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="1dfd6-1551">20 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1551">December 20, 2018</span></span>

<span data-ttu-id="1dfd6-1552">Versão 2.0.54</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1552">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="1dfd6-1553">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1553">Appservice</span></span>
* <span data-ttu-id="1dfd6-1554">Corrigido o problema que causava falha na reimplantação do `webapp up`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1554">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="1dfd6-1555">Adicionado suporte para listar e restaurar instantâneos de aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1555">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="1dfd6-1556">Adicionado suporte para o sinalizador `--runtime` para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1556">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="1dfd6-1557">IoT Central</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1557">IoTCentral</span></span>
* <span data-ttu-id="1dfd6-1558">Corrigida a chamada à API do comando de atualização</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1558">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-1559">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1559">Role</span></span>
* <span data-ttu-id="1dfd6-1560">[ALTERAÇÃO SIGNIFICATIVA]`ad [app|sp] list` alterado para listar somente os 100 primeiros objetos por padrão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1560">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-1561">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1561">SQL</span></span>
* <span data-ttu-id="1dfd6-1562">Adicionado suporte para ordenação personalizada nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1562">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-1563">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1563">VM</span></span>
* <span data-ttu-id="1dfd6-1564">Parâmetro `---os-type` adicionado a `disk create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1564">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="1dfd6-1565">18 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1565">December 18, 2018</span></span>

<span data-ttu-id="1dfd6-1566">Versão 2.0.53</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1566">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="1dfd6-1567">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1567">ACR</span></span>
* <span data-ttu-id="1dfd6-1568">Adicionado suporte para importação de imagem de Registros de Contêiner externos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1568">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="1dfd6-1569">Simplificado o layout da tabela para a lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1569">Condensed the table layout for task list</span></span>
* <span data-ttu-id="1dfd6-1570">Adicionado suporte para URLs do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1570">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-1571">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1571">ACS</span></span>
* <span data-ttu-id="1dfd6-1572">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1572">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="1dfd6-1573">Removido “(VISUALIZAÇÃO)” de argumentos do AAD para `aks create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1573">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="1dfd6-1574">[PRETERIDO] Comandos `az acs` preteridos.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1574">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="1dfd6-1575">O serviço ACS será desativado em 31 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1575">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="1dfd6-1576">Adicionado suporte da Política de Rede durante a criação de novos clusters AKS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1576">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="1dfd6-1577">Removido o requisito do argumento `--nodepool-name` para `aks scale` se houver apenas um pool de nós</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1577">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-1578">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1578">Appservice</span></span>
* <span data-ttu-id="1dfd6-1579">Corrigido o problema em que `webapp config container` não honra o parâmetro `--slot`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1579">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="1dfd6-1580">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1580">Botservice</span></span>
* <span data-ttu-id="1dfd6-1581">Suporte adicionado para análise do arquivo `.bot` ao chamar `bot show`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1581">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="1dfd6-1582">Corrigido o bug de provisionamento do AppInsights</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1582">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="1dfd6-1583">Corrigido o bug de espaço em branco ao lidar com caminhos de arquivo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1583">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="1dfd6-1584">Reduzidas as chamadas de rede do Kudu</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1584">Reduced Kudu network calls</span></span>
* <span data-ttu-id="1dfd6-1585">Melhorias de UX para comandos gerais</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1585">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="1dfd6-1586">Consumo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1586">Consumption</span></span>
* <span data-ttu-id="1dfd6-1587">Corrigidos os bugs da API de orçamento ao mostrar notificações</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1587">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1dfd6-1588">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1588">CosmosDB</span></span>
* <span data-ttu-id="1dfd6-1589">Suporte adicionado para atualizar a conta de vários mestres para mestre único</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1589">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="1dfd6-1590">Mapas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1590">Maps</span></span>
* <span data-ttu-id="1dfd6-1591">Adicionado suporte ao SKU S1 para `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1591">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-1592">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1592">Network</span></span>
* <span data-ttu-id="1dfd6-1593">Adicionado suporte para `--format` e `--log-version` para `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1593">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="1dfd6-1594">Corrigido o problema com `dns zone update` em que usar "" para limpar a resolução e o registro de redes virtuais não funcionava</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1594">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-1595">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1595">Resource</span></span>
* <span data-ttu-id="1dfd6-1596">Corrigido o tratamento do parâmetro de escopo para grupos de gerenciamento do `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1596">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="1dfd6-1597">Adicionado o novo comando `resource wait`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1597">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-1598">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1598">Storage</span></span>
*  <span data-ttu-id="1dfd6-1599">Adicionada a capacidade de atualizar a versão do esquema de log para serviços de armazenamento no `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1599">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-1600">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1600">VM</span></span>
* <span data-ttu-id="1dfd6-1601">Corrigida a falha em `vm identity remove` quando a VM especificada não tem nenhuma identidade de serviço gerenciado atribuída</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1601">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="1dfd6-1602">4 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1602">December 4, 2018</span></span>

<span data-ttu-id="1dfd6-1603">Versão 2.0.52</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1603">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="1dfd6-1604">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1604">Core</span></span>
* <span data-ttu-id="1dfd6-1605">Adicionado suporte para provisionamento de recursos de locatários cruzados para a entidade de serviço de multilocatários</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1605">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="1dfd6-1606">Corrigido o bug onde as ids enviadas por pipe de um comando com a saída tsv eram analisados incorretamente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1606">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-1607">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1607">Appservice</span></span>
* <span data-ttu-id="1dfd6-1608">[VERSÃO PRÉVIA] Adicionado o comando `webapp up` que ajuda a criar e implantar conteúdo em aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1608">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="1dfd6-1609">Corrigido um bug no aplicativo com base em contêiner do Windows devido à alteração de back-end</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1609">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-1610">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1610">Network</span></span>
* <span data-ttu-id="1dfd6-1611">Adicionado o argumento `--exclusion` a `application-gateway waf-config set` para dar suporte a exclusões de WAF</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1611">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-1612">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1612">Role</span></span>
* <span data-ttu-id="1dfd6-1613">Adicionado suporte para identificadores personalizados para a credencial de senha</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1613">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="1dfd6-1614">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1614">VM</span></span>
* <span data-ttu-id="1dfd6-1615">[PRETERIDO] Parâmetro `vm extension [show|wait] --expand` preterido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1615">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="1dfd6-1616">Adicionado parâmetro `--force` a `vm restart` para reimplantar as VMs sem resposta</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1616">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="1dfd6-1617">Alterado `[vm|vmss] create --authentication-type` para aceitar "todos" para criar uma VM com senha e autenticação SSH</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1617">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="1dfd6-1618">Adicionado parâmetro `image create --os-disk-caching` para definir o cache de disco do sistema operacional para uma imagem</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1618">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="1dfd6-1619">20 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1619">November 20, 2018</span></span>

<span data-ttu-id="1dfd6-1620">Versão 2.0.51</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1620">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="1dfd6-1621">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1621">Core</span></span>
* <span data-ttu-id="1dfd6-1622">Logon do MSI alterado para não reutilizar o nome da assinatura na identidade</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1622">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-1623">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1623">ACR</span></span>
* <span data-ttu-id="1dfd6-1624">Token de contexto adicionado à etapa da tarefa</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1624">Added context token to task step</span></span>
* <span data-ttu-id="1dfd6-1625">Suporte adicionado para definir segredos na execução do acr para espelhar a tarefa do acr</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1625">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="1dfd6-1626">Suporte aprimorado para `--top` e `--orderby` para os comandos `show-tags` e `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1626">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-1627">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1627">Appservice</span></span>
* <span data-ttu-id="1dfd6-1628">Tempo limite padrão para a implantação do zip alterado para sondar o status aumentado para 5 minutos, também adicionando uma propriedade de tempo limite para personalizar esse valor</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1628">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="1dfd6-1629">Padrão `node_version` atualizado.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1629">Updated the default `node_version`.</span></span> <span data-ttu-id="1dfd6-1630">Redefinir a ação de troca de slots durante uma troca de duas fases preserva todas as configurações do aplicativo e cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1630">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="1dfd6-1631">Verificação da SKU no lado do cliente removida para o Linux criar o plano do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1631">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="1dfd6-1632">Erro corrigido ao tentar obter o status de implantação do zip</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1632">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="1dfd6-1633">Iot Central</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1633">IotCentral</span></span>
* <span data-ttu-id="1dfd6-1634">Verificação de disponibilidade do subdomínio adicionada ao criar um aplicativo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1634">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="1dfd6-1635">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1635">KeyVault</span></span>
* <span data-ttu-id="1dfd6-1636">Bug corrigido em que os erros podem ter sido ignorados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1636">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-1637">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1637">Network</span></span>
* <span data-ttu-id="1dfd6-1638">Subcomandos `root-cert` adicionados a `application-gateway` para lidar com os certificados de raiz confiável</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1638">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="1dfd6-1639">Opções `--min-capacity` e `--custom-error-pages` adicionadas a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1639">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="1dfd6-1640">`--zones` adicionado para suporte da zona de disponibilidade a `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1640">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="1dfd6-1641">Argumentos `--file-upload-limit`, `--max-request-body-size` e `--request-body-check` a `application-gateway waf-config set` adicionados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1641">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="1dfd6-1642">Rdbms</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1642">Rdbms</span></span>
* <span data-ttu-id="1dfd6-1643">Comandos vnet do mariadb adicionados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1643">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="1dfd6-1644">Rbac</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1644">Rbac</span></span>
* <span data-ttu-id="1dfd6-1645">Um problema corrigido ao tentar atualizar credenciais inalteradas em `ad app update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1645">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="1dfd6-1646">Avisos de saída adicionados para comunicar alterações de falha em um futuro próximo para `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1646">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="1dfd6-1647">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1647">Storage</span></span>
* <span data-ttu-id="1dfd6-1648">Melhor manipulação de casos incomuns para os comandos da cópia de armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1648">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="1dfd6-1649">Corrigido o problema em que `storage blob copy start-batch` não usava credenciais de logon quando as contas de origem e destino eram iguais</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1649">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="1dfd6-1650">Bug corrigido com `storage [blob|file] url` em que `sas_token` não foi incorporado na URL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1650">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="1dfd6-1651">Aviso de alteração da falha adicionado a `[blob|container] list`: produzirá apenas os primeiros 5.000 resultados por padrão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1651">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-1652">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1652">VM</span></span>
* <span data-ttu-id="1dfd6-1653">Suporte adicionado a `[vm|vmss] create --storage-sku` para especificar a SKU da conta de armazenamento para o SO gerenciado e os discos de dados separadamente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1653">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="1dfd6-1654">Parâmetros do nome da versão alterados de `sig image-version` para `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1654">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="1dfd6-1655">Argumento `sig image-version` preterido `--image-version-name`, substituído por `--image-version`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1655">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="1dfd6-1656">Suporte adicionado para usar o disco local do SO a `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1656">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="1dfd6-1657">Adicionado o suporte ao `--no-wait` para `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1657">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="1dfd6-1658">Adicionado o comando `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1658">Added `snapshot wait` command</span></span>
* <span data-ttu-id="1dfd6-1659">Suporte adicionado para usar o nome da instância com `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1659">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="1dfd6-1660">6 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1660">November 6, 2018</span></span>

<span data-ttu-id="1dfd6-1661">Versão 2.0.50</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1661">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-1662">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1662">Core</span></span>
* <span data-ttu-id="1dfd6-1663">Foi adicionado suporte para o serviço principal sn + autenticação do emissor</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1663">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-1664">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1664">ACR</span></span>
* <span data-ttu-id="1dfd6-1665">Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1665">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="1dfd6-1666">Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1666">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-1667">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1667">ACS</span></span>
* <span data-ttu-id="1dfd6-1668">[ALTERAÇÃO SIGNIFICATIVA]`enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1668">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="1dfd6-1669">Supervisor</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1669">Advisor</span></span>
* <span data-ttu-id="1dfd6-1670">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1670">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="1dfd6-1671">AMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1671">AMS</span></span>
* <span data-ttu-id="1dfd6-1672">Novos grupos de comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1672">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="1dfd6-1673">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1673">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="1dfd6-1674">Adicionados parâmetros de criptografia com suporte para `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1674">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="1dfd6-1675">O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1675">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="1dfd6-1676">Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1676">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="1dfd6-1677">Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1677">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="1dfd6-1678">Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1678">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="1dfd6-1679">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming locator` foi substituído por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1679">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="1dfd6-1680">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--content-keys` de `ams streaming locator` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1680">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="1dfd6-1681">[ALTERAÇÃO SIGNIFICATIVA]`--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1681">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="1dfd6-1682">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming policy` foi substituído por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1682">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="1dfd6-1683">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1683">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="1dfd6-1684">Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1684">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="1dfd6-1685">Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1685">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="1dfd6-1686">[ALTERAÇÃO SIGNIFICATIVA]`--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1686">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="1dfd6-1687">Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1687">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="1dfd6-1688">Um ativo sem rótulo pode ser enviado assim: 'assetName='</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1688">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-1689">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1689">AppService</span></span>
* <span data-ttu-id="1dfd6-1690">Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1690">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="1dfd6-1691">Configurar</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1691">Configure</span></span>
* <span data-ttu-id="1dfd6-1692">O YAML foi adicionado às opções de formato de saída</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1692">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="1dfd6-1693">Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1693">Container</span></span>
* <span data-ttu-id="1dfd6-1694">Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1694">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="1dfd6-1695">EventHub</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1695">EventHub</span></span>
* <span data-ttu-id="1dfd6-1696">O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1696">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="1dfd6-1697">Interativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1697">Interactive</span></span>
* <span data-ttu-id="1dfd6-1698">O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1698">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="1dfd6-1699">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1699">Monitor</span></span>
* <span data-ttu-id="1dfd6-1700">Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) para `--condition` em `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1700">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-1701">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1701">Network</span></span>
* <span data-ttu-id="1dfd6-1702">Os nomes de comandos `network interface-endpoint` foram preteridos em benefício de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1702">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="1dfd6-1703">Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1703">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="1dfd6-1704">Foi corrigido um problema onde `--ip-tags` não funcionava corretamente com `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1704">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="1dfd6-1705">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1705">Profile</span></span>
* <span data-ttu-id="1dfd6-1706">`--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1706">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="1dfd6-1707">RDBMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1707">RDBMS</span></span>
* <span data-ttu-id="1dfd6-1708">Adicionados comandos da réplica mysql</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1708">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-1709">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1709">Resource</span></span>
* <span data-ttu-id="1dfd6-1710">Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1710">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-1711">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1711">Role</span></span>
* <span data-ttu-id="1dfd6-1712">Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1712">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="1dfd6-1713">`ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1713">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="1dfd6-1714">Suporte adicionado para conceder permissões a aplicativos do AAD</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1714">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-1715">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1715">Storage</span></span>
* <span data-ttu-id="1dfd6-1716">Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1716">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-1717">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1717">VM</span></span>
* <span data-ttu-id="1dfd6-1718">O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1718">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="1dfd6-1719">O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1719">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="1dfd6-1720">O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1720">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="1dfd6-1721">`vm secret format` foi alterado para exigir a saída json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1721">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="1dfd6-1722">Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1722">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="1dfd6-1723">Validação de argumento aprimorado para `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1723">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="1dfd6-1724">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1724">October 23, 2018</span></span>

<span data-ttu-id="1dfd6-1725">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1725">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-1726">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1726">Core</span></span>
* <span data-ttu-id="1dfd6-1727">Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1727">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="1dfd6-1728">Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1728">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-1729">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1729">ACR</span></span>
* <span data-ttu-id="1dfd6-1730">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1730">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="1dfd6-1731">CDN</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1731">CDN</span></span>
* <span data-ttu-id="1dfd6-1732">[ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1732">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="1dfd6-1733">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1733">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="1dfd6-1734">Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1734">Container</span></span>
* <span data-ttu-id="1dfd6-1735">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1735">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="1dfd6-1736">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1736">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="1dfd6-1737">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1737">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="1dfd6-1738">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1738">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="1dfd6-1739">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1739">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="1dfd6-1740">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1740">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="1dfd6-1741">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1741">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1dfd6-1742">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1742">CosmosDB</span></span>
* <span data-ttu-id="1dfd6-1743">Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1743">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="1dfd6-1744">Interativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1744">Interactive</span></span>
* <span data-ttu-id="1dfd6-1745">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1745">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="1dfd6-1746">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1746">IoT Central</span></span>
* <span data-ttu-id="1dfd6-1747">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1747">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="1dfd6-1748">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1748">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="1dfd6-1749">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1749">Monitor</span></span>
* <span data-ttu-id="1dfd6-1750">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1750">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="1dfd6-1751">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1751">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="1dfd6-1752">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1752">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="1dfd6-1753">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1753">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="1dfd6-1754">Adicionado `--namespace` como alias para a opção preterida `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1754">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="1dfd6-1755">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1755">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="1dfd6-1756">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1756">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="1dfd6-1757">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1757">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="1dfd6-1758">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1758">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="1dfd6-1759">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1759">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-1760">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1760">Network</span></span>
* <span data-ttu-id="1dfd6-1761">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1761">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="1dfd6-1762">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1762">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="1dfd6-1763">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1763">ServiceBus</span></span>
* <span data-ttu-id="1dfd6-1764">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1764">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-1765">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1765">SQL</span></span>
* <span data-ttu-id="1dfd6-1766">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1766">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-1767">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1767">Storage</span></span>
* <span data-ttu-id="1dfd6-1768">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1768">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="1dfd6-1769">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1769">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-1770">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1770">VM</span></span>
* <span data-ttu-id="1dfd6-1771">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1771">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="1dfd6-1772">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1772">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="1dfd6-1773">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1773">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="1dfd6-1774">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1774">October 16, 2018</span></span>

<span data-ttu-id="1dfd6-1775">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1775">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-1776">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1776">VM</span></span>
* <span data-ttu-id="1dfd6-1777">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1777">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="1dfd6-1778">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1778">October 9, 2018</span></span>

<span data-ttu-id="1dfd6-1779">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1779">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-1780">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1780">Core</span></span>
* <span data-ttu-id="1dfd6-1781">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1781">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-1782">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1782">ACR</span></span>
* <span data-ttu-id="1dfd6-1783">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1783">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-1784">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1784">ACS</span></span>
* <span data-ttu-id="1dfd6-1785">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1785">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="1dfd6-1786">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1786">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="1dfd6-1787">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1787">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="1dfd6-1788">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1788">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="1dfd6-1789">Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1789">Container</span></span>
* <span data-ttu-id="1dfd6-1790">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um runtime específico</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1790">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="1dfd6-1791">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1791">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="1dfd6-1792">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1792">Event Hub</span></span>
* <span data-ttu-id="1dfd6-1793">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1793">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="1dfd6-1794">[ALTERAÇÃO SIGNIFICATIVA]`list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1794">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="1dfd6-1795">Extensões</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1795">Extensions</span></span>
* <span data-ttu-id="1dfd6-1796">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1796">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1dfd6-1797">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1797">HDInsight</span></span>
* <span data-ttu-id="1dfd6-1798">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1798">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="1dfd6-1799">IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1799">IoT</span></span>
* <span data-ttu-id="1dfd6-1800">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1800">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="1dfd6-1801">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1801">KeyVault</span></span>
* <span data-ttu-id="1dfd6-1802">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1802">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-1803">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1803">Network</span></span>
* <span data-ttu-id="1dfd6-1804">Corrigido `network dns zone create`: O comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1804">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="1dfd6-1805">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1805">See #6052</span></span>
* <span data-ttu-id="1dfd6-1806">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1806">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="1dfd6-1807">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1807">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="1dfd6-1808">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1808">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="1dfd6-1809">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1809">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="1dfd6-1810">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1810">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="1dfd6-1811">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1811">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-1812">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1812">Role</span></span>
* <span data-ttu-id="1dfd6-1813">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1813">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="1dfd6-1814">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1814">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="1dfd6-1815">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1815">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="1dfd6-1816">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1816">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="1dfd6-1817">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1817">Service Bus</span></span>
* <span data-ttu-id="1dfd6-1818">[ALTERAÇÃO SIGNIFICATIVA]`list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1818">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-1819">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1819">VM</span></span>
* <span data-ttu-id="1dfd6-1820">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1820">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="1dfd6-1821">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1821">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="1dfd6-1822">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1822">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="1dfd6-1823">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1823">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="1dfd6-1824">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1824">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="1dfd6-1825">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1825">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="1dfd6-1826">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1826">September 21, 2018</span></span>

<span data-ttu-id="1dfd6-1827">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1827">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-1828">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1828">ACR</span></span>
* <span data-ttu-id="1dfd6-1829">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1829">Added ACR Task commands</span></span>
* <span data-ttu-id="1dfd6-1830">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1830">Added quick run command</span></span>
* <span data-ttu-id="1dfd6-1831">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1831">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="1dfd6-1832">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1832">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="1dfd6-1833">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1833">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="1dfd6-1834">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1834">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-1835">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1835">ACS</span></span>
* <span data-ttu-id="1dfd6-1836">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1836">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="1dfd6-1837">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1837">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-1838">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1838">AppService</span></span>

* <span data-ttu-id="1dfd6-1839">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1839">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="1dfd6-1840">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1840">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="1dfd6-1841">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1841">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="1dfd6-1842">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1842">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="1dfd6-1843">Lote</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1843">Batch</span></span>
* <span data-ttu-id="1dfd6-1844">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1844">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="1dfd6-1845">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1845">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="1dfd6-1846">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1846">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="1dfd6-1847">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1847">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="1dfd6-1848">Lote AI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1848">Batch AI</span></span> 
* <span data-ttu-id="1dfd6-1849">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1849">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="1dfd6-1850">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1850">Cognitive Services</span></span>
* <span data-ttu-id="1dfd6-1851">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1851">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="1dfd6-1852">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1852">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="1dfd6-1853">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1853">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="1dfd6-1854">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1854">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="1dfd6-1855">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1855">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="1dfd6-1856">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1856">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="1dfd6-1857">Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1857">Container</span></span>
* <span data-ttu-id="1dfd6-1858">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1858">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="1dfd6-1859">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1859">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="1dfd6-1860">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1860">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="1dfd6-1861">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1861">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="1dfd6-1862">DataLake</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1862">Datalake</span></span>
* <span data-ttu-id="1dfd6-1863">Comandos adicionados para regras da rede virtual</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1863">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="1dfd6-1864">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1864">Interactive Shell</span></span>
* <span data-ttu-id="1dfd6-1865">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1865">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="1dfd6-1866">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1866">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="1dfd6-1867">IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1867">IoT</span></span>
* <span data-ttu-id="1dfd6-1868">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1868">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="1dfd6-1869">Key Vault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1869">Key Vault</span></span>
* <span data-ttu-id="1dfd6-1870">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1870">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-1871">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1871">Network</span></span>
* <span data-ttu-id="1dfd6-1872">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1872">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="1dfd6-1873">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1873">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="1dfd6-1874">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1874">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="1dfd6-1875">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1875">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="1dfd6-1876">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1876">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="1dfd6-1877">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1877">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="1dfd6-1878">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1878">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="1dfd6-1879">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1879">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="1dfd6-1880">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1880">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="1dfd6-1881">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1881">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="1dfd6-1882">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1882">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="1dfd6-1883">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1883">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="1dfd6-1884">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1884">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="1dfd6-1885">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1885">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="1dfd6-1886">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1886">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="1dfd6-1887">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1887">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="1dfd6-1888">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1888">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="1dfd6-1889">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1889">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="1dfd6-1890">RDBMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1890">RDBMS</span></span>
* <span data-ttu-id="1dfd6-1891">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1891">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="1dfd6-1892">Reserva</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1892">Reservation</span></span>
* <span data-ttu-id="1dfd6-1893">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1893">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="1dfd6-1894">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1894">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="1dfd6-1895">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1895">Manage App</span></span>
* <span data-ttu-id="1dfd6-1896">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1896">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="1dfd6-1897">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1897">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-1898">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1898">Role</span></span>
* <span data-ttu-id="1dfd6-1899">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1899">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="1dfd6-1900">SignalR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1900">SignalR</span></span>
* <span data-ttu-id="1dfd6-1901">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1901">First release</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-1902">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1902">Storage</span></span>
* <span data-ttu-id="1dfd6-1903">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1903">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="1dfd6-1904">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1904">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-1905">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1905">VM</span></span>
* <span data-ttu-id="1dfd6-1906">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1906">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="1dfd6-1907">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1907">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="1dfd6-1908">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1908">August 28, 2018</span></span>

<span data-ttu-id="1dfd6-1909">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1909">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-1910">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1910">Core</span></span>

* <span data-ttu-id="1dfd6-1911">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1911">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="1dfd6-1912">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1912">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-1913">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1913">ACR</span></span>

* <span data-ttu-id="1dfd6-1914">Adicionada uma solução alternativa para operações de runtime sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1914">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="1dfd6-1915">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1915">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-1916">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1916">ACS</span></span>

* <span data-ttu-id="1dfd6-1917">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1917">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="1dfd6-1918">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1918">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-1919">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1919">AppService</span></span>

* <span data-ttu-id="1dfd6-1920">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1920">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="1dfd6-1921">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1921">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="1dfd6-1922">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1922">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="1dfd6-1923">Backup</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1923">Backup</span></span>

* <span data-ttu-id="1dfd6-1924">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1924">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="1dfd6-1925">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1925">Bot Service</span></span>

* <span data-ttu-id="1dfd6-1926">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1926">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="1dfd6-1927">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1927">Cognitive Services</span></span>

* <span data-ttu-id="1dfd6-1928">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1928">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="1dfd6-1929">IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1929">IoT</span></span>

* <span data-ttu-id="1dfd6-1930">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1930">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="1dfd6-1931">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1931">Monitor</span></span>

* <span data-ttu-id="1dfd6-1932">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1932">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="1dfd6-1933">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1933">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-1934">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1934">Network</span></span>

* <span data-ttu-id="1dfd6-1935">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1935">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-1936">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1936">Resource</span></span>

* <span data-ttu-id="1dfd6-1937">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1937">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-1938">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1938">Storage</span></span>

* <span data-ttu-id="1dfd6-1939">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1939">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-1940">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1940">VM</span></span>

* <span data-ttu-id="1dfd6-1941">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1941">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="1dfd6-1942">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1942">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="1dfd6-1943">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1943">Auguest 14, 2018</span></span>

<span data-ttu-id="1dfd6-1944">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1944">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-1945">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1945">Core</span></span>

* <span data-ttu-id="1dfd6-1946">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1946">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="1dfd6-1947">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1947">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="1dfd6-1948">Telemetria</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1948">Telemetry</span></span>

* <span data-ttu-id="1dfd6-1949">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1949">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-1950">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1950">ACR</span></span>

* <span data-ttu-id="1dfd6-1951">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1951">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="1dfd6-1952">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1952">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-1953">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1953">ACS</span></span>

* <span data-ttu-id="1dfd6-1954">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1954">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="1dfd6-1955">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1955">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="1dfd6-1956">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1956">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="1dfd6-1957">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1957">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="1dfd6-1958">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1958">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="1dfd6-1959">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1959">AppService</span></span>

* <span data-ttu-id="1dfd6-1960">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1960">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="1dfd6-1961">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1961">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="1dfd6-1962">BatchAI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1962">BatchAI</span></span>

* <span data-ttu-id="1dfd6-1963">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1963">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="1dfd6-1964">Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1964">Container</span></span>

* <span data-ttu-id="1dfd6-1965">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1965">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="1dfd6-1966">IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1966">IoT</span></span>

* <span data-ttu-id="1dfd6-1967">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1967">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="1dfd6-1968">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1968">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="1dfd6-1969">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1969">Iot Central</span></span>

* <span data-ttu-id="1dfd6-1970">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1970">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="1dfd6-1971">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1971">KeyVault</span></span>


* <span data-ttu-id="1dfd6-1972">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1972">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="1dfd6-1973">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1973">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="1dfd6-1974">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1974">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="1dfd6-1975">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1975">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="1dfd6-1976">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1976">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="1dfd6-1977">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1977">Relay</span></span>

* <span data-ttu-id="1dfd6-1978">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1978">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-1979">Sql</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1979">Sql</span></span>

* <span data-ttu-id="1dfd6-1980">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1980">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-1981">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1981">Storage</span></span>

* <span data-ttu-id="1dfd6-1982">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1982">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="1dfd6-1983">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1983">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="1dfd6-1984">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1984">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="1dfd6-1985">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1985">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="1dfd6-1986">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1986">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-1987">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1987">VM</span></span>

* <span data-ttu-id="1dfd6-1988">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1988">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="1dfd6-1989">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1989">July 31, 2018</span></span>

<span data-ttu-id="1dfd6-1990">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1990">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-1991">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1991">ACR</span></span>

* <span data-ttu-id="1dfd6-1992">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1992">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="1dfd6-1993">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1993">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-1994">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1994">ACS</span></span>

* <span data-ttu-id="1dfd6-1995">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1995">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="1dfd6-1996">Lote</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1996">Batch</span></span>

* <span data-ttu-id="1dfd6-1997">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1997">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="1dfd6-1998">Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1998">Container</span></span>

* <span data-ttu-id="1dfd6-1999">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="1dfd6-1999">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-2000">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2000">Network</span></span>

* <span data-ttu-id="1dfd6-2001">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2001">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="1dfd6-2002">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2002">Resource</span></span>

* <span data-ttu-id="1dfd6-2003">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2003">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="1dfd6-2004">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2004">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-2005">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2005">Role</span></span>

* <span data-ttu-id="1dfd6-2006">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2006">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="1dfd6-2007">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2007">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="1dfd6-2008">Search</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2008">Search</span></span>

* <span data-ttu-id="1dfd6-2009">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2009">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="1dfd6-2010">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2010">Service Bus</span></span>

* <span data-ttu-id="1dfd6-2011">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2011">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="1dfd6-2012">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2012">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="1dfd6-2013">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2013">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="1dfd6-2014">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2014">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-2015">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2015">Storage</span></span>

* <span data-ttu-id="1dfd6-2016">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2016">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="1dfd6-2017">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2017">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2018">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2018">VM</span></span>

* <span data-ttu-id="1dfd6-2019">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2019">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="1dfd6-2020">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2020">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="1dfd6-2021">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2021">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="1dfd6-2022">[ALTERAÇÃO SIGNIFICATIVA]`[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2022">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="1dfd6-2023">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2023">July 18, 2018</span></span>

<span data-ttu-id="1dfd6-2024">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2024">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-2025">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2025">Core</span></span>

* <span data-ttu-id="1dfd6-2026">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2026">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="1dfd6-2027">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2027">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="1dfd6-2028">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2028">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-2029">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2029">ACR</span></span>

* <span data-ttu-id="1dfd6-2030">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2030">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="1dfd6-2031">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2031">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="1dfd6-2032">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2032">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="1dfd6-2033">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2033">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-2034">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2034">ACS</span></span>

* <span data-ttu-id="1dfd6-2035">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2035">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-2036">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2036">AppService</span></span>

* <span data-ttu-id="1dfd6-2037">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2037">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="1dfd6-2038">Lote</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2038">Batch</span></span>

* <span data-ttu-id="1dfd6-2039">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2039">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="1dfd6-2040">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2040">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="1dfd6-2041">Lote AI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2041">Batch AI</span></span>

* <span data-ttu-id="1dfd6-2042">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2042">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="1dfd6-2043">Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2043">Container</span></span>

* <span data-ttu-id="1dfd6-2044">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2044">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="1dfd6-2045">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2045">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-2046">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2046">Network</span></span>

* <span data-ttu-id="1dfd6-2047">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2047">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="1dfd6-2048">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2048">Added `network nic wait`</span></span>
* <span data-ttu-id="1dfd6-2049">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2049">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="1dfd6-2050">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2050">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="1dfd6-2051">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2051">Resource</span></span>

* <span data-ttu-id="1dfd6-2052">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2052">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="1dfd6-2053">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2053">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="1dfd6-2054">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2054">Added `deployment wait` command</span></span>
* <span data-ttu-id="1dfd6-2055">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2055">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-2056">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2056">SQL</span></span>

* <span data-ttu-id="1dfd6-2057">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2057">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="1dfd6-2058">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2058">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="1dfd6-2059">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2059">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-2060">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2060">Storage</span></span>

* <span data-ttu-id="1dfd6-2061">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2061">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2062">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2062">VM</span></span>

* <span data-ttu-id="1dfd6-2063">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2063">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="1dfd6-2064">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2064">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="1dfd6-2065">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2065">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="1dfd6-2066">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2066">July 3, 2018</span></span>

<span data-ttu-id="1dfd6-2067">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2067">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="1dfd6-2068">AKS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2068">AKS</span></span>

* <span data-ttu-id="1dfd6-2069">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2069">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="1dfd6-2070">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2070">July 3, 2018</span></span>

<span data-ttu-id="1dfd6-2071">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2071">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-2072">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2072">Core</span></span>

* <span data-ttu-id="1dfd6-2073">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2073">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-2074">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2074">ACR</span></span>

* <span data-ttu-id="1dfd6-2075">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2075">Added polling build status</span></span>
* <span data-ttu-id="1dfd6-2076">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2076">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="1dfd6-2077">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2077">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-2078">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2078">ACS</span></span>

* <span data-ttu-id="1dfd6-2079">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2079">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="1dfd6-2080">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2080">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="1dfd6-2081">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2081">Updated options for `aks browse` command.</span></span> <span data-ttu-id="1dfd6-2082">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2082">Added `--listen-port` support</span></span>
* <span data-ttu-id="1dfd6-2083">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2083">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="1dfd6-2084">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2084">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="1dfd6-2085">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2085">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-2086">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2086">AppService</span></span>

* <span data-ttu-id="1dfd6-2087">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2087">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="1dfd6-2088">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2088">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="1dfd6-2089">Backup</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2089">Backup</span></span>

* <span data-ttu-id="1dfd6-2090">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2090">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="1dfd6-2091">BatchAI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2091">BatchAI</span></span>

* <span data-ttu-id="1dfd6-2092">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2092">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="1dfd6-2093">Nuvem</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2093">Cloud</span></span>

* <span data-ttu-id="1dfd6-2094">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2094">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="1dfd6-2095">Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2095">Container</span></span>

* <span data-ttu-id="1dfd6-2096">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2096">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="1dfd6-2097">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2097">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="1dfd6-2098">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2098">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="1dfd6-2099">Extensão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2099">Extension</span></span>

* <span data-ttu-id="1dfd6-2100">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2100">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-2101">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2101">Network</span></span>

* <span data-ttu-id="1dfd6-2102">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2102">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="1dfd6-2103">Rdbms</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2103">Rdbms</span></span>

* <span data-ttu-id="1dfd6-2104">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2104">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-2105">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2105">Resource</span></span>

* <span data-ttu-id="1dfd6-2106">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2106">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2107">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2107">VM</span></span>

* <span data-ttu-id="1dfd6-2108">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2108">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="1dfd6-2109">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2109">June 25, 2018</span></span>

<span data-ttu-id="1dfd6-2110">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2110">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="1dfd6-2111">CLI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2111">CLI</span></span>

* <span data-ttu-id="1dfd6-2112">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2112">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="1dfd6-2113">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2113">June 19, 2018</span></span>

<span data-ttu-id="1dfd6-2114">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2114">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-2115">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2115">Core</span></span>

* <span data-ttu-id="1dfd6-2116">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2116">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-2117">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2117">ACR</span></span>

* <span data-ttu-id="1dfd6-2118">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2118">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="1dfd6-2119">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2119">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-2120">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2120">ACS</span></span>

* <span data-ttu-id="1dfd6-2121">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2121">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="1dfd6-2122">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2122">Added `--update` support</span></span>
* <span data-ttu-id="1dfd6-2123">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2123">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="1dfd6-2124">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2124">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="1dfd6-2125">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2125">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="1dfd6-2126">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2126">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="1dfd6-2127">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2127">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="1dfd6-2128">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2128">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-2129">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2129">AppService</span></span>

* <span data-ttu-id="1dfd6-2130">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2130">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="1dfd6-2131">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2131">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="1dfd6-2132">Lote</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2132">Batch</span></span>

* <span data-ttu-id="1dfd6-2133">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2133">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="1dfd6-2134">Lote AI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2134">Batch AI</span></span>

* <span data-ttu-id="1dfd6-2135">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2135">Added support for workspaces.</span></span> <span data-ttu-id="1dfd6-2136">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2136">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="1dfd6-2137">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2137">Added support for experiments.</span></span> <span data-ttu-id="1dfd6-2138">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2138">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="1dfd6-2139">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2139">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="1dfd6-2140">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2140">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="1dfd6-2141">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2141">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="1dfd6-2142">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2142">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="1dfd6-2143">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2143">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="1dfd6-2144">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2144">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="1dfd6-2145">[ALTERAÇÃO SIGNIFICATIVA]`--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2145">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="1dfd6-2146">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2146">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="1dfd6-2147">[ALTERAÇÃO SIGNIFICATIVA]`--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2147">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="1dfd6-2148">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2148">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="1dfd6-2149">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2149">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="1dfd6-2150">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2150">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="1dfd6-2151">[ALTERAÇÃO SIGNIFICATIVA]`--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2151">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="1dfd6-2152">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2152">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="1dfd6-2153">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2153">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="1dfd6-2154">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2154">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="1dfd6-2155">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2155">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="1dfd6-2156">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2156">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="1dfd6-2157">Mapas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2157">Maps</span></span>

* <span data-ttu-id="1dfd6-2158">[ALTERAÇÃO SIGNIFICATIVA]`maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2158">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-2159">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2159">Network</span></span>

* <span data-ttu-id="1dfd6-2160">Suporte adicionado para `https` a `network lb probe create` [nº6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2160">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="1dfd6-2161">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2161">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="1dfd6-2162">#6502</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2162">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="1dfd6-2163">Reservas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2163">Reservations</span></span>

* <span data-ttu-id="1dfd6-2164">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2164">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="1dfd6-2165">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2165">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="1dfd6-2166">[ALTERAÇÃO SIGNIFICATIVA]`kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2166">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="1dfd6-2167">[ALTERAÇÃO SIGNIFICATIVA]`capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2167">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="1dfd6-2168">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2168">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="1dfd6-2169">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2169">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-2170">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2170">Role</span></span>

* <span data-ttu-id="1dfd6-2171">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2171">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-2172">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2172">SQL</span></span>

* <span data-ttu-id="1dfd6-2173">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2173">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-2174">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2174">Storage</span></span>

* <span data-ttu-id="1dfd6-2175">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2175">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2176">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2176">VM</span></span>

* <span data-ttu-id="1dfd6-2177">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2177">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="1dfd6-2178">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2178">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="1dfd6-2179">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2179">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="1dfd6-2180">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2180">June 13, 2018</span></span>

<span data-ttu-id="1dfd6-2181">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2181">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-2182">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2182">Core</span></span>

* <span data-ttu-id="1dfd6-2183">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2183">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="1dfd6-2184">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2184">June 13, 2018</span></span>

<span data-ttu-id="1dfd6-2185">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2185">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="1dfd6-2186">AKS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2186">AKS</span></span>

* <span data-ttu-id="1dfd6-2187">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2187">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="1dfd6-2188">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2188">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="1dfd6-2189">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2189">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="1dfd6-2190">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2190">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="1dfd6-2191">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2191">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-2192">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2192">AppService</span></span>

* <span data-ttu-id="1dfd6-2193">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2193">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="1dfd6-2194">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2194">June 5, 2018</span></span>

<span data-ttu-id="1dfd6-2195">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2195">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="1dfd6-2196">Interativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2196">Interactive</span></span>

* <span data-ttu-id="1dfd6-2197">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2197">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="1dfd6-2198">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2198">June 5, 2018</span></span>

<span data-ttu-id="1dfd6-2199">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2199">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-2200">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2200">Core</span></span>

* <span data-ttu-id="1dfd6-2201">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2201">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="1dfd6-2202">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2202">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-2203">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2203">ACR</span></span>

* <span data-ttu-id="1dfd6-2204">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2204">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="1dfd6-2205">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2205">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="1dfd6-2206">AKS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2206">AKS</span></span>

* <span data-ttu-id="1dfd6-2207">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2207">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="1dfd6-2208">Lote</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2208">Batch</span></span>

* <span data-ttu-id="1dfd6-2209">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2209">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="1dfd6-2210">IOT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2210">IOT</span></span>

* <span data-ttu-id="1dfd6-2211">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2211">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-2212">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2212">Network</span></span>

* <span data-ttu-id="1dfd6-2213">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2213">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="1dfd6-2214">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2214">Policy Insights</span></span>

* <span data-ttu-id="1dfd6-2215">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2215">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="1dfd6-2216">ARM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2216">ARM</span></span>

* <span data-ttu-id="1dfd6-2217">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2217">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-2218">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2218">SQL</span></span>

* <span data-ttu-id="1dfd6-2219">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2219">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="1dfd6-2220">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2220">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="1dfd6-2221">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2221">Storage</span></span>

* <span data-ttu-id="1dfd6-2222">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2222">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2223">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2223">VM</span></span>

* <span data-ttu-id="1dfd6-2224">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2224">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="1dfd6-2225">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2225">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="1dfd6-2226">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2226">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="1dfd6-2227">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2227">May 22, 2018</span></span>

<span data-ttu-id="1dfd6-2228">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2228">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-2229">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2229">Core</span></span>

* <span data-ttu-id="1dfd6-2230">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2230">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-2231">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2231">ACS</span></span>

* <span data-ttu-id="1dfd6-2232">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2232">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="1dfd6-2233">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2233">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-2234">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2234">AppService</span></span>

* <span data-ttu-id="1dfd6-2235">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2235">Improved generic update commands</span></span>
* <span data-ttu-id="1dfd6-2236">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2236">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="1dfd6-2237">Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2237">Container</span></span>

* <span data-ttu-id="1dfd6-2238">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2238">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="1dfd6-2239">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2239">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="1dfd6-2240">Extensão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2240">Extension</span></span>

* <span data-ttu-id="1dfd6-2241">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2241">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="1dfd6-2242">Interativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2242">Interactive</span></span>

* <span data-ttu-id="1dfd6-2243">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2243">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="1dfd6-2244">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2244">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="1dfd6-2245">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2245">KeyVault</span></span>

* <span data-ttu-id="1dfd6-2246">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2246">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-2247">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2247">Network</span></span>

* <span data-ttu-id="1dfd6-2248">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2248">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="1dfd6-2249">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2249">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-2250">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2250">SQL</span></span>

* <span data-ttu-id="1dfd6-2251">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2251">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="1dfd6-2252">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2252">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="1dfd6-2253">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2253">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="1dfd6-2254">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2254">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="1dfd6-2255">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2255">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="1dfd6-2256">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2256">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="1dfd6-2257">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2257">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="1dfd6-2258">`edition`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2258">`edition`.</span></span> <span data-ttu-id="1dfd6-2259">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2259">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="1dfd6-2260">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2260">`elasticPoolName`.</span></span> <span data-ttu-id="1dfd6-2261">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2261">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="1dfd6-2262">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2262">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="1dfd6-2263">`edition`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2263">`edition`.</span></span> <span data-ttu-id="1dfd6-2264">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2264">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="1dfd6-2265">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2265">`dtu`.</span></span> <span data-ttu-id="1dfd6-2266">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2266">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="1dfd6-2267">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2267">`databaseDtuMin`.</span></span> <span data-ttu-id="1dfd6-2268">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2268">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="1dfd6-2269">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2269">`databaseDtuMax`.</span></span> <span data-ttu-id="1dfd6-2270">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2270">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="1dfd6-2271">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2271">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="1dfd6-2272">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2272">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-2273">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2273">Storage</span></span>

* <span data-ttu-id="1dfd6-2274">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2274">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="1dfd6-2275">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2275">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2276">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2276">VM</span></span>

* <span data-ttu-id="1dfd6-2277">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2277">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="1dfd6-2278">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2278">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="1dfd6-2279">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2279">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="1dfd6-2280">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2280">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="1dfd6-2281">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2281">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="1dfd6-2282">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2282">May 7, 2018</span></span>

<span data-ttu-id="1dfd6-2283">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2283">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-2284">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2284">Core</span></span>

* <span data-ttu-id="1dfd6-2285">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2285">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="1dfd6-2286">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2286">Added limited support for positional arguments</span></span>
* <span data-ttu-id="1dfd6-2287">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2287">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="1dfd6-2288">#5591</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2288">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="1dfd6-2289">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2289">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="1dfd6-2290">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2290">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="1dfd6-2291">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2291">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="1dfd6-2292">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2292">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="1dfd6-2293">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2293">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-2294">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2294">ACR</span></span>

* <span data-ttu-id="1dfd6-2295">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2295">Added ACR Build commands</span></span>
* <span data-ttu-id="1dfd6-2296">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2296">Improved resource not found error messages</span></span>
* <span data-ttu-id="1dfd6-2297">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2297">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="1dfd6-2298">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2298">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="1dfd6-2299">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2299">Improved repository commands error messages</span></span>
* <span data-ttu-id="1dfd6-2300">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2300">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-2301">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2301">ACS</span></span>

* <span data-ttu-id="1dfd6-2302">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2302">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="1dfd6-2303">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2303">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="1dfd6-2304">AMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2304">AMS</span></span>

* <span data-ttu-id="1dfd6-2305">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2305">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-2306">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2306">Appservice</span></span>

* <span data-ttu-id="1dfd6-2307">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2307">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="1dfd6-2308">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2308">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="1dfd6-2309">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2309">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="1dfd6-2310">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2310">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="1dfd6-2311">Lote AI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2311">Batch AI</span></span>

* <span data-ttu-id="1dfd6-2312">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2312">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="1dfd6-2313">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2313">Cognitive Services</span></span>

* <span data-ttu-id="1dfd6-2314">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create`[#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2314">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="1dfd6-2315">Consumo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2315">Consumption</span></span>

* <span data-ttu-id="1dfd6-2316">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2316">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="1dfd6-2317">Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2317">Container</span></span>

* <span data-ttu-id="1dfd6-2318">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2318">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="1dfd6-2319">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2319">Cosmos DB</span></span>

* <span data-ttu-id="1dfd6-2320">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2320">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="1dfd6-2321">DMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2321">DMS</span></span>

* <span data-ttu-id="1dfd6-2322">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2322">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="1dfd6-2323">Extensão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2323">Extension</span></span>

* <span data-ttu-id="1dfd6-2324">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2324">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="1dfd6-2325">Interativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2325">Interactive</span></span>

* <span data-ttu-id="1dfd6-2326">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2326">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="1dfd6-2327">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2327">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="1dfd6-2328">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2328">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="1dfd6-2329">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2329">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="1dfd6-2330">Laboratório</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2330">Lab</span></span>

* <span data-ttu-id="1dfd6-2331">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2331">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-2332">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2332">Network</span></span>

* <span data-ttu-id="1dfd6-2333">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2333">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="1dfd6-2334">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2334">Profile</span></span>

* <span data-ttu-id="1dfd6-2335">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2335">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="1dfd6-2336">[ALTERAÇÃO SIGNIFICATIVA]`--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2336">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="1dfd6-2337">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2337">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="1dfd6-2338">Redis</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2338">Redis</span></span>

* <span data-ttu-id="1dfd6-2339">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2339">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="1dfd6-2340">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2340">Deprecated `redis list-all`.</span></span> <span data-ttu-id="1dfd6-2341">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2341">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="1dfd6-2342">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2342">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="1dfd6-2343">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2343">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-2344">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2344">Role</span></span>

* <span data-ttu-id="1dfd6-2345">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2345">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-2346">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2346">Storage</span></span>

* <span data-ttu-id="1dfd6-2347">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2347">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="1dfd6-2348">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2348">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="1dfd6-2349">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2349">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="1dfd6-2350">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2350">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="1dfd6-2351">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2351">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2352">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2352">VM</span></span>

* <span data-ttu-id="1dfd6-2353">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2353">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="1dfd6-2354">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2354">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="1dfd6-2355">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2355">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="1dfd6-2356">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2356">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="1dfd6-2357">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2357">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="1dfd6-2358">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2358">Added write accelerator support</span></span>
* <span data-ttu-id="1dfd6-2359">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2359">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="1dfd6-2360">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2360">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="1dfd6-2361">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2361">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="1dfd6-2362">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2362">April 10, 2018</span></span>

<span data-ttu-id="1dfd6-2363">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2363">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-2364">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2364">ACR</span></span>

* <span data-ttu-id="1dfd6-2365">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2365">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-2366">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2366">ACS</span></span>

* <span data-ttu-id="1dfd6-2367">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2367">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-2368">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2368">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="1dfd6-2370">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2370">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="1dfd6-2371">BatchAI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2371">BatchAI</span></span>

* <span data-ttu-id="1dfd6-2372">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2372">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="1dfd6-2373">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2373">Job level mounting</span></span>
  - <span data-ttu-id="1dfd6-2374">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2374">Environment variables with secret values</span></span>
  - <span data-ttu-id="1dfd6-2375">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2375">Performance counters settings</span></span>
  - <span data-ttu-id="1dfd6-2376">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2376">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="1dfd6-2377">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2377">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="1dfd6-2378">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2378">Usage and limits reporting</span></span>
  - <span data-ttu-id="1dfd6-2379">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2379">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="1dfd6-2380">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2380">Support for custom images</span></span>
  - <span data-ttu-id="1dfd6-2381">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2381">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="1dfd6-2382">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2382">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="1dfd6-2383">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2383">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="1dfd6-2384">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2384">National clouds are supported</span></span>
* <span data-ttu-id="1dfd6-2385">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2385">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="1dfd6-2386">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2386">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="1dfd6-2387">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2387">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="1dfd6-2388">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2388">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="1dfd6-2389">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2389">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="1dfd6-2390">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2390">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="1dfd6-2391">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2391">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="1dfd6-2392">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2392">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="1dfd6-2393">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2393">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="1dfd6-2394">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2394">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="1dfd6-2395">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2395">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="1dfd6-2396">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2396">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="1dfd6-2397">[ALTERAÇÃO SIGNIFICATIVA]`--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2397">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="1dfd6-2398">Cobrança</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2398">Billing</span></span>

* <span data-ttu-id="1dfd6-2399">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2399">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="1dfd6-2400">Consumo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2400">Consumption</span></span>

* <span data-ttu-id="1dfd6-2401">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2401">Added `marketplace` commands</span></span>
* <span data-ttu-id="1dfd6-2402">[ALTERAÇÃO SIGNIFICATIVA]`reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2402">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="1dfd6-2403">[ALTERAÇÃO SIGNIFICATIVA]`reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2403">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="1dfd6-2404">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2404">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="1dfd6-2405">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2405">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="1dfd6-2406">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2406">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="1dfd6-2407">Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2407">Container</span></span>

* <span data-ttu-id="1dfd6-2408">Adição dos parâmetros de montagem de volume do Repositório Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2408">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="1dfd6-2409">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2409">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="1dfd6-2410">Extensão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2410">Extension</span></span>

* <span data-ttu-id="1dfd6-2411">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2411">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="1dfd6-2412">Interativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2412">Interactive</span></span>

* <span data-ttu-id="1dfd6-2413">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2413">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="1dfd6-2414">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2414">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="1dfd6-2415">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2415">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-2416">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2416">Network</span></span>

* <span data-ttu-id="1dfd6-2417">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2417">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="1dfd6-2418">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2418">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="1dfd6-2419">#4910</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2419">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="1dfd6-2420">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2420">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="1dfd6-2421">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2421">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="1dfd6-2422">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2422">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="1dfd6-2423">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2423">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="1dfd6-2424">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2424">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="1dfd6-2425">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2425">Profile</span></span>

* <span data-ttu-id="1dfd6-2426">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2426">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="1dfd6-2427">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2427">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="1dfd6-2428">RDBMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2428">RDBMS</span></span>

* <span data-ttu-id="1dfd6-2429">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2429">Added `georestore` command</span></span>
* <span data-ttu-id="1dfd6-2430">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2430">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-2431">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2431">Resource</span></span>

* <span data-ttu-id="1dfd6-2432">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2432">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="1dfd6-2433">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2433">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-2434">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2434">SQL</span></span>

* <span data-ttu-id="1dfd6-2435">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2435">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-2436">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2436">Storage</span></span>

* <span data-ttu-id="1dfd6-2437">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2437">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2438">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2438">VM</span></span>

* <span data-ttu-id="1dfd6-2439">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2439">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="1dfd6-2440">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2440">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="1dfd6-2442">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2442">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="1dfd6-2443">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2443">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="1dfd6-2444">#5718</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2444">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="1dfd6-2445">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2445">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="1dfd6-2446">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2446">March 27, 2018</span></span>

<span data-ttu-id="1dfd6-2447">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2447">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-2448">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2448">Core</span></span>

* <span data-ttu-id="1dfd6-2449">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2449">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-2450">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2450">ACS</span></span>

* <span data-ttu-id="1dfd6-2451">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2451">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-2452">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2452">Appservice</span></span>

* <span data-ttu-id="1dfd6-2453">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2453">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="1dfd6-2454">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2454">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="1dfd6-2455">Backup</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2455">Backup</span></span>

* <span data-ttu-id="1dfd6-2456">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2456">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="1dfd6-2457">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2457">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="1dfd6-2458">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2458">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="1dfd6-2459">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2459">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="1dfd6-2460">Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2460">Container</span></span>

* <span data-ttu-id="1dfd6-2461">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2461">Added `container exec` command.</span></span> <span data-ttu-id="1dfd6-2462">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2462">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="1dfd6-2463">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2463">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="1dfd6-2464">Extensão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2464">Extension</span></span>

* <span data-ttu-id="1dfd6-2465">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2465">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="1dfd6-2466">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2466">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="1dfd6-2467">[ALTERAÇÃO SIGNIFICATIVA]`extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2467">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="1dfd6-2468">Interativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2468">Interactive</span></span>

* <span data-ttu-id="1dfd6-2469">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2469">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="1dfd6-2470">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2470">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="1dfd6-2471">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2471">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="1dfd6-2472">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2472">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="1dfd6-2473">Laboratório</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2473">Lab</span></span>

* <span data-ttu-id="1dfd6-2474">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2474">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="1dfd6-2475">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2475">Monitor</span></span>

* <span data-ttu-id="1dfd6-2476">Adicionado suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [nº5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2476">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="1dfd6-2477">Corrigido [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2477">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="1dfd6-2478">Suporte adicionado para `--namespace` a `metrics list-definitions` [nº5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2478">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-2479">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2479">Network</span></span>

* <span data-ttu-id="1dfd6-2480">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2480">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="1dfd6-2481">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2481">Profile</span></span>

* <span data-ttu-id="1dfd6-2482">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2482">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="1dfd6-2483">RDBMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2483">RDBMS</span></span>

* <span data-ttu-id="1dfd6-2484">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2484">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-2485">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2485">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="1dfd6-2487">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2487">Role</span></span>

* <span data-ttu-id="1dfd6-2488">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2488">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="1dfd6-2489">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2489">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="1dfd6-2490">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2490">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="1dfd6-2491">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2491">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="1dfd6-2492">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2492">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-2493">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2493">Storage</span></span>

* <span data-ttu-id="1dfd6-2494">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2494">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="1dfd6-2495">Corrigido [#4049](https://github.com/Azure/azure-cli/issues/4049): problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2495">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2496">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2496">VM</span></span>

* <span data-ttu-id="1dfd6-2497">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2497">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="1dfd6-2498">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2498">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="1dfd6-2499">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2499">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="1dfd6-2500">[ALTERAÇÃO SIGNIFICATIVA]`vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2500">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="1dfd6-2501">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2501">March 13, 2018</span></span>

<span data-ttu-id="1dfd6-2502">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2502">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-2503">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2503">ACR</span></span>

* <span data-ttu-id="1dfd6-2504">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2504">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="1dfd6-2505">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2505">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="1dfd6-2506">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2506">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-2507">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2507">ACS</span></span>

* <span data-ttu-id="1dfd6-2508">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2508">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="1dfd6-2509">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2509">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="1dfd6-2510">Supervisor</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2510">Advisor</span></span>

* <span data-ttu-id="1dfd6-2511">[ALTERAÇÃO SIGNIFICATIVA]`advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2511">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="1dfd6-2512">[ALTERAÇÃO SIGNIFICATIVA]`advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2512">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="1dfd6-2513">[ALTERAÇÃO SIGNIFICATIVA]`advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2513">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="1dfd6-2514">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2514">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="1dfd6-2515">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2515">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-2516">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2516">Appservice</span></span>

* <span data-ttu-id="1dfd6-2517">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2517">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="1dfd6-2518">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2518">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="1dfd6-2519">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2519">Eventhubs</span></span>

* <span data-ttu-id="1dfd6-2520">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2520">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="1dfd6-2521">Extensão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2521">Extension</span></span>

* <span data-ttu-id="1dfd6-2522">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2522">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="1dfd6-2523">Interativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2523">Interactive</span></span>

* <span data-ttu-id="1dfd6-2524">Corrigido [#5625](https://github.com/Azure/azure-cli/issues/5625): manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2524">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="1dfd6-2525">Corrigido [#3016](https://github.com/Azure/azure-cli/issues/3016): histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2525">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="1dfd6-2526">Corrigido [#5688](https://github.com/Azure/azure-cli/issues/5688): as conclusões não aparecerão se o carregamento da tabela de comando encontrar uma exceção</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2526">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="1dfd6-2527">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2527">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="1dfd6-2528">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2528">Monitor</span></span>

* <span data-ttu-id="1dfd6-2529">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2529">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="1dfd6-2530">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2530">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="1dfd6-2531">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2531">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="1dfd6-2532">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2532">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-2533">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2533">Network</span></span>

* <span data-ttu-id="1dfd6-2534">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2534">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="1dfd6-2535">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2535">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="1dfd6-2536">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2536">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="1dfd6-2537">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2537">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="1dfd6-2538">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2538">Profile</span></span>

* <span data-ttu-id="1dfd6-2539">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2539">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="1dfd6-2540">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2540">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="1dfd6-2541">RDBMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2541">RDBMS</span></span>

* <span data-ttu-id="1dfd6-2542">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2542">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="1dfd6-2543">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2543">Service Bus</span></span>

* <span data-ttu-id="1dfd6-2544">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2544">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-2545">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2545">Storage</span></span>

* <span data-ttu-id="1dfd6-2546">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2546">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="1dfd6-2547">Corrigido [#5286](https://github.com/Azure/azure-cli/issues/5286): os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2547">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2548">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2548">VM</span></span>

* <span data-ttu-id="1dfd6-2549">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2549">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="1dfd6-2550">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2550">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="1dfd6-2551">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2551">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="1dfd6-2552">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2552">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="1dfd6-2553">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2553">February 27, 2018</span></span>

<span data-ttu-id="1dfd6-2554">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2554">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-2555">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2555">Core</span></span>

* <span data-ttu-id="1dfd6-2556">Corrigido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2556">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="1dfd6-2557">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2557">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="1dfd6-2558">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2558">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-2559">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2559">ACS</span></span>

* <span data-ttu-id="1dfd6-2560">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2560">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="1dfd6-2561">Problema corrigido: permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2561">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="1dfd6-2562">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2562">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="1dfd6-2563">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2563">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-2564">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2564">Appservice</span></span>

* <span data-ttu-id="1dfd6-2565">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2565">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="1dfd6-2566">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2566">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="1dfd6-2567">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2567">Cognitive Services</span></span>

* <span data-ttu-id="1dfd6-2568">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2568">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="1dfd6-2569">Consumo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2569">Consumption</span></span>

* <span data-ttu-id="1dfd6-2570">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2570">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="1dfd6-2571">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2571">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="1dfd6-2572">Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2572">Container</span></span>

* <span data-ttu-id="1dfd6-2573">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2573">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-2574">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2574">Network</span></span>

* <span data-ttu-id="1dfd6-2575">Corrigido [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2575">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-2576">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2576">Resource</span></span>

* <span data-ttu-id="1dfd6-2577">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2577">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-2578">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2578">Role</span></span>

* <span data-ttu-id="1dfd6-2579">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2579">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-2580">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2580">SQL</span></span>

* <span data-ttu-id="1dfd6-2581">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2581">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-2582">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2582">Storage</span></span>

* <span data-ttu-id="1dfd6-2583">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2583">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2584">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2584">VM</span></span>

* <span data-ttu-id="1dfd6-2585">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2585">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="1dfd6-2586">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2586">February 13, 2018</span></span>

<span data-ttu-id="1dfd6-2587">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2587">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-2588">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2588">Core</span></span>

* <span data-ttu-id="1dfd6-2589">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2589">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-2590">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2590">ACS</span></span>

* <span data-ttu-id="1dfd6-2591">[ALTERAÇÃO SIGNIFICATIVA]`aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2591">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="1dfd6-2592">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2592">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="1dfd6-2593">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2593">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="1dfd6-2594">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2594">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="1dfd6-2595">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2595">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="1dfd6-2596">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2596">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="1dfd6-2597">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2597">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="1dfd6-2598">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2598">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-2599">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2599">Appservice</span></span>

* <span data-ttu-id="1dfd6-2600">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2600">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="1dfd6-2601">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2601">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="1dfd6-2602">CDN</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2602">CDN</span></span>

* <span data-ttu-id="1dfd6-2603">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2603">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="1dfd6-2604">Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2604">Container</span></span>

* <span data-ttu-id="1dfd6-2605">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2605">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="1dfd6-2606">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2606">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1dfd6-2607">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2607">CosmosDB</span></span>

* <span data-ttu-id="1dfd6-2608">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2608">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="1dfd6-2609">Extensão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2609">Extension</span></span>

* <span data-ttu-id="1dfd6-2610">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2610">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="1dfd6-2611">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2611">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="1dfd6-2612">Comentários</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2612">Feedback</span></span>

* <span data-ttu-id="1dfd6-2613">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2613">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="1dfd6-2614">Interativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2614">Interactive</span></span>

* <span data-ttu-id="1dfd6-2615">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2615">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="1dfd6-2616">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2616">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="1dfd6-2617">IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2617">IoT</span></span>

* <span data-ttu-id="1dfd6-2618">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2618">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="1dfd6-2619">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2619">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="1dfd6-2620">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2620">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="1dfd6-2621">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2621">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="1dfd6-2622">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2622">Monitor</span></span>

* <span data-ttu-id="1dfd6-2623">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2623">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-2624">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2624">Network</span></span>

* <span data-ttu-id="1dfd6-2625">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2625">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="1dfd6-2626">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2626">Profile</span></span>

* <span data-ttu-id="1dfd6-2627">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2627">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-2628">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2628">Resource</span></span>

* <span data-ttu-id="1dfd6-2629">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2629">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-2630">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2630">Role</span></span>

* <span data-ttu-id="1dfd6-2631">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2631">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-2632">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2632">SQL</span></span>

* <span data-ttu-id="1dfd6-2633">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2633">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="1dfd6-2634">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2634">Added `sql db rename`</span></span>
* <span data-ttu-id="1dfd6-2635">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2635">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-2636">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2636">Storage</span></span>

* <span data-ttu-id="1dfd6-2637">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2637">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2638">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2638">VM</span></span>

* <span data-ttu-id="1dfd6-2639">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2639">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="1dfd6-2640">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2640">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="1dfd6-2641">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2641">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="1dfd6-2642">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2642">January 31, 2018</span></span>

<span data-ttu-id="1dfd6-2643">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2643">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-2644">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2644">Core</span></span>

* <span data-ttu-id="1dfd6-2645">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2645">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="1dfd6-2646">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2646">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="1dfd6-2647">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2647">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="1dfd6-2648">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2648">Use `--verbose` to see</span></span>
* <span data-ttu-id="1dfd6-2649">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2649">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-2650">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2650">ACS</span></span>

* <span data-ttu-id="1dfd6-2651">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2651">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="1dfd6-2652">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2652">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-2653">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2653">Appservice</span></span>

* <span data-ttu-id="1dfd6-2654">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2654">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="1dfd6-2655">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2655">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="1dfd6-2656">CDN</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2656">CDN</span></span>

* <span data-ttu-id="1dfd6-2657">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2657">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1dfd6-2658">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2658">CosmosDB</span></span>

* <span data-ttu-id="1dfd6-2659">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2659">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="1dfd6-2660">Interativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2660">Interactive</span></span>

* <span data-ttu-id="1dfd6-2661">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2661">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-2662">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2662">Network</span></span>

* <span data-ttu-id="1dfd6-2663">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2663">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="1dfd6-2664">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2664">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="1dfd6-2665">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2665">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="1dfd6-2666">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2666">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="1dfd6-2667">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2667">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="1dfd6-2668">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2668">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="1dfd6-2669">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2669">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="1dfd6-2670">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2670">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="1dfd6-2671">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2671">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="1dfd6-2672">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2672">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="1dfd6-2673">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2673">Profile</span></span>

* <span data-ttu-id="1dfd6-2674">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2674">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-2675">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2675">Resource</span></span>

* <span data-ttu-id="1dfd6-2676">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2676">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-2677">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2677">Storage</span></span>

* <span data-ttu-id="1dfd6-2678">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2678">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="1dfd6-2679">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2679">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="1dfd6-2680">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2680">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="1dfd6-2681">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2681">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="1dfd6-2682">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2682">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2683">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2683">VM</span></span>

* <span data-ttu-id="1dfd6-2684">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2684">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="1dfd6-2685">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2685">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="1dfd6-2686">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2686">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="1dfd6-2687">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2687">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="1dfd6-2688">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2688">January 17, 2018</span></span>

<span data-ttu-id="1dfd6-2689">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2689">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-2690">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2690">ACR</span></span>

* <span data-ttu-id="1dfd6-2691">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2691">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="1dfd6-2692">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2692">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-2693">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2693">ACS</span></span>

* <span data-ttu-id="1dfd6-2694">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2694">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="1dfd6-2695">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2695">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-2696">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2696">Appservice</span></span>

* <span data-ttu-id="1dfd6-2697">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2697">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="1dfd6-2698">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2698">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="1dfd6-2699">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2699">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="1dfd6-2700">Backup</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2700">Backup</span></span>

* <span data-ttu-id="1dfd6-2701">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2701">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="1dfd6-2702">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2702">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="1dfd6-2703">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2703">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="1dfd6-2704">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2704">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="1dfd6-2705">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2705">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="1dfd6-2706">Lote</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2706">Batch</span></span>

* <span data-ttu-id="1dfd6-2707">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2707">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="1dfd6-2708">Nuvem</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2708">Cloud</span></span>

* <span data-ttu-id="1dfd6-2709">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2709">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="1dfd6-2710">Consumo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2710">Consumption</span></span>

* <span data-ttu-id="1dfd6-2711">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2711">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="1dfd6-2712">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2712">Event Grid</span></span>

* <span data-ttu-id="1dfd6-2713">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2713">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="1dfd6-2714">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2714">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="1dfd6-2715">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2715">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="1dfd6-2716">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2716">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="1dfd6-2717">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2717">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="1dfd6-2718">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2718">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="1dfd6-2719">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2719">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="1dfd6-2720">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2720">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="1dfd6-2721">Interativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2721">Interactive</span></span>

* <span data-ttu-id="1dfd6-2722">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2722">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="1dfd6-2723">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2723">Fixed errors on startup</span></span>
* <span data-ttu-id="1dfd6-2724">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2724">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="1dfd6-2725">IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2725">IoT</span></span>

* <span data-ttu-id="1dfd6-2726">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2726">Added support for device provisioning service</span></span>
* <span data-ttu-id="1dfd6-2727">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2727">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="1dfd6-2728">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2728">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="1dfd6-2729">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2729">Monitor</span></span>

* <span data-ttu-id="1dfd6-2730">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2730">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="1dfd6-2731">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2731">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="1dfd6-2732">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2732">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-2733">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2733">Network</span></span>

* <span data-ttu-id="1dfd6-2734">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2734">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="1dfd6-2735">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2735">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="1dfd6-2736">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2736">Profile</span></span>

* <span data-ttu-id="1dfd6-2737">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2737">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-2738">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2738">Role</span></span>

* <span data-ttu-id="1dfd6-2739">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2739">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="1dfd6-2740">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2740">Service Fabric</span></span>

* <span data-ttu-id="1dfd6-2741">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2741">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="1dfd6-2742">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2742">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2743">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2743">VM</span></span>

* <span data-ttu-id="1dfd6-2744">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2744">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="1dfd6-2745">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2745">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="1dfd6-2746">[ALTERAÇÃO SIGNIFICATIVA]`externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2746">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="1dfd6-2747">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2747">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="1dfd6-2748">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2748">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="1dfd6-2749">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2749">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="1dfd6-2750">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2750">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="1dfd6-2751">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2751">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="1dfd6-2752">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2752">December 19, 2017</span></span>

<span data-ttu-id="1dfd6-2753">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2753">Version 2.0.23</span></span>

* <span data-ttu-id="1dfd6-2754">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2754">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="1dfd6-2755">Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2755">Container</span></span>

* <span data-ttu-id="1dfd6-2756">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2756">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-2757">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2757">Network</span></span>

* <span data-ttu-id="1dfd6-2758">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2758">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="1dfd6-2759">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2759">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-2760">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2760">Storage</span></span>

* <span data-ttu-id="1dfd6-2761">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2761">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2762">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2762">VM</span></span>

* <span data-ttu-id="1dfd6-2763">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2763">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="1dfd6-2764">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2764">December 5, 2017</span></span>

<span data-ttu-id="1dfd6-2765">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2765">Version 2.0.22</span></span>

* <span data-ttu-id="1dfd6-2766">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2766">Removed `az component` commands.</span></span> <span data-ttu-id="1dfd6-2767">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2767">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-2768">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2768">Core</span></span>
* <span data-ttu-id="1dfd6-2769">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2769">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="1dfd6-2770">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2770">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-2771">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2771">ACS</span></span>

* <span data-ttu-id="1dfd6-2772">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2772">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="1dfd6-2773">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2773">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="1dfd6-2774">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2774">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="1dfd6-2775">Supervisor</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2775">Advisor</span></span>

* <span data-ttu-id="1dfd6-2776">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2776">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-2777">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2777">Appservice</span></span>

* <span data-ttu-id="1dfd6-2778">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2778">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="1dfd6-2779">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2779">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="1dfd6-2780">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2780">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="1dfd6-2781">Consumo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2781">Consumption</span></span>

* <span data-ttu-id="1dfd6-2782">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2782">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="1dfd6-2783">Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2783">Container</span></span>

* <span data-ttu-id="1dfd6-2784">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2784">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="1dfd6-2785">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2785">Monitor</span></span>

* <span data-ttu-id="1dfd6-2786">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2786">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-2787">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2787">Resource</span></span>

* <span data-ttu-id="1dfd6-2788">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2788">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-2789">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2789">Role</span></span>

* <span data-ttu-id="1dfd6-2790">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2790">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="1dfd6-2791">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2791">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="1dfd6-2792">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2792">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-2793">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2793">SQL</span></span>

* <span data-ttu-id="1dfd6-2794">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2794">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="1dfd6-2795">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2795">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2796">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2796">VM</span></span>

* <span data-ttu-id="1dfd6-2797">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2797">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="1dfd6-2798">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2798">November 14, 2017</span></span>

<span data-ttu-id="1dfd6-2799">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2799">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-2800">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2800">ACR</span></span>

* <span data-ttu-id="1dfd6-2801">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2801">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="1dfd6-2802">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2802">ACS</span></span>

* <span data-ttu-id="1dfd6-2803">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2803">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="1dfd6-2804">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2804">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="1dfd6-2805">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2805">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="1dfd6-2806">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2806">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="1dfd6-2807">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2807">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-2808">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2808">Appservice</span></span>

* <span data-ttu-id="1dfd6-2809">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2809">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="1dfd6-2810">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2810">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="1dfd6-2811">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2811">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="1dfd6-2812">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2812">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="1dfd6-2813">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2813">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="1dfd6-2814">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2814">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="1dfd6-2815">Lote</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2815">Batch</span></span>

* <span data-ttu-id="1dfd6-2816">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2816">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="1dfd6-2817">Batchai</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2817">Batchai</span></span>

* <span data-ttu-id="1dfd6-2818">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2818">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="1dfd6-2819">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2819">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="1dfd6-2820">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2820">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="1dfd6-2821">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2821">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="1dfd6-2822">Nuvem</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2822">Cloud</span></span>

* <span data-ttu-id="1dfd6-2823">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2823">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="1dfd6-2824">Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2824">Container</span></span>

* <span data-ttu-id="1dfd6-2825">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2825">Added support to open multiple ports</span></span>
* <span data-ttu-id="1dfd6-2826">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2826">Added container group restart policy</span></span>
* <span data-ttu-id="1dfd6-2827">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2827">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="1dfd6-2828">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2828">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="1dfd6-2829">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2829">Data Lake Analytics</span></span>

* <span data-ttu-id="1dfd6-2830">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2830">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="1dfd6-2831">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2831">Data Lake Store</span></span>

* <span data-ttu-id="1dfd6-2832">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2832">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="1dfd6-2833">Extensão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2833">Extension</span></span>

* <span data-ttu-id="1dfd6-2834">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2834">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="1dfd6-2835">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2835">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="1dfd6-2836">IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2836">IoT</span></span>

* <span data-ttu-id="1dfd6-2837">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2837">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="1dfd6-2838">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2838">Monitor</span></span>

* <span data-ttu-id="1dfd6-2839">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2839">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-2840">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2840">Network</span></span>

* <span data-ttu-id="1dfd6-2841">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2841">Added support for CAA DNS records</span></span>
* <span data-ttu-id="1dfd6-2842">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2842">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="1dfd6-2843">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2843">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="1dfd6-2844">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2844">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="1dfd6-2845">Reservas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2845">Reservations</span></span>

* <span data-ttu-id="1dfd6-2846">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2846">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-2847">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2847">Resource</span></span>

* <span data-ttu-id="1dfd6-2848">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2848">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-2849">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2849">SQL</span></span>

* <span data-ttu-id="1dfd6-2850">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2850">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-2851">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2851">Storage</span></span>

* <span data-ttu-id="1dfd6-2852">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2852">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="1dfd6-2853">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2853">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="1dfd6-2854">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2854">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="1dfd6-2855">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2855">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="1dfd6-2856">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2856">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="1dfd6-2857">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2857">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="1dfd6-2858">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2858">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2859">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2859">VM</span></span>

* <span data-ttu-id="1dfd6-2860">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2860">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="1dfd6-2861">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2861">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="1dfd6-2862">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2862">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="1dfd6-2863">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2863">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="1dfd6-2864">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2864">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="1dfd6-2865">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2865">October 24, 2017</span></span>

<span data-ttu-id="1dfd6-2866">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2866">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-2867">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2867">Core</span></span>

* <span data-ttu-id="1dfd6-2868">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2868">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-2869">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2869">ACR</span></span>

* <span data-ttu-id="1dfd6-2870">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2870">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="1dfd6-2871">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2871">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="1dfd6-2872">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2872">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-2873">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2873">ACS</span></span>

* <span data-ttu-id="1dfd6-2874">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2874">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="1dfd6-2875">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2875">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-2876">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2876">Appservice</span></span>

* <span data-ttu-id="1dfd6-2877">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2877">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="1dfd6-2878">Componente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2878">Component</span></span>

* <span data-ttu-id="1dfd6-2879">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2879">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="1dfd6-2880">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2880">Monitor</span></span>

* <span data-ttu-id="1dfd6-2881">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2881">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-2882">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2882">Resource</span></span>

* <span data-ttu-id="1dfd6-2883">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2883">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="1dfd6-2884">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2884">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2885">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2885">VM</span></span>

* <span data-ttu-id="1dfd6-2886">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2886">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="1dfd6-2887">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2887">October 9, 2017</span></span>

<span data-ttu-id="1dfd6-2888">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2888">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-2889">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2889">Core</span></span>

* <span data-ttu-id="1dfd6-2890">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2890">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-2891">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2891">Appservice</span></span>

* <span data-ttu-id="1dfd6-2892">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2892">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="1dfd6-2893">Lote</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2893">Batch</span></span>

* <span data-ttu-id="1dfd6-2894">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2894">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="1dfd6-2895">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2895">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="1dfd6-2896">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2896">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="1dfd6-2897">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2897">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="1dfd6-2898">Batchai</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2898">Batchai</span></span>

* <span data-ttu-id="1dfd6-2899">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2899">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="1dfd6-2900">Keyvault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2900">Keyvault</span></span>

* <span data-ttu-id="1dfd6-2901">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2901">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="1dfd6-2902">(#4448)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2902">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="1dfd6-2903">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2903">Network</span></span>

* <span data-ttu-id="1dfd6-2904">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2904">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="1dfd6-2905">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2905">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-2906">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2906">Resource</span></span>

* <span data-ttu-id="1dfd6-2907">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2907">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="1dfd6-2908">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2908">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="1dfd6-2909">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2909">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="1dfd6-2910">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2910">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-2911">Sql</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2911">Sql</span></span>

* <span data-ttu-id="1dfd6-2912">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2912">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="1dfd6-2913">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2913">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="1dfd6-2914">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2914">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-2915">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2915">Storage</span></span>

* <span data-ttu-id="1dfd6-2916">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2916">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2917">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2917">Vm</span></span>

* <span data-ttu-id="1dfd6-2918">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2918">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="1dfd6-2919">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2919">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="1dfd6-2920">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2920">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="1dfd6-2921">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2921">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="1dfd6-2922">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2922">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="1dfd6-2923">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2923">September 22, 2017</span></span>

<span data-ttu-id="1dfd6-2924">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2924">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-2925">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2925">Resource</span></span>

* <span data-ttu-id="1dfd6-2926">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2926">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="1dfd6-2927">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2927">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="1dfd6-2928">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2928">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="1dfd6-2929">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2929">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-2930">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2930">Network</span></span>

* <span data-ttu-id="1dfd6-2931">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2931">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="1dfd6-2932">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2932">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="1dfd6-2933">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2933">Added `asg` application security group commands</span></span>
* <span data-ttu-id="1dfd6-2934">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2934">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="1dfd6-2935">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2935">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="1dfd6-2936">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2936">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="1dfd6-2937">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2937">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-2938">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2938">Storage</span></span>

* <span data-ttu-id="1dfd6-2939">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2939">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="1dfd6-2940">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2940">Eventgrid</span></span>

* <span data-ttu-id="1dfd6-2941">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2941">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-2942">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2942">SQL</span></span>

* <span data-ttu-id="1dfd6-2943">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2943">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="1dfd6-2944">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2944">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="1dfd6-2945">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2945">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="1dfd6-2946">Keyvault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2946">Keyvault</span></span>

* <span data-ttu-id="1dfd6-2947">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2947">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2948">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2948">VM</span></span>

* <span data-ttu-id="1dfd6-2949">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2949">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="1dfd6-2950">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2950">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="1dfd6-2951">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2951">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="1dfd6-2952">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2952">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="1dfd6-2953">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2953">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="1dfd6-2954">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2954">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-2955">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2955">ACS</span></span>

* <span data-ttu-id="1dfd6-2956">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2956">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-2957">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2957">Appservice</span></span>

* <span data-ttu-id="1dfd6-2958">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2958">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="1dfd6-2959">Backup</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2959">Backup</span></span>

* <span data-ttu-id="1dfd6-2960">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2960">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="1dfd6-2961">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2961">September 11, 2017</span></span>

<span data-ttu-id="1dfd6-2962">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2962">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="1dfd6-2963">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2963">Core</span></span>

* <span data-ttu-id="1dfd6-2964">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2964">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="1dfd6-2965">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2965">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-2966">Acs</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2966">Acs</span></span>

* <span data-ttu-id="1dfd6-2967">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2967">Added `acs list-locations` command</span></span>
* <span data-ttu-id="1dfd6-2968">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2968">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-2969">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2969">Appservice</span></span>

* <span data-ttu-id="1dfd6-2970">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2970">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="1dfd6-2971">CDN</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2971">CDN</span></span>

* <span data-ttu-id="1dfd6-2972">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2972">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="1dfd6-2973">Extensão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2973">Extension</span></span>

* <span data-ttu-id="1dfd6-2974">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2974">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="1dfd6-2975">Keyvault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2975">Keyvault</span></span>

* <span data-ttu-id="1dfd6-2976">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2976">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-2977">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2977">Network</span></span>

* <span data-ttu-id="1dfd6-2978">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2978">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="1dfd6-2979">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2979">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="1dfd6-2980">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2980">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="1dfd6-2981">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2981">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="1dfd6-2982">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2982">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-2983">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2983">Resource</span></span>

* <span data-ttu-id="1dfd6-2984">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2984">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="1dfd6-2985">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2985">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="1dfd6-2986">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2986">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="1dfd6-2987">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2987">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-2988">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2988">SQL</span></span>

* <span data-ttu-id="1dfd6-2989">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2989">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-2990">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2990">VM</span></span>

* <span data-ttu-id="1dfd6-2991">Corrigido: não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2991">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="1dfd6-2992">Corrigido: usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2992">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="1dfd6-2993">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2993">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="1dfd6-2994">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2994">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="1dfd6-2995">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2995">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="1dfd6-2996">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2996">August 31, 2017</span></span>

<span data-ttu-id="1dfd6-2997">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2997">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="1dfd6-2998">Keyvault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2998">Keyvault</span></span>

* <span data-ttu-id="1dfd6-2999">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-2999">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="1dfd6-3000">Sf</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3000">Sf</span></span>

* <span data-ttu-id="1dfd6-3001">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3001">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-3002">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3002">Storage</span></span>

* <span data-ttu-id="1dfd6-3003">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3003">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="1dfd6-3004">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3004">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="1dfd6-3005">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3005">August 28, 2017</span></span>

<span data-ttu-id="1dfd6-3006">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3006">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="1dfd6-3007">CLI</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3007">CLI</span></span>

* <span data-ttu-id="1dfd6-3008">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3008">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-3009">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3009">ACS</span></span>

* <span data-ttu-id="1dfd6-3010">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3010">Corrected preview regions</span></span>
* <span data-ttu-id="1dfd6-3011">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3011">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="1dfd6-3012">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3012">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-3013">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3013">Appservice</span></span>

* <span data-ttu-id="1dfd6-3014">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3014">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="1dfd6-3015">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3015">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="1dfd6-3016">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3016">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="1dfd6-3017">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3017">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="1dfd6-3018">Corrigido: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3018">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="1dfd6-3019">IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3019">IoT</span></span>

* <span data-ttu-id="1dfd6-3020">Corrigido #3934: a criação de uma política não limpa mais as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3020">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-3021">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3021">Network</span></span>

* <span data-ttu-id="1dfd6-3022">[ALTERAÇÃO SIGNIFICATIVA]`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3022">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="1dfd6-3023">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3023">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="1dfd6-3024">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3024">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="1dfd6-3025">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3025">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="1dfd6-3026">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3026">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="1dfd6-3027">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3027">Profile</span></span>

* <span data-ttu-id="1dfd6-3028">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3028">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="1dfd6-3029">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3029">Service Fabric</span></span>

* <span data-ttu-id="1dfd6-3030">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3030">Preview release</span></span>
* <span data-ttu-id="1dfd6-3031">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3031">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="1dfd6-3032">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3032">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="1dfd6-3033">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3033">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-3034">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3034">Storage</span></span>

* <span data-ttu-id="1dfd6-3035">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3035">Enabled setting blob tier</span></span>
* <span data-ttu-id="1dfd6-3036">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3036">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="1dfd6-3037">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3037">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="1dfd6-3038">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3038">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="1dfd6-3039">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3039">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="1dfd6-3040">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3040">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-3041">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3041">VM</span></span>

* <span data-ttu-id="1dfd6-3042">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3042">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="1dfd6-3043">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3043">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="1dfd6-3044">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3044">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="1dfd6-3045">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3045">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="1dfd6-3046">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3046">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="1dfd6-3047">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3047">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="1dfd6-3048">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3048">August 15, 2017</span></span>

<span data-ttu-id="1dfd6-3049">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3049">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-3050">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3050">ACS</span></span>

* <span data-ttu-id="1dfd6-3051">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3051">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-3052">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3052">Appservice</span></span>

* <span data-ttu-id="1dfd6-3053">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3053">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="1dfd6-3054">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3054">Event Grid</span></span>

* <span data-ttu-id="1dfd6-3055">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3055">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="1dfd6-3056">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3056">August 11, 2017</span></span>

<span data-ttu-id="1dfd6-3057">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3057">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-3058">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3058">ACS</span></span>

* <span data-ttu-id="1dfd6-3059">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3059">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="1dfd6-3060">Lote</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3060">Batch</span></span>

* <span data-ttu-id="1dfd6-3061">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3061">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="1dfd6-3062">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3062">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="1dfd6-3063">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3063">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="1dfd6-3064">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://”</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3064">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="1dfd6-3065">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3065">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="1dfd6-3066">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3066">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="1dfd6-3067">Componente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3067">Component</span></span>

* <span data-ttu-id="1dfd6-3068">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3068">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="1dfd6-3069">Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3069">Container</span></span>

* <span data-ttu-id="1dfd6-3070">`create`: corrigido o problema em que o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3070">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="1dfd6-3071">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3071">Data Lake Store</span></span>

* <span data-ttu-id="1dfd6-3072">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3072">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="1dfd6-3073">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3073">Event Grid</span></span>

* <span data-ttu-id="1dfd6-3074">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3074">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-3075">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3075">Network</span></span>

* <span data-ttu-id="1dfd6-3076">`lb`: corrigido o problema em que os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3076">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="1dfd6-3077">`application-gateway {subresource} delete`: corrigido o problema em que `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3077">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="1dfd6-3078">`application-gateway http-settings update`: corrigido o problema em que `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3078">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="1dfd6-3079">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3079">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="1dfd6-3080">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3080">Profile</span></span>

* <span data-ttu-id="1dfd6-3081">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3081">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-3082">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3082">Storage</span></span>

* <span data-ttu-id="1dfd6-3083">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3083">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-3084">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3084">VM</span></span>

* <span data-ttu-id="1dfd6-3085">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3085">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="1dfd6-3086">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3086">Exposed `list-skus` command</span></span>
* <span data-ttu-id="1dfd6-3087">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3087">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="1dfd6-3088">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3088">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="1dfd6-3089">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3089">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="1dfd6-3090">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3090">July 28, 2017</span></span>

<span data-ttu-id="1dfd6-3091">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3091">Version 2.0.12</span></span>

* <span data-ttu-id="1dfd6-3092">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3092">Added container commands</span></span>
* <span data-ttu-id="1dfd6-3093">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3093">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="1dfd6-3094">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3094">Core</span></span>

* <span data-ttu-id="1dfd6-3095">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3095">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="1dfd6-3096">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3096">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="1dfd6-3097">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3097">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="1dfd6-3098">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3098">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="1dfd6-3099">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3099">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="1dfd6-3100">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3100">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="1dfd6-3101">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3101">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="1dfd6-3102">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3102">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="1dfd6-3103">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3103">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="1dfd6-3104">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3104">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="1dfd6-3105">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3105">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="1dfd6-3106">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3106">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="1dfd6-3107">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3107">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="1dfd6-3108">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3108">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="1dfd6-3109">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3109">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="1dfd6-3110">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3110">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="1dfd6-3111">ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3111">ACR</span></span>

* <span data-ttu-id="1dfd6-3112">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3112">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="1dfd6-3113">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3113">Support SKU update for managed registries</span></span>
* <span data-ttu-id="1dfd6-3114">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3114">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="1dfd6-3115">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3115">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="1dfd6-3116">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3116">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="1dfd6-3117">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3117">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-3118">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3118">ACS</span></span>

* <span data-ttu-id="1dfd6-3119">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3119">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-3120">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3120">Appservice</span></span>

* <span data-ttu-id="1dfd6-3121">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3121">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="1dfd6-3122">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3122">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="1dfd6-3123">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3123">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="1dfd6-3124">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3124">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="1dfd6-3125">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3125">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="1dfd6-3126">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3126">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="1dfd6-3127">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3127">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="1dfd6-3128">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3128">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="1dfd6-3129">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3129">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="1dfd6-3130">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3130">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="1dfd6-3131">Lote</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3131">Batch</span></span>

* <span data-ttu-id="1dfd6-3132">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3132">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="1dfd6-3133">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3133">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="1dfd6-3134">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3134">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="1dfd6-3135">CDN</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3135">CDN</span></span>

* <span data-ttu-id="1dfd6-3136">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3136">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="1dfd6-3137">Nuvem</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3137">Cloud</span></span>

* <span data-ttu-id="1dfd6-3138">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3138">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="1dfd6-3139">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3139">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="1dfd6-3140">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3140">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="1dfd6-3141">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3141">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="1dfd6-3142">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3142">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1dfd6-3143">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3143">CosmosDB</span></span>

* <span data-ttu-id="1dfd6-3144">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3144">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="1dfd6-3145">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3145">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="1dfd6-3146">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3146">Data Lake Analytics</span></span>

* <span data-ttu-id="1dfd6-3147">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3147">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="1dfd6-3148">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3148">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="1dfd6-3149">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3149">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="1dfd6-3150">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3150">Data Lake Store</span></span>

* <span data-ttu-id="1dfd6-3151">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3151">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="1dfd6-3152">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3152">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="1dfd6-3153">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3153">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="1dfd6-3154">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3154">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="1dfd6-3155">Interativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3155">Interactive</span></span>

* <span data-ttu-id="1dfd6-3156">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3156">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="1dfd6-3157">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3157">Increased test coverage</span></span>
* <span data-ttu-id="1dfd6-3158">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3158">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="1dfd6-3159">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3159">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="1dfd6-3160">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3160">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="1dfd6-3161">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3161">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="1dfd6-3162">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3162">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="1dfd6-3163">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3163">Added `--progress` flag</span></span>
* <span data-ttu-id="1dfd6-3164">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3164">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="1dfd6-3165">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3165">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="1dfd6-3166">IoT</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3166">IoT</span></span>

* <span data-ttu-id="1dfd6-3167">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3167">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="1dfd6-3168">(#3934)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3168">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="1dfd6-3169">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3169">Key vault</span></span>

* <span data-ttu-id="1dfd6-3170">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3170">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="1dfd6-3171">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3171">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="1dfd6-3172">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3172">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="1dfd6-3173">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3173">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="1dfd6-3174">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3174">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="1dfd6-3175">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3175">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="1dfd6-3176">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3176">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="1dfd6-3177">(#3307)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3177">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="1dfd6-3178">Laboratório</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3178">Lab</span></span>

* <span data-ttu-id="1dfd6-3179">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3179">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="1dfd6-3180">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3180">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="1dfd6-3181">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3181">Monitor</span></span>

* <span data-ttu-id="1dfd6-3182">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3182">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="1dfd6-3183">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3183">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="1dfd6-3184">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3184">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="1dfd6-3185">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3185">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="1dfd6-3186">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3186">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="1dfd6-3187">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3187">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="1dfd6-3188">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3188">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="1dfd6-3189">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3189">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="1dfd6-3190">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3190">`location` no longer required</span></span>
  * <span data-ttu-id="1dfd6-3191">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3191">Add name and ID support for target</span></span>
  * <span data-ttu-id="1dfd6-3192">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3192">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="1dfd6-3193">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3193">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="1dfd6-3194">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3194">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="1dfd6-3195">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3195">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="1dfd6-3196">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3196">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="1dfd6-3197">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3197">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-3198">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3198">Network</span></span>

* <span data-ttu-id="1dfd6-3199">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3199">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="1dfd6-3200">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3200">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="1dfd6-3201">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3201">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="1dfd6-3202">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3202">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="1dfd6-3203">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3203">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="1dfd6-3204">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3204">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="1dfd6-3205">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3205">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="1dfd6-3206">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3206">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="1dfd6-3207">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3207">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="1dfd6-3208">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3208">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="1dfd6-3209">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3209">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="1dfd6-3210">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3210">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="1dfd6-3211">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3211">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="1dfd6-3212">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3212">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="1dfd6-3213">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3213">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="1dfd6-3214">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3214">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="1dfd6-3215">Adicionado o suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para --dns-servers</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3215">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="1dfd6-3216">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3216">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="1dfd6-3217">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3217">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="1dfd6-3218">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3218">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="1dfd6-3219">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3219">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="1dfd6-3220">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3220">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="1dfd6-3221">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3221">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="1dfd6-3222">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3222">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="1dfd6-3223">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3223">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="1dfd6-3224">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3224">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="1dfd6-3225">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3225">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="1dfd6-3226">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3226">Profile</span></span>

* <span data-ttu-id="1dfd6-3227">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3227">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="1dfd6-3228">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3228">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="1dfd6-3229">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3229">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="1dfd6-3230">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3230">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="1dfd6-3231">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3231">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="1dfd6-3232">RDBMS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3232">RDBMS</span></span>

* <span data-ttu-id="1dfd6-3233">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3233">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="1dfd6-3234">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3234">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="1dfd6-3235">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3235">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="1dfd6-3236">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3236">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-3237">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3237">Resource</span></span>

* <span data-ttu-id="1dfd6-3238">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3238">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="1dfd6-3239">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3239">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="1dfd6-3240">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3240">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="1dfd6-3241">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3241">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="1dfd6-3242">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3242">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="1dfd6-3243">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3243">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="1dfd6-3244">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3244">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="1dfd6-3245">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3245">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-3246">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3246">Role</span></span>

* <span data-ttu-id="1dfd6-3247">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3247">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="1dfd6-3248">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3248">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="1dfd6-3249">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3249">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="1dfd6-3250">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3250">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="1dfd6-3251">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3251">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="1dfd6-3252">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3252">Service Fabric</span></span>
* <span data-ttu-id="1dfd6-3253">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3253">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="1dfd6-3254">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3254">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="1dfd6-3255">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3255">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-3256">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3256">SQL</span></span>

* <span data-ttu-id="1dfd6-3257">Removido o parâmetro `sql server create` `--identity` desfeito</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3257">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="1dfd6-3258">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3258">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="1dfd6-3259">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3259">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-3260">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3260">Storage</span></span>

* <span data-ttu-id="1dfd6-3261">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3261">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="1dfd6-3262">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3262">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="1dfd6-3263">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3263">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="1dfd6-3264">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3264">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="1dfd6-3265">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3265">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="1dfd6-3266">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3266">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-3267">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3267">VM</span></span>

* <span data-ttu-id="1dfd6-3268">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3268">Support configuring nsg</span></span>
* <span data-ttu-id="1dfd6-3269">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3269">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="1dfd6-3270">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3270">Support managed service identities</span></span>
* <span data-ttu-id="1dfd6-3271">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3271">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="1dfd6-3272">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3272">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="1dfd6-3273">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3273">May 10, 2017</span></span>

<span data-ttu-id="1dfd6-3274">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3274">Version 2.0.6</span></span>

* <span data-ttu-id="1dfd6-3275">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3275">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="1dfd6-3276">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3276">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="1dfd6-3277">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3277">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="1dfd6-3278">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3278">Include Cognitive Services module</span></span>
* <span data-ttu-id="1dfd6-3279">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3279">Include Service Fabric module</span></span>
* <span data-ttu-id="1dfd6-3280">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3280">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="1dfd6-3281">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3281">Add support for CDN commands</span></span>
* <span data-ttu-id="1dfd6-3282">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3282">Remove Container module</span></span>
* <span data-ttu-id="1dfd6-3283">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3283">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="1dfd6-3284">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3284">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="1dfd6-3285">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3285">Core</span></span>

* <span data-ttu-id="1dfd6-3286">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3286">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="1dfd6-3287">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3287">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="1dfd6-3288">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3288">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="1dfd6-3289">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3289">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="1dfd6-3290">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3290">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="1dfd6-3291">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3291">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="1dfd6-3292">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3292">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="1dfd6-3293">núcleo: permitir que o caminho do arquivo accessTokens.json seja configurável por meio de uma variável de ambiente ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3293">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="1dfd6-3294">núcleo: permitir que padrões configurados sejam aplicados em argumentos opcionais ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3294">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="1dfd6-3295">núcleo: desempenho aprimorado</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3295">core: Improved performance</span></span>
* <span data-ttu-id="1dfd6-3296">núcleo: certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3296">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="1dfd6-3297">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3297">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-3298">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3298">ACS</span></span>

* <span data-ttu-id="1dfd6-3299">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3299">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="1dfd6-3300">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3300">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="1dfd6-3301">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3301">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="1dfd6-3302">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3302">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-3303">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3303">AppService</span></span>

* <span data-ttu-id="1dfd6-3304">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3304">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="1dfd6-3305">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3305">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="1dfd6-3306">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3306">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="1dfd6-3307">Exposição de argumentos para configurar a implantação e as “pilhas em runtime” em webapp create</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3307">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="1dfd6-3308">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3308">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="1dfd6-3309">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3309">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="1dfd6-3310">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3310">support slot swap with preview</span></span>
* <span data-ttu-id="1dfd6-3311">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3311">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="1dfd6-3312">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3312">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1dfd6-3313">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3313">CosmosDB</span></span>

* <span data-ttu-id="1dfd6-3314">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3314">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="1dfd6-3315">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3315">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="1dfd6-3316">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3316">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="1dfd6-3317">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3317">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="1dfd6-3318">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3318">Data Lake Analytics</span></span>

* <span data-ttu-id="1dfd6-3319">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3319">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="1dfd6-3320">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3320">Add support for new catalog item type: package.</span></span> <span data-ttu-id="1dfd6-3321">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3321">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="1dfd6-3322">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3322">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="1dfd6-3323">Tabela</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3323">Table</span></span>
  * <span data-ttu-id="1dfd6-3324">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3324">Table valued function</span></span>
  * <span data-ttu-id="1dfd6-3325">Visualizar</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3325">View</span></span>
  * <span data-ttu-id="1dfd6-3326">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3326">Table Statistics.</span></span> <span data-ttu-id="1dfd6-3327">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3327">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="1dfd6-3328">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3328">Data Lake Store</span></span>

* <span data-ttu-id="1dfd6-3329">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3329">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="1dfd6-3330">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3330">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="1dfd6-3331">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3331">missed help for access show.</span></span> <span data-ttu-id="1dfd6-3332">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3332">adding it.</span></span> <span data-ttu-id="1dfd6-3333">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3333">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="1dfd6-3334">Localizar</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3334">Find</span></span>

* <span data-ttu-id="1dfd6-3335">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3335">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="1dfd6-3336">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3336">KeyVault</span></span>

* <span data-ttu-id="1dfd6-3337">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3337">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="1dfd6-3338">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois estes parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3338">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="1dfd6-3339">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3339">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="1dfd6-3340">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3340">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="1dfd6-3341">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3341">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="1dfd6-3342">Laboratório</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3342">Lab</span></span>

* <span data-ttu-id="1dfd6-3343">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3343">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="1dfd6-3344">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3344">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="1dfd6-3345">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3345">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="1dfd6-3346">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3346">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="1dfd6-3347">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3347">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="1dfd6-3348">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3348">Monitor</span></span>

* <span data-ttu-id="1dfd6-3349">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3349">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="1dfd6-3350">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3350">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="1dfd6-3351">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3351">Network</span></span>

* <span data-ttu-id="1dfd6-3352">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3352">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="1dfd6-3353">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3353">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="1dfd6-3354">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3354">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="1dfd6-3355">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3355">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="1dfd6-3356">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3356">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="1dfd6-3357">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3357">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="1dfd6-3358">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3358">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="1dfd6-3359">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3359">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="1dfd6-3360">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3360">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="1dfd6-3361">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3361">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="1dfd6-3362">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3362">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="1dfd6-3363">BC: corrigido um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3363">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="1dfd6-3364">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3364">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="1dfd6-3365">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3365">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="1dfd6-3366">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3366">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="1dfd6-3367">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3367">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="1dfd6-3368">Perfil</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3368">Profile</span></span>

* <span data-ttu-id="1dfd6-3369">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3369">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="1dfd6-3370">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3370">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="1dfd6-3371">Redis</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3371">Redis</span></span>

* <span data-ttu-id="1dfd6-3372">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3372">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="1dfd6-3373">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3373">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="1dfd6-3374">Recurso</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3374">Resource</span></span>

* <span data-ttu-id="1dfd6-3375">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3375">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="1dfd6-3376">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3376">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="1dfd6-3377">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3377">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="1dfd6-3378">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3378">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="1dfd6-3379">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3379">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="1dfd6-3380">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3380">Add docs for az lock update.</span></span> <span data-ttu-id="1dfd6-3381">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3381">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="1dfd6-3382">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3382">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="1dfd6-3383">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3383">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="1dfd6-3384">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3384">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="1dfd6-3385">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3385">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="1dfd6-3386">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3386">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="1dfd6-3387">Função</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3387">Role</span></span>

* <span data-ttu-id="1dfd6-3388">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3388">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="1dfd6-3389">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3389">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="1dfd6-3390">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3390">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="1dfd6-3391">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3391">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="1dfd6-3392">SQL</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3392">SQL</span></span>

* <span data-ttu-id="1dfd6-3393">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3393">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="1dfd6-3394">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3394">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="1dfd6-3395">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3395">Storage</span></span>

* <span data-ttu-id="1dfd6-3396">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3396">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="1dfd6-3397">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3397">Add support for incremental blob copy</span></span>
* <span data-ttu-id="1dfd6-3398">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3398">Add support for large block blob upload</span></span>
* <span data-ttu-id="1dfd6-3399">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3399">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-3400">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3400">VM</span></span>

* <span data-ttu-id="1dfd6-3401">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3401">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="1dfd6-3402">observação: em comandos da VM em nuvens soberanas, evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3402">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="1dfd6-3403">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3403">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="1dfd6-3404">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3404">az vm/vmss disk</span></span>
  3. <span data-ttu-id="1dfd6-3405">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3405">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="1dfd6-3406">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3406">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="1dfd6-3407">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3407">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="1dfd6-3408">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3408">April 3, 2017</span></span>

<span data-ttu-id="1dfd6-3409">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3409">Version 2.0.2</span></span>

<span data-ttu-id="1dfd6-3410">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3410">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="1dfd6-3411">Núcleo</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3411">Core</span></span>

* <span data-ttu-id="1dfd6-3412">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3412">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="1dfd6-3413">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3413">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="1dfd6-3414">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3414">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="1dfd6-3415">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3415">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="1dfd6-3416">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3416">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="1dfd6-3417">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3417">Add prompting for missing template parameters.</span></span> <span data-ttu-id="1dfd6-3418">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3418">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="1dfd6-3419">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3419">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="1dfd6-3420">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3420">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="1dfd6-3421">ACS</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3421">ACS</span></span>

* <span data-ttu-id="1dfd6-3422">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3422">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="1dfd6-3423">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3423">Add support for ssh key password prompting.</span></span> <span data-ttu-id="1dfd6-3424">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3424">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="1dfd6-3425">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3425">Add support for windows clusters.</span></span> <span data-ttu-id="1dfd6-3426">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3426">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="1dfd6-3427">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3427">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="1dfd6-3428">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3428">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="1dfd6-3429">AppService</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3429">AppService</span></span>

* <span data-ttu-id="1dfd6-3430">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3430">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="1dfd6-3431">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3431">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="1dfd6-3432">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3432">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="1dfd6-3433">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3433">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="1dfd6-3434">DataLake</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3434">DataLake</span></span>

* <span data-ttu-id="1dfd6-3435">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3435">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="1dfd6-3436">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3436">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="1dfd6-3437">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3437">DocuemntDB</span></span>

* <span data-ttu-id="1dfd6-3438">DocumentDB: adicionado suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3438">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="1dfd6-3439">VM</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3439">VM</span></span>

* <span data-ttu-id="1dfd6-3440">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3440">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="1dfd6-3441">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3441">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="1dfd6-3442">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3442">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="1dfd6-3443">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3443">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="1dfd6-3444">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3444">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="1dfd6-3445">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3445">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="1dfd6-3446">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3446">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="1dfd6-3447">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3447">February 27, 2017</span></span>

<span data-ttu-id="1dfd6-3448">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3448">Version 2.0.0</span></span>

<span data-ttu-id="1dfd6-3449">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3449">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="1dfd6-3450">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3450">Container Service (acs)</span></span>
- <span data-ttu-id="1dfd6-3451">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3451">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="1dfd6-3452">Rede</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3452">Networking</span></span>
- <span data-ttu-id="1dfd6-3453">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3453">Storage</span></span>

<span data-ttu-id="1dfd6-3454">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3454">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="1dfd6-3455">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3455">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="1dfd6-3456">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3456">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="1dfd6-3457">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3457">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="1dfd6-3458">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3458">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="1dfd6-3459">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3459">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="1dfd6-3460">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3460">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="1dfd6-3461">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3461">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="1dfd6-3462">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="1dfd6-3462">Provide feedback from the command line with the `az feedback` command</span></span>
