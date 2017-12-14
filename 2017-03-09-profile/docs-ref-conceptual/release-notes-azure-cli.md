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
ms.openlocfilehash: e02b84891f4bf60cde12591b8e85987f4b3c9e79
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="ed2da-104">Notas de versão da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="ed2da-104">Azure CLI 2.0 release notes</span></span>

## <a name="december-5-2017"></a><span data-ttu-id="ed2da-105">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="ed2da-105">December 5, 2017</span></span>

<span data-ttu-id="ed2da-106">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="ed2da-106">Version 2.0.22</span></span>

* <span data-ttu-id="ed2da-107">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="ed2da-107">Removed `az component` commands.</span></span> <span data-ttu-id="ed2da-108">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="ed2da-108">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="ed2da-109">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ed2da-109">Core</span></span>
* <span data-ttu-id="ed2da-110">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="ed2da-110">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="ed2da-111">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="ed2da-111">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="ed2da-112">ACS</span><span class="sxs-lookup"><span data-stu-id="ed2da-112">ACS</span></span>

* <span data-ttu-id="ed2da-113">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="ed2da-113">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="ed2da-114">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-114">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="ed2da-115">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="ed2da-115">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="ed2da-116">Supervisor</span><span class="sxs-lookup"><span data-stu-id="ed2da-116">Advisor</span></span>

* <span data-ttu-id="ed2da-117">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="ed2da-117">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="ed2da-118">AppService</span><span class="sxs-lookup"><span data-stu-id="ed2da-118">Appservice</span></span>

* <span data-ttu-id="ed2da-119">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="ed2da-119">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="ed2da-120">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="ed2da-120">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="ed2da-121">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="ed2da-121">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="ed2da-122">Consumo</span><span class="sxs-lookup"><span data-stu-id="ed2da-122">Consumption</span></span>

* <span data-ttu-id="ed2da-123">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="ed2da-123">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="ed2da-124">Contêiner</span><span class="sxs-lookup"><span data-stu-id="ed2da-124">Container</span></span>

* <span data-ttu-id="ed2da-125">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="ed2da-125">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="ed2da-126">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="ed2da-126">Monitor</span></span>

* <span data-ttu-id="ed2da-127">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="ed2da-127">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="ed2da-128">Recurso</span><span class="sxs-lookup"><span data-stu-id="ed2da-128">Resource</span></span>

* <span data-ttu-id="ed2da-129">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="ed2da-129">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="ed2da-130">Função</span><span class="sxs-lookup"><span data-stu-id="ed2da-130">Role</span></span>

* <span data-ttu-id="ed2da-131">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="ed2da-131">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="ed2da-132">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="ed2da-132">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="ed2da-133">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="ed2da-133">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="ed2da-134">SQL</span><span class="sxs-lookup"><span data-stu-id="ed2da-134">SQL</span></span>

* <span data-ttu-id="ed2da-135">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="ed2da-135">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="ed2da-136">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="ed2da-136">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="ed2da-137">VM</span><span class="sxs-lookup"><span data-stu-id="ed2da-137">VM</span></span>

* <span data-ttu-id="ed2da-138">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="ed2da-138">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="ed2da-139">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="ed2da-139">November 14, 2017</span></span>

<span data-ttu-id="ed2da-140">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="ed2da-140">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="ed2da-141">ACR</span><span class="sxs-lookup"><span data-stu-id="ed2da-141">ACR</span></span>

* <span data-ttu-id="ed2da-142">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="ed2da-142">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="ed2da-143">ACS</span><span class="sxs-lookup"><span data-stu-id="ed2da-143">ACS</span></span>

* <span data-ttu-id="ed2da-144">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="ed2da-144">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="ed2da-145">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-145">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="ed2da-146">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="ed2da-146">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="ed2da-147">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="ed2da-147">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="ed2da-148">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="ed2da-148">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="ed2da-149">AppService</span><span class="sxs-lookup"><span data-stu-id="ed2da-149">Appservice</span></span>

* <span data-ttu-id="ed2da-150">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="ed2da-150">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="ed2da-151">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="ed2da-151">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="ed2da-152">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="ed2da-152">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="ed2da-153">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="ed2da-153">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="ed2da-154">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="ed2da-154">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="ed2da-155">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="ed2da-155">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="ed2da-156">Batch</span><span class="sxs-lookup"><span data-stu-id="ed2da-156">Batch</span></span>

* <span data-ttu-id="ed2da-157">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="ed2da-157">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="ed2da-158">Batchai</span><span class="sxs-lookup"><span data-stu-id="ed2da-158">Batchai</span></span>

* <span data-ttu-id="ed2da-159">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-159">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="ed2da-160">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-160">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="ed2da-161">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="ed2da-161">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="ed2da-162">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-162">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="ed2da-163">Nuvem</span><span class="sxs-lookup"><span data-stu-id="ed2da-163">Cloud</span></span>

* <span data-ttu-id="ed2da-164">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="ed2da-164">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="ed2da-165">Contêiner</span><span class="sxs-lookup"><span data-stu-id="ed2da-165">Container</span></span>

* <span data-ttu-id="ed2da-166">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="ed2da-166">Added support to open multiple ports</span></span>
* <span data-ttu-id="ed2da-167">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="ed2da-167">Added container group restart policy</span></span>
* <span data-ttu-id="ed2da-168">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="ed2da-168">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="ed2da-169">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="ed2da-169">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ed2da-170">Análises Data Lake</span><span class="sxs-lookup"><span data-stu-id="ed2da-170">Data Lake Analytics</span></span>

* <span data-ttu-id="ed2da-171">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="ed2da-171">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ed2da-172">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="ed2da-172">Data Lake Store</span></span>

* <span data-ttu-id="ed2da-173">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="ed2da-173">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="ed2da-174">Extensão</span><span class="sxs-lookup"><span data-stu-id="ed2da-174">Extension</span></span>

* <span data-ttu-id="ed2da-175">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="ed2da-175">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="ed2da-176">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="ed2da-176">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="ed2da-177">IoT</span><span class="sxs-lookup"><span data-stu-id="ed2da-177">IoT</span></span>

* <span data-ttu-id="ed2da-178">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="ed2da-178">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="ed2da-179">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="ed2da-179">Monitor</span></span>

* <span data-ttu-id="ed2da-180">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="ed2da-180">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="ed2da-181">Rede</span><span class="sxs-lookup"><span data-stu-id="ed2da-181">Network</span></span>

