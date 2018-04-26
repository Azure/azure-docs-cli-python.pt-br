---
title: Notas de versão da CLI do Azure 2.0
description: Saiba mais sobre as últimas atualizações da CLI do Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 04/10/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 1e6bd4cd8bab853fb417ed9c4dd71d56e5de7cdc
ms.sourcegitcommit: 204fd027d3668959b98b936969ccb41eada0fd29
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="bf606-103">Notas de versão da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="bf606-103">Azure CLI 2.0 release notes</span></span>

## <a name="april-10-2018"></a><span data-ttu-id="bf606-104">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="bf606-104">April 10, 2018</span></span>

<span data-ttu-id="bf606-105">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="bf606-105">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="bf606-106">ACR</span><span class="sxs-lookup"><span data-stu-id="bf606-106">ACR</span></span>

* <span data-ttu-id="bf606-107">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="bf606-107">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="bf606-108">ACS</span><span class="sxs-lookup"><span data-stu-id="bf606-108">ACS</span></span>

* <span data-ttu-id="bf606-109">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="bf606-109">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="bf606-110">AppService</span><span class="sxs-lookup"><span data-stu-id="bf606-110">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="bf606-112">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="bf606-112">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="bf606-113">BatchAI</span><span class="sxs-lookup"><span data-stu-id="bf606-113">BatchAI</span></span>

* <span data-ttu-id="bf606-114">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="bf606-114">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="bf606-115">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="bf606-115">Job level mounting</span></span>
 - <span data-ttu-id="bf606-116">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="bf606-116">Environment variables with secret values</span></span>
 - <span data-ttu-id="bf606-117">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="bf606-117">Performance counters settings</span></span>
 - <span data-ttu-id="bf606-118">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="bf606-118">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="bf606-119">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="bf606-119">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="bf606-120">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="bf606-120">Usage and limits reporting</span></span>
 - <span data-ttu-id="bf606-121">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="bf606-121">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="bf606-122">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="bf606-122">Support for custom images</span></span>
 - <span data-ttu-id="bf606-123">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="bf606-123">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="bf606-124">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="bf606-124">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="bf606-125">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="bf606-125">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="bf606-126">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="bf606-126">National clouds are supported</span></span>
