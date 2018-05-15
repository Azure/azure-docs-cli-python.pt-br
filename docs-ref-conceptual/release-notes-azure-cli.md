---
title: Notas de versão da CLI do Azure 2.0
description: Saiba mais sobre as últimas atualizações da CLI do Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 04/10/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 254c7b306440d921cef6b611268839150fdf3196
ms.sourcegitcommit: 15d6dfaee2075d0abceb2aa2423f0b6ef7b2ac9b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="90c50-103">Notas de versão da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="90c50-103">Azure CLI 2.0 release notes</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="90c50-104">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="90c50-104">May 7, 2018</span></span>

<span data-ttu-id="90c50-105">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="90c50-105">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="90c50-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="90c50-106">Core</span></span>

* <span data-ttu-id="90c50-107">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="90c50-107">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="90c50-108">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="90c50-108">Added limited support for positional arguments</span></span>
* <span data-ttu-id="90c50-109">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="90c50-109">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="90c50-110">#5591</span><span class="sxs-lookup"><span data-stu-id="90c50-110">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="90c50-111">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="90c50-111">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="90c50-112">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="90c50-112">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="90c50-113">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="90c50-113">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="90c50-114">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="90c50-114">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="90c50-115">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="90c50-115">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="90c50-116">ACR</span><span class="sxs-lookup"><span data-stu-id="90c50-116">ACR</span></span>

* <span data-ttu-id="90c50-117">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="90c50-117">Added ACR Build commands</span></span>
* <span data-ttu-id="90c50-118">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="90c50-118">Improved resource not found error messages</span></span>
* <span data-ttu-id="90c50-119">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="90c50-119">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="90c50-120">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="90c50-120">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="90c50-121">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="90c50-121">Improved repository commands error messages</span></span>
* <span data-ttu-id="90c50-122">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="90c50-122">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="90c50-123">ACS</span><span class="sxs-lookup"><span data-stu-id="90c50-123">ACS</span></span>

* <span data-ttu-id="90c50-124">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="90c50-124">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="90c50-125">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="90c50-125">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="90c50-126">AMS</span><span class="sxs-lookup"><span data-stu-id="90c50-126">AMS</span></span>

* <span data-ttu-id="90c50-127">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="90c50-127">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="90c50-128">AppService</span><span class="sxs-lookup"><span data-stu-id="90c50-128">Appservice</span></span>

* <span data-ttu-id="90c50-129">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="90c50-129">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="90c50-130">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="90c50-130">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="90c50-131">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="90c50-131">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="90c50-132">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="90c50-132">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="90c50-133">Lote AI</span><span class="sxs-lookup"><span data-stu-id="90c50-133">Batch AI</span></span>

* <span data-ttu-id="90c50-134">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="90c50-134">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="90c50-135">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="90c50-135">Cognitive Services</span></span>

* <span data-ttu-id="90c50-136">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="90c50-136">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="90c50-137">Consumo</span><span class="sxs-lookup"><span data-stu-id="90c50-137">Consumption</span></span>

* <span data-ttu-id="90c50-138">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="90c50-138">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="90c50-139">Contêiner</span><span class="sxs-lookup"><span data-stu-id="90c50-139">Container</span></span>

* <span data-ttu-id="90c50-140">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="90c50-140">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="90c50-141">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="90c50-141">Cosmos DB</span></span>

* <span data-ttu-id="90c50-142">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="90c50-142">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="90c50-143">DMS</span><span class="sxs-lookup"><span data-stu-id="90c50-143">DMS</span></span>

* <span data-ttu-id="90c50-144">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="90c50-144">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="90c50-145">Extensão</span><span class="sxs-lookup"><span data-stu-id="90c50-145">Extension</span></span>

* <span data-ttu-id="90c50-146">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="90c50-146">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="90c50-147">Interativo</span><span class="sxs-lookup"><span data-stu-id="90c50-147">Interactive</span></span>

* <span data-ttu-id="90c50-148">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="90c50-148">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="90c50-149">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="90c50-149">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="90c50-150">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="90c50-150">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="90c50-151">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="90c50-151">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="90c50-152">Laboratório</span><span class="sxs-lookup"><span data-stu-id="90c50-152">Lab</span></span>

* <span data-ttu-id="90c50-153">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="90c50-153">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="90c50-154">Rede</span><span class="sxs-lookup"><span data-stu-id="90c50-154">Network</span></span>