* <span data-ttu-id="ed2da-182">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="ed2da-182">Added support for CAA DNS records</span></span>
* <span data-ttu-id="ed2da-183">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="ed2da-183">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="ed2da-184">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="ed2da-184">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="ed2da-185">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="ed2da-185">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="ed2da-186">Reservas</span><span class="sxs-lookup"><span data-stu-id="ed2da-186">Reservations</span></span>

* <span data-ttu-id="ed2da-187">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="ed2da-187">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="ed2da-188">Recurso</span><span class="sxs-lookup"><span data-stu-id="ed2da-188">Resource</span></span>

* <span data-ttu-id="ed2da-189">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="ed2da-189">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="ed2da-190">SQL</span><span class="sxs-lookup"><span data-stu-id="ed2da-190">SQL</span></span>

* <span data-ttu-id="ed2da-191">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ed2da-191">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="ed2da-192">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="ed2da-192">Storage</span></span>

* <span data-ttu-id="ed2da-193">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="ed2da-193">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="ed2da-194">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="ed2da-194">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="ed2da-195">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="ed2da-195">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="ed2da-196">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="ed2da-196">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="ed2da-197">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="ed2da-197">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="ed2da-198">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="ed2da-198">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="ed2da-199">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ed2da-199">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="ed2da-200">VM</span><span class="sxs-lookup"><span data-stu-id="ed2da-200">VM</span></span>

* <span data-ttu-id="ed2da-201">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="ed2da-201">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="ed2da-202">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="ed2da-202">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="ed2da-203">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="ed2da-203">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="ed2da-204">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="ed2da-204">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="ed2da-205">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="ed2da-205">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="ed2da-206">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="ed2da-206">October 24, 2017</span></span>

<span data-ttu-id="ed2da-207">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="ed2da-207">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="ed2da-208">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ed2da-208">Core</span></span>

* <span data-ttu-id="ed2da-209">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="ed2da-209">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="ed2da-210">ACR</span><span class="sxs-lookup"><span data-stu-id="ed2da-210">ACR</span></span>

* <span data-ttu-id="ed2da-211">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="ed2da-211">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="ed2da-212">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="ed2da-212">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="ed2da-213">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="ed2da-213">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="ed2da-214">ACS</span><span class="sxs-lookup"><span data-stu-id="ed2da-214">ACS</span></span>

* <span data-ttu-id="ed2da-215">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="ed2da-215">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="ed2da-216">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="ed2da-216">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="ed2da-217">AppService</span><span class="sxs-lookup"><span data-stu-id="ed2da-217">Appservice</span></span>

* <span data-ttu-id="ed2da-218">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="ed2da-218">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="ed2da-219">Componente</span><span class="sxs-lookup"><span data-stu-id="ed2da-219">Component</span></span>

* <span data-ttu-id="ed2da-220">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="ed2da-220">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="ed2da-221">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="ed2da-221">Monitor</span></span>

* <span data-ttu-id="ed2da-222">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="ed2da-222">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="ed2da-223">Recurso</span><span class="sxs-lookup"><span data-stu-id="ed2da-223">Resource</span></span>

* <span data-ttu-id="ed2da-224">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="ed2da-224">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="ed2da-225">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="ed2da-225">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="ed2da-226">VM</span><span class="sxs-lookup"><span data-stu-id="ed2da-226">VM</span></span>

* <span data-ttu-id="ed2da-227">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-227">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="ed2da-228">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="ed2da-228">October 9, 2017</span></span>

<span data-ttu-id="ed2da-229">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="ed2da-229">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="ed2da-230">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ed2da-230">Core</span></span>

* <span data-ttu-id="ed2da-231">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="ed2da-231">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="ed2da-232">AppService</span><span class="sxs-lookup"><span data-stu-id="ed2da-232">Appservice</span></span>

* <span data-ttu-id="ed2da-233">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="ed2da-233">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="ed2da-234">Batch</span><span class="sxs-lookup"><span data-stu-id="ed2da-234">Batch</span></span>

* <span data-ttu-id="ed2da-235">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="ed2da-235">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="ed2da-236">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="ed2da-236">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="ed2da-237">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="ed2da-237">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="ed2da-238">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="ed2da-238">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="ed2da-239">Batchai</span><span class="sxs-lookup"><span data-stu-id="ed2da-239">Batchai</span></span>

* <span data-ttu-id="ed2da-240">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="ed2da-240">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="ed2da-241">Keyvault</span><span class="sxs-lookup"><span data-stu-id="ed2da-241">Keyvault</span></span>