* <span data-ttu-id="bf606-127">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="bf606-127">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="bf606-128">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="bf606-128">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="bf606-129">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="bf606-129">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="bf606-130">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="bf606-130">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="bf606-131">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="bf606-131">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="bf606-132">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="bf606-132">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="bf606-133">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="bf606-133">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="bf606-134">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="bf606-134">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="bf606-135">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="bf606-135">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="bf606-136">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="bf606-136">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="bf606-137">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="bf606-137">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="bf606-138">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="bf606-138">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="bf606-139">[ALTERAÇÃO SIGNIFICATIVA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="bf606-139">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="bf606-140">Cobrança</span><span class="sxs-lookup"><span data-stu-id="bf606-140">Billing</span></span>

* <span data-ttu-id="bf606-141">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="bf606-141">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="bf606-142">Consumo</span><span class="sxs-lookup"><span data-stu-id="bf606-142">Consumption</span></span>

* <span data-ttu-id="bf606-143">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="bf606-143">Added `marketplace` commands</span></span>
* <span data-ttu-id="bf606-144">[ALTERAÇÃO SIGNIFICATIVA] `reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="bf606-144">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="bf606-145">[ALTERAÇÃO SIGNIFICATIVA] `reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="bf606-145">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="bf606-146">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="bf606-146">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="bf606-147">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="bf606-147">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="bf606-148">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="bf606-148">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="bf606-149">Contêiner</span><span class="sxs-lookup"><span data-stu-id="bf606-149">Container</span></span>

* <span data-ttu-id="bf606-150">Adição dos parâmetros de montagem de volume de repositório git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="bf606-150">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="bf606-151">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="bf606-151">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="bf606-152">Extensão</span><span class="sxs-lookup"><span data-stu-id="bf606-152">Extension</span></span>

* <span data-ttu-id="bf606-153">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="bf606-153">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="bf606-154">Interativo</span><span class="sxs-lookup"><span data-stu-id="bf606-154">Interactive</span></span>

* <span data-ttu-id="bf606-155">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="bf606-155">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="bf606-156">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="bf606-156">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="bf606-157">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="bf606-157">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="bf606-158">Rede</span><span class="sxs-lookup"><span data-stu-id="bf606-158">Network</span></span>

* <span data-ttu-id="bf606-159">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="bf606-159">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="bf606-160">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bf606-160">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="bf606-161">#4910</span><span class="sxs-lookup"><span data-stu-id="bf606-161">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="bf606-162">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="bf606-162">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="bf606-163">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="bf606-163">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="bf606-164">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bf606-164">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="bf606-165">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bf606-165">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="bf606-166">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="bf606-166">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="bf606-167">Perfil</span><span class="sxs-lookup"><span data-stu-id="bf606-167">Profile</span></span>

* <span data-ttu-id="bf606-168">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="bf606-168">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="bf606-169">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="bf606-169">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="bf606-170">RDBMS</span><span class="sxs-lookup"><span data-stu-id="bf606-170">RDBMS</span></span>

* <span data-ttu-id="bf606-171">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="bf606-171">Added `georestore` command</span></span>
* <span data-ttu-id="bf606-172">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="bf606-172">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="bf606-173">Recurso</span><span class="sxs-lookup"><span data-stu-id="bf606-173">Resource</span></span>

* <span data-ttu-id="bf606-174">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="bf606-174">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="bf606-175">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="bf606-175">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="bf606-176">SQL</span><span class="sxs-lookup"><span data-stu-id="bf606-176">SQL</span></span>

* <span data-ttu-id="bf606-177">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="bf606-177">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="bf606-178">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="bf606-178">Storage</span></span>

* <span data-ttu-id="bf606-179">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="bf606-179">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="bf606-180">VM</span><span class="sxs-lookup"><span data-stu-id="bf606-180">VM</span></span>

* <span data-ttu-id="bf606-181">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="bf606-181">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="bf606-182">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="bf606-182">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="bf606-184">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="bf606-184">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="bf606-185">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="bf606-185">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="bf606-186">#5718</span><span class="sxs-lookup"><span data-stu-id="bf606-186">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="bf606-187">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="bf606-187">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="bf606-188">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="bf606-188">March 27, 2018</span></span>

<span data-ttu-id="bf606-189">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="bf606-189">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="bf606-190">Núcleo</span><span class="sxs-lookup"><span data-stu-id="bf606-190">Core</span></span>

* <span data-ttu-id="bf606-191">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="bf606-191">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="bf606-192">ACS</span><span class="sxs-lookup"><span data-stu-id="bf606-192">ACS</span></span>

* <span data-ttu-id="bf606-193">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="bf606-193">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="bf606-194">AppService</span><span class="sxs-lookup"><span data-stu-id="bf606-194">Appservice</span></span>

* <span data-ttu-id="bf606-195">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="bf606-195">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="bf606-196">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="bf606-196">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="bf606-197">Backup</span><span class="sxs-lookup"><span data-stu-id="bf606-197">Backup</span></span>

* <span data-ttu-id="bf606-198">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="bf606-198">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="bf606-199">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="bf606-199">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="bf606-200">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="bf606-200">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="bf606-201">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="bf606-201">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="bf606-202">Contêiner</span><span class="sxs-lookup"><span data-stu-id="bf606-202">Container</span></span>

* <span data-ttu-id="bf606-203">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="bf606-203">Added `container exec` command.</span></span> <span data-ttu-id="bf606-204">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="bf606-204">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="bf606-205">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="bf606-205">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="bf606-206">Extensão</span><span class="sxs-lookup"><span data-stu-id="bf606-206">Extension</span></span>

* <span data-ttu-id="bf606-207">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="bf606-207">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="bf606-208">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="bf606-208">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="bf606-209">[ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="bf606-209">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="bf606-210">Interativo</span><span class="sxs-lookup"><span data-stu-id="bf606-210">Interactive</span></span>

* <span data-ttu-id="bf606-211">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="bf606-211">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="bf606-212">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="bf606-212">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="bf606-213">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="bf606-213">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="bf606-214">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="bf606-214">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="bf606-215">Laboratório</span><span class="sxs-lookup"><span data-stu-id="bf606-215">Lab</span></span>

* <span data-ttu-id="bf606-216">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="bf606-216">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="bf606-217">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="bf606-217">Monitor</span></span>

* <span data-ttu-id="bf606-218">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="bf606-218">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="bf606-219">[#4529](https://github.com/Azure/azure-cli/issues/5785) corrigido: `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="bf606-219">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="bf606-220">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="bf606-220">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="bf606-221">Rede</span><span class="sxs-lookup"><span data-stu-id="bf606-221">Network</span></span>

* <span data-ttu-id="bf606-222">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="bf606-222">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="bf606-223">Perfil</span><span class="sxs-lookup"><span data-stu-id="bf606-223">Profile</span></span>

* <span data-ttu-id="bf606-224">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="bf606-224">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="bf606-225">RDBMS</span><span class="sxs-lookup"><span data-stu-id="bf606-225">RDBMS</span></span>

* <span data-ttu-id="bf606-226">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="bf606-226">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="bf606-227">Recurso</span><span class="sxs-lookup"><span data-stu-id="bf606-227">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="bf606-229">Função</span><span class="sxs-lookup"><span data-stu-id="bf606-229">Role</span></span>

* <span data-ttu-id="bf606-230">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="bf606-230">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="bf606-231">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="bf606-231">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="bf606-232">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="bf606-232">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="bf606-233">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="bf606-233">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="bf606-234">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="bf606-234">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="bf606-235">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="bf606-235">Storage</span></span>

* <span data-ttu-id="bf606-236">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="bf606-236">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="bf606-237">[4049#](https://github.com/Azure/azure-cli/issues/4049) corrigido: problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="bf606-237">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="bf606-238">VM</span><span class="sxs-lookup"><span data-stu-id="bf606-238">VM</span></span>

* <span data-ttu-id="bf606-239">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="bf606-239">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="bf606-240">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="bf606-240">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="bf606-241">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="bf606-241">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="bf606-242">[ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="bf606-242">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="bf606-243">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="bf606-243">March 13, 2018</span></span>

<span data-ttu-id="bf606-244">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="bf606-244">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="bf606-245">ACR</span><span class="sxs-lookup"><span data-stu-id="bf606-245">ACR</span></span>

* <span data-ttu-id="bf606-246">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="bf606-246">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="bf606-247">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="bf606-247">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="bf606-248">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="bf606-248">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="bf606-249">ACS</span><span class="sxs-lookup"><span data-stu-id="bf606-249">ACS</span></span>

* <span data-ttu-id="bf606-250">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="bf606-250">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="bf606-251">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="bf606-251">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="bf606-252">Supervisor</span><span class="sxs-lookup"><span data-stu-id="bf606-252">Advisor</span></span>

* <span data-ttu-id="bf606-253">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="bf606-253">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="bf606-254">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="bf606-254">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="bf606-255">[ALTERAÇÃO SIGNIFICATIVA] `advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="bf606-255">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="bf606-256">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="bf606-256">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="bf606-257">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="bf606-257">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="bf606-258">AppService</span><span class="sxs-lookup"><span data-stu-id="bf606-258">Appservice</span></span>

* <span data-ttu-id="bf606-259">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="bf606-259">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="bf606-260">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="bf606-260">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="bf606-261">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="bf606-261">Eventhubs</span></span>

* <span data-ttu-id="bf606-262">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="bf606-262">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="bf606-263">Extensão</span><span class="sxs-lookup"><span data-stu-id="bf606-263">Extension</span></span>

* <span data-ttu-id="bf606-264">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="bf606-264">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="bf606-265">Interativo</span><span class="sxs-lookup"><span data-stu-id="bf606-265">Interactive</span></span>

* <span data-ttu-id="bf606-266">[5625](https://github.com/Azure/azure-cli/issues/5625) corrigido: manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="bf606-266">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="bf606-267">[3016](https://github.com/Azure/azure-cli/issues/3016) corrigido: histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="bf606-267">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="bf606-268">[5688](https://github.com/Azure/azure-cli/issues/5688) corrigido: as conclusões não aparecerão se o carregamento da tabela de comando encontrou uma exceção</span><span class="sxs-lookup"><span data-stu-id="bf606-268">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="bf606-269">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="bf606-269">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="bf606-270">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="bf606-270">Monitor</span></span>

* <span data-ttu-id="bf606-271">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="bf606-271">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="bf606-272">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="bf606-272">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="bf606-273">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="bf606-273">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="bf606-274">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="bf606-274">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="bf606-275">Rede</span><span class="sxs-lookup"><span data-stu-id="bf606-275">Network</span></span>

* <span data-ttu-id="bf606-276">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="bf606-276">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="bf606-277">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="bf606-277">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="bf606-278">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="bf606-278">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="bf606-279">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="bf606-279">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="bf606-280">Perfil</span><span class="sxs-lookup"><span data-stu-id="bf606-280">Profile</span></span>

* <span data-ttu-id="bf606-281">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="bf606-281">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="bf606-282">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="bf606-282">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="bf606-283">RDBMS</span><span class="sxs-lookup"><span data-stu-id="bf606-283">RDBMS</span></span>

* <span data-ttu-id="bf606-284">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="bf606-284">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="bf606-285">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="bf606-285">Service Bus</span></span>

* <span data-ttu-id="bf606-286">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="bf606-286">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="bf606-287">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="bf606-287">Storage</span></span>

* <span data-ttu-id="bf606-288">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="bf606-288">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="bf606-289">[5286](https://github.com/Azure/azure-cli/issues/5286) corrigido: os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="bf606-289">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="bf606-290">VM</span><span class="sxs-lookup"><span data-stu-id="bf606-290">VM</span></span>

* <span data-ttu-id="bf606-291">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="bf606-291">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="bf606-292">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="bf606-292">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="bf606-293">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="bf606-293">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="bf606-294">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="bf606-294">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="bf606-295">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="bf606-295">February 27, 2018</span></span>

<span data-ttu-id="bf606-296">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="bf606-296">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="bf606-297">Núcleo</span><span class="sxs-lookup"><span data-stu-id="bf606-297">Core</span></span>

* <span data-ttu-id="bf606-298">Correção [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="bf606-298">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="bf606-299">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="bf606-299">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="bf606-300">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="bf606-300">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="bf606-301">ACS</span><span class="sxs-lookup"><span data-stu-id="bf606-301">ACS</span></span>

* <span data-ttu-id="bf606-302">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="bf606-302">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="bf606-303">Correção do problema de permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="bf606-303">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="bf606-304">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="bf606-304">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="bf606-305">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="bf606-305">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="bf606-306">AppService</span><span class="sxs-lookup"><span data-stu-id="bf606-306">Appservice</span></span>

* <span data-ttu-id="bf606-307">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="bf606-307">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="bf606-308">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="bf606-308">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="bf606-309">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="bf606-309">Cognitive Services</span></span>

* <span data-ttu-id="bf606-310">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="bf606-310">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="bf606-311">Consumo</span><span class="sxs-lookup"><span data-stu-id="bf606-311">Consumption</span></span>

* <span data-ttu-id="bf606-312">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="bf606-312">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="bf606-313">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="bf606-313">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="bf606-314">Contêiner</span><span class="sxs-lookup"><span data-stu-id="bf606-314">Container</span></span>

* <span data-ttu-id="bf606-315">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="bf606-315">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="bf606-316">Rede</span><span class="sxs-lookup"><span data-stu-id="bf606-316">Network</span></span>

* <span data-ttu-id="bf606-317">Correção [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="bf606-317">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="bf606-318">Recurso</span><span class="sxs-lookup"><span data-stu-id="bf606-318">Resource</span></span>

* <span data-ttu-id="bf606-319">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="bf606-319">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="bf606-320">Função</span><span class="sxs-lookup"><span data-stu-id="bf606-320">Role</span></span>

* <span data-ttu-id="bf606-321">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="bf606-321">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="bf606-322">SQL</span><span class="sxs-lookup"><span data-stu-id="bf606-322">SQL</span></span>

* <span data-ttu-id="bf606-323">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="bf606-323">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="bf606-324">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="bf606-324">Storage</span></span>

* <span data-ttu-id="bf606-325">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="bf606-325">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="bf606-326">VM</span><span class="sxs-lookup"><span data-stu-id="bf606-326">VM</span></span>

* <span data-ttu-id="bf606-327">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="bf606-327">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="bf606-328">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="bf606-328">February 13, 2018</span></span>

<span data-ttu-id="bf606-329">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="bf606-329">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="bf606-330">Núcleo</span><span class="sxs-lookup"><span data-stu-id="bf606-330">Core</span></span>

* <span data-ttu-id="bf606-331">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="bf606-331">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="bf606-332">ACS</span><span class="sxs-lookup"><span data-stu-id="bf606-332">ACS</span></span>

* <span data-ttu-id="bf606-333">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="bf606-333">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="bf606-334">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="bf606-334">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="bf606-335">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="bf606-335">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="bf606-336">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="bf606-336">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="bf606-337">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="bf606-337">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="bf606-338">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="bf606-338">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="bf606-339">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="bf606-339">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="bf606-340">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="bf606-340">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="bf606-341">AppService</span><span class="sxs-lookup"><span data-stu-id="bf606-341">Appservice</span></span>

* <span data-ttu-id="bf606-342">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="bf606-342">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="bf606-343">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="bf606-343">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="bf606-344">CDN</span><span class="sxs-lookup"><span data-stu-id="bf606-344">CDN</span></span>

* <span data-ttu-id="bf606-345">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="bf606-345">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="bf606-346">Contêiner</span><span class="sxs-lookup"><span data-stu-id="bf606-346">Container</span></span>

* <span data-ttu-id="bf606-347">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="bf606-347">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="bf606-348">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="bf606-348">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bf606-349">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="bf606-349">CosmosDB</span></span>

* <span data-ttu-id="bf606-350">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="bf606-350">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="bf606-351">Extensão</span><span class="sxs-lookup"><span data-stu-id="bf606-351">Extension</span></span>

* <span data-ttu-id="bf606-352">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="bf606-352">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="bf606-353">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="bf606-353">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="bf606-354">Comentários</span><span class="sxs-lookup"><span data-stu-id="bf606-354">Feedback</span></span>

* <span data-ttu-id="bf606-355">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="bf606-355">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="bf606-356">Interativo</span><span class="sxs-lookup"><span data-stu-id="bf606-356">Interactive</span></span>

* <span data-ttu-id="bf606-357">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="bf606-357">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="bf606-358">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="bf606-358">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="bf606-359">IoT</span><span class="sxs-lookup"><span data-stu-id="bf606-359">IoT</span></span>

* <span data-ttu-id="bf606-360">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="bf606-360">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="bf606-361">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="bf606-361">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="bf606-362">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bf606-362">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="bf606-363">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="bf606-363">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="bf606-364">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="bf606-364">Monitor</span></span>

* <span data-ttu-id="bf606-365">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="bf606-365">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="bf606-366">Rede</span><span class="sxs-lookup"><span data-stu-id="bf606-366">Network</span></span>

* <span data-ttu-id="bf606-367">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="bf606-367">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="bf606-368">Perfil</span><span class="sxs-lookup"><span data-stu-id="bf606-368">Profile</span></span>

* <span data-ttu-id="bf606-369">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="bf606-369">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="bf606-370">Recurso</span><span class="sxs-lookup"><span data-stu-id="bf606-370">Resource</span></span>

* <span data-ttu-id="bf606-371">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="bf606-371">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="bf606-372">Função</span><span class="sxs-lookup"><span data-stu-id="bf606-372">Role</span></span>

* <span data-ttu-id="bf606-373">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="bf606-373">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="bf606-374">SQL</span><span class="sxs-lookup"><span data-stu-id="bf606-374">SQL</span></span>

* <span data-ttu-id="bf606-375">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="bf606-375">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="bf606-376">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="bf606-376">Added `sql db rename`</span></span>
* <span data-ttu-id="bf606-377">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="bf606-377">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="bf606-378">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="bf606-378">Storage</span></span>

* <span data-ttu-id="bf606-379">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="bf606-379">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="bf606-380">VM</span><span class="sxs-lookup"><span data-stu-id="bf606-380">VM</span></span>

* <span data-ttu-id="bf606-381">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="bf606-381">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="bf606-382">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="bf606-382">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="bf606-383">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="bf606-383">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="bf606-384">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="bf606-384">January 31, 2018</span></span>

<span data-ttu-id="bf606-385">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="bf606-385">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="bf606-386">Núcleo</span><span class="sxs-lookup"><span data-stu-id="bf606-386">Core</span></span>

* <span data-ttu-id="bf606-387">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="bf606-387">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="bf606-388">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="bf606-388">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="bf606-389">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="bf606-389">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="bf606-390">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="bf606-390">Use `--verbose` to see</span></span>
* <span data-ttu-id="bf606-391">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="bf606-391">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="bf606-392">ACS</span><span class="sxs-lookup"><span data-stu-id="bf606-392">ACS</span></span>

* <span data-ttu-id="bf606-393">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="bf606-393">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="bf606-394">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="bf606-394">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="bf606-395">AppService</span><span class="sxs-lookup"><span data-stu-id="bf606-395">Appservice</span></span>

* <span data-ttu-id="bf606-396">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="bf606-396">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="bf606-397">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="bf606-397">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="bf606-398">CDN</span><span class="sxs-lookup"><span data-stu-id="bf606-398">CDN</span></span>

* <span data-ttu-id="bf606-399">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="bf606-399">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bf606-400">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="bf606-400">CosmosDB</span></span>

* <span data-ttu-id="bf606-401">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="bf606-401">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="bf606-402">Interativo</span><span class="sxs-lookup"><span data-stu-id="bf606-402">Interactive</span></span>

* <span data-ttu-id="bf606-403">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="bf606-403">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="bf606-404">Rede</span><span class="sxs-lookup"><span data-stu-id="bf606-404">Network</span></span>

* <span data-ttu-id="bf606-405">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="bf606-405">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="bf606-406">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="bf606-406">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="bf606-407">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="bf606-407">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="bf606-408">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="bf606-408">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="bf606-409">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="bf606-409">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="bf606-410">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="bf606-410">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="bf606-411">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="bf606-411">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="bf606-412">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="bf606-412">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="bf606-413">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="bf606-413">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="bf606-414">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="bf606-414">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="bf606-415">Perfil</span><span class="sxs-lookup"><span data-stu-id="bf606-415">Profile</span></span>

* <span data-ttu-id="bf606-416">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="bf606-416">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="bf606-417">Recurso</span><span class="sxs-lookup"><span data-stu-id="bf606-417">Resource</span></span>

* <span data-ttu-id="bf606-418">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="bf606-418">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="bf606-419">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="bf606-419">Storage</span></span>

* <span data-ttu-id="bf606-420">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="bf606-420">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="bf606-421">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="bf606-421">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="bf606-422">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="bf606-422">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="bf606-423">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="bf606-423">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="bf606-424">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="bf606-424">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="bf606-425">VM</span><span class="sxs-lookup"><span data-stu-id="bf606-425">VM</span></span>

* <span data-ttu-id="bf606-426">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="bf606-426">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="bf606-427">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="bf606-427">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="bf606-428">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="bf606-428">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="bf606-429">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="bf606-429">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="bf606-430">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="bf606-430">January 17, 2018</span></span>

<span data-ttu-id="bf606-431">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="bf606-431">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="bf606-432">ACR</span><span class="sxs-lookup"><span data-stu-id="bf606-432">ACR</span></span>

* <span data-ttu-id="bf606-433">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="bf606-433">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="bf606-434">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="bf606-434">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="bf606-435">ACS</span><span class="sxs-lookup"><span data-stu-id="bf606-435">ACS</span></span>

* <span data-ttu-id="bf606-436">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="bf606-436">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="bf606-437">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="bf606-437">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="bf606-438">AppService</span><span class="sxs-lookup"><span data-stu-id="bf606-438">Appservice</span></span>

* <span data-ttu-id="bf606-439">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="bf606-439">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="bf606-440">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="bf606-440">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="bf606-441">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="bf606-441">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="bf606-442">Backup</span><span class="sxs-lookup"><span data-stu-id="bf606-442">Backup</span></span>

* <span data-ttu-id="bf606-443">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="bf606-443">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="bf606-444">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="bf606-444">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="bf606-445">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="bf606-445">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="bf606-446">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="bf606-446">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="bf606-447">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="bf606-447">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="bf606-448">Batch</span><span class="sxs-lookup"><span data-stu-id="bf606-448">Batch</span></span>

* <span data-ttu-id="bf606-449">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="bf606-449">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="bf606-450">Nuvem</span><span class="sxs-lookup"><span data-stu-id="bf606-450">Cloud</span></span>

* <span data-ttu-id="bf606-451">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="bf606-451">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="bf606-452">Consumo</span><span class="sxs-lookup"><span data-stu-id="bf606-452">Consumption</span></span>

* <span data-ttu-id="bf606-453">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="bf606-453">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="bf606-454">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="bf606-454">Event Grid</span></span>

* <span data-ttu-id="bf606-455">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="bf606-455">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="bf606-456">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="bf606-456">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="bf606-457">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="bf606-457">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="bf606-458">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="bf606-458">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="bf606-459">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="bf606-459">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="bf606-460">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="bf606-460">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="bf606-461">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="bf606-461">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="bf606-462">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="bf606-462">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="bf606-463">Interativo</span><span class="sxs-lookup"><span data-stu-id="bf606-463">Interactive</span></span>

* <span data-ttu-id="bf606-464">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="bf606-464">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="bf606-465">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="bf606-465">Fixed errors on startup</span></span>
* <span data-ttu-id="bf606-466">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="bf606-466">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="bf606-467">IoT</span><span class="sxs-lookup"><span data-stu-id="bf606-467">IoT</span></span>

* <span data-ttu-id="bf606-468">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="bf606-468">Added support for device provisioning service</span></span>
* <span data-ttu-id="bf606-469">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="bf606-469">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="bf606-470">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="bf606-470">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="bf606-471">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="bf606-471">Monitor</span></span>

* <span data-ttu-id="bf606-472">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="bf606-472">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="bf606-473">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="bf606-473">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="bf606-474">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="bf606-474">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="bf606-475">Rede</span><span class="sxs-lookup"><span data-stu-id="bf606-475">Network</span></span>

* <span data-ttu-id="bf606-476">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="bf606-476">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="bf606-477">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bf606-477">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="bf606-478">Perfil</span><span class="sxs-lookup"><span data-stu-id="bf606-478">Profile</span></span>

* <span data-ttu-id="bf606-479">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="bf606-479">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="bf606-480">Função</span><span class="sxs-lookup"><span data-stu-id="bf606-480">Role</span></span>

* <span data-ttu-id="bf606-481">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="bf606-481">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="bf606-482">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="bf606-482">Service Fabric</span></span>

* <span data-ttu-id="bf606-483">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="bf606-483">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="bf606-484">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="bf606-484">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="bf606-485">VM</span><span class="sxs-lookup"><span data-stu-id="bf606-485">VM</span></span>

* <span data-ttu-id="bf606-486">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="bf606-486">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="bf606-487">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="bf606-487">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="bf606-488">[ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="bf606-488">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="bf606-489">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="bf606-489">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="bf606-490">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="bf606-490">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="bf606-491">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="bf606-491">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="bf606-492">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="bf606-492">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="bf606-493">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="bf606-493">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="bf606-494">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="bf606-494">December 19, 2017</span></span>

<span data-ttu-id="bf606-495">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="bf606-495">Version 2.0.23</span></span>

* <span data-ttu-id="bf606-496">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="bf606-496">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="bf606-497">Contêiner</span><span class="sxs-lookup"><span data-stu-id="bf606-497">Container</span></span>

* <span data-ttu-id="bf606-498">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="bf606-498">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="bf606-499">Rede</span><span class="sxs-lookup"><span data-stu-id="bf606-499">Network</span></span>

* <span data-ttu-id="bf606-500">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bf606-500">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="bf606-501">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bf606-501">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="bf606-502">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="bf606-502">Storage</span></span>

* <span data-ttu-id="bf606-503">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="bf606-503">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="bf606-504">VM</span><span class="sxs-lookup"><span data-stu-id="bf606-504">VM</span></span>

* <span data-ttu-id="bf606-505">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="bf606-505">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="bf606-506">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="bf606-506">December 5, 2017</span></span>

<span data-ttu-id="bf606-507">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="bf606-507">Version 2.0.22</span></span>

* <span data-ttu-id="bf606-508">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="bf606-508">Removed `az component` commands.</span></span> <span data-ttu-id="bf606-509">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="bf606-509">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="bf606-510">Núcleo</span><span class="sxs-lookup"><span data-stu-id="bf606-510">Core</span></span>
* <span data-ttu-id="bf606-511">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="bf606-511">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="bf606-512">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="bf606-512">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="bf606-513">ACS</span><span class="sxs-lookup"><span data-stu-id="bf606-513">ACS</span></span>

* <span data-ttu-id="bf606-514">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="bf606-514">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="bf606-515">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="bf606-515">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="bf606-516">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="bf606-516">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="bf606-517">Supervisor</span><span class="sxs-lookup"><span data-stu-id="bf606-517">Advisor</span></span>

* <span data-ttu-id="bf606-518">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="bf606-518">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="bf606-519">AppService</span><span class="sxs-lookup"><span data-stu-id="bf606-519">Appservice</span></span>

* <span data-ttu-id="bf606-520">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="bf606-520">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="bf606-521">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="bf606-521">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="bf606-522">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="bf606-522">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="bf606-523">Consumo</span><span class="sxs-lookup"><span data-stu-id="bf606-523">Consumption</span></span>

* <span data-ttu-id="bf606-524">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="bf606-524">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="bf606-525">Contêiner</span><span class="sxs-lookup"><span data-stu-id="bf606-525">Container</span></span>

* <span data-ttu-id="bf606-526">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="bf606-526">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="bf606-527">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="bf606-527">Monitor</span></span>

* <span data-ttu-id="bf606-528">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="bf606-528">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="bf606-529">Recurso</span><span class="sxs-lookup"><span data-stu-id="bf606-529">Resource</span></span>

* <span data-ttu-id="bf606-530">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="bf606-530">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="bf606-531">Função</span><span class="sxs-lookup"><span data-stu-id="bf606-531">Role</span></span>

* <span data-ttu-id="bf606-532">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="bf606-532">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="bf606-533">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="bf606-533">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="bf606-534">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="bf606-534">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="bf606-535">SQL</span><span class="sxs-lookup"><span data-stu-id="bf606-535">SQL</span></span>

* <span data-ttu-id="bf606-536">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="bf606-536">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="bf606-537">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="bf606-537">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="bf606-538">VM</span><span class="sxs-lookup"><span data-stu-id="bf606-538">VM</span></span>

* <span data-ttu-id="bf606-539">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="bf606-539">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="bf606-540">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="bf606-540">November 14, 2017</span></span>

<span data-ttu-id="bf606-541">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="bf606-541">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="bf606-542">ACR</span><span class="sxs-lookup"><span data-stu-id="bf606-542">ACR</span></span>

* <span data-ttu-id="bf606-543">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="bf606-543">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="bf606-544">ACS</span><span class="sxs-lookup"><span data-stu-id="bf606-544">ACS</span></span>

* <span data-ttu-id="bf606-545">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="bf606-545">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="bf606-546">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="bf606-546">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="bf606-547">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="bf606-547">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="bf606-548">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="bf606-548">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="bf606-549">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="bf606-549">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="bf606-550">AppService</span><span class="sxs-lookup"><span data-stu-id="bf606-550">Appservice</span></span>

* <span data-ttu-id="bf606-551">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="bf606-551">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="bf606-552">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="bf606-552">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="bf606-553">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="bf606-553">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="bf606-554">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="bf606-554">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="bf606-555">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="bf606-555">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="bf606-556">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="bf606-556">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="bf606-557">Batch</span><span class="sxs-lookup"><span data-stu-id="bf606-557">Batch</span></span>

* <span data-ttu-id="bf606-558">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="bf606-558">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="bf606-559">Batchai</span><span class="sxs-lookup"><span data-stu-id="bf606-559">Batchai</span></span>

* <span data-ttu-id="bf606-560">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="bf606-560">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="bf606-561">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="bf606-561">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="bf606-562">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="bf606-562">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="bf606-563">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="bf606-563">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="bf606-564">Nuvem</span><span class="sxs-lookup"><span data-stu-id="bf606-564">Cloud</span></span>

* <span data-ttu-id="bf606-565">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="bf606-565">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="bf606-566">Contêiner</span><span class="sxs-lookup"><span data-stu-id="bf606-566">Container</span></span>

* <span data-ttu-id="bf606-567">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="bf606-567">Added support to open multiple ports</span></span>
* <span data-ttu-id="bf606-568">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="bf606-568">Added container group restart policy</span></span>
* <span data-ttu-id="bf606-569">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="bf606-569">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="bf606-570">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="bf606-570">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="bf606-571">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="bf606-571">Data Lake Analytics</span></span>

* <span data-ttu-id="bf606-572">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="bf606-572">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="bf606-573">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="bf606-573">Data Lake Store</span></span>

* <span data-ttu-id="bf606-574">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="bf606-574">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="bf606-575">Extensão</span><span class="sxs-lookup"><span data-stu-id="bf606-575">Extension</span></span>

* <span data-ttu-id="bf606-576">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="bf606-576">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="bf606-577">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="bf606-577">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="bf606-578">IoT</span><span class="sxs-lookup"><span data-stu-id="bf606-578">IoT</span></span>

* <span data-ttu-id="bf606-579">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="bf606-579">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="bf606-580">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="bf606-580">Monitor</span></span>

* <span data-ttu-id="bf606-581">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="bf606-581">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="bf606-582">Rede</span><span class="sxs-lookup"><span data-stu-id="bf606-582">Network</span></span>

* <span data-ttu-id="bf606-583">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="bf606-583">Added support for CAA DNS records</span></span>
* <span data-ttu-id="bf606-584">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="bf606-584">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="bf606-585">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="bf606-585">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="bf606-586">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="bf606-586">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="bf606-587">Reservas</span><span class="sxs-lookup"><span data-stu-id="bf606-587">Reservations</span></span>

* <span data-ttu-id="bf606-588">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="bf606-588">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="bf606-589">Recurso</span><span class="sxs-lookup"><span data-stu-id="bf606-589">Resource</span></span>

* <span data-ttu-id="bf606-590">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="bf606-590">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="bf606-591">SQL</span><span class="sxs-lookup"><span data-stu-id="bf606-591">SQL</span></span>

* <span data-ttu-id="bf606-592">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bf606-592">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="bf606-593">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="bf606-593">Storage</span></span>

* <span data-ttu-id="bf606-594">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="bf606-594">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="bf606-595">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="bf606-595">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="bf606-596">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="bf606-596">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="bf606-597">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="bf606-597">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="bf606-598">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="bf606-598">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="bf606-599">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="bf606-599">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="bf606-600">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bf606-600">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="bf606-601">VM</span><span class="sxs-lookup"><span data-stu-id="bf606-601">VM</span></span>

* <span data-ttu-id="bf606-602">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="bf606-602">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="bf606-603">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="bf606-603">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="bf606-604">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="bf606-604">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="bf606-605">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="bf606-605">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="bf606-606">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="bf606-606">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="bf606-607">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="bf606-607">October 24, 2017</span></span>

<span data-ttu-id="bf606-608">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="bf606-608">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="bf606-609">Núcleo</span><span class="sxs-lookup"><span data-stu-id="bf606-609">Core</span></span>

* <span data-ttu-id="bf606-610">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="bf606-610">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="bf606-611">ACR</span><span class="sxs-lookup"><span data-stu-id="bf606-611">ACR</span></span>

* <span data-ttu-id="bf606-612">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="bf606-612">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="bf606-613">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="bf606-613">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="bf606-614">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="bf606-614">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="bf606-615">ACS</span><span class="sxs-lookup"><span data-stu-id="bf606-615">ACS</span></span>

* <span data-ttu-id="bf606-616">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="bf606-616">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="bf606-617">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="bf606-617">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="bf606-618">AppService</span><span class="sxs-lookup"><span data-stu-id="bf606-618">Appservice</span></span>

* <span data-ttu-id="bf606-619">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="bf606-619">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="bf606-620">Componente</span><span class="sxs-lookup"><span data-stu-id="bf606-620">Component</span></span>

* <span data-ttu-id="bf606-621">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="bf606-621">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="bf606-622">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="bf606-622">Monitor</span></span>

* <span data-ttu-id="bf606-623">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="bf606-623">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="bf606-624">Recurso</span><span class="sxs-lookup"><span data-stu-id="bf606-624">Resource</span></span>

* <span data-ttu-id="bf606-625">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="bf606-625">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="bf606-626">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="bf606-626">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="bf606-627">VM</span><span class="sxs-lookup"><span data-stu-id="bf606-627">VM</span></span>

* <span data-ttu-id="bf606-628">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="bf606-628">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="bf606-629">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="bf606-629">October 9, 2017</span></span>

<span data-ttu-id="bf606-630">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="bf606-630">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="bf606-631">Núcleo</span><span class="sxs-lookup"><span data-stu-id="bf606-631">Core</span></span>

* <span data-ttu-id="bf606-632">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="bf606-632">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="bf606-633">AppService</span><span class="sxs-lookup"><span data-stu-id="bf606-633">Appservice</span></span>

* <span data-ttu-id="bf606-634">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="bf606-634">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="bf606-635">Batch</span><span class="sxs-lookup"><span data-stu-id="bf606-635">Batch</span></span>

* <span data-ttu-id="bf606-636">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="bf606-636">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="bf606-637">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="bf606-637">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="bf606-638">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="bf606-638">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="bf606-639">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="bf606-639">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="bf606-640">Batchai</span><span class="sxs-lookup"><span data-stu-id="bf606-640">Batchai</span></span>

* <span data-ttu-id="bf606-641">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="bf606-641">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="bf606-642">Keyvault</span><span class="sxs-lookup"><span data-stu-id="bf606-642">Keyvault</span></span>

* <span data-ttu-id="bf606-643">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="bf606-643">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="bf606-644">(#4448)</span><span class="sxs-lookup"><span data-stu-id="bf606-644">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="bf606-645">Rede</span><span class="sxs-lookup"><span data-stu-id="bf606-645">Network</span></span>

* <span data-ttu-id="bf606-646">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="bf606-646">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="bf606-647">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="bf606-647">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="bf606-648">Recurso</span><span class="sxs-lookup"><span data-stu-id="bf606-648">Resource</span></span>

* <span data-ttu-id="bf606-649">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="bf606-649">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="bf606-650">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="bf606-650">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="bf606-651">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="bf606-651">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="bf606-652">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="bf606-652">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="bf606-653">Sql</span><span class="sxs-lookup"><span data-stu-id="bf606-653">Sql</span></span>

* <span data-ttu-id="bf606-654">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="bf606-654">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="bf606-655">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="bf606-655">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="bf606-656">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="bf606-656">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="bf606-657">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="bf606-657">Storage</span></span>

* <span data-ttu-id="bf606-658">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="bf606-658">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="bf606-659">VM</span><span class="sxs-lookup"><span data-stu-id="bf606-659">Vm</span></span>

* <span data-ttu-id="bf606-660">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="bf606-660">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="bf606-661">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="bf606-661">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="bf606-662">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="bf606-662">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="bf606-663">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="bf606-663">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="bf606-664">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="bf606-664">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="bf606-665">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="bf606-665">September 22, 2017</span></span>

<span data-ttu-id="bf606-666">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="bf606-666">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="bf606-667">Recurso</span><span class="sxs-lookup"><span data-stu-id="bf606-667">Resource</span></span>

* <span data-ttu-id="bf606-668">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="bf606-668">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="bf606-669">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="bf606-669">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="bf606-670">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="bf606-670">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="bf606-671">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="bf606-671">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="bf606-672">Rede</span><span class="sxs-lookup"><span data-stu-id="bf606-672">Network</span></span>

* <span data-ttu-id="bf606-673">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="bf606-673">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="bf606-674">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="bf606-674">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="bf606-675">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf606-675">Added `asg` application security group commands</span></span>
* <span data-ttu-id="bf606-676">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="bf606-676">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="bf606-677">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bf606-677">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="bf606-678">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bf606-678">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="bf606-679">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="bf606-679">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="bf606-680">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="bf606-680">Storage</span></span>

* <span data-ttu-id="bf606-681">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="bf606-681">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="bf606-682">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="bf606-682">Eventgrid</span></span>

* <span data-ttu-id="bf606-683">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="bf606-683">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="bf606-684">SQL</span><span class="sxs-lookup"><span data-stu-id="bf606-684">SQL</span></span>

* <span data-ttu-id="bf606-685">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="bf606-685">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="bf606-686">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="bf606-686">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="bf606-687">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bf606-687">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="bf606-688">Keyvault</span><span class="sxs-lookup"><span data-stu-id="bf606-688">Keyvault</span></span>

* <span data-ttu-id="bf606-689">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="bf606-689">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="bf606-690">VM</span><span class="sxs-lookup"><span data-stu-id="bf606-690">VM</span></span>

* <span data-ttu-id="bf606-691">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="bf606-691">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="bf606-692">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="bf606-692">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="bf606-693">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="bf606-693">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="bf606-694">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="bf606-694">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="bf606-695">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="bf606-695">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="bf606-696">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="bf606-696">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="bf606-697">ACS</span><span class="sxs-lookup"><span data-stu-id="bf606-697">ACS</span></span>

* <span data-ttu-id="bf606-698">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="bf606-698">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="bf606-699">AppService</span><span class="sxs-lookup"><span data-stu-id="bf606-699">Appservice</span></span>

* <span data-ttu-id="bf606-700">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="bf606-700">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="bf606-701">Backup</span><span class="sxs-lookup"><span data-stu-id="bf606-701">Backup</span></span>

* <span data-ttu-id="bf606-702">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="bf606-702">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="bf606-703">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="bf606-703">September 11, 2017</span></span>

<span data-ttu-id="bf606-704">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="bf606-704">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="bf606-705">Núcleo</span><span class="sxs-lookup"><span data-stu-id="bf606-705">Core</span></span>

* <span data-ttu-id="bf606-706">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="bf606-706">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="bf606-707">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="bf606-707">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="bf606-708">Acs</span><span class="sxs-lookup"><span data-stu-id="bf606-708">Acs</span></span>

* <span data-ttu-id="bf606-709">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="bf606-709">Added `acs list-locations` command</span></span>
* <span data-ttu-id="bf606-710">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="bf606-710">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="bf606-711">AppService</span><span class="sxs-lookup"><span data-stu-id="bf606-711">Appservice</span></span>

* <span data-ttu-id="bf606-712">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="bf606-712">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="bf606-713">CDN</span><span class="sxs-lookup"><span data-stu-id="bf606-713">CDN</span></span>

* <span data-ttu-id="bf606-714">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="bf606-714">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="bf606-715">Extensão</span><span class="sxs-lookup"><span data-stu-id="bf606-715">Extension</span></span>

* <span data-ttu-id="bf606-716">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="bf606-716">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="bf606-717">Keyvault</span><span class="sxs-lookup"><span data-stu-id="bf606-717">Keyvault</span></span>

* <span data-ttu-id="bf606-718">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="bf606-718">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="bf606-719">Rede</span><span class="sxs-lookup"><span data-stu-id="bf606-719">Network</span></span>

* <span data-ttu-id="bf606-720">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="bf606-720">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="bf606-721">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="bf606-721">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="bf606-722">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="bf606-722">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="bf606-723">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="bf606-723">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="bf606-724">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="bf606-724">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="bf606-725">Recurso</span><span class="sxs-lookup"><span data-stu-id="bf606-725">Resource</span></span>

* <span data-ttu-id="bf606-726">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="bf606-726">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="bf606-727">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="bf606-727">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="bf606-728">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="bf606-728">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="bf606-729">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="bf606-729">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="bf606-730">SQL</span><span class="sxs-lookup"><span data-stu-id="bf606-730">SQL</span></span>

* <span data-ttu-id="bf606-731">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="bf606-731">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="bf606-732">VM</span><span class="sxs-lookup"><span data-stu-id="bf606-732">VM</span></span>

* <span data-ttu-id="bf606-733">Corrigido: Não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="bf606-733">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="bf606-734">Corrigido: Usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="bf606-734">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="bf606-735">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="bf606-735">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="bf606-736">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="bf606-736">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="bf606-737">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="bf606-737">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="bf606-738">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="bf606-738">August 31, 2017</span></span>

<span data-ttu-id="bf606-739">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="bf606-739">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="bf606-740">Keyvault</span><span class="sxs-lookup"><span data-stu-id="bf606-740">Keyvault</span></span>

* <span data-ttu-id="bf606-741">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="bf606-741">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="bf606-742">Sf</span><span class="sxs-lookup"><span data-stu-id="bf606-742">Sf</span></span>

* <span data-ttu-id="bf606-743">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="bf606-743">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="bf606-744">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="bf606-744">Storage</span></span>

* <span data-ttu-id="bf606-745">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="bf606-745">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="bf606-746">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="bf606-746">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="bf606-747">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="bf606-747">August 28, 2017</span></span>

<span data-ttu-id="bf606-748">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="bf606-748">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="bf606-749">CLI</span><span class="sxs-lookup"><span data-stu-id="bf606-749">CLI</span></span>

* <span data-ttu-id="bf606-750">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="bf606-750">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="bf606-751">ACS</span><span class="sxs-lookup"><span data-stu-id="bf606-751">ACS</span></span>

* <span data-ttu-id="bf606-752">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="bf606-752">Corrected preview regions</span></span>
* <span data-ttu-id="bf606-753">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="bf606-753">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="bf606-754">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="bf606-754">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="bf606-755">AppService</span><span class="sxs-lookup"><span data-stu-id="bf606-755">Appservice</span></span>

* <span data-ttu-id="bf606-756">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="bf606-756">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="bf606-757">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="bf606-757">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="bf606-758">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="bf606-758">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="bf606-759">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf606-759">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="bf606-760">Correção: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="bf606-760">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="bf606-761">IoT</span><span class="sxs-lookup"><span data-stu-id="bf606-761">IoT</span></span>

* <span data-ttu-id="bf606-762">Correção #3934: Criação de política não limpa as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="bf606-762">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="bf606-763">Rede</span><span class="sxs-lookup"><span data-stu-id="bf606-763">Network</span></span>

* <span data-ttu-id="bf606-764">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="bf606-764">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="bf606-765">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bf606-765">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="bf606-766">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bf606-766">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="bf606-767">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="bf606-767">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="bf606-768">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="bf606-768">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="bf606-769">Perfil</span><span class="sxs-lookup"><span data-stu-id="bf606-769">Profile</span></span>

* <span data-ttu-id="bf606-770">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="bf606-770">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="bf606-771">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="bf606-771">Service Fabric</span></span>

* <span data-ttu-id="bf606-772">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="bf606-772">Preview release</span></span>
* <span data-ttu-id="bf606-773">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="bf606-773">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="bf606-774">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="bf606-774">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="bf606-775">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="bf606-775">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="bf606-776">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="bf606-776">Storage</span></span>

* <span data-ttu-id="bf606-777">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="bf606-777">Enabled setting blob tier</span></span>
* <span data-ttu-id="bf606-778">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="bf606-778">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="bf606-779">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="bf606-779">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="bf606-780">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="bf606-780">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="bf606-781">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="bf606-781">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="bf606-782">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="bf606-782">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="bf606-783">VM</span><span class="sxs-lookup"><span data-stu-id="bf606-783">VM</span></span>

* <span data-ttu-id="bf606-784">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="bf606-784">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="bf606-785">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="bf606-785">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="bf606-786">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="bf606-786">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="bf606-787">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="bf606-787">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="bf606-788">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="bf606-788">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="bf606-789">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="bf606-789">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="bf606-790">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="bf606-790">August 15, 2017</span></span>

<span data-ttu-id="bf606-791">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="bf606-791">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="bf606-792">ACS</span><span class="sxs-lookup"><span data-stu-id="bf606-792">ACS</span></span>

* <span data-ttu-id="bf606-793">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="bf606-793">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="bf606-794">AppService</span><span class="sxs-lookup"><span data-stu-id="bf606-794">Appservice</span></span>

* <span data-ttu-id="bf606-795">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="bf606-795">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="bf606-796">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="bf606-796">Event Grid</span></span>

* <span data-ttu-id="bf606-797">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="bf606-797">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="bf606-798">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="bf606-798">August 11, 2017</span></span>

<span data-ttu-id="bf606-799">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="bf606-799">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="bf606-800">ACS</span><span class="sxs-lookup"><span data-stu-id="bf606-800">ACS</span></span>

* <span data-ttu-id="bf606-801">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="bf606-801">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="bf606-802">Batch</span><span class="sxs-lookup"><span data-stu-id="bf606-802">Batch</span></span>

* <span data-ttu-id="bf606-803">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="bf606-803">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="bf606-804">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="bf606-804">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="bf606-805">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="bf606-805">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="bf606-806">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="bf606-806">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="bf606-807">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="bf606-807">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="bf606-808">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="bf606-808">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="bf606-809">Componente</span><span class="sxs-lookup"><span data-stu-id="bf606-809">Component</span></span>

* <span data-ttu-id="bf606-810">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="bf606-810">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="bf606-811">Contêiner</span><span class="sxs-lookup"><span data-stu-id="bf606-811">Container</span></span>

* <span data-ttu-id="bf606-812">`create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="bf606-812">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="bf606-813">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="bf606-813">Data Lake Store</span></span>

* <span data-ttu-id="bf606-814">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="bf606-814">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="bf606-815">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="bf606-815">Event Grid</span></span>

* <span data-ttu-id="bf606-816">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="bf606-816">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="bf606-817">Rede</span><span class="sxs-lookup"><span data-stu-id="bf606-817">Network</span></span>

* <span data-ttu-id="bf606-818">`lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="bf606-818">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="bf606-819">`application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="bf606-819">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="bf606-820">`application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="bf606-820">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="bf606-821">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="bf606-821">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="bf606-822">Perfil</span><span class="sxs-lookup"><span data-stu-id="bf606-822">Profile</span></span>

* <span data-ttu-id="bf606-823">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="bf606-823">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="bf606-824">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="bf606-824">Storage</span></span>

* <span data-ttu-id="bf606-825">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="bf606-825">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="bf606-826">VM</span><span class="sxs-lookup"><span data-stu-id="bf606-826">VM</span></span>

* <span data-ttu-id="bf606-827">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="bf606-827">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="bf606-828">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="bf606-828">Exposed `list-skus` command</span></span>
* <span data-ttu-id="bf606-829">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="bf606-829">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="bf606-830">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="bf606-830">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="bf606-831">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="bf606-831">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="bf606-832">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="bf606-832">July 28, 2017</span></span>

<span data-ttu-id="bf606-833">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="bf606-833">Version 2.0.12</span></span>

* <span data-ttu-id="bf606-834">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="bf606-834">Added container commands</span></span>
* <span data-ttu-id="bf606-835">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="bf606-835">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="bf606-836">Núcleo</span><span class="sxs-lookup"><span data-stu-id="bf606-836">Core</span></span>

* <span data-ttu-id="bf606-837">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="bf606-837">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="bf606-838">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="bf606-838">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="bf606-839">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="bf606-839">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="bf606-840">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="bf606-840">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="bf606-841">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="bf606-841">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="bf606-842">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="bf606-842">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="bf606-843">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="bf606-843">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="bf606-844">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="bf606-844">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="bf606-845">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="bf606-845">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="bf606-846">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="bf606-846">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="bf606-847">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="bf606-847">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="bf606-848">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="bf606-848">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="bf606-849">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="bf606-849">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="bf606-850">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="bf606-850">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="bf606-851">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="bf606-851">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="bf606-852">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="bf606-852">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="bf606-853">ACR</span><span class="sxs-lookup"><span data-stu-id="bf606-853">ACR</span></span>

* <span data-ttu-id="bf606-854">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="bf606-854">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="bf606-855">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="bf606-855">Support SKU update for managed registries</span></span>
* <span data-ttu-id="bf606-856">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="bf606-856">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="bf606-857">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="bf606-857">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="bf606-858">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="bf606-858">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="bf606-859">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="bf606-859">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="bf606-860">ACS</span><span class="sxs-lookup"><span data-stu-id="bf606-860">ACS</span></span>

* <span data-ttu-id="bf606-861">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="bf606-861">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="bf606-862">AppService</span><span class="sxs-lookup"><span data-stu-id="bf606-862">Appservice</span></span>

* <span data-ttu-id="bf606-863">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="bf606-863">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="bf606-864">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="bf606-864">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="bf606-865">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="bf606-865">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="bf606-866">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="bf606-866">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="bf606-867">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="bf606-867">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="bf606-868">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="bf606-868">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="bf606-869">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="bf606-869">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="bf606-870">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="bf606-870">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="bf606-871">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="bf606-871">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="bf606-872">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="bf606-872">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="bf606-873">Batch</span><span class="sxs-lookup"><span data-stu-id="bf606-873">Batch</span></span>

* <span data-ttu-id="bf606-874">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="bf606-874">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="bf606-875">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="bf606-875">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="bf606-876">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="bf606-876">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="bf606-877">CDN</span><span class="sxs-lookup"><span data-stu-id="bf606-877">CDN</span></span>

* <span data-ttu-id="bf606-878">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="bf606-878">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="bf606-879">Nuvem</span><span class="sxs-lookup"><span data-stu-id="bf606-879">Cloud</span></span>

* <span data-ttu-id="bf606-880">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="bf606-880">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="bf606-881">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="bf606-881">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="bf606-882">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="bf606-882">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="bf606-883">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="bf606-883">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="bf606-884">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="bf606-884">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bf606-885">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="bf606-885">CosmosDB</span></span>

* <span data-ttu-id="bf606-886">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="bf606-886">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="bf606-887">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="bf606-887">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="bf606-888">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="bf606-888">Data Lake Analytics</span></span>

* <span data-ttu-id="bf606-889">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="bf606-889">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="bf606-890">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="bf606-890">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="bf606-891">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="bf606-891">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="bf606-892">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="bf606-892">Data Lake Store</span></span>

* <span data-ttu-id="bf606-893">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="bf606-893">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="bf606-894">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="bf606-894">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="bf606-895">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="bf606-895">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="bf606-896">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="bf606-896">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="bf606-897">Interativo</span><span class="sxs-lookup"><span data-stu-id="bf606-897">Interactive</span></span>

* <span data-ttu-id="bf606-898">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="bf606-898">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="bf606-899">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="bf606-899">Increased test coverage</span></span>
* <span data-ttu-id="bf606-900">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="bf606-900">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="bf606-901">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="bf606-901">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="bf606-902">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="bf606-902">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="bf606-903">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="bf606-903">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="bf606-904">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="bf606-904">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="bf606-905">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="bf606-905">Added `--progress` flag</span></span>
* <span data-ttu-id="bf606-906">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="bf606-906">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="bf606-907">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="bf606-907">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="bf606-908">IoT</span><span class="sxs-lookup"><span data-stu-id="bf606-908">IoT</span></span>

* <span data-ttu-id="bf606-909">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="bf606-909">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="bf606-910">(#3934)</span><span class="sxs-lookup"><span data-stu-id="bf606-910">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="bf606-911">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="bf606-911">Key vault</span></span>

* <span data-ttu-id="bf606-912">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="bf606-912">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="bf606-913">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="bf606-913">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="bf606-914">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="bf606-914">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="bf606-915">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="bf606-915">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="bf606-916">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="bf606-916">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="bf606-917">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="bf606-917">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="bf606-918">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="bf606-918">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="bf606-919">(#3307)</span><span class="sxs-lookup"><span data-stu-id="bf606-919">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="bf606-920">Laboratório</span><span class="sxs-lookup"><span data-stu-id="bf606-920">Lab</span></span>

* <span data-ttu-id="bf606-921">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="bf606-921">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="bf606-922">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="bf606-922">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="bf606-923">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="bf606-923">Monitor</span></span>

* <span data-ttu-id="bf606-924">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="bf606-924">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="bf606-925">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="bf606-925">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="bf606-926">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="bf606-926">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="bf606-927">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="bf606-927">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="bf606-928">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="bf606-928">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="bf606-929">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="bf606-929">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="bf606-930">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="bf606-930">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="bf606-931">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="bf606-931">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="bf606-932">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="bf606-932">`location` no longer required</span></span>
  * <span data-ttu-id="bf606-933">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="bf606-933">Add name and ID support for target</span></span>
  * <span data-ttu-id="bf606-934">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="bf606-934">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="bf606-935">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="bf606-935">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="bf606-936">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="bf606-936">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="bf606-937">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="bf606-937">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="bf606-938">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="bf606-938">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="bf606-939">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="bf606-939">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="bf606-940">Rede</span><span class="sxs-lookup"><span data-stu-id="bf606-940">Network</span></span>

* <span data-ttu-id="bf606-941">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="bf606-941">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="bf606-942">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="bf606-942">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="bf606-943">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="bf606-943">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="bf606-944">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="bf606-944">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="bf606-945">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="bf606-945">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="bf606-946">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="bf606-946">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="bf606-947">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="bf606-947">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="bf606-948">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="bf606-948">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="bf606-949">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="bf606-949">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="bf606-950">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="bf606-950">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="bf606-951">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="bf606-951">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="bf606-952">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="bf606-952">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="bf606-953">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="bf606-953">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="bf606-954">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="bf606-954">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="bf606-955">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="bf606-955">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="bf606-956">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="bf606-956">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="bf606-957">Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS</span><span class="sxs-lookup"><span data-stu-id="bf606-957">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="bf606-958">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="bf606-958">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="bf606-959">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="bf606-959">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="bf606-960">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="bf606-960">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="bf606-961">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="bf606-961">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="bf606-962">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="bf606-962">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="bf606-963">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="bf606-963">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="bf606-964">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="bf606-964">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="bf606-965">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="bf606-965">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="bf606-966">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="bf606-966">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="bf606-967">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="bf606-967">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="bf606-968">Perfil</span><span class="sxs-lookup"><span data-stu-id="bf606-968">Profile</span></span>

* <span data-ttu-id="bf606-969">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="bf606-969">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="bf606-970">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="bf606-970">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="bf606-971">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="bf606-971">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="bf606-972">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="bf606-972">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="bf606-973">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="bf606-973">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="bf606-974">RDBMS</span><span class="sxs-lookup"><span data-stu-id="bf606-974">RDBMS</span></span>

* <span data-ttu-id="bf606-975">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="bf606-975">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="bf606-976">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="bf606-976">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="bf606-977">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="bf606-977">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="bf606-978">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="bf606-978">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="bf606-979">Recurso</span><span class="sxs-lookup"><span data-stu-id="bf606-979">Resource</span></span>

* <span data-ttu-id="bf606-980">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="bf606-980">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="bf606-981">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="bf606-981">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="bf606-982">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="bf606-982">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="bf606-983">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="bf606-983">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="bf606-984">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="bf606-984">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="bf606-985">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="bf606-985">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="bf606-986">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="bf606-986">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="bf606-987">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="bf606-987">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="bf606-988">Função</span><span class="sxs-lookup"><span data-stu-id="bf606-988">Role</span></span>

* <span data-ttu-id="bf606-989">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="bf606-989">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="bf606-990">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="bf606-990">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="bf606-991">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="bf606-991">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="bf606-992">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="bf606-992">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="bf606-993">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="bf606-993">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="bf606-994">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="bf606-994">Service Fabric</span></span>
* <span data-ttu-id="bf606-995">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="bf606-995">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="bf606-996">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="bf606-996">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="bf606-997">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="bf606-997">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="bf606-998">SQL</span><span class="sxs-lookup"><span data-stu-id="bf606-998">SQL</span></span>

* <span data-ttu-id="bf606-999">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="bf606-999">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="bf606-1000">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="bf606-1000">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="bf606-1001">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="bf606-1001">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="bf606-1002">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="bf606-1002">Storage</span></span>

* <span data-ttu-id="bf606-1003">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="bf606-1003">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="bf606-1004">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="bf606-1004">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="bf606-1005">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="bf606-1005">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="bf606-1006">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="bf606-1006">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="bf606-1007">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="bf606-1007">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="bf606-1008">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="bf606-1008">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="bf606-1009">VM</span><span class="sxs-lookup"><span data-stu-id="bf606-1009">VM</span></span>

* <span data-ttu-id="bf606-1010">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="bf606-1010">Support configuring nsg</span></span>
* <span data-ttu-id="bf606-1011">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="bf606-1011">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="bf606-1012">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="bf606-1012">Support managed service identities</span></span>
* <span data-ttu-id="bf606-1013">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="bf606-1013">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="bf606-1014">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="bf606-1014">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="bf606-1015">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="bf606-1015">May 10, 2017</span></span>

<span data-ttu-id="bf606-1016">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="bf606-1016">Version 2.0.6</span></span>

* <span data-ttu-id="bf606-1017">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="bf606-1017">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="bf606-1018">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="bf606-1018">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="bf606-1019">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="bf606-1019">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="bf606-1020">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="bf606-1020">Include Cognitive Services module</span></span>
* <span data-ttu-id="bf606-1021">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="bf606-1021">Include Service Fabric module</span></span>
* <span data-ttu-id="bf606-1022">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="bf606-1022">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="bf606-1023">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="bf606-1023">Add support for CDN commands</span></span>
* <span data-ttu-id="bf606-1024">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="bf606-1024">Remove Container module</span></span>
* <span data-ttu-id="bf606-1025">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="bf606-1025">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="bf606-1026">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="bf606-1026">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="bf606-1027">Núcleo</span><span class="sxs-lookup"><span data-stu-id="bf606-1027">Core</span></span>

* <span data-ttu-id="bf606-1028">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="bf606-1028">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="bf606-1029">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="bf606-1029">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="bf606-1030">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="bf606-1030">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="bf606-1031">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="bf606-1031">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="bf606-1032">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="bf606-1032">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="bf606-1033">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="bf606-1033">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="bf606-1034">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="bf606-1034">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="bf606-1035">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="bf606-1035">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="bf606-1036">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="bf606-1036">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="bf606-1037">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="bf606-1037">core: Improved performance</span></span>
* <span data-ttu-id="bf606-1038">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="bf606-1038">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="bf606-1039">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="bf606-1039">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="bf606-1040">ACS</span><span class="sxs-lookup"><span data-stu-id="bf606-1040">ACS</span></span>

* <span data-ttu-id="bf606-1041">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf606-1041">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="bf606-1042">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="bf606-1042">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="bf606-1043">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="bf606-1043">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="bf606-1044">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="bf606-1044">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="bf606-1045">AppService</span><span class="sxs-lookup"><span data-stu-id="bf606-1045">AppService</span></span>

* <span data-ttu-id="bf606-1046">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="bf606-1046">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="bf606-1047">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="bf606-1047">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="bf606-1048">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="bf606-1048">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="bf606-1049">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="bf606-1049">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="bf606-1050">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="bf606-1050">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="bf606-1051">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="bf606-1051">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="bf606-1052">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="bf606-1052">support slot swap with preview</span></span>
* <span data-ttu-id="bf606-1053">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="bf606-1053">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="bf606-1054">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="bf606-1054">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bf606-1055">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="bf606-1055">CosmosDB</span></span>

* <span data-ttu-id="bf606-1056">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="bf606-1056">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="bf606-1057">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="bf606-1057">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="bf606-1058">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="bf606-1058">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="bf606-1059">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="bf606-1059">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="bf606-1060">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="bf606-1060">Data Lake Analytics</span></span>

* <span data-ttu-id="bf606-1061">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="bf606-1061">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="bf606-1062">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="bf606-1062">Add support for new catalog item type: package.</span></span> <span data-ttu-id="bf606-1063">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="bf606-1063">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="bf606-1064">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="bf606-1064">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="bf606-1065">Tabela</span><span class="sxs-lookup"><span data-stu-id="bf606-1065">Table</span></span>
  * <span data-ttu-id="bf606-1066">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="bf606-1066">Table valued function</span></span>
  * <span data-ttu-id="bf606-1067">Visualizar</span><span class="sxs-lookup"><span data-stu-id="bf606-1067">View</span></span>
  * <span data-ttu-id="bf606-1068">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="bf606-1068">Table Statistics.</span></span> <span data-ttu-id="bf606-1069">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="bf606-1069">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="bf606-1070">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="bf606-1070">Data Lake Store</span></span>

* <span data-ttu-id="bf606-1071">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="bf606-1071">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="bf606-1072">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="bf606-1072">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="bf606-1073">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="bf606-1073">missed help for access show.</span></span> <span data-ttu-id="bf606-1074">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="bf606-1074">adding it.</span></span> <span data-ttu-id="bf606-1075">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="bf606-1075">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="bf606-1076">Localizar</span><span class="sxs-lookup"><span data-stu-id="bf606-1076">Find</span></span>

* <span data-ttu-id="bf606-1077">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="bf606-1077">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="bf606-1078">KeyVault</span><span class="sxs-lookup"><span data-stu-id="bf606-1078">KeyVault</span></span>

* <span data-ttu-id="bf606-1079">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="bf606-1079">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="bf606-1080">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="bf606-1080">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="bf606-1081">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="bf606-1081">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="bf606-1082">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="bf606-1082">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="bf606-1083">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="bf606-1083">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="bf606-1084">Laboratório</span><span class="sxs-lookup"><span data-stu-id="bf606-1084">Lab</span></span>

* <span data-ttu-id="bf606-1085">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="bf606-1085">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="bf606-1086">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="bf606-1086">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="bf606-1087">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="bf606-1087">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="bf606-1088">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="bf606-1088">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="bf606-1089">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="bf606-1089">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="bf606-1090">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="bf606-1090">Monitor</span></span>

* <span data-ttu-id="bf606-1091">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="bf606-1091">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="bf606-1092">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="bf606-1092">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="bf606-1093">Rede</span><span class="sxs-lookup"><span data-stu-id="bf606-1093">Network</span></span>

* <span data-ttu-id="bf606-1094">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="bf606-1094">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="bf606-1095">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="bf606-1095">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="bf606-1096">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf606-1096">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="bf606-1097">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf606-1097">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="bf606-1098">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="bf606-1098">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="bf606-1099">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="bf606-1099">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="bf606-1100">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="bf606-1100">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="bf606-1101">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="bf606-1101">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="bf606-1102">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="bf606-1102">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="bf606-1103">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="bf606-1103">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="bf606-1104">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="bf606-1104">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="bf606-1105">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="bf606-1105">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="bf606-1106">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="bf606-1106">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="bf606-1107">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="bf606-1107">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="bf606-1108">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="bf606-1108">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="bf606-1109">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="bf606-1109">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="bf606-1110">Perfil</span><span class="sxs-lookup"><span data-stu-id="bf606-1110">Profile</span></span>

* <span data-ttu-id="bf606-1111">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="bf606-1111">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="bf606-1112">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="bf606-1112">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="bf606-1113">Redis</span><span class="sxs-lookup"><span data-stu-id="bf606-1113">Redis</span></span>

* <span data-ttu-id="bf606-1114">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="bf606-1114">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="bf606-1115">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="bf606-1115">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="bf606-1116">Recurso</span><span class="sxs-lookup"><span data-stu-id="bf606-1116">Resource</span></span>

* <span data-ttu-id="bf606-1117">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="bf606-1117">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="bf606-1118">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="bf606-1118">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="bf606-1119">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="bf606-1119">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="bf606-1120">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="bf606-1120">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="bf606-1121">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="bf606-1121">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="bf606-1122">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="bf606-1122">Add docs for az lock update.</span></span> <span data-ttu-id="bf606-1123">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="bf606-1123">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="bf606-1124">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="bf606-1124">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="bf606-1125">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="bf606-1125">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="bf606-1126">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="bf606-1126">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="bf606-1127">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="bf606-1127">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="bf606-1128">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="bf606-1128">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="bf606-1129">Função</span><span class="sxs-lookup"><span data-stu-id="bf606-1129">Role</span></span>

* <span data-ttu-id="bf606-1130">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="bf606-1130">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="bf606-1131">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="bf606-1131">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="bf606-1132">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="bf606-1132">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="bf606-1133">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="bf606-1133">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="bf606-1134">SQL</span><span class="sxs-lookup"><span data-stu-id="bf606-1134">SQL</span></span>

* <span data-ttu-id="bf606-1135">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="bf606-1135">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="bf606-1136">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="bf606-1136">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="bf606-1137">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="bf606-1137">Storage</span></span>

* <span data-ttu-id="bf606-1138">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="bf606-1138">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="bf606-1139">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="bf606-1139">Add support for incremental blob copy</span></span>
* <span data-ttu-id="bf606-1140">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="bf606-1140">Add support for large block blob upload</span></span>
* <span data-ttu-id="bf606-1141">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="bf606-1141">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="bf606-1142">VM</span><span class="sxs-lookup"><span data-stu-id="bf606-1142">VM</span></span>

* <span data-ttu-id="bf606-1143">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="bf606-1143">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="bf606-1144">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="bf606-1144">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="bf606-1145">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="bf606-1145">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="bf606-1146">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="bf606-1146">az vm/vmss disk</span></span>
  3. <span data-ttu-id="bf606-1147">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="bf606-1147">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="bf606-1148">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="bf606-1148">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="bf606-1149">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="bf606-1149">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="bf606-1150">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="bf606-1150">April 3, 2017</span></span>

<span data-ttu-id="bf606-1151">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="bf606-1151">Version 2.0.2</span></span>

<span data-ttu-id="bf606-1152">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="bf606-1152">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="bf606-1153">Núcleo</span><span class="sxs-lookup"><span data-stu-id="bf606-1153">Core</span></span>

* <span data-ttu-id="bf606-1154">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="bf606-1154">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="bf606-1155">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="bf606-1155">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="bf606-1156">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="bf606-1156">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="bf606-1157">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="bf606-1157">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="bf606-1158">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="bf606-1158">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="bf606-1159">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="bf606-1159">Add prompting for missing template parameters.</span></span> <span data-ttu-id="bf606-1160">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="bf606-1160">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="bf606-1161">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="bf606-1161">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="bf606-1162">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="bf606-1162">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="bf606-1163">ACS</span><span class="sxs-lookup"><span data-stu-id="bf606-1163">ACS</span></span>

* <span data-ttu-id="bf606-1164">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="bf606-1164">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="bf606-1165">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="bf606-1165">Add support for ssh key password prompting.</span></span> <span data-ttu-id="bf606-1166">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="bf606-1166">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="bf606-1167">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="bf606-1167">Add support for windows clusters.</span></span> <span data-ttu-id="bf606-1168">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="bf606-1168">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="bf606-1169">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="bf606-1169">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="bf606-1170">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="bf606-1170">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="bf606-1171">AppService</span><span class="sxs-lookup"><span data-stu-id="bf606-1171">AppService</span></span>

* <span data-ttu-id="bf606-1172">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="bf606-1172">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="bf606-1173">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="bf606-1173">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="bf606-1174">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="bf606-1174">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="bf606-1175">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="bf606-1175">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="bf606-1176">DataLake</span><span class="sxs-lookup"><span data-stu-id="bf606-1176">DataLake</span></span>

* <span data-ttu-id="bf606-1177">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="bf606-1177">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="bf606-1178">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="bf606-1178">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="bf606-1179">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="bf606-1179">DocuemntDB</span></span>

* <span data-ttu-id="bf606-1180">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="bf606-1180">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="bf606-1181">VM</span><span class="sxs-lookup"><span data-stu-id="bf606-1181">VM</span></span>

* <span data-ttu-id="bf606-1182">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="bf606-1182">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="bf606-1183">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="bf606-1183">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="bf606-1184">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="bf606-1184">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="bf606-1185">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="bf606-1185">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="bf606-1186">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="bf606-1186">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="bf606-1187">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="bf606-1187">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="bf606-1188">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="bf606-1188">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="bf606-1189">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="bf606-1189">February 27, 2017</span></span>

<span data-ttu-id="bf606-1190">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="bf606-1190">Version 2.0.0</span></span>

<span data-ttu-id="bf606-1191">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="bf606-1191">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="bf606-1192">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="bf606-1192">Container Service (acs)</span></span>
- <span data-ttu-id="bf606-1193">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="bf606-1193">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="bf606-1194">Rede</span><span class="sxs-lookup"><span data-stu-id="bf606-1194">Networking</span></span>
- <span data-ttu-id="bf606-1195">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="bf606-1195">Storage</span></span>

<span data-ttu-id="bf606-1196">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="bf606-1196">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="bf606-1197">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="bf606-1197">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="bf606-1198">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="bf606-1198">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="bf606-1199">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="bf606-1199">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="bf606-1200">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="bf606-1200">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="bf606-1201">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="bf606-1201">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="bf606-1202">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="bf606-1202">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="bf606-1203">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="bf606-1203">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="bf606-1204">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="bf606-1204">Provide feedback from the command line with the `az feedback` command</span></span>