* <span data-ttu-id="90c50-155">[ALTERAÇÃO DA FALHA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="90c50-155">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span> 
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="90c50-156">Perfil</span><span class="sxs-lookup"><span data-stu-id="90c50-156">Profile</span></span>

* <span data-ttu-id="90c50-157">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="90c50-157">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="90c50-158">[ALTERAÇÃO DA FALHA] `--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="90c50-158">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="90c50-159">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="90c50-159">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="90c50-160">Redis</span><span class="sxs-lookup"><span data-stu-id="90c50-160">Redis</span></span>

* <span data-ttu-id="90c50-161">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="90c50-161">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="90c50-162">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="90c50-162">Deprecated `redis list-all`.</span></span> <span data-ttu-id="90c50-163">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="90c50-163">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="90c50-164">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="90c50-164">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="90c50-165">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="90c50-165">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="90c50-166">Função</span><span class="sxs-lookup"><span data-stu-id="90c50-166">Role</span></span>

* <span data-ttu-id="90c50-167">[ALTERAÇÃO DA FALHA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="90c50-167">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="90c50-168">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="90c50-168">Storage</span></span>

* <span data-ttu-id="90c50-169">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="90c50-169">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="90c50-170">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="90c50-170">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="90c50-171">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="90c50-171">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="90c50-172">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="90c50-172">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="90c50-173">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="90c50-173">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="90c50-174">VM</span><span class="sxs-lookup"><span data-stu-id="90c50-174">VM</span></span>

* <span data-ttu-id="90c50-175">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="90c50-175">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="90c50-176">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="90c50-176">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="90c50-177">[ALTERAÇÃO DA FALHA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="90c50-177">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="90c50-178">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="90c50-178">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="90c50-179">[ALTERAÇÃO DA FALHA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="90c50-179">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="90c50-180">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="90c50-180">Added write accelerator support</span></span> 
* <span data-ttu-id="90c50-181">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="90c50-181">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="90c50-182">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="90c50-182">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="90c50-183">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="90c50-183">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="90c50-184">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="90c50-184">April 10, 2018</span></span>

<span data-ttu-id="90c50-185">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="90c50-185">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="90c50-186">ACR</span><span class="sxs-lookup"><span data-stu-id="90c50-186">ACR</span></span>

* <span data-ttu-id="90c50-187">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="90c50-187">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="90c50-188">ACS</span><span class="sxs-lookup"><span data-stu-id="90c50-188">ACS</span></span>

* <span data-ttu-id="90c50-189">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="90c50-189">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="90c50-190">AppService</span><span class="sxs-lookup"><span data-stu-id="90c50-190">Appservice</span></span>

* [ALTERAÇÃO DA FALHA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="90c50-192">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="90c50-192">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="90c50-193">BatchAI</span><span class="sxs-lookup"><span data-stu-id="90c50-193">BatchAI</span></span>

* <span data-ttu-id="90c50-194">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="90c50-194">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="90c50-195">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="90c50-195">Job level mounting</span></span>
 - <span data-ttu-id="90c50-196">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="90c50-196">Environment variables with secret values</span></span>
 - <span data-ttu-id="90c50-197">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="90c50-197">Performance counters settings</span></span>
 - <span data-ttu-id="90c50-198">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="90c50-198">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="90c50-199">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="90c50-199">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="90c50-200">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="90c50-200">Usage and limits reporting</span></span>
 - <span data-ttu-id="90c50-201">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="90c50-201">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="90c50-202">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="90c50-202">Support for custom images</span></span>
 - <span data-ttu-id="90c50-203">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="90c50-203">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="90c50-204">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="90c50-204">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="90c50-205">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="90c50-205">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="90c50-206">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="90c50-206">National clouds are supported</span></span>
* <span data-ttu-id="90c50-207">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="90c50-207">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="90c50-208">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="90c50-208">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="90c50-209">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="90c50-209">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="90c50-210">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="90c50-210">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="90c50-211">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="90c50-211">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="90c50-212">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="90c50-212">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="90c50-213">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="90c50-213">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="90c50-214">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="90c50-214">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="90c50-215">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="90c50-215">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="90c50-216">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="90c50-216">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="90c50-217">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="90c50-217">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="90c50-218">[ALTERAÇÃO DA FALHA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="90c50-218">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="90c50-219">[ALTERAÇÃO DA FALHA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="90c50-219">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="90c50-220">Cobrança</span><span class="sxs-lookup"><span data-stu-id="90c50-220">Billing</span></span>

* <span data-ttu-id="90c50-221">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="90c50-221">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="90c50-222">Consumo</span><span class="sxs-lookup"><span data-stu-id="90c50-222">Consumption</span></span>

* <span data-ttu-id="90c50-223">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="90c50-223">Added `marketplace` commands</span></span>
* <span data-ttu-id="90c50-224">[ALTERAÇÃO DA FALHA] `reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="90c50-224">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="90c50-225">[ALTERAÇÃO DA FALHA] `reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="90c50-225">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="90c50-226">[ALTERAÇÃO DA FALHA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="90c50-226">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="90c50-227">[ALTERAÇÃO DA FALHA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="90c50-227">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="90c50-228">[ALTERAÇÃO DA FALHA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="90c50-228">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="90c50-229">Contêiner</span><span class="sxs-lookup"><span data-stu-id="90c50-229">Container</span></span>

* <span data-ttu-id="90c50-230">Adição dos parâmetros de montagem de volume de repositório git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="90c50-230">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="90c50-231">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="90c50-231">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="90c50-232">Extensão</span><span class="sxs-lookup"><span data-stu-id="90c50-232">Extension</span></span>

* <span data-ttu-id="90c50-233">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="90c50-233">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="90c50-234">Interativo</span><span class="sxs-lookup"><span data-stu-id="90c50-234">Interactive</span></span>

* <span data-ttu-id="90c50-235">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="90c50-235">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="90c50-236">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="90c50-236">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="90c50-237">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="90c50-237">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="90c50-238">Rede</span><span class="sxs-lookup"><span data-stu-id="90c50-238">Network</span></span>

* <span data-ttu-id="90c50-239">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="90c50-239">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="90c50-240">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="90c50-240">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="90c50-241">#4910</span><span class="sxs-lookup"><span data-stu-id="90c50-241">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="90c50-242">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="90c50-242">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="90c50-243">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="90c50-243">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="90c50-244">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="90c50-244">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="90c50-245">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="90c50-245">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="90c50-246">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="90c50-246">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="90c50-247">Perfil</span><span class="sxs-lookup"><span data-stu-id="90c50-247">Profile</span></span>

* <span data-ttu-id="90c50-248">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="90c50-248">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="90c50-249">[ALTERAÇÃO DA FALHA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="90c50-249">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="90c50-250">RDBMS</span><span class="sxs-lookup"><span data-stu-id="90c50-250">RDBMS</span></span>

* <span data-ttu-id="90c50-251">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="90c50-251">Added `georestore` command</span></span>
* <span data-ttu-id="90c50-252">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="90c50-252">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="90c50-253">Recurso</span><span class="sxs-lookup"><span data-stu-id="90c50-253">Resource</span></span>

* <span data-ttu-id="90c50-254">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="90c50-254">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="90c50-255">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="90c50-255">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="90c50-256">SQL</span><span class="sxs-lookup"><span data-stu-id="90c50-256">SQL</span></span>

* <span data-ttu-id="90c50-257">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="90c50-257">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="90c50-258">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="90c50-258">Storage</span></span>

* <span data-ttu-id="90c50-259">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="90c50-259">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="90c50-260">VM</span><span class="sxs-lookup"><span data-stu-id="90c50-260">VM</span></span>

* <span data-ttu-id="90c50-261">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="90c50-261">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="90c50-262">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="90c50-262">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="90c50-264">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="90c50-264">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="90c50-265">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="90c50-265">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="90c50-266">#5718</span><span class="sxs-lookup"><span data-stu-id="90c50-266">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="90c50-267">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="90c50-267">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="90c50-268">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="90c50-268">March 27, 2018</span></span>

<span data-ttu-id="90c50-269">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="90c50-269">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="90c50-270">Núcleo</span><span class="sxs-lookup"><span data-stu-id="90c50-270">Core</span></span>

* <span data-ttu-id="90c50-271">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="90c50-271">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="90c50-272">ACS</span><span class="sxs-lookup"><span data-stu-id="90c50-272">ACS</span></span>

* <span data-ttu-id="90c50-273">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="90c50-273">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="90c50-274">AppService</span><span class="sxs-lookup"><span data-stu-id="90c50-274">Appservice</span></span>

* <span data-ttu-id="90c50-275">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="90c50-275">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="90c50-276">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="90c50-276">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="90c50-277">Backup</span><span class="sxs-lookup"><span data-stu-id="90c50-277">Backup</span></span>

* <span data-ttu-id="90c50-278">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="90c50-278">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="90c50-279">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="90c50-279">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="90c50-280">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="90c50-280">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="90c50-281">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="90c50-281">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="90c50-282">Contêiner</span><span class="sxs-lookup"><span data-stu-id="90c50-282">Container</span></span>

* <span data-ttu-id="90c50-283">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="90c50-283">Added `container exec` command.</span></span> <span data-ttu-id="90c50-284">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="90c50-284">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="90c50-285">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="90c50-285">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="90c50-286">Extensão</span><span class="sxs-lookup"><span data-stu-id="90c50-286">Extension</span></span>

* <span data-ttu-id="90c50-287">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="90c50-287">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="90c50-288">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="90c50-288">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="90c50-289">[ALTERAÇÃO DA FALHA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="90c50-289">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="90c50-290">Interativo</span><span class="sxs-lookup"><span data-stu-id="90c50-290">Interactive</span></span>

* <span data-ttu-id="90c50-291">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="90c50-291">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="90c50-292">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="90c50-292">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="90c50-293">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="90c50-293">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="90c50-294">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="90c50-294">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="90c50-295">Laboratório</span><span class="sxs-lookup"><span data-stu-id="90c50-295">Lab</span></span>

* <span data-ttu-id="90c50-296">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="90c50-296">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="90c50-297">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="90c50-297">Monitor</span></span>

* <span data-ttu-id="90c50-298">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="90c50-298">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="90c50-299">[#4529](https://github.com/Azure/azure-cli/issues/5785) corrigido: `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="90c50-299">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="90c50-300">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="90c50-300">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="90c50-301">Rede</span><span class="sxs-lookup"><span data-stu-id="90c50-301">Network</span></span>

* <span data-ttu-id="90c50-302">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="90c50-302">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="90c50-303">Perfil</span><span class="sxs-lookup"><span data-stu-id="90c50-303">Profile</span></span>

* <span data-ttu-id="90c50-304">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="90c50-304">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="90c50-305">RDBMS</span><span class="sxs-lookup"><span data-stu-id="90c50-305">RDBMS</span></span>

* <span data-ttu-id="90c50-306">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="90c50-306">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="90c50-307">Recurso</span><span class="sxs-lookup"><span data-stu-id="90c50-307">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="90c50-309">Função</span><span class="sxs-lookup"><span data-stu-id="90c50-309">Role</span></span>

* <span data-ttu-id="90c50-310">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="90c50-310">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="90c50-311">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="90c50-311">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="90c50-312">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="90c50-312">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="90c50-313">[ALTERAÇÃO DA FALHA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="90c50-313">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="90c50-314">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="90c50-314">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="90c50-315">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="90c50-315">Storage</span></span>

* <span data-ttu-id="90c50-316">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="90c50-316">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="90c50-317">[4049#](https://github.com/Azure/azure-cli/issues/4049) corrigido: problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="90c50-317">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="90c50-318">VM</span><span class="sxs-lookup"><span data-stu-id="90c50-318">VM</span></span>

* <span data-ttu-id="90c50-319">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="90c50-319">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="90c50-320">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="90c50-320">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="90c50-321">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="90c50-321">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="90c50-322">[ALTERAÇÃO DA FALHA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="90c50-322">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="90c50-323">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="90c50-323">March 13, 2018</span></span>

<span data-ttu-id="90c50-324">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="90c50-324">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="90c50-325">ACR</span><span class="sxs-lookup"><span data-stu-id="90c50-325">ACR</span></span>

* <span data-ttu-id="90c50-326">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="90c50-326">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="90c50-327">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="90c50-327">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="90c50-328">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="90c50-328">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="90c50-329">ACS</span><span class="sxs-lookup"><span data-stu-id="90c50-329">ACS</span></span>

* <span data-ttu-id="90c50-330">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="90c50-330">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="90c50-331">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="90c50-331">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="90c50-332">Supervisor</span><span class="sxs-lookup"><span data-stu-id="90c50-332">Advisor</span></span>

* <span data-ttu-id="90c50-333">[ALTERAÇÃO DA FALHA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="90c50-333">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="90c50-334">[ALTERAÇÃO DA FALHA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="90c50-334">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="90c50-335">[ALTERAÇÃO DA FALHA] `advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="90c50-335">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="90c50-336">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="90c50-336">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="90c50-337">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="90c50-337">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="90c50-338">AppService</span><span class="sxs-lookup"><span data-stu-id="90c50-338">Appservice</span></span>

* <span data-ttu-id="90c50-339">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="90c50-339">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="90c50-340">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="90c50-340">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="90c50-341">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="90c50-341">Eventhubs</span></span>

* <span data-ttu-id="90c50-342">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="90c50-342">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="90c50-343">Extensão</span><span class="sxs-lookup"><span data-stu-id="90c50-343">Extension</span></span>

* <span data-ttu-id="90c50-344">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="90c50-344">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="90c50-345">Interativo</span><span class="sxs-lookup"><span data-stu-id="90c50-345">Interactive</span></span>

* <span data-ttu-id="90c50-346">[5625](https://github.com/Azure/azure-cli/issues/5625) corrigido: manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="90c50-346">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="90c50-347">[3016](https://github.com/Azure/azure-cli/issues/3016) corrigido: histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="90c50-347">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="90c50-348">[5688](https://github.com/Azure/azure-cli/issues/5688) corrigido: as conclusões não aparecerão se o carregamento da tabela de comando encontrou uma exceção</span><span class="sxs-lookup"><span data-stu-id="90c50-348">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="90c50-349">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="90c50-349">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="90c50-350">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="90c50-350">Monitor</span></span>

* <span data-ttu-id="90c50-351">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="90c50-351">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="90c50-352">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="90c50-352">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="90c50-353">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="90c50-353">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="90c50-354">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="90c50-354">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="90c50-355">Rede</span><span class="sxs-lookup"><span data-stu-id="90c50-355">Network</span></span>

* <span data-ttu-id="90c50-356">[ALTERAÇÃO DA FALHA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="90c50-356">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="90c50-357">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="90c50-357">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="90c50-358">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="90c50-358">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="90c50-359">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="90c50-359">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="90c50-360">Perfil</span><span class="sxs-lookup"><span data-stu-id="90c50-360">Profile</span></span>

* <span data-ttu-id="90c50-361">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="90c50-361">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="90c50-362">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="90c50-362">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="90c50-363">RDBMS</span><span class="sxs-lookup"><span data-stu-id="90c50-363">RDBMS</span></span>

* <span data-ttu-id="90c50-364">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="90c50-364">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="90c50-365">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="90c50-365">Service Bus</span></span>

* <span data-ttu-id="90c50-366">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="90c50-366">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="90c50-367">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="90c50-367">Storage</span></span>

* <span data-ttu-id="90c50-368">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="90c50-368">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="90c50-369">[5286](https://github.com/Azure/azure-cli/issues/5286) corrigido: os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="90c50-369">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="90c50-370">VM</span><span class="sxs-lookup"><span data-stu-id="90c50-370">VM</span></span>

* <span data-ttu-id="90c50-371">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="90c50-371">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="90c50-372">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="90c50-372">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="90c50-373">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="90c50-373">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="90c50-374">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="90c50-374">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="90c50-375">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="90c50-375">February 27, 2018</span></span>

<span data-ttu-id="90c50-376">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="90c50-376">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="90c50-377">Núcleo</span><span class="sxs-lookup"><span data-stu-id="90c50-377">Core</span></span>

* <span data-ttu-id="90c50-378">Correção [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="90c50-378">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="90c50-379">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="90c50-379">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="90c50-380">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="90c50-380">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="90c50-381">ACS</span><span class="sxs-lookup"><span data-stu-id="90c50-381">ACS</span></span>

* <span data-ttu-id="90c50-382">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="90c50-382">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="90c50-383">Correção do problema de permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="90c50-383">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="90c50-384">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="90c50-384">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="90c50-385">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="90c50-385">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="90c50-386">AppService</span><span class="sxs-lookup"><span data-stu-id="90c50-386">Appservice</span></span>

* <span data-ttu-id="90c50-387">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="90c50-387">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="90c50-388">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="90c50-388">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="90c50-389">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="90c50-389">Cognitive Services</span></span>

* <span data-ttu-id="90c50-390">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="90c50-390">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="90c50-391">Consumo</span><span class="sxs-lookup"><span data-stu-id="90c50-391">Consumption</span></span>

* <span data-ttu-id="90c50-392">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="90c50-392">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="90c50-393">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="90c50-393">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="90c50-394">Contêiner</span><span class="sxs-lookup"><span data-stu-id="90c50-394">Container</span></span>

* <span data-ttu-id="90c50-395">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="90c50-395">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="90c50-396">Rede</span><span class="sxs-lookup"><span data-stu-id="90c50-396">Network</span></span>

* <span data-ttu-id="90c50-397">Correção [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="90c50-397">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="90c50-398">Recurso</span><span class="sxs-lookup"><span data-stu-id="90c50-398">Resource</span></span>

* <span data-ttu-id="90c50-399">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="90c50-399">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="90c50-400">Função</span><span class="sxs-lookup"><span data-stu-id="90c50-400">Role</span></span>

* <span data-ttu-id="90c50-401">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="90c50-401">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="90c50-402">SQL</span><span class="sxs-lookup"><span data-stu-id="90c50-402">SQL</span></span>

* <span data-ttu-id="90c50-403">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="90c50-403">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="90c50-404">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="90c50-404">Storage</span></span>

* <span data-ttu-id="90c50-405">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="90c50-405">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="90c50-406">VM</span><span class="sxs-lookup"><span data-stu-id="90c50-406">VM</span></span>

* <span data-ttu-id="90c50-407">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="90c50-407">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="90c50-408">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="90c50-408">February 13, 2018</span></span>

<span data-ttu-id="90c50-409">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="90c50-409">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="90c50-410">Núcleo</span><span class="sxs-lookup"><span data-stu-id="90c50-410">Core</span></span>

* <span data-ttu-id="90c50-411">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="90c50-411">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="90c50-412">ACS</span><span class="sxs-lookup"><span data-stu-id="90c50-412">ACS</span></span>

* <span data-ttu-id="90c50-413">[ALTERAÇÃO DA FALHA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="90c50-413">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="90c50-414">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="90c50-414">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="90c50-415">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="90c50-415">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="90c50-416">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="90c50-416">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="90c50-417">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="90c50-417">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="90c50-418">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="90c50-418">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="90c50-419">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="90c50-419">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="90c50-420">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="90c50-420">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="90c50-421">AppService</span><span class="sxs-lookup"><span data-stu-id="90c50-421">Appservice</span></span>

* <span data-ttu-id="90c50-422">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="90c50-422">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="90c50-423">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="90c50-423">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="90c50-424">CDN</span><span class="sxs-lookup"><span data-stu-id="90c50-424">CDN</span></span>

* <span data-ttu-id="90c50-425">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="90c50-425">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="90c50-426">Contêiner</span><span class="sxs-lookup"><span data-stu-id="90c50-426">Container</span></span>

* <span data-ttu-id="90c50-427">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="90c50-427">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="90c50-428">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="90c50-428">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="90c50-429">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="90c50-429">CosmosDB</span></span>

* <span data-ttu-id="90c50-430">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="90c50-430">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="90c50-431">Extensão</span><span class="sxs-lookup"><span data-stu-id="90c50-431">Extension</span></span>

* <span data-ttu-id="90c50-432">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="90c50-432">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="90c50-433">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="90c50-433">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="90c50-434">Comentários</span><span class="sxs-lookup"><span data-stu-id="90c50-434">Feedback</span></span>

* <span data-ttu-id="90c50-435">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="90c50-435">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="90c50-436">Interativo</span><span class="sxs-lookup"><span data-stu-id="90c50-436">Interactive</span></span>

* <span data-ttu-id="90c50-437">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="90c50-437">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="90c50-438">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="90c50-438">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="90c50-439">IoT</span><span class="sxs-lookup"><span data-stu-id="90c50-439">IoT</span></span>

* <span data-ttu-id="90c50-440">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="90c50-440">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="90c50-441">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="90c50-441">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="90c50-442">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="90c50-442">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="90c50-443">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="90c50-443">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="90c50-444">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="90c50-444">Monitor</span></span>

* <span data-ttu-id="90c50-445">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="90c50-445">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="90c50-446">Rede</span><span class="sxs-lookup"><span data-stu-id="90c50-446">Network</span></span>

* <span data-ttu-id="90c50-447">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="90c50-447">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="90c50-448">Perfil</span><span class="sxs-lookup"><span data-stu-id="90c50-448">Profile</span></span>

* <span data-ttu-id="90c50-449">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="90c50-449">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="90c50-450">Recurso</span><span class="sxs-lookup"><span data-stu-id="90c50-450">Resource</span></span>

* <span data-ttu-id="90c50-451">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="90c50-451">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="90c50-452">Função</span><span class="sxs-lookup"><span data-stu-id="90c50-452">Role</span></span>

* <span data-ttu-id="90c50-453">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="90c50-453">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="90c50-454">SQL</span><span class="sxs-lookup"><span data-stu-id="90c50-454">SQL</span></span>

* <span data-ttu-id="90c50-455">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="90c50-455">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="90c50-456">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="90c50-456">Added `sql db rename`</span></span>
* <span data-ttu-id="90c50-457">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="90c50-457">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="90c50-458">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="90c50-458">Storage</span></span>

* <span data-ttu-id="90c50-459">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="90c50-459">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="90c50-460">VM</span><span class="sxs-lookup"><span data-stu-id="90c50-460">VM</span></span>

* <span data-ttu-id="90c50-461">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="90c50-461">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="90c50-462">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="90c50-462">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="90c50-463">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="90c50-463">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="90c50-464">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="90c50-464">January 31, 2018</span></span>

<span data-ttu-id="90c50-465">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="90c50-465">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="90c50-466">Núcleo</span><span class="sxs-lookup"><span data-stu-id="90c50-466">Core</span></span>

* <span data-ttu-id="90c50-467">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="90c50-467">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="90c50-468">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="90c50-468">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="90c50-469">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="90c50-469">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="90c50-470">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="90c50-470">Use `--verbose` to see</span></span>
* <span data-ttu-id="90c50-471">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="90c50-471">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="90c50-472">ACS</span><span class="sxs-lookup"><span data-stu-id="90c50-472">ACS</span></span>

* <span data-ttu-id="90c50-473">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="90c50-473">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="90c50-474">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="90c50-474">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="90c50-475">AppService</span><span class="sxs-lookup"><span data-stu-id="90c50-475">Appservice</span></span>

* <span data-ttu-id="90c50-476">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="90c50-476">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="90c50-477">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="90c50-477">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="90c50-478">CDN</span><span class="sxs-lookup"><span data-stu-id="90c50-478">CDN</span></span>

* <span data-ttu-id="90c50-479">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="90c50-479">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="90c50-480">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="90c50-480">CosmosDB</span></span>

* <span data-ttu-id="90c50-481">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="90c50-481">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="90c50-482">Interativo</span><span class="sxs-lookup"><span data-stu-id="90c50-482">Interactive</span></span>

* <span data-ttu-id="90c50-483">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="90c50-483">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="90c50-484">Rede</span><span class="sxs-lookup"><span data-stu-id="90c50-484">Network</span></span>

* <span data-ttu-id="90c50-485">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="90c50-485">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="90c50-486">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="90c50-486">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="90c50-487">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="90c50-487">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="90c50-488">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="90c50-488">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="90c50-489">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="90c50-489">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="90c50-490">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="90c50-490">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="90c50-491">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="90c50-491">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="90c50-492">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="90c50-492">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="90c50-493">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="90c50-493">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="90c50-494">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="90c50-494">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="90c50-495">Perfil</span><span class="sxs-lookup"><span data-stu-id="90c50-495">Profile</span></span>

* <span data-ttu-id="90c50-496">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="90c50-496">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="90c50-497">Recurso</span><span class="sxs-lookup"><span data-stu-id="90c50-497">Resource</span></span>

* <span data-ttu-id="90c50-498">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="90c50-498">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="90c50-499">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="90c50-499">Storage</span></span>

* <span data-ttu-id="90c50-500">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="90c50-500">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="90c50-501">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="90c50-501">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="90c50-502">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="90c50-502">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="90c50-503">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="90c50-503">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="90c50-504">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="90c50-504">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="90c50-505">VM</span><span class="sxs-lookup"><span data-stu-id="90c50-505">VM</span></span>

* <span data-ttu-id="90c50-506">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="90c50-506">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="90c50-507">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="90c50-507">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="90c50-508">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="90c50-508">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="90c50-509">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="90c50-509">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="90c50-510">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="90c50-510">January 17, 2018</span></span>

<span data-ttu-id="90c50-511">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="90c50-511">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="90c50-512">ACR</span><span class="sxs-lookup"><span data-stu-id="90c50-512">ACR</span></span>

* <span data-ttu-id="90c50-513">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="90c50-513">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="90c50-514">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="90c50-514">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="90c50-515">ACS</span><span class="sxs-lookup"><span data-stu-id="90c50-515">ACS</span></span>

* <span data-ttu-id="90c50-516">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="90c50-516">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="90c50-517">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="90c50-517">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="90c50-518">AppService</span><span class="sxs-lookup"><span data-stu-id="90c50-518">Appservice</span></span>

* <span data-ttu-id="90c50-519">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="90c50-519">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="90c50-520">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="90c50-520">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="90c50-521">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="90c50-521">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="90c50-522">Backup</span><span class="sxs-lookup"><span data-stu-id="90c50-522">Backup</span></span>

* <span data-ttu-id="90c50-523">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="90c50-523">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="90c50-524">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="90c50-524">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="90c50-525">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="90c50-525">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="90c50-526">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="90c50-526">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="90c50-527">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="90c50-527">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="90c50-528">Lote</span><span class="sxs-lookup"><span data-stu-id="90c50-528">Batch</span></span>

* <span data-ttu-id="90c50-529">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="90c50-529">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="90c50-530">Nuvem</span><span class="sxs-lookup"><span data-stu-id="90c50-530">Cloud</span></span>

* <span data-ttu-id="90c50-531">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="90c50-531">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="90c50-532">Consumo</span><span class="sxs-lookup"><span data-stu-id="90c50-532">Consumption</span></span>

* <span data-ttu-id="90c50-533">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="90c50-533">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="90c50-534">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="90c50-534">Event Grid</span></span>

* <span data-ttu-id="90c50-535">[ALTERAÇÃO DA FALHA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="90c50-535">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="90c50-536">[ALTERAÇÃO DA FALHA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="90c50-536">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="90c50-537">[ALTERAÇÃO DA FALHA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="90c50-537">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="90c50-538">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="90c50-538">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="90c50-539">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="90c50-539">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="90c50-540">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="90c50-540">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="90c50-541">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="90c50-541">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="90c50-542">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="90c50-542">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="90c50-543">Interativo</span><span class="sxs-lookup"><span data-stu-id="90c50-543">Interactive</span></span>

* <span data-ttu-id="90c50-544">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="90c50-544">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="90c50-545">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="90c50-545">Fixed errors on startup</span></span>
* <span data-ttu-id="90c50-546">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="90c50-546">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="90c50-547">IoT</span><span class="sxs-lookup"><span data-stu-id="90c50-547">IoT</span></span>

* <span data-ttu-id="90c50-548">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="90c50-548">Added support for device provisioning service</span></span>
* <span data-ttu-id="90c50-549">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="90c50-549">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="90c50-550">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="90c50-550">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="90c50-551">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="90c50-551">Monitor</span></span>

* <span data-ttu-id="90c50-552">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="90c50-552">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="90c50-553">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="90c50-553">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="90c50-554">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="90c50-554">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="90c50-555">Rede</span><span class="sxs-lookup"><span data-stu-id="90c50-555">Network</span></span>

* <span data-ttu-id="90c50-556">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="90c50-556">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="90c50-557">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="90c50-557">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="90c50-558">Perfil</span><span class="sxs-lookup"><span data-stu-id="90c50-558">Profile</span></span>

* <span data-ttu-id="90c50-559">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="90c50-559">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="90c50-560">Função</span><span class="sxs-lookup"><span data-stu-id="90c50-560">Role</span></span>

* <span data-ttu-id="90c50-561">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="90c50-561">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="90c50-562">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="90c50-562">Service Fabric</span></span>

* <span data-ttu-id="90c50-563">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="90c50-563">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="90c50-564">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="90c50-564">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="90c50-565">VM</span><span class="sxs-lookup"><span data-stu-id="90c50-565">VM</span></span>

* <span data-ttu-id="90c50-566">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="90c50-566">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="90c50-567">[ALTERAÇÃO DA FALHA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="90c50-567">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="90c50-568">[ALTERAÇÃO DA FALHA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="90c50-568">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="90c50-569">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="90c50-569">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="90c50-570">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="90c50-570">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="90c50-571">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="90c50-571">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="90c50-572">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="90c50-572">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="90c50-573">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="90c50-573">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="90c50-574">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="90c50-574">December 19, 2017</span></span>

<span data-ttu-id="90c50-575">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="90c50-575">Version 2.0.23</span></span>

* <span data-ttu-id="90c50-576">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="90c50-576">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="90c50-577">Contêiner</span><span class="sxs-lookup"><span data-stu-id="90c50-577">Container</span></span>

* <span data-ttu-id="90c50-578">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="90c50-578">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="90c50-579">Rede</span><span class="sxs-lookup"><span data-stu-id="90c50-579">Network</span></span>

* <span data-ttu-id="90c50-580">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="90c50-580">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="90c50-581">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="90c50-581">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="90c50-582">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="90c50-582">Storage</span></span>

* <span data-ttu-id="90c50-583">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="90c50-583">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="90c50-584">VM</span><span class="sxs-lookup"><span data-stu-id="90c50-584">VM</span></span>

* <span data-ttu-id="90c50-585">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="90c50-585">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="90c50-586">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="90c50-586">December 5, 2017</span></span>

<span data-ttu-id="90c50-587">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="90c50-587">Version 2.0.22</span></span>

* <span data-ttu-id="90c50-588">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="90c50-588">Removed `az component` commands.</span></span> <span data-ttu-id="90c50-589">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="90c50-589">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="90c50-590">Núcleo</span><span class="sxs-lookup"><span data-stu-id="90c50-590">Core</span></span>
* <span data-ttu-id="90c50-591">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="90c50-591">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="90c50-592">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="90c50-592">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="90c50-593">ACS</span><span class="sxs-lookup"><span data-stu-id="90c50-593">ACS</span></span>

* <span data-ttu-id="90c50-594">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="90c50-594">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="90c50-595">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="90c50-595">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="90c50-596">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="90c50-596">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="90c50-597">Supervisor</span><span class="sxs-lookup"><span data-stu-id="90c50-597">Advisor</span></span>

* <span data-ttu-id="90c50-598">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="90c50-598">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="90c50-599">AppService</span><span class="sxs-lookup"><span data-stu-id="90c50-599">Appservice</span></span>

* <span data-ttu-id="90c50-600">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="90c50-600">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="90c50-601">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="90c50-601">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="90c50-602">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="90c50-602">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="90c50-603">Consumo</span><span class="sxs-lookup"><span data-stu-id="90c50-603">Consumption</span></span>

* <span data-ttu-id="90c50-604">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="90c50-604">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="90c50-605">Contêiner</span><span class="sxs-lookup"><span data-stu-id="90c50-605">Container</span></span>

* <span data-ttu-id="90c50-606">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="90c50-606">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="90c50-607">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="90c50-607">Monitor</span></span>

* <span data-ttu-id="90c50-608">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="90c50-608">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="90c50-609">Recurso</span><span class="sxs-lookup"><span data-stu-id="90c50-609">Resource</span></span>

* <span data-ttu-id="90c50-610">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="90c50-610">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="90c50-611">Função</span><span class="sxs-lookup"><span data-stu-id="90c50-611">Role</span></span>

* <span data-ttu-id="90c50-612">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="90c50-612">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="90c50-613">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="90c50-613">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="90c50-614">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="90c50-614">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="90c50-615">SQL</span><span class="sxs-lookup"><span data-stu-id="90c50-615">SQL</span></span>

* <span data-ttu-id="90c50-616">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="90c50-616">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="90c50-617">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="90c50-617">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="90c50-618">VM</span><span class="sxs-lookup"><span data-stu-id="90c50-618">VM</span></span>

* <span data-ttu-id="90c50-619">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="90c50-619">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="90c50-620">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="90c50-620">November 14, 2017</span></span>

<span data-ttu-id="90c50-621">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="90c50-621">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="90c50-622">ACR</span><span class="sxs-lookup"><span data-stu-id="90c50-622">ACR</span></span>

* <span data-ttu-id="90c50-623">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="90c50-623">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="90c50-624">ACS</span><span class="sxs-lookup"><span data-stu-id="90c50-624">ACS</span></span>

* <span data-ttu-id="90c50-625">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="90c50-625">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="90c50-626">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="90c50-626">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="90c50-627">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="90c50-627">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="90c50-628">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="90c50-628">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="90c50-629">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="90c50-629">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="90c50-630">AppService</span><span class="sxs-lookup"><span data-stu-id="90c50-630">Appservice</span></span>

* <span data-ttu-id="90c50-631">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="90c50-631">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="90c50-632">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="90c50-632">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="90c50-633">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="90c50-633">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="90c50-634">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="90c50-634">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="90c50-635">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="90c50-635">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="90c50-636">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="90c50-636">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="90c50-637">Lote</span><span class="sxs-lookup"><span data-stu-id="90c50-637">Batch</span></span>

* <span data-ttu-id="90c50-638">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="90c50-638">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="90c50-639">Batchai</span><span class="sxs-lookup"><span data-stu-id="90c50-639">Batchai</span></span>

* <span data-ttu-id="90c50-640">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="90c50-640">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="90c50-641">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="90c50-641">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="90c50-642">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="90c50-642">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="90c50-643">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="90c50-643">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="90c50-644">Nuvem</span><span class="sxs-lookup"><span data-stu-id="90c50-644">Cloud</span></span>

* <span data-ttu-id="90c50-645">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="90c50-645">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="90c50-646">Contêiner</span><span class="sxs-lookup"><span data-stu-id="90c50-646">Container</span></span>

* <span data-ttu-id="90c50-647">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="90c50-647">Added support to open multiple ports</span></span>
* <span data-ttu-id="90c50-648">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="90c50-648">Added container group restart policy</span></span>
* <span data-ttu-id="90c50-649">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="90c50-649">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="90c50-650">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="90c50-650">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="90c50-651">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="90c50-651">Data Lake Analytics</span></span>

* <span data-ttu-id="90c50-652">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="90c50-652">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="90c50-653">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="90c50-653">Data Lake Store</span></span>

* <span data-ttu-id="90c50-654">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="90c50-654">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="90c50-655">Extensão</span><span class="sxs-lookup"><span data-stu-id="90c50-655">Extension</span></span>

* <span data-ttu-id="90c50-656">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="90c50-656">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="90c50-657">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="90c50-657">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="90c50-658">IoT</span><span class="sxs-lookup"><span data-stu-id="90c50-658">IoT</span></span>

* <span data-ttu-id="90c50-659">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="90c50-659">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="90c50-660">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="90c50-660">Monitor</span></span>

* <span data-ttu-id="90c50-661">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="90c50-661">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="90c50-662">Rede</span><span class="sxs-lookup"><span data-stu-id="90c50-662">Network</span></span>

* <span data-ttu-id="90c50-663">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="90c50-663">Added support for CAA DNS records</span></span>
* <span data-ttu-id="90c50-664">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="90c50-664">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="90c50-665">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="90c50-665">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="90c50-666">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="90c50-666">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="90c50-667">Reservas</span><span class="sxs-lookup"><span data-stu-id="90c50-667">Reservations</span></span>

* <span data-ttu-id="90c50-668">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="90c50-668">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="90c50-669">Recurso</span><span class="sxs-lookup"><span data-stu-id="90c50-669">Resource</span></span>

* <span data-ttu-id="90c50-670">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="90c50-670">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="90c50-671">SQL</span><span class="sxs-lookup"><span data-stu-id="90c50-671">SQL</span></span>

* <span data-ttu-id="90c50-672">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="90c50-672">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="90c50-673">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="90c50-673">Storage</span></span>

* <span data-ttu-id="90c50-674">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="90c50-674">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="90c50-675">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="90c50-675">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="90c50-676">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="90c50-676">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="90c50-677">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="90c50-677">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="90c50-678">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="90c50-678">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="90c50-679">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="90c50-679">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="90c50-680">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="90c50-680">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="90c50-681">VM</span><span class="sxs-lookup"><span data-stu-id="90c50-681">VM</span></span>

* <span data-ttu-id="90c50-682">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="90c50-682">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="90c50-683">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="90c50-683">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="90c50-684">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="90c50-684">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="90c50-685">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="90c50-685">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="90c50-686">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="90c50-686">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="90c50-687">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="90c50-687">October 24, 2017</span></span>

<span data-ttu-id="90c50-688">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="90c50-688">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="90c50-689">Núcleo</span><span class="sxs-lookup"><span data-stu-id="90c50-689">Core</span></span>

* <span data-ttu-id="90c50-690">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="90c50-690">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="90c50-691">ACR</span><span class="sxs-lookup"><span data-stu-id="90c50-691">ACR</span></span>

* <span data-ttu-id="90c50-692">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="90c50-692">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="90c50-693">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="90c50-693">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="90c50-694">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="90c50-694">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="90c50-695">ACS</span><span class="sxs-lookup"><span data-stu-id="90c50-695">ACS</span></span>

* <span data-ttu-id="90c50-696">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="90c50-696">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="90c50-697">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="90c50-697">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="90c50-698">AppService</span><span class="sxs-lookup"><span data-stu-id="90c50-698">Appservice</span></span>

* <span data-ttu-id="90c50-699">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="90c50-699">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="90c50-700">Componente</span><span class="sxs-lookup"><span data-stu-id="90c50-700">Component</span></span>

* <span data-ttu-id="90c50-701">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="90c50-701">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="90c50-702">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="90c50-702">Monitor</span></span>

* <span data-ttu-id="90c50-703">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="90c50-703">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="90c50-704">Recurso</span><span class="sxs-lookup"><span data-stu-id="90c50-704">Resource</span></span>

* <span data-ttu-id="90c50-705">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="90c50-705">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="90c50-706">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="90c50-706">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="90c50-707">VM</span><span class="sxs-lookup"><span data-stu-id="90c50-707">VM</span></span>

* <span data-ttu-id="90c50-708">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="90c50-708">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="90c50-709">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="90c50-709">October 9, 2017</span></span>

<span data-ttu-id="90c50-710">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="90c50-710">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="90c50-711">Núcleo</span><span class="sxs-lookup"><span data-stu-id="90c50-711">Core</span></span>

* <span data-ttu-id="90c50-712">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="90c50-712">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="90c50-713">AppService</span><span class="sxs-lookup"><span data-stu-id="90c50-713">Appservice</span></span>

* <span data-ttu-id="90c50-714">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="90c50-714">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="90c50-715">Lote</span><span class="sxs-lookup"><span data-stu-id="90c50-715">Batch</span></span>

* <span data-ttu-id="90c50-716">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="90c50-716">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="90c50-717">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="90c50-717">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="90c50-718">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="90c50-718">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="90c50-719">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="90c50-719">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="90c50-720">Batchai</span><span class="sxs-lookup"><span data-stu-id="90c50-720">Batchai</span></span>

* <span data-ttu-id="90c50-721">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="90c50-721">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="90c50-722">Keyvault</span><span class="sxs-lookup"><span data-stu-id="90c50-722">Keyvault</span></span>

* <span data-ttu-id="90c50-723">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="90c50-723">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="90c50-724">(#4448)</span><span class="sxs-lookup"><span data-stu-id="90c50-724">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="90c50-725">Rede</span><span class="sxs-lookup"><span data-stu-id="90c50-725">Network</span></span>

* <span data-ttu-id="90c50-726">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="90c50-726">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="90c50-727">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="90c50-727">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="90c50-728">Recurso</span><span class="sxs-lookup"><span data-stu-id="90c50-728">Resource</span></span>

* <span data-ttu-id="90c50-729">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="90c50-729">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="90c50-730">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="90c50-730">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="90c50-731">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="90c50-731">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="90c50-732">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="90c50-732">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="90c50-733">Sql</span><span class="sxs-lookup"><span data-stu-id="90c50-733">Sql</span></span>

* <span data-ttu-id="90c50-734">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="90c50-734">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="90c50-735">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="90c50-735">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="90c50-736">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="90c50-736">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="90c50-737">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="90c50-737">Storage</span></span>

* <span data-ttu-id="90c50-738">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="90c50-738">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="90c50-739">VM</span><span class="sxs-lookup"><span data-stu-id="90c50-739">Vm</span></span>

* <span data-ttu-id="90c50-740">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="90c50-740">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="90c50-741">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="90c50-741">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="90c50-742">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="90c50-742">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="90c50-743">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="90c50-743">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="90c50-744">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="90c50-744">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="90c50-745">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="90c50-745">September 22, 2017</span></span>

<span data-ttu-id="90c50-746">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="90c50-746">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="90c50-747">Recurso</span><span class="sxs-lookup"><span data-stu-id="90c50-747">Resource</span></span>

* <span data-ttu-id="90c50-748">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="90c50-748">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="90c50-749">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="90c50-749">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="90c50-750">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="90c50-750">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="90c50-751">[ALTERAÇÃO DA FALHA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="90c50-751">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="90c50-752">Rede</span><span class="sxs-lookup"><span data-stu-id="90c50-752">Network</span></span>

* <span data-ttu-id="90c50-753">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="90c50-753">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="90c50-754">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="90c50-754">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="90c50-755">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="90c50-755">Added `asg` application security group commands</span></span>
* <span data-ttu-id="90c50-756">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="90c50-756">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="90c50-757">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="90c50-757">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="90c50-758">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="90c50-758">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="90c50-759">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="90c50-759">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="90c50-760">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="90c50-760">Storage</span></span>

* <span data-ttu-id="90c50-761">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="90c50-761">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="90c50-762">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="90c50-762">Eventgrid</span></span>

* <span data-ttu-id="90c50-763">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="90c50-763">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="90c50-764">SQL</span><span class="sxs-lookup"><span data-stu-id="90c50-764">SQL</span></span>

* <span data-ttu-id="90c50-765">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="90c50-765">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="90c50-766">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="90c50-766">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="90c50-767">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="90c50-767">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="90c50-768">Keyvault</span><span class="sxs-lookup"><span data-stu-id="90c50-768">Keyvault</span></span>

* <span data-ttu-id="90c50-769">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="90c50-769">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="90c50-770">VM</span><span class="sxs-lookup"><span data-stu-id="90c50-770">VM</span></span>

* <span data-ttu-id="90c50-771">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="90c50-771">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="90c50-772">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="90c50-772">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="90c50-773">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="90c50-773">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="90c50-774">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="90c50-774">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="90c50-775">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="90c50-775">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="90c50-776">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="90c50-776">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="90c50-777">ACS</span><span class="sxs-lookup"><span data-stu-id="90c50-777">ACS</span></span>

* <span data-ttu-id="90c50-778">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="90c50-778">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="90c50-779">AppService</span><span class="sxs-lookup"><span data-stu-id="90c50-779">Appservice</span></span>

* <span data-ttu-id="90c50-780">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="90c50-780">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="90c50-781">Backup</span><span class="sxs-lookup"><span data-stu-id="90c50-781">Backup</span></span>

* <span data-ttu-id="90c50-782">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="90c50-782">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="90c50-783">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="90c50-783">September 11, 2017</span></span>

<span data-ttu-id="90c50-784">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="90c50-784">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="90c50-785">Núcleo</span><span class="sxs-lookup"><span data-stu-id="90c50-785">Core</span></span>

* <span data-ttu-id="90c50-786">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="90c50-786">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="90c50-787">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="90c50-787">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="90c50-788">Acs</span><span class="sxs-lookup"><span data-stu-id="90c50-788">Acs</span></span>

* <span data-ttu-id="90c50-789">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="90c50-789">Added `acs list-locations` command</span></span>
* <span data-ttu-id="90c50-790">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="90c50-790">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="90c50-791">AppService</span><span class="sxs-lookup"><span data-stu-id="90c50-791">Appservice</span></span>

* <span data-ttu-id="90c50-792">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="90c50-792">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="90c50-793">CDN</span><span class="sxs-lookup"><span data-stu-id="90c50-793">CDN</span></span>

* <span data-ttu-id="90c50-794">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="90c50-794">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="90c50-795">Extensão</span><span class="sxs-lookup"><span data-stu-id="90c50-795">Extension</span></span>

* <span data-ttu-id="90c50-796">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="90c50-796">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="90c50-797">Keyvault</span><span class="sxs-lookup"><span data-stu-id="90c50-797">Keyvault</span></span>

* <span data-ttu-id="90c50-798">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="90c50-798">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="90c50-799">Rede</span><span class="sxs-lookup"><span data-stu-id="90c50-799">Network</span></span>

* <span data-ttu-id="90c50-800">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="90c50-800">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="90c50-801">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="90c50-801">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="90c50-802">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="90c50-802">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="90c50-803">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="90c50-803">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="90c50-804">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="90c50-804">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="90c50-805">Recurso</span><span class="sxs-lookup"><span data-stu-id="90c50-805">Resource</span></span>

* <span data-ttu-id="90c50-806">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="90c50-806">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="90c50-807">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="90c50-807">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="90c50-808">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="90c50-808">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="90c50-809">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="90c50-809">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="90c50-810">SQL</span><span class="sxs-lookup"><span data-stu-id="90c50-810">SQL</span></span>

* <span data-ttu-id="90c50-811">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="90c50-811">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="90c50-812">VM</span><span class="sxs-lookup"><span data-stu-id="90c50-812">VM</span></span>

* <span data-ttu-id="90c50-813">Corrigido: Não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="90c50-813">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="90c50-814">Corrigido: Usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="90c50-814">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="90c50-815">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="90c50-815">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="90c50-816">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="90c50-816">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="90c50-817">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="90c50-817">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="90c50-818">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="90c50-818">August 31, 2017</span></span>

<span data-ttu-id="90c50-819">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="90c50-819">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="90c50-820">Keyvault</span><span class="sxs-lookup"><span data-stu-id="90c50-820">Keyvault</span></span>

* <span data-ttu-id="90c50-821">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="90c50-821">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="90c50-822">Sf</span><span class="sxs-lookup"><span data-stu-id="90c50-822">Sf</span></span>

* <span data-ttu-id="90c50-823">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="90c50-823">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="90c50-824">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="90c50-824">Storage</span></span>

* <span data-ttu-id="90c50-825">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="90c50-825">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="90c50-826">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="90c50-826">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="90c50-827">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="90c50-827">August 28, 2017</span></span>

<span data-ttu-id="90c50-828">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="90c50-828">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="90c50-829">CLI</span><span class="sxs-lookup"><span data-stu-id="90c50-829">CLI</span></span>

* <span data-ttu-id="90c50-830">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="90c50-830">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="90c50-831">ACS</span><span class="sxs-lookup"><span data-stu-id="90c50-831">ACS</span></span>

* <span data-ttu-id="90c50-832">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="90c50-832">Corrected preview regions</span></span>
* <span data-ttu-id="90c50-833">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="90c50-833">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="90c50-834">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="90c50-834">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="90c50-835">AppService</span><span class="sxs-lookup"><span data-stu-id="90c50-835">Appservice</span></span>

* <span data-ttu-id="90c50-836">[ALTERAÇÃO DA FALHA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="90c50-836">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="90c50-837">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="90c50-837">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="90c50-838">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="90c50-838">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="90c50-839">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="90c50-839">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="90c50-840">Correção: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="90c50-840">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="90c50-841">IoT</span><span class="sxs-lookup"><span data-stu-id="90c50-841">IoT</span></span>

* <span data-ttu-id="90c50-842">Correção #3934: Criação de política não limpa as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="90c50-842">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="90c50-843">Rede</span><span class="sxs-lookup"><span data-stu-id="90c50-843">Network</span></span>

* <span data-ttu-id="90c50-844">[ALTERAÇÃO DA FALHA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="90c50-844">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="90c50-845">[ALTERAÇÃO DA FALHA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="90c50-845">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="90c50-846">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="90c50-846">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="90c50-847">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="90c50-847">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="90c50-848">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="90c50-848">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="90c50-849">Perfil</span><span class="sxs-lookup"><span data-stu-id="90c50-849">Profile</span></span>

* <span data-ttu-id="90c50-850">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="90c50-850">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="90c50-851">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="90c50-851">Service Fabric</span></span>

* <span data-ttu-id="90c50-852">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="90c50-852">Preview release</span></span>
* <span data-ttu-id="90c50-853">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="90c50-853">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="90c50-854">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="90c50-854">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="90c50-855">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="90c50-855">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="90c50-856">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="90c50-856">Storage</span></span>

* <span data-ttu-id="90c50-857">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="90c50-857">Enabled setting blob tier</span></span>
* <span data-ttu-id="90c50-858">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="90c50-858">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="90c50-859">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="90c50-859">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="90c50-860">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="90c50-860">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="90c50-861">[ALTERAÇÃO DA FALHA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="90c50-861">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="90c50-862">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="90c50-862">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="90c50-863">VM</span><span class="sxs-lookup"><span data-stu-id="90c50-863">VM</span></span>

* <span data-ttu-id="90c50-864">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="90c50-864">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="90c50-865">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="90c50-865">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="90c50-866">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="90c50-866">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="90c50-867">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="90c50-867">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="90c50-868">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="90c50-868">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="90c50-869">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="90c50-869">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="90c50-870">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="90c50-870">August 15, 2017</span></span>

<span data-ttu-id="90c50-871">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="90c50-871">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="90c50-872">ACS</span><span class="sxs-lookup"><span data-stu-id="90c50-872">ACS</span></span>

* <span data-ttu-id="90c50-873">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="90c50-873">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="90c50-874">AppService</span><span class="sxs-lookup"><span data-stu-id="90c50-874">Appservice</span></span>

* <span data-ttu-id="90c50-875">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="90c50-875">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="90c50-876">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="90c50-876">Event Grid</span></span>

* <span data-ttu-id="90c50-877">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="90c50-877">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="90c50-878">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="90c50-878">August 11, 2017</span></span>

<span data-ttu-id="90c50-879">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="90c50-879">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="90c50-880">ACS</span><span class="sxs-lookup"><span data-stu-id="90c50-880">ACS</span></span>

* <span data-ttu-id="90c50-881">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="90c50-881">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="90c50-882">Lote</span><span class="sxs-lookup"><span data-stu-id="90c50-882">Batch</span></span>

* <span data-ttu-id="90c50-883">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="90c50-883">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="90c50-884">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="90c50-884">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="90c50-885">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="90c50-885">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="90c50-886">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="90c50-886">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="90c50-887">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="90c50-887">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="90c50-888">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="90c50-888">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="90c50-889">Componente</span><span class="sxs-lookup"><span data-stu-id="90c50-889">Component</span></span>

* <span data-ttu-id="90c50-890">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="90c50-890">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="90c50-891">Contêiner</span><span class="sxs-lookup"><span data-stu-id="90c50-891">Container</span></span>

* <span data-ttu-id="90c50-892">`create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="90c50-892">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="90c50-893">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="90c50-893">Data Lake Store</span></span>

* <span data-ttu-id="90c50-894">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="90c50-894">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="90c50-895">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="90c50-895">Event Grid</span></span>

* <span data-ttu-id="90c50-896">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="90c50-896">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="90c50-897">Rede</span><span class="sxs-lookup"><span data-stu-id="90c50-897">Network</span></span>

* <span data-ttu-id="90c50-898">`lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="90c50-898">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="90c50-899">`application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="90c50-899">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="90c50-900">`application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="90c50-900">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="90c50-901">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="90c50-901">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="90c50-902">Perfil</span><span class="sxs-lookup"><span data-stu-id="90c50-902">Profile</span></span>

* <span data-ttu-id="90c50-903">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="90c50-903">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="90c50-904">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="90c50-904">Storage</span></span>

* <span data-ttu-id="90c50-905">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="90c50-905">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="90c50-906">VM</span><span class="sxs-lookup"><span data-stu-id="90c50-906">VM</span></span>

* <span data-ttu-id="90c50-907">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="90c50-907">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="90c50-908">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="90c50-908">Exposed `list-skus` command</span></span>
* <span data-ttu-id="90c50-909">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="90c50-909">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="90c50-910">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="90c50-910">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="90c50-911">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="90c50-911">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="90c50-912">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="90c50-912">July 28, 2017</span></span>

<span data-ttu-id="90c50-913">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="90c50-913">Version 2.0.12</span></span>

* <span data-ttu-id="90c50-914">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="90c50-914">Added container commands</span></span>
* <span data-ttu-id="90c50-915">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="90c50-915">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="90c50-916">Núcleo</span><span class="sxs-lookup"><span data-stu-id="90c50-916">Core</span></span>

* <span data-ttu-id="90c50-917">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="90c50-917">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="90c50-918">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="90c50-918">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="90c50-919">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="90c50-919">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="90c50-920">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="90c50-920">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="90c50-921">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="90c50-921">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="90c50-922">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="90c50-922">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="90c50-923">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="90c50-923">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="90c50-924">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="90c50-924">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="90c50-925">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="90c50-925">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="90c50-926">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="90c50-926">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="90c50-927">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="90c50-927">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="90c50-928">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="90c50-928">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="90c50-929">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="90c50-929">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="90c50-930">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="90c50-930">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="90c50-931">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="90c50-931">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="90c50-932">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="90c50-932">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="90c50-933">ACR</span><span class="sxs-lookup"><span data-stu-id="90c50-933">ACR</span></span>

* <span data-ttu-id="90c50-934">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="90c50-934">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="90c50-935">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="90c50-935">Support SKU update for managed registries</span></span>
* <span data-ttu-id="90c50-936">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="90c50-936">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="90c50-937">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="90c50-937">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="90c50-938">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="90c50-938">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="90c50-939">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="90c50-939">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="90c50-940">ACS</span><span class="sxs-lookup"><span data-stu-id="90c50-940">ACS</span></span>

* <span data-ttu-id="90c50-941">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="90c50-941">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="90c50-942">AppService</span><span class="sxs-lookup"><span data-stu-id="90c50-942">Appservice</span></span>

* <span data-ttu-id="90c50-943">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="90c50-943">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="90c50-944">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="90c50-944">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="90c50-945">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="90c50-945">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="90c50-946">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="90c50-946">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="90c50-947">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="90c50-947">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="90c50-948">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="90c50-948">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="90c50-949">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="90c50-949">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="90c50-950">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="90c50-950">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="90c50-951">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="90c50-951">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="90c50-952">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="90c50-952">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="90c50-953">Lote</span><span class="sxs-lookup"><span data-stu-id="90c50-953">Batch</span></span>

* <span data-ttu-id="90c50-954">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="90c50-954">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="90c50-955">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="90c50-955">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="90c50-956">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="90c50-956">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="90c50-957">CDN</span><span class="sxs-lookup"><span data-stu-id="90c50-957">CDN</span></span>

* <span data-ttu-id="90c50-958">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="90c50-958">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="90c50-959">Nuvem</span><span class="sxs-lookup"><span data-stu-id="90c50-959">Cloud</span></span>

* <span data-ttu-id="90c50-960">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="90c50-960">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="90c50-961">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="90c50-961">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="90c50-962">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="90c50-962">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="90c50-963">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="90c50-963">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="90c50-964">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="90c50-964">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="90c50-965">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="90c50-965">CosmosDB</span></span>

* <span data-ttu-id="90c50-966">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="90c50-966">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="90c50-967">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="90c50-967">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="90c50-968">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="90c50-968">Data Lake Analytics</span></span>

* <span data-ttu-id="90c50-969">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="90c50-969">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="90c50-970">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="90c50-970">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="90c50-971">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="90c50-971">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="90c50-972">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="90c50-972">Data Lake Store</span></span>

* <span data-ttu-id="90c50-973">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="90c50-973">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="90c50-974">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="90c50-974">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="90c50-975">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="90c50-975">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="90c50-976">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="90c50-976">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="90c50-977">Interativo</span><span class="sxs-lookup"><span data-stu-id="90c50-977">Interactive</span></span>

* <span data-ttu-id="90c50-978">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="90c50-978">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="90c50-979">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="90c50-979">Increased test coverage</span></span>
* <span data-ttu-id="90c50-980">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="90c50-980">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="90c50-981">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="90c50-981">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="90c50-982">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="90c50-982">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="90c50-983">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="90c50-983">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="90c50-984">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="90c50-984">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="90c50-985">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="90c50-985">Added `--progress` flag</span></span>
* <span data-ttu-id="90c50-986">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="90c50-986">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="90c50-987">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="90c50-987">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="90c50-988">IoT</span><span class="sxs-lookup"><span data-stu-id="90c50-988">IoT</span></span>

* <span data-ttu-id="90c50-989">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="90c50-989">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="90c50-990">(#3934)</span><span class="sxs-lookup"><span data-stu-id="90c50-990">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="90c50-991">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="90c50-991">Key vault</span></span>

* <span data-ttu-id="90c50-992">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="90c50-992">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="90c50-993">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="90c50-993">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="90c50-994">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="90c50-994">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="90c50-995">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="90c50-995">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="90c50-996">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="90c50-996">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="90c50-997">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="90c50-997">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="90c50-998">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="90c50-998">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="90c50-999">(#3307)</span><span class="sxs-lookup"><span data-stu-id="90c50-999">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="90c50-1000">Laboratório</span><span class="sxs-lookup"><span data-stu-id="90c50-1000">Lab</span></span>

* <span data-ttu-id="90c50-1001">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="90c50-1001">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="90c50-1002">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="90c50-1002">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="90c50-1003">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="90c50-1003">Monitor</span></span>

* <span data-ttu-id="90c50-1004">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="90c50-1004">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="90c50-1005">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="90c50-1005">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="90c50-1006">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="90c50-1006">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="90c50-1007">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="90c50-1007">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="90c50-1008">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="90c50-1008">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="90c50-1009">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="90c50-1009">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="90c50-1010">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="90c50-1010">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="90c50-1011">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="90c50-1011">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="90c50-1012">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="90c50-1012">`location` no longer required</span></span>
  * <span data-ttu-id="90c50-1013">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="90c50-1013">Add name and ID support for target</span></span>
  * <span data-ttu-id="90c50-1014">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="90c50-1014">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="90c50-1015">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="90c50-1015">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="90c50-1016">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="90c50-1016">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="90c50-1017">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="90c50-1017">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="90c50-1018">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="90c50-1018">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="90c50-1019">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="90c50-1019">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="90c50-1020">Rede</span><span class="sxs-lookup"><span data-stu-id="90c50-1020">Network</span></span>

* <span data-ttu-id="90c50-1021">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="90c50-1021">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="90c50-1022">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="90c50-1022">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="90c50-1023">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="90c50-1023">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="90c50-1024">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="90c50-1024">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="90c50-1025">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="90c50-1025">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="90c50-1026">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="90c50-1026">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="90c50-1027">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="90c50-1027">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="90c50-1028">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="90c50-1028">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="90c50-1029">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="90c50-1029">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="90c50-1030">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="90c50-1030">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="90c50-1031">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="90c50-1031">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="90c50-1032">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="90c50-1032">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="90c50-1033">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="90c50-1033">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="90c50-1034">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="90c50-1034">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="90c50-1035">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="90c50-1035">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="90c50-1036">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="90c50-1036">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="90c50-1037">Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS</span><span class="sxs-lookup"><span data-stu-id="90c50-1037">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="90c50-1038">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="90c50-1038">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="90c50-1039">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="90c50-1039">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="90c50-1040">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="90c50-1040">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="90c50-1041">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="90c50-1041">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="90c50-1042">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="90c50-1042">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="90c50-1043">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="90c50-1043">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="90c50-1044">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="90c50-1044">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="90c50-1045">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="90c50-1045">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="90c50-1046">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="90c50-1046">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="90c50-1047">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="90c50-1047">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="90c50-1048">Perfil</span><span class="sxs-lookup"><span data-stu-id="90c50-1048">Profile</span></span>

* <span data-ttu-id="90c50-1049">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="90c50-1049">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="90c50-1050">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="90c50-1050">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="90c50-1051">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="90c50-1051">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="90c50-1052">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="90c50-1052">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="90c50-1053">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="90c50-1053">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="90c50-1054">RDBMS</span><span class="sxs-lookup"><span data-stu-id="90c50-1054">RDBMS</span></span>

* <span data-ttu-id="90c50-1055">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="90c50-1055">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="90c50-1056">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="90c50-1056">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="90c50-1057">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="90c50-1057">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="90c50-1058">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="90c50-1058">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="90c50-1059">Recurso</span><span class="sxs-lookup"><span data-stu-id="90c50-1059">Resource</span></span>

* <span data-ttu-id="90c50-1060">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="90c50-1060">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="90c50-1061">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="90c50-1061">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="90c50-1062">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="90c50-1062">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="90c50-1063">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="90c50-1063">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="90c50-1064">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="90c50-1064">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="90c50-1065">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="90c50-1065">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="90c50-1066">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="90c50-1066">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="90c50-1067">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="90c50-1067">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="90c50-1068">Função</span><span class="sxs-lookup"><span data-stu-id="90c50-1068">Role</span></span>

* <span data-ttu-id="90c50-1069">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="90c50-1069">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="90c50-1070">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="90c50-1070">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="90c50-1071">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="90c50-1071">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="90c50-1072">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="90c50-1072">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="90c50-1073">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="90c50-1073">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="90c50-1074">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="90c50-1074">Service Fabric</span></span>
* <span data-ttu-id="90c50-1075">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="90c50-1075">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="90c50-1076">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="90c50-1076">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="90c50-1077">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="90c50-1077">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="90c50-1078">SQL</span><span class="sxs-lookup"><span data-stu-id="90c50-1078">SQL</span></span>

* <span data-ttu-id="90c50-1079">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="90c50-1079">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="90c50-1080">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="90c50-1080">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="90c50-1081">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="90c50-1081">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="90c50-1082">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="90c50-1082">Storage</span></span>

* <span data-ttu-id="90c50-1083">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="90c50-1083">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="90c50-1084">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="90c50-1084">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="90c50-1085">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="90c50-1085">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="90c50-1086">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="90c50-1086">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="90c50-1087">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="90c50-1087">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="90c50-1088">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="90c50-1088">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="90c50-1089">VM</span><span class="sxs-lookup"><span data-stu-id="90c50-1089">VM</span></span>

* <span data-ttu-id="90c50-1090">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="90c50-1090">Support configuring nsg</span></span>
* <span data-ttu-id="90c50-1091">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="90c50-1091">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="90c50-1092">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="90c50-1092">Support managed service identities</span></span>
* <span data-ttu-id="90c50-1093">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="90c50-1093">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="90c50-1094">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="90c50-1094">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="90c50-1095">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="90c50-1095">May 10, 2017</span></span>

<span data-ttu-id="90c50-1096">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="90c50-1096">Version 2.0.6</span></span>

* <span data-ttu-id="90c50-1097">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="90c50-1097">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="90c50-1098">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="90c50-1098">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="90c50-1099">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="90c50-1099">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="90c50-1100">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="90c50-1100">Include Cognitive Services module</span></span>
* <span data-ttu-id="90c50-1101">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="90c50-1101">Include Service Fabric module</span></span>
* <span data-ttu-id="90c50-1102">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="90c50-1102">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="90c50-1103">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="90c50-1103">Add support for CDN commands</span></span>
* <span data-ttu-id="90c50-1104">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="90c50-1104">Remove Container module</span></span>
* <span data-ttu-id="90c50-1105">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="90c50-1105">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="90c50-1106">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="90c50-1106">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="90c50-1107">Núcleo</span><span class="sxs-lookup"><span data-stu-id="90c50-1107">Core</span></span>

* <span data-ttu-id="90c50-1108">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="90c50-1108">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="90c50-1109">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="90c50-1109">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="90c50-1110">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="90c50-1110">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="90c50-1111">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="90c50-1111">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="90c50-1112">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="90c50-1112">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="90c50-1113">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="90c50-1113">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="90c50-1114">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="90c50-1114">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="90c50-1115">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="90c50-1115">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="90c50-1116">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="90c50-1116">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="90c50-1117">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="90c50-1117">core: Improved performance</span></span>
* <span data-ttu-id="90c50-1118">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="90c50-1118">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="90c50-1119">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="90c50-1119">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="90c50-1120">ACS</span><span class="sxs-lookup"><span data-stu-id="90c50-1120">ACS</span></span>

* <span data-ttu-id="90c50-1121">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="90c50-1121">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="90c50-1122">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="90c50-1122">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="90c50-1123">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="90c50-1123">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="90c50-1124">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="90c50-1124">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="90c50-1125">AppService</span><span class="sxs-lookup"><span data-stu-id="90c50-1125">AppService</span></span>

* <span data-ttu-id="90c50-1126">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="90c50-1126">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="90c50-1127">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="90c50-1127">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="90c50-1128">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="90c50-1128">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="90c50-1129">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="90c50-1129">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="90c50-1130">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="90c50-1130">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="90c50-1131">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="90c50-1131">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="90c50-1132">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="90c50-1132">support slot swap with preview</span></span>
* <span data-ttu-id="90c50-1133">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="90c50-1133">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="90c50-1134">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="90c50-1134">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="90c50-1135">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="90c50-1135">CosmosDB</span></span>

* <span data-ttu-id="90c50-1136">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="90c50-1136">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="90c50-1137">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="90c50-1137">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="90c50-1138">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="90c50-1138">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="90c50-1139">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="90c50-1139">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="90c50-1140">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="90c50-1140">Data Lake Analytics</span></span>

* <span data-ttu-id="90c50-1141">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="90c50-1141">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="90c50-1142">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="90c50-1142">Add support for new catalog item type: package.</span></span> <span data-ttu-id="90c50-1143">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="90c50-1143">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="90c50-1144">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="90c50-1144">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="90c50-1145">Tabela</span><span class="sxs-lookup"><span data-stu-id="90c50-1145">Table</span></span>
  * <span data-ttu-id="90c50-1146">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="90c50-1146">Table valued function</span></span>
  * <span data-ttu-id="90c50-1147">Visualizar</span><span class="sxs-lookup"><span data-stu-id="90c50-1147">View</span></span>
  * <span data-ttu-id="90c50-1148">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="90c50-1148">Table Statistics.</span></span> <span data-ttu-id="90c50-1149">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="90c50-1149">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="90c50-1150">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="90c50-1150">Data Lake Store</span></span>

* <span data-ttu-id="90c50-1151">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="90c50-1151">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="90c50-1152">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="90c50-1152">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="90c50-1153">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="90c50-1153">missed help for access show.</span></span> <span data-ttu-id="90c50-1154">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="90c50-1154">adding it.</span></span> <span data-ttu-id="90c50-1155">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="90c50-1155">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="90c50-1156">Localizar</span><span class="sxs-lookup"><span data-stu-id="90c50-1156">Find</span></span>

* <span data-ttu-id="90c50-1157">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="90c50-1157">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="90c50-1158">KeyVault</span><span class="sxs-lookup"><span data-stu-id="90c50-1158">KeyVault</span></span>

* <span data-ttu-id="90c50-1159">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="90c50-1159">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="90c50-1160">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="90c50-1160">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="90c50-1161">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="90c50-1161">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="90c50-1162">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="90c50-1162">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="90c50-1163">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="90c50-1163">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="90c50-1164">Laboratório</span><span class="sxs-lookup"><span data-stu-id="90c50-1164">Lab</span></span>

* <span data-ttu-id="90c50-1165">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="90c50-1165">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="90c50-1166">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="90c50-1166">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="90c50-1167">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="90c50-1167">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="90c50-1168">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="90c50-1168">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="90c50-1169">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="90c50-1169">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="90c50-1170">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="90c50-1170">Monitor</span></span>

* <span data-ttu-id="90c50-1171">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="90c50-1171">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="90c50-1172">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="90c50-1172">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="90c50-1173">Rede</span><span class="sxs-lookup"><span data-stu-id="90c50-1173">Network</span></span>

* <span data-ttu-id="90c50-1174">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="90c50-1174">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="90c50-1175">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="90c50-1175">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="90c50-1176">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90c50-1176">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="90c50-1177">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90c50-1177">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="90c50-1178">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="90c50-1178">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="90c50-1179">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="90c50-1179">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="90c50-1180">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="90c50-1180">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="90c50-1181">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="90c50-1181">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="90c50-1182">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="90c50-1182">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="90c50-1183">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="90c50-1183">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="90c50-1184">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="90c50-1184">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="90c50-1185">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="90c50-1185">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="90c50-1186">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="90c50-1186">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="90c50-1187">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="90c50-1187">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="90c50-1188">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="90c50-1188">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="90c50-1189">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="90c50-1189">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="90c50-1190">Perfil</span><span class="sxs-lookup"><span data-stu-id="90c50-1190">Profile</span></span>

* <span data-ttu-id="90c50-1191">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="90c50-1191">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="90c50-1192">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="90c50-1192">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="90c50-1193">Redis</span><span class="sxs-lookup"><span data-stu-id="90c50-1193">Redis</span></span>

* <span data-ttu-id="90c50-1194">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="90c50-1194">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="90c50-1195">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="90c50-1195">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="90c50-1196">Recurso</span><span class="sxs-lookup"><span data-stu-id="90c50-1196">Resource</span></span>

* <span data-ttu-id="90c50-1197">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="90c50-1197">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="90c50-1198">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="90c50-1198">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="90c50-1199">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="90c50-1199">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="90c50-1200">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="90c50-1200">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="90c50-1201">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="90c50-1201">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="90c50-1202">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="90c50-1202">Add docs for az lock update.</span></span> <span data-ttu-id="90c50-1203">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="90c50-1203">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="90c50-1204">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="90c50-1204">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="90c50-1205">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="90c50-1205">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="90c50-1206">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="90c50-1206">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="90c50-1207">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="90c50-1207">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="90c50-1208">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="90c50-1208">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="90c50-1209">Função</span><span class="sxs-lookup"><span data-stu-id="90c50-1209">Role</span></span>

* <span data-ttu-id="90c50-1210">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="90c50-1210">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="90c50-1211">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="90c50-1211">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="90c50-1212">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="90c50-1212">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="90c50-1213">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="90c50-1213">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="90c50-1214">SQL</span><span class="sxs-lookup"><span data-stu-id="90c50-1214">SQL</span></span>

* <span data-ttu-id="90c50-1215">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="90c50-1215">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="90c50-1216">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="90c50-1216">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="90c50-1217">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="90c50-1217">Storage</span></span>

* <span data-ttu-id="90c50-1218">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="90c50-1218">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="90c50-1219">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="90c50-1219">Add support for incremental blob copy</span></span>
* <span data-ttu-id="90c50-1220">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="90c50-1220">Add support for large block blob upload</span></span>
* <span data-ttu-id="90c50-1221">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="90c50-1221">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="90c50-1222">VM</span><span class="sxs-lookup"><span data-stu-id="90c50-1222">VM</span></span>

* <span data-ttu-id="90c50-1223">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="90c50-1223">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="90c50-1224">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="90c50-1224">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="90c50-1225">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="90c50-1225">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="90c50-1226">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="90c50-1226">az vm/vmss disk</span></span>
  3. <span data-ttu-id="90c50-1227">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="90c50-1227">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="90c50-1228">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="90c50-1228">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="90c50-1229">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="90c50-1229">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="90c50-1230">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="90c50-1230">April 3, 2017</span></span>

<span data-ttu-id="90c50-1231">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="90c50-1231">Version 2.0.2</span></span>

<span data-ttu-id="90c50-1232">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="90c50-1232">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="90c50-1233">Núcleo</span><span class="sxs-lookup"><span data-stu-id="90c50-1233">Core</span></span>

* <span data-ttu-id="90c50-1234">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="90c50-1234">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="90c50-1235">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="90c50-1235">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="90c50-1236">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="90c50-1236">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="90c50-1237">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="90c50-1237">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="90c50-1238">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="90c50-1238">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="90c50-1239">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="90c50-1239">Add prompting for missing template parameters.</span></span> <span data-ttu-id="90c50-1240">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="90c50-1240">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="90c50-1241">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="90c50-1241">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="90c50-1242">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="90c50-1242">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="90c50-1243">ACS</span><span class="sxs-lookup"><span data-stu-id="90c50-1243">ACS</span></span>

* <span data-ttu-id="90c50-1244">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="90c50-1244">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="90c50-1245">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="90c50-1245">Add support for ssh key password prompting.</span></span> <span data-ttu-id="90c50-1246">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="90c50-1246">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="90c50-1247">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="90c50-1247">Add support for windows clusters.</span></span> <span data-ttu-id="90c50-1248">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="90c50-1248">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="90c50-1249">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="90c50-1249">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="90c50-1250">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="90c50-1250">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="90c50-1251">AppService</span><span class="sxs-lookup"><span data-stu-id="90c50-1251">AppService</span></span>

* <span data-ttu-id="90c50-1252">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="90c50-1252">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="90c50-1253">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="90c50-1253">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="90c50-1254">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="90c50-1254">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="90c50-1255">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="90c50-1255">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="90c50-1256">DataLake</span><span class="sxs-lookup"><span data-stu-id="90c50-1256">DataLake</span></span>

* <span data-ttu-id="90c50-1257">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="90c50-1257">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="90c50-1258">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="90c50-1258">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="90c50-1259">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="90c50-1259">DocuemntDB</span></span>

* <span data-ttu-id="90c50-1260">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="90c50-1260">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="90c50-1261">VM</span><span class="sxs-lookup"><span data-stu-id="90c50-1261">VM</span></span>

* <span data-ttu-id="90c50-1262">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="90c50-1262">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="90c50-1263">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="90c50-1263">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="90c50-1264">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="90c50-1264">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="90c50-1265">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="90c50-1265">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="90c50-1266">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="90c50-1266">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="90c50-1267">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="90c50-1267">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="90c50-1268">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="90c50-1268">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="90c50-1269">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="90c50-1269">February 27, 2017</span></span>

<span data-ttu-id="90c50-1270">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="90c50-1270">Version 2.0.0</span></span>

<span data-ttu-id="90c50-1271">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="90c50-1271">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="90c50-1272">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="90c50-1272">Container Service (acs)</span></span>
- <span data-ttu-id="90c50-1273">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="90c50-1273">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="90c50-1274">Rede</span><span class="sxs-lookup"><span data-stu-id="90c50-1274">Networking</span></span>
- <span data-ttu-id="90c50-1275">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="90c50-1275">Storage</span></span>

<span data-ttu-id="90c50-1276">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="90c50-1276">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="90c50-1277">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="90c50-1277">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="90c50-1278">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="90c50-1278">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="90c50-1279">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="90c50-1279">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="90c50-1280">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="90c50-1280">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="90c50-1281">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="90c50-1281">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="90c50-1282">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="90c50-1282">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="90c50-1283">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="90c50-1283">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="90c50-1284">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="90c50-1284">Provide feedback from the command line with the `az feedback` command</span></span>