* <span data-ttu-id="ed2da-242">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="ed2da-242">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="ed2da-243">(#4448)</span><span class="sxs-lookup"><span data-stu-id="ed2da-243">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="ed2da-244">Rede</span><span class="sxs-lookup"><span data-stu-id="ed2da-244">Network</span></span>

* <span data-ttu-id="ed2da-245">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="ed2da-245">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="ed2da-246">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="ed2da-246">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="ed2da-247">Recurso</span><span class="sxs-lookup"><span data-stu-id="ed2da-247">Resource</span></span>

* <span data-ttu-id="ed2da-248">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="ed2da-248">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="ed2da-249">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="ed2da-249">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="ed2da-250">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="ed2da-250">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="ed2da-251">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="ed2da-251">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="ed2da-252">Sql</span><span class="sxs-lookup"><span data-stu-id="ed2da-252">Sql</span></span>

* <span data-ttu-id="ed2da-253">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="ed2da-253">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="ed2da-254">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="ed2da-254">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="ed2da-255">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="ed2da-255">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="ed2da-256">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="ed2da-256">Storage</span></span>

* <span data-ttu-id="ed2da-257">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="ed2da-257">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="ed2da-258">VM</span><span class="sxs-lookup"><span data-stu-id="ed2da-258">Vm</span></span>

* <span data-ttu-id="ed2da-259">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="ed2da-259">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="ed2da-260">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-260">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="ed2da-261">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="ed2da-261">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="ed2da-262">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-262">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="ed2da-263">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-263">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="ed2da-264">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="ed2da-264">September 22, 2017</span></span>

<span data-ttu-id="ed2da-265">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="ed2da-265">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="ed2da-266">Recurso</span><span class="sxs-lookup"><span data-stu-id="ed2da-266">Resource</span></span>

* <span data-ttu-id="ed2da-267">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="ed2da-267">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="ed2da-268">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="ed2da-268">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="ed2da-269">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-269">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="ed2da-270">[ALTERAÇÃO SIGNIFICATIVA] O tipo de recurso `managedapp` foi alterado de `appliances` para `applications` e `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="ed2da-270">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="ed2da-271">Rede</span><span class="sxs-lookup"><span data-stu-id="ed2da-271">Network</span></span>

* <span data-ttu-id="ed2da-272">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="ed2da-272">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="ed2da-273">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="ed2da-273">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="ed2da-274">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed2da-274">Added `asg` application security group commands</span></span>
* <span data-ttu-id="ed2da-275">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="ed2da-275">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="ed2da-276">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ed2da-276">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="ed2da-277">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ed2da-277">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="ed2da-278">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="ed2da-278">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="ed2da-279">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="ed2da-279">Storage</span></span>

* <span data-ttu-id="ed2da-280">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="ed2da-280">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="ed2da-281">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="ed2da-281">Eventgrid</span></span>

* <span data-ttu-id="ed2da-282">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="ed2da-282">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="ed2da-283">SQL</span><span class="sxs-lookup"><span data-stu-id="ed2da-283">SQL</span></span>

* <span data-ttu-id="ed2da-284">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="ed2da-284">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="ed2da-285">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="ed2da-285">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="ed2da-286">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ed2da-286">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="ed2da-287">Keyvault</span><span class="sxs-lookup"><span data-stu-id="ed2da-287">Keyvault</span></span>

* <span data-ttu-id="ed2da-288">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="ed2da-288">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="ed2da-289">VM</span><span class="sxs-lookup"><span data-stu-id="ed2da-289">VM</span></span>

* <span data-ttu-id="ed2da-290">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-290">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="ed2da-291">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="ed2da-291">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="ed2da-292">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-292">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="ed2da-293">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="ed2da-293">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="ed2da-294">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="ed2da-294">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="ed2da-295">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="ed2da-295">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="ed2da-296">ACS</span><span class="sxs-lookup"><span data-stu-id="ed2da-296">ACS</span></span>

* <span data-ttu-id="ed2da-297">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="ed2da-297">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="ed2da-298">AppService</span><span class="sxs-lookup"><span data-stu-id="ed2da-298">Appservice</span></span>

* <span data-ttu-id="ed2da-299">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="ed2da-299">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="ed2da-300">Backup</span><span class="sxs-lookup"><span data-stu-id="ed2da-300">Backup</span></span>

* <span data-ttu-id="ed2da-301">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="ed2da-301">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="ed2da-302">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="ed2da-302">September 11, 2017</span></span>

<span data-ttu-id="ed2da-303">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="ed2da-303">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="ed2da-304">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ed2da-304">Core</span></span>

* <span data-ttu-id="ed2da-305">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="ed2da-305">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="ed2da-306">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="ed2da-306">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="ed2da-307">Acs</span><span class="sxs-lookup"><span data-stu-id="ed2da-307">Acs</span></span>

* <span data-ttu-id="ed2da-308">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="ed2da-308">Added `acs list-locations` command</span></span>
* <span data-ttu-id="ed2da-309">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="ed2da-309">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="ed2da-310">AppService</span><span class="sxs-lookup"><span data-stu-id="ed2da-310">Appservice</span></span>

* <span data-ttu-id="ed2da-311">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="ed2da-311">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="ed2da-312">CDN</span><span class="sxs-lookup"><span data-stu-id="ed2da-312">CDN</span></span>

* <span data-ttu-id="ed2da-313">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="ed2da-313">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="ed2da-314">Extensão</span><span class="sxs-lookup"><span data-stu-id="ed2da-314">Extension</span></span>

* <span data-ttu-id="ed2da-315">Versão Inicial.</span><span class="sxs-lookup"><span data-stu-id="ed2da-315">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="ed2da-316">Keyvault</span><span class="sxs-lookup"><span data-stu-id="ed2da-316">Keyvault</span></span>

* <span data-ttu-id="ed2da-317">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="ed2da-317">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="ed2da-318">Rede</span><span class="sxs-lookup"><span data-stu-id="ed2da-318">Network</span></span>

* <span data-ttu-id="ed2da-319">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="ed2da-319">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="ed2da-320">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="ed2da-320">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="ed2da-321">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="ed2da-321">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="ed2da-322">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-322">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="ed2da-323">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-323">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="ed2da-324">Recurso</span><span class="sxs-lookup"><span data-stu-id="ed2da-324">Resource</span></span>

* <span data-ttu-id="ed2da-325">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="ed2da-325">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="ed2da-326">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-326">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="ed2da-327">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="ed2da-327">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="ed2da-328">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="ed2da-328">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="ed2da-329">SQL</span><span class="sxs-lookup"><span data-stu-id="ed2da-329">SQL</span></span>

* <span data-ttu-id="ed2da-330">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="ed2da-330">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="ed2da-331">VM</span><span class="sxs-lookup"><span data-stu-id="ed2da-331">VM</span></span>

* <span data-ttu-id="ed2da-332">Corrigido: Não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="ed2da-332">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="ed2da-333">Corrigido: Usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="ed2da-333">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="ed2da-334">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-334">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="ed2da-335">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="ed2da-335">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="ed2da-336">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="ed2da-336">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="ed2da-337">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="ed2da-337">August 31, 2017</span></span>

<span data-ttu-id="ed2da-338">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="ed2da-338">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="ed2da-339">Keyvault</span><span class="sxs-lookup"><span data-stu-id="ed2da-339">Keyvault</span></span>

* <span data-ttu-id="ed2da-340">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="ed2da-340">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="ed2da-341">Sf</span><span class="sxs-lookup"><span data-stu-id="ed2da-341">Sf</span></span>

* <span data-ttu-id="ed2da-342">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="ed2da-342">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="ed2da-343">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="ed2da-343">Storage</span></span>

* <span data-ttu-id="ed2da-344">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="ed2da-344">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="ed2da-345">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="ed2da-345">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="ed2da-346">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="ed2da-346">August 28, 2017</span></span>

<span data-ttu-id="ed2da-347">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="ed2da-347">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="ed2da-348">CLI</span><span class="sxs-lookup"><span data-stu-id="ed2da-348">CLI</span></span>

* <span data-ttu-id="ed2da-349">Nota legal adicionada ao `--version`.</span><span class="sxs-lookup"><span data-stu-id="ed2da-349">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="ed2da-350">ACS</span><span class="sxs-lookup"><span data-stu-id="ed2da-350">ACS</span></span>

* <span data-ttu-id="ed2da-351">Corrigidas as regiões de visualização.</span><span class="sxs-lookup"><span data-stu-id="ed2da-351">Corrected preview regions.</span></span>
* <span data-ttu-id="ed2da-352">Corrigida a formatação padrão de `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="ed2da-352">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="ed2da-353">Saída de comando ACS otimizada.</span><span class="sxs-lookup"><span data-stu-id="ed2da-353">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="ed2da-354">AppService</span><span class="sxs-lookup"><span data-stu-id="ed2da-354">Appservice</span></span>

* <span data-ttu-id="ed2da-355">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="ed2da-355">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="ed2da-356">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="ed2da-356">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="ed2da-357">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="ed2da-357">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="ed2da-358">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed2da-358">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="ed2da-359">Correção: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="ed2da-359">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="ed2da-360">IoT</span><span class="sxs-lookup"><span data-stu-id="ed2da-360">IoT</span></span>

* <span data-ttu-id="ed2da-361">Correção #3934: Criação de política não limpa as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="ed2da-361">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="ed2da-362">Rede</span><span class="sxs-lookup"><span data-stu-id="ed2da-362">Network</span></span>

* <span data-ttu-id="ed2da-363">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="ed2da-363">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="ed2da-364">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ed2da-364">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="ed2da-365">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ed2da-365">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="ed2da-366">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-366">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="ed2da-367">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-367">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="ed2da-368">Perfil</span><span class="sxs-lookup"><span data-stu-id="ed2da-368">Profile</span></span>

* <span data-ttu-id="ed2da-369">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ed2da-369">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ed2da-370">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ed2da-370">Service Fabric</span></span>

* <span data-ttu-id="ed2da-371">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="ed2da-371">Preview release</span></span>
* <span data-ttu-id="ed2da-372">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="ed2da-372">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="ed2da-373">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="ed2da-373">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="ed2da-374">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="ed2da-374">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="ed2da-375">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="ed2da-375">Storage</span></span>

* <span data-ttu-id="ed2da-376">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="ed2da-376">Enabled setting blob tier</span></span>
* <span data-ttu-id="ed2da-377">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="ed2da-377">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="ed2da-378">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="ed2da-378">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="ed2da-379">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="ed2da-379">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="ed2da-380">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="ed2da-380">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="ed2da-381">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="ed2da-381">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="ed2da-382">VM</span><span class="sxs-lookup"><span data-stu-id="ed2da-382">VM</span></span>

* <span data-ttu-id="ed2da-383">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="ed2da-383">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="ed2da-384">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="ed2da-384">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="ed2da-385">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-385">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="ed2da-386">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="ed2da-386">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="ed2da-387">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="ed2da-387">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="ed2da-388">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-388">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="ed2da-389">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="ed2da-389">August 15, 2017</span></span>

<span data-ttu-id="ed2da-390">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="ed2da-390">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="ed2da-391">ACS</span><span class="sxs-lookup"><span data-stu-id="ed2da-391">ACS</span></span>

* <span data-ttu-id="ed2da-392">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="ed2da-392">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="ed2da-393">AppService</span><span class="sxs-lookup"><span data-stu-id="ed2da-393">Appservice</span></span>

* <span data-ttu-id="ed2da-394">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="ed2da-394">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="ed2da-395">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="ed2da-395">Event Grid</span></span>

* <span data-ttu-id="ed2da-396">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="ed2da-396">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="ed2da-397">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="ed2da-397">August 11, 2017</span></span>

<span data-ttu-id="ed2da-398">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="ed2da-398">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="ed2da-399">ACS</span><span class="sxs-lookup"><span data-stu-id="ed2da-399">ACS</span></span>

* <span data-ttu-id="ed2da-400">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="ed2da-400">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="ed2da-401">Batch</span><span class="sxs-lookup"><span data-stu-id="ed2da-401">Batch</span></span>

* <span data-ttu-id="ed2da-402">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="ed2da-402">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="ed2da-403">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="ed2da-403">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="ed2da-404">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="ed2da-404">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="ed2da-405">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="ed2da-405">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="ed2da-406">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="ed2da-406">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="ed2da-407">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="ed2da-407">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="ed2da-408">Componente</span><span class="sxs-lookup"><span data-stu-id="ed2da-408">Component</span></span>

* <span data-ttu-id="ed2da-409">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="ed2da-409">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="ed2da-410">Contêiner</span><span class="sxs-lookup"><span data-stu-id="ed2da-410">Container</span></span>

* <span data-ttu-id="ed2da-411">`create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="ed2da-411">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="ed2da-412">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ed2da-412">Data Lake Store</span></span>

* <span data-ttu-id="ed2da-413">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="ed2da-413">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="ed2da-414">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="ed2da-414">Event Grid</span></span>

* <span data-ttu-id="ed2da-415">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="ed2da-415">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="ed2da-416">Rede</span><span class="sxs-lookup"><span data-stu-id="ed2da-416">Network</span></span>

* <span data-ttu-id="ed2da-417">`lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="ed2da-417">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="ed2da-418">`application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="ed2da-418">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="ed2da-419">`application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="ed2da-419">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="ed2da-420">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="ed2da-420">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="ed2da-421">Perfil</span><span class="sxs-lookup"><span data-stu-id="ed2da-421">Profile</span></span>

* <span data-ttu-id="ed2da-422">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="ed2da-422">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="ed2da-423">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="ed2da-423">Storage</span></span>

* <span data-ttu-id="ed2da-424">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="ed2da-424">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="ed2da-425">VM</span><span class="sxs-lookup"><span data-stu-id="ed2da-425">VM</span></span>

* <span data-ttu-id="ed2da-426">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="ed2da-426">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="ed2da-427">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="ed2da-427">Exposed `list-skus` command</span></span>
* <span data-ttu-id="ed2da-428">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="ed2da-428">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="ed2da-429">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="ed2da-429">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="ed2da-430">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="ed2da-430">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="ed2da-431">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="ed2da-431">July 28, 2017</span></span>

<span data-ttu-id="ed2da-432">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="ed2da-432">Version 2.0.12</span></span>

* <span data-ttu-id="ed2da-433">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="ed2da-433">Added container commands</span></span>
* <span data-ttu-id="ed2da-434">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="ed2da-434">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="ed2da-435">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ed2da-435">Core</span></span>

* <span data-ttu-id="ed2da-436">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="ed2da-436">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="ed2da-437">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="ed2da-437">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="ed2da-438">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="ed2da-438">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="ed2da-439">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="ed2da-439">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="ed2da-440">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="ed2da-440">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="ed2da-441">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="ed2da-441">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="ed2da-442">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="ed2da-442">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="ed2da-443">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="ed2da-443">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="ed2da-444">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="ed2da-444">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="ed2da-445">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="ed2da-445">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="ed2da-446">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="ed2da-446">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="ed2da-447">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="ed2da-447">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="ed2da-448">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="ed2da-448">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="ed2da-449">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="ed2da-449">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="ed2da-450">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="ed2da-450">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="ed2da-451">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="ed2da-451">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="ed2da-452">ACR</span><span class="sxs-lookup"><span data-stu-id="ed2da-452">ACR</span></span>

* <span data-ttu-id="ed2da-453">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="ed2da-453">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="ed2da-454">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="ed2da-454">Support SKU update for managed registries</span></span>
* <span data-ttu-id="ed2da-455">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="ed2da-455">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="ed2da-456">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="ed2da-456">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="ed2da-457">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="ed2da-457">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="ed2da-458">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="ed2da-458">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="ed2da-459">ACS</span><span class="sxs-lookup"><span data-stu-id="ed2da-459">ACS</span></span>

* <span data-ttu-id="ed2da-460">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="ed2da-460">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="ed2da-461">AppService</span><span class="sxs-lookup"><span data-stu-id="ed2da-461">Appservice</span></span>

* <span data-ttu-id="ed2da-462">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="ed2da-462">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="ed2da-463">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="ed2da-463">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="ed2da-464">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="ed2da-464">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="ed2da-465">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="ed2da-465">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="ed2da-466">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="ed2da-466">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="ed2da-467">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="ed2da-467">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="ed2da-468">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="ed2da-468">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="ed2da-469">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="ed2da-469">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="ed2da-470">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="ed2da-470">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="ed2da-471">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="ed2da-471">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="ed2da-472">Batch</span><span class="sxs-lookup"><span data-stu-id="ed2da-472">Batch</span></span>

* <span data-ttu-id="ed2da-473">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="ed2da-473">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="ed2da-474">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="ed2da-474">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="ed2da-475">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="ed2da-475">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="ed2da-476">CDN</span><span class="sxs-lookup"><span data-stu-id="ed2da-476">CDN</span></span>

* <span data-ttu-id="ed2da-477">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir.</span><span class="sxs-lookup"><span data-stu-id="ed2da-477">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="ed2da-478">Nuvem</span><span class="sxs-lookup"><span data-stu-id="ed2da-478">Cloud</span></span>

* <span data-ttu-id="ed2da-479">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="ed2da-479">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="ed2da-480">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="ed2da-480">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="ed2da-481">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="ed2da-481">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="ed2da-482">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="ed2da-482">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="ed2da-483">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="ed2da-483">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ed2da-484">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ed2da-484">CosmosDB</span></span>

* <span data-ttu-id="ed2da-485">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="ed2da-485">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="ed2da-486">Adicionado suporte para o TTL padrão de coleção.</span><span class="sxs-lookup"><span data-stu-id="ed2da-486">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ed2da-487">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ed2da-487">Data Lake Analytics</span></span>

* <span data-ttu-id="ed2da-488">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="ed2da-488">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="ed2da-489">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="ed2da-489">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="ed2da-490">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="ed2da-490">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ed2da-491">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ed2da-491">Data Lake Store</span></span>

* <span data-ttu-id="ed2da-492">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="ed2da-492">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="ed2da-493">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="ed2da-493">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="ed2da-494">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="ed2da-494">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="ed2da-495">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ed2da-495">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="ed2da-496">Interativo</span><span class="sxs-lookup"><span data-stu-id="ed2da-496">Interactive</span></span>

* <span data-ttu-id="ed2da-497">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="ed2da-497">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="ed2da-498">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="ed2da-498">Increased test coverage</span></span>
* <span data-ttu-id="ed2da-499">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="ed2da-499">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="ed2da-500">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="ed2da-500">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="ed2da-501">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="ed2da-501">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="ed2da-502">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="ed2da-502">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="ed2da-503">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="ed2da-503">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="ed2da-504">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="ed2da-504">Added `--progress` flag</span></span>
* <span data-ttu-id="ed2da-505">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="ed2da-505">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="ed2da-506">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="ed2da-506">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="ed2da-507">IoT</span><span class="sxs-lookup"><span data-stu-id="ed2da-507">IoT</span></span>

* <span data-ttu-id="ed2da-508">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="ed2da-508">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="ed2da-509">(#3934)</span><span class="sxs-lookup"><span data-stu-id="ed2da-509">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="ed2da-510">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="ed2da-510">Key vault</span></span>

* <span data-ttu-id="ed2da-511">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="ed2da-511">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="ed2da-512">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="ed2da-512">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="ed2da-513">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="ed2da-513">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="ed2da-514">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="ed2da-514">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="ed2da-515">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="ed2da-515">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="ed2da-516">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="ed2da-516">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="ed2da-517">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="ed2da-517">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="ed2da-518">(#3307)</span><span class="sxs-lookup"><span data-stu-id="ed2da-518">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="ed2da-519">Laboratório</span><span class="sxs-lookup"><span data-stu-id="ed2da-519">Lab</span></span>

* <span data-ttu-id="ed2da-520">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="ed2da-520">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="ed2da-521">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="ed2da-521">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="ed2da-522">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="ed2da-522">Monitor</span></span>

* <span data-ttu-id="ed2da-523">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="ed2da-523">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="ed2da-524">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="ed2da-524">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="ed2da-525">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="ed2da-525">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="ed2da-526">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="ed2da-526">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="ed2da-527">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="ed2da-527">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="ed2da-528">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="ed2da-528">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="ed2da-529">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="ed2da-529">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="ed2da-530">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="ed2da-530">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="ed2da-531">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="ed2da-531">`location` no longer required</span></span>
  * <span data-ttu-id="ed2da-532">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="ed2da-532">Add name and ID support for target</span></span>
  * <span data-ttu-id="ed2da-533">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="ed2da-533">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="ed2da-534">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="ed2da-534">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="ed2da-535">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="ed2da-535">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="ed2da-536">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="ed2da-536">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="ed2da-537">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="ed2da-537">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="ed2da-538">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="ed2da-538">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="ed2da-539">Rede</span><span class="sxs-lookup"><span data-stu-id="ed2da-539">Network</span></span>

* <span data-ttu-id="ed2da-540">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="ed2da-540">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="ed2da-541">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="ed2da-541">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="ed2da-542">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="ed2da-542">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="ed2da-543">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="ed2da-543">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="ed2da-544">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="ed2da-544">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="ed2da-545">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="ed2da-545">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="ed2da-546">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="ed2da-546">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="ed2da-547">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="ed2da-547">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="ed2da-548">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="ed2da-548">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="ed2da-549">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="ed2da-549">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="ed2da-550">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-550">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="ed2da-551">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="ed2da-551">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="ed2da-552">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="ed2da-552">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="ed2da-553">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="ed2da-553">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="ed2da-554">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="ed2da-554">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="ed2da-555">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-555">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="ed2da-556">Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS</span><span class="sxs-lookup"><span data-stu-id="ed2da-556">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="ed2da-557">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="ed2da-557">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="ed2da-558">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="ed2da-558">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="ed2da-559">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-559">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="ed2da-560">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="ed2da-560">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="ed2da-561">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="ed2da-561">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="ed2da-562">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="ed2da-562">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="ed2da-563">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="ed2da-563">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="ed2da-564">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="ed2da-564">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="ed2da-565">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="ed2da-565">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="ed2da-566">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="ed2da-566">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="ed2da-567">Perfil</span><span class="sxs-lookup"><span data-stu-id="ed2da-567">Profile</span></span>

* <span data-ttu-id="ed2da-568">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="ed2da-568">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="ed2da-569">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="ed2da-569">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="ed2da-570">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="ed2da-570">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="ed2da-571">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="ed2da-571">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="ed2da-572">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="ed2da-572">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="ed2da-573">RDBMS</span><span class="sxs-lookup"><span data-stu-id="ed2da-573">RDBMS</span></span>

* <span data-ttu-id="ed2da-574">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="ed2da-574">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="ed2da-575">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="ed2da-575">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="ed2da-576">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="ed2da-576">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="ed2da-577">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="ed2da-577">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="ed2da-578">Recurso</span><span class="sxs-lookup"><span data-stu-id="ed2da-578">Resource</span></span>

* <span data-ttu-id="ed2da-579">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-579">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="ed2da-580">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="ed2da-580">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="ed2da-581">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="ed2da-581">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="ed2da-582">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="ed2da-582">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="ed2da-583">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="ed2da-583">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="ed2da-584">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="ed2da-584">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="ed2da-585">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="ed2da-585">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="ed2da-586">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="ed2da-586">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="ed2da-587">Função</span><span class="sxs-lookup"><span data-stu-id="ed2da-587">Role</span></span>

* <span data-ttu-id="ed2da-588">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="ed2da-588">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="ed2da-589">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="ed2da-589">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="ed2da-590">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="ed2da-590">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="ed2da-591">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="ed2da-591">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="ed2da-592">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="ed2da-592">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ed2da-593">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ed2da-593">Service Fabric</span></span>
* <span data-ttu-id="ed2da-594">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="ed2da-594">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="ed2da-595">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="ed2da-595">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="ed2da-596">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="ed2da-596">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="ed2da-597">SQL</span><span class="sxs-lookup"><span data-stu-id="ed2da-597">SQL</span></span>

* <span data-ttu-id="ed2da-598">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="ed2da-598">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="ed2da-599">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="ed2da-599">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="ed2da-600">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="ed2da-600">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="ed2da-601">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="ed2da-601">Storage</span></span>

* <span data-ttu-id="ed2da-602">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="ed2da-602">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="ed2da-603">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="ed2da-603">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="ed2da-604">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="ed2da-604">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="ed2da-605">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="ed2da-605">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="ed2da-606">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="ed2da-606">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="ed2da-607">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="ed2da-607">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="ed2da-608">VM</span><span class="sxs-lookup"><span data-stu-id="ed2da-608">VM</span></span>

* <span data-ttu-id="ed2da-609">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="ed2da-609">Support configuring nsg</span></span>
* <span data-ttu-id="ed2da-610">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="ed2da-610">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="ed2da-611">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="ed2da-611">Support managed service identities</span></span>
* <span data-ttu-id="ed2da-612">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="ed2da-612">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="ed2da-613">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="ed2da-613">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="ed2da-614">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="ed2da-614">May 10, 2017</span></span>

<span data-ttu-id="ed2da-615">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="ed2da-615">Version 2.0.6</span></span>

* <span data-ttu-id="ed2da-616">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ed2da-616">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="ed2da-617">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="ed2da-617">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="ed2da-618">Inclusão dos módulos Data Lake Analytics e Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="ed2da-618">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="ed2da-619">Inclusão do módulo Serviços Cognitivos.</span><span class="sxs-lookup"><span data-stu-id="ed2da-619">Include Cognitive Services module.</span></span>
* <span data-ttu-id="ed2da-620">Inclusão do módulo Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="ed2da-620">Include Service Fabric module.</span></span>
* <span data-ttu-id="ed2da-621">Inclusão do módulo Interativo (renomeação de az-shell).</span><span class="sxs-lookup"><span data-stu-id="ed2da-621">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="ed2da-622">Adição de suporte para comandos CDN.</span><span class="sxs-lookup"><span data-stu-id="ed2da-622">Add support for CDN commands.</span></span>
* <span data-ttu-id="ed2da-623">Remoção do módulo Contêiner.</span><span class="sxs-lookup"><span data-stu-id="ed2da-623">Remove Container module.</span></span>
* <span data-ttu-id="ed2da-624">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="ed2da-624">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="ed2da-625">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="ed2da-625">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="ed2da-626">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ed2da-626">Core</span></span>

* <span data-ttu-id="ed2da-627">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="ed2da-627">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="ed2da-628">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="ed2da-628">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="ed2da-629">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="ed2da-629">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="ed2da-630">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="ed2da-630">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="ed2da-631">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="ed2da-631">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="ed2da-632">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="ed2da-632">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="ed2da-633">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="ed2da-633">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="ed2da-634">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="ed2da-634">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="ed2da-635">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="ed2da-635">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="ed2da-636">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="ed2da-636">core: Improved performance</span></span>
* <span data-ttu-id="ed2da-637">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="ed2da-637">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="ed2da-638">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="ed2da-638">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="ed2da-639">ACS</span><span class="sxs-lookup"><span data-stu-id="ed2da-639">ACS</span></span>

* <span data-ttu-id="ed2da-640">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed2da-640">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="ed2da-641">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="ed2da-641">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="ed2da-642">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="ed2da-642">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="ed2da-643">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="ed2da-643">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="ed2da-644">AppService</span><span class="sxs-lookup"><span data-stu-id="ed2da-644">AppService</span></span>

* <span data-ttu-id="ed2da-645">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="ed2da-645">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="ed2da-646">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="ed2da-646">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="ed2da-647">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="ed2da-647">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="ed2da-648">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="ed2da-648">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="ed2da-649">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="ed2da-649">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="ed2da-650">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="ed2da-650">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="ed2da-651">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="ed2da-651">support slot swap with preview</span></span>
* <span data-ttu-id="ed2da-652">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="ed2da-652">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="ed2da-653">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="ed2da-653">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ed2da-654">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ed2da-654">CosmosDB</span></span>

* <span data-ttu-id="ed2da-655">Renomeação do módulo DocumentDB para CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="ed2da-655">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="ed2da-656">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="ed2da-656">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="ed2da-657">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="ed2da-657">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="ed2da-658">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="ed2da-658">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ed2da-659">Análises Data Lake</span><span class="sxs-lookup"><span data-stu-id="ed2da-659">Data Lake Analytics</span></span>

* <span data-ttu-id="ed2da-660">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro.</span><span class="sxs-lookup"><span data-stu-id="ed2da-660">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="ed2da-661">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="ed2da-661">Add support for new catalog item type: package.</span></span> <span data-ttu-id="ed2da-662">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="ed2da-662">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="ed2da-663">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="ed2da-663">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="ed2da-664">Tabela</span><span class="sxs-lookup"><span data-stu-id="ed2da-664">Table</span></span>
  * <span data-ttu-id="ed2da-665">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="ed2da-665">Table valued function</span></span>
  * <span data-ttu-id="ed2da-666">Visualizar</span><span class="sxs-lookup"><span data-stu-id="ed2da-666">View</span></span>
  * <span data-ttu-id="ed2da-667">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="ed2da-667">Table Statistics.</span></span> <span data-ttu-id="ed2da-668">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela.</span><span class="sxs-lookup"><span data-stu-id="ed2da-668">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ed2da-669">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="ed2da-669">Data Lake Store</span></span>

* <span data-ttu-id="ed2da-670">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor.</span><span class="sxs-lookup"><span data-stu-id="ed2da-670">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="ed2da-671">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="ed2da-671">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="ed2da-672">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="ed2da-672">missed help for access show.</span></span> <span data-ttu-id="ed2da-673">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="ed2da-673">adding it.</span></span> <span data-ttu-id="ed2da-674">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="ed2da-674">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="ed2da-675">Localizar</span><span class="sxs-lookup"><span data-stu-id="ed2da-675">Find</span></span>

* <span data-ttu-id="ed2da-676">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="ed2da-676">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="ed2da-677">KeyVault</span><span class="sxs-lookup"><span data-stu-id="ed2da-677">KeyVault</span></span>

* <span data-ttu-id="ed2da-678">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="ed2da-678">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="ed2da-679">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço.</span><span class="sxs-lookup"><span data-stu-id="ed2da-679">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="ed2da-680">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="ed2da-680">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="ed2da-681">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”.</span><span class="sxs-lookup"><span data-stu-id="ed2da-681">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="ed2da-682">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="ed2da-682">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="ed2da-683">Laboratório</span><span class="sxs-lookup"><span data-stu-id="ed2da-683">Lab</span></span>

* <span data-ttu-id="ed2da-684">Adição dos comandos create, show, delete e list ao ambiente do laboratório.</span><span class="sxs-lookup"><span data-stu-id="ed2da-684">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="ed2da-685">Adição dos comandos show e list para exibir modelos ARM no laboratório.</span><span class="sxs-lookup"><span data-stu-id="ed2da-685">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="ed2da-686">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório.</span><span class="sxs-lookup"><span data-stu-id="ed2da-686">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="ed2da-687">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório.</span><span class="sxs-lookup"><span data-stu-id="ed2da-687">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="ed2da-688">Adição de comandos para gerenciar segredos em um Laboratório.</span><span class="sxs-lookup"><span data-stu-id="ed2da-688">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="ed2da-689">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="ed2da-689">Monitor</span></span>

* <span data-ttu-id="ed2da-690">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="ed2da-690">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="ed2da-691">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="ed2da-691">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="ed2da-692">Rede</span><span class="sxs-lookup"><span data-stu-id="ed2da-692">Network</span></span>

* <span data-ttu-id="ed2da-693">Adição do comando `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="ed2da-693">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="ed2da-694">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="ed2da-694">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="ed2da-695">Adição de suporte para drenagem de conexão do Gateway de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ed2da-695">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="ed2da-696">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ed2da-696">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="ed2da-697">Adição de suporte para filtros de rota e regras do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="ed2da-697">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="ed2da-698">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="ed2da-698">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="ed2da-699">Adição de suporte para seletores de tráfego baseados em política da conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="ed2da-699">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="ed2da-700">Adição de suporte para políticas IPsec da conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="ed2da-700">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="ed2da-701">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`.</span><span class="sxs-lookup"><span data-stu-id="ed2da-701">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="ed2da-702">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="ed2da-702">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="ed2da-703">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="ed2da-703">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="ed2da-704">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="ed2da-704">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="ed2da-705">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente.</span><span class="sxs-lookup"><span data-stu-id="ed2da-705">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="ed2da-706">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente.</span><span class="sxs-lookup"><span data-stu-id="ed2da-706">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="ed2da-707">Correção de um bug em que `traffic-manager endpoint update` não funciona.</span><span class="sxs-lookup"><span data-stu-id="ed2da-707">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="ed2da-708">Adição de comandos de visualização “network watcher”.</span><span class="sxs-lookup"><span data-stu-id="ed2da-708">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="ed2da-709">Perfil</span><span class="sxs-lookup"><span data-stu-id="ed2da-709">Profile</span></span>

* <span data-ttu-id="ed2da-710">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="ed2da-710">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="ed2da-711">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="ed2da-711">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="ed2da-712">Redis</span><span class="sxs-lookup"><span data-stu-id="ed2da-712">Redis</span></span>

* <span data-ttu-id="ed2da-713">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="ed2da-713">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="ed2da-714">Preterição do comando “update-settings”.</span><span class="sxs-lookup"><span data-stu-id="ed2da-714">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="ed2da-715">Recurso</span><span class="sxs-lookup"><span data-stu-id="ed2da-715">Resource</span></span>

* <span data-ttu-id="ed2da-716">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="ed2da-716">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="ed2da-717">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="ed2da-717">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="ed2da-718">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="ed2da-718">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="ed2da-719">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="ed2da-719">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="ed2da-720">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="ed2da-720">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="ed2da-721">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="ed2da-721">Add docs for az lock update.</span></span> <span data-ttu-id="ed2da-722">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="ed2da-722">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="ed2da-723">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="ed2da-723">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="ed2da-724">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="ed2da-724">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="ed2da-725">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="ed2da-725">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="ed2da-726">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="ed2da-726">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="ed2da-727">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="ed2da-727">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="ed2da-728">Função</span><span class="sxs-lookup"><span data-stu-id="ed2da-728">Role</span></span>

* <span data-ttu-id="ed2da-729">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="ed2da-729">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="ed2da-730">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="ed2da-730">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="ed2da-731">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="ed2da-731">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="ed2da-732">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="ed2da-732">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="ed2da-733">SQL</span><span class="sxs-lookup"><span data-stu-id="ed2da-733">SQL</span></span>

* <span data-ttu-id="ed2da-734">Adição dos comandos az sql server list-usages e az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="ed2da-734">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="ed2da-735">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="ed2da-735">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="ed2da-736">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="ed2da-736">Storage</span></span>

* <span data-ttu-id="ed2da-737">Localização padrão da localização do grupo de recursos de `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="ed2da-737">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="ed2da-738">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="ed2da-738">Add support for incremental blob copy</span></span>
* <span data-ttu-id="ed2da-739">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="ed2da-739">Add support for large block blob upload</span></span>
* <span data-ttu-id="ed2da-740">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="ed2da-740">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="ed2da-741">VM</span><span class="sxs-lookup"><span data-stu-id="ed2da-741">VM</span></span>

* <span data-ttu-id="ed2da-742">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="ed2da-742">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="ed2da-743">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="ed2da-743">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="ed2da-744">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="ed2da-744">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="ed2da-745">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="ed2da-745">az vm/vmss disk</span></span>
  3. <span data-ttu-id="ed2da-746">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="ed2da-746">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="ed2da-747">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="ed2da-747">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="ed2da-748">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="ed2da-748">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="ed2da-749">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="ed2da-749">April 3, 2017</span></span>

<span data-ttu-id="ed2da-750">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="ed2da-750">Version 2.0.2</span></span>

<span data-ttu-id="ed2da-751">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão.</span><span class="sxs-lookup"><span data-stu-id="ed2da-751">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="ed2da-752">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ed2da-752">Core</span></span>

* <span data-ttu-id="ed2da-753">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão.</span><span class="sxs-lookup"><span data-stu-id="ed2da-753">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="ed2da-754">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="ed2da-754">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="ed2da-755">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="ed2da-755">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="ed2da-756">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="ed2da-756">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="ed2da-757">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="ed2da-757">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="ed2da-758">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="ed2da-758">Add prompting for missing template parameters.</span></span> <span data-ttu-id="ed2da-759">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="ed2da-759">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="ed2da-760">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="ed2da-760">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="ed2da-761">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="ed2da-761">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="ed2da-762">ACS</span><span class="sxs-lookup"><span data-stu-id="ed2da-762">ACS</span></span>

* <span data-ttu-id="ed2da-763">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="ed2da-763">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="ed2da-764">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="ed2da-764">Add support for ssh key password prompting.</span></span> <span data-ttu-id="ed2da-765">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="ed2da-765">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="ed2da-766">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="ed2da-766">Add support for windows clusters.</span></span> <span data-ttu-id="ed2da-767">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="ed2da-767">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="ed2da-768">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="ed2da-768">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="ed2da-769">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="ed2da-769">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="ed2da-770">AppService</span><span class="sxs-lookup"><span data-stu-id="ed2da-770">AppService</span></span>

* <span data-ttu-id="ed2da-771">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="ed2da-771">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="ed2da-772">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="ed2da-772">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="ed2da-773">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="ed2da-773">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="ed2da-774">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="ed2da-774">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="ed2da-775">DataLake</span><span class="sxs-lookup"><span data-stu-id="ed2da-775">DataLake</span></span>

* <span data-ttu-id="ed2da-776">Versão inicial do módulo do Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="ed2da-776">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="ed2da-777">Versão inicial do módulo do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="ed2da-777">Initial release of Data Lake Store module.</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="ed2da-778">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="ed2da-778">DocuemntDB</span></span>

* <span data-ttu-id="ed2da-779">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="ed2da-779">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="ed2da-780">VM</span><span class="sxs-lookup"><span data-stu-id="ed2da-780">VM</span></span>

* <span data-ttu-id="ed2da-781">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="ed2da-781">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="ed2da-782">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="ed2da-782">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="ed2da-783">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="ed2da-783">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="ed2da-784">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="ed2da-784">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="ed2da-785">Conjunto de dimensionamento de máquinas virtuais: suporte à * para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="ed2da-785">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="ed2da-786">Adicionar --secrets para o conjunto de dimensionamento de máquinas virtuais e VM ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="ed2da-786">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="ed2da-787">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="ed2da-787">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="ed2da-788">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="ed2da-788">February 27, 2017</span></span>

<span data-ttu-id="ed2da-789">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="ed2da-789">Version 2.0.0</span></span>

<span data-ttu-id="ed2da-790">Essa versão da CLI do Azure 2.0 é a primeira versão “Disponível”.</span><span class="sxs-lookup"><span data-stu-id="ed2da-790">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="ed2da-791">A disponibilidade se aplica a esses módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="ed2da-791">General availability applies to these command modules:</span></span>
- <span data-ttu-id="ed2da-792">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="ed2da-792">Container Service (acs)</span></span>
- <span data-ttu-id="ed2da-793">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="ed2da-793">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="ed2da-794">Rede</span><span class="sxs-lookup"><span data-stu-id="ed2da-794">Networking</span></span>
- <span data-ttu-id="ed2da-795">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="ed2da-795">Storage</span></span>

<span data-ttu-id="ed2da-796">Esses módulos de comando podem ser usados na produção e são compatíveis com o SLA do Microsoft padrão.</span><span class="sxs-lookup"><span data-stu-id="ed2da-796">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="ed2da-797">Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="ed2da-797">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="ed2da-798">Você pode fazer perguntas sobre [StackOverflow usando a marcação azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) ou entrar em contato com a equipe do produto pelo endereço [ azfeedback@microsoft.com ](mailto:azfeedback@microsoft.com). Você pode fornecer comentários a partir da linha de comando com o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="ed2da-798">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="ed2da-799">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="ed2da-799">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="ed2da-800">Para verificar a versão da CLI, utilize `az --version`.</span><span class="sxs-lookup"><span data-stu-id="ed2da-800">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="ed2da-801">A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando.</span><span class="sxs-lookup"><span data-stu-id="ed2da-801">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="ed2da-802">Alguns dos módulos de comando têm um “b*n*” ou “rc*n*” pós-fixado.</span><span class="sxs-lookup"><span data-stu-id="ed2da-802">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="ed2da-803">Esses módulos de comando ainda estão em visualização e estarão disponíveis no futuro.</span><span class="sxs-lookup"><span data-stu-id="ed2da-803">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="ed2da-804">Também temos compilações de visualização diárias da CLI.</span><span class="sxs-lookup"><span data-stu-id="ed2da-804">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="ed2da-805">Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="ed2da-805">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="ed2da-806">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="ed2da-806">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="ed2da-807">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="ed2da-807">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="ed2da-808">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="ed2da-808">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="ed2da-809">Forneça comentários a partir da linha de comando com o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="ed2da-809">Provide feedback from the command line with the `az feedback` command.</span></span>

