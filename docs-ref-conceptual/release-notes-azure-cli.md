---
title: "Notas de versão da CLI do Azure 2.0"
description: "Saiba mais sobre as últimas atualizações da CLI do Azure 2.0"
keywords: "Notas da versão, CLI do Azure 2.0"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/03/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ce0428f7-0a59-4e72-9237-d907b171af51
ms.openlocfilehash: 3bd4b9c059da3b841fc0757a11bc7ce78ec64b08
ms.sourcegitcommit: 66d997a5afcf32143a4d4817ec1608cbdf58a59f
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="ab154-104">Notas de versão da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="ab154-104">Azure CLI 2.0 release notes</span></span>

## <a name="may-10-2017"></a><span data-ttu-id="ab154-105">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="ab154-105">May 10, 2017</span></span>

<span data-ttu-id="ab154-106">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="ab154-106">Version 2.0.6</span></span>

* <span data-ttu-id="ab154-107">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ab154-107">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="ab154-108">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="ab154-108">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="ab154-109">Inclusão dos módulos Data Lake Analytics e Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="ab154-109">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="ab154-110">Inclusão do módulo Serviços Cognitivos.</span><span class="sxs-lookup"><span data-stu-id="ab154-110">Include Cognitive Services module.</span></span>
* <span data-ttu-id="ab154-111">Inclusão do módulo Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="ab154-111">Include Service Fabric module.</span></span>
* <span data-ttu-id="ab154-112">Inclusão do módulo Interativo (renomeação de az-shell).</span><span class="sxs-lookup"><span data-stu-id="ab154-112">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="ab154-113">Adição de suporte para comandos CDN.</span><span class="sxs-lookup"><span data-stu-id="ab154-113">Add support for CDN commands.</span></span>
* <span data-ttu-id="ab154-114">Remoção do módulo Contêiner.</span><span class="sxs-lookup"><span data-stu-id="ab154-114">Remove Container module.</span></span>
* <span data-ttu-id="ab154-115">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="ab154-115">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="ab154-116">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="ab154-116">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="ab154-117">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ab154-117">Core</span></span>

* <span data-ttu-id="ab154-118">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="ab154-118">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="ab154-119">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="ab154-119">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="ab154-120">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="ab154-120">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="ab154-121">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="ab154-121">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="ab154-122">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="ab154-122">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="ab154-123">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="ab154-123">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="ab154-124">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="ab154-124">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="ab154-125">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="ab154-125">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="ab154-126">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="ab154-126">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="ab154-127">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="ab154-127">core: Improved performance</span></span>
* <span data-ttu-id="ab154-128">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="ab154-128">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="ab154-129">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="ab154-129">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="ab154-130">ACS</span><span class="sxs-lookup"><span data-stu-id="ab154-130">ACS</span></span>

* <span data-ttu-id="ab154-131">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab154-131">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="ab154-132">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="ab154-132">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="ab154-133">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="ab154-133">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="ab154-134">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="ab154-134">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="ab154-135">AppService</span><span class="sxs-lookup"><span data-stu-id="ab154-135">AppService</span></span>

* <span data-ttu-id="ab154-136">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="ab154-136">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="ab154-137">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="ab154-137">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="ab154-138">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="ab154-138">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="ab154-139">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="ab154-139">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="ab154-140">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="ab154-140">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="ab154-141">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="ab154-141">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="ab154-142">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="ab154-142">support slot swap with preview</span></span>
* <span data-ttu-id="ab154-143">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="ab154-143">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="ab154-144">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="ab154-144">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ab154-145">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ab154-145">CosmosDB</span></span>

* <span data-ttu-id="ab154-146">Renomeação do módulo DocumentDB para CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="ab154-146">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="ab154-147">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="ab154-147">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="ab154-148">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="ab154-148">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="ab154-149">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="ab154-149">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ab154-150">Análises Data Lake</span><span class="sxs-lookup"><span data-stu-id="ab154-150">Data Lake Analytics</span></span>

* <span data-ttu-id="ab154-151">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro.</span><span class="sxs-lookup"><span data-stu-id="ab154-151">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="ab154-152">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="ab154-152">Add support for new catalog item type: package.</span></span> <span data-ttu-id="ab154-153">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="ab154-153">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="ab154-154">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="ab154-154">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="ab154-155">Tabela</span><span class="sxs-lookup"><span data-stu-id="ab154-155">Table</span></span>
  * <span data-ttu-id="ab154-156">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="ab154-156">Table valued function</span></span>
  * <span data-ttu-id="ab154-157">Visualizar</span><span class="sxs-lookup"><span data-stu-id="ab154-157">View</span></span>
  * <span data-ttu-id="ab154-158">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="ab154-158">Table Statistics.</span></span> <span data-ttu-id="ab154-159">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela.</span><span class="sxs-lookup"><span data-stu-id="ab154-159">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ab154-160">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="ab154-160">Data Lake Store</span></span>

* <span data-ttu-id="ab154-161">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor.</span><span class="sxs-lookup"><span data-stu-id="ab154-161">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="ab154-162">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="ab154-162">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="ab154-163">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="ab154-163">missed help for access show.</span></span> <span data-ttu-id="ab154-164">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="ab154-164">adding it.</span></span> <span data-ttu-id="ab154-165">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="ab154-165">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="ab154-166">Localizar</span><span class="sxs-lookup"><span data-stu-id="ab154-166">Find</span></span>

* <span data-ttu-id="ab154-167">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="ab154-167">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="ab154-168">KeyVault</span><span class="sxs-lookup"><span data-stu-id="ab154-168">KeyVault</span></span>

* <span data-ttu-id="ab154-169">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="ab154-169">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="ab154-170">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço.</span><span class="sxs-lookup"><span data-stu-id="ab154-170">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="ab154-171">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="ab154-171">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="ab154-172">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”.</span><span class="sxs-lookup"><span data-stu-id="ab154-172">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="ab154-173">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="ab154-173">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="ab154-174">Laboratório</span><span class="sxs-lookup"><span data-stu-id="ab154-174">Lab</span></span>

* <span data-ttu-id="ab154-175">Adição dos comandos create, show, delete e list ao ambiente do laboratório.</span><span class="sxs-lookup"><span data-stu-id="ab154-175">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="ab154-176">Adição dos comandos show e list para exibir modelos ARM no laboratório.</span><span class="sxs-lookup"><span data-stu-id="ab154-176">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="ab154-177">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório.</span><span class="sxs-lookup"><span data-stu-id="ab154-177">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="ab154-178">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório.</span><span class="sxs-lookup"><span data-stu-id="ab154-178">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="ab154-179">Adição de comandos para gerenciar segredos em um Laboratório.</span><span class="sxs-lookup"><span data-stu-id="ab154-179">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="ab154-180">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="ab154-180">Monitor</span></span>

* <span data-ttu-id="ab154-181">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="ab154-181">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="ab154-182">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="ab154-182">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="ab154-183">Rede</span><span class="sxs-lookup"><span data-stu-id="ab154-183">Network</span></span>

* <span data-ttu-id="ab154-184">Adição do comando `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="ab154-184">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="ab154-185">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="ab154-185">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="ab154-186">Adição de suporte para drenagem de conexão do Gateway de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ab154-186">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="ab154-187">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ab154-187">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="ab154-188">Adição de suporte para filtros de rota e regras do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="ab154-188">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="ab154-189">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="ab154-189">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="ab154-190">Adição de suporte para seletores de tráfego baseados em política da conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="ab154-190">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="ab154-191">Adição de suporte para políticas IPsec da conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="ab154-191">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="ab154-192">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`.</span><span class="sxs-lookup"><span data-stu-id="ab154-192">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="ab154-193">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="ab154-193">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="ab154-194">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="ab154-194">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="ab154-195">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="ab154-195">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="ab154-196">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente.</span><span class="sxs-lookup"><span data-stu-id="ab154-196">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="ab154-197">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente.</span><span class="sxs-lookup"><span data-stu-id="ab154-197">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="ab154-198">Correção de um bug em que `traffic-manager endpoint update` não funciona.</span><span class="sxs-lookup"><span data-stu-id="ab154-198">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="ab154-199">Adição de comandos de visualização “network watcher”.</span><span class="sxs-lookup"><span data-stu-id="ab154-199">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="ab154-200">Perfil</span><span class="sxs-lookup"><span data-stu-id="ab154-200">Profile</span></span>

* <span data-ttu-id="ab154-201">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="ab154-201">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="ab154-202">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="ab154-202">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="ab154-203">Redis</span><span class="sxs-lookup"><span data-stu-id="ab154-203">Redis</span></span>

* <span data-ttu-id="ab154-204">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="ab154-204">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="ab154-205">Preterição do comando “update-settings”.</span><span class="sxs-lookup"><span data-stu-id="ab154-205">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="ab154-206">Recurso</span><span class="sxs-lookup"><span data-stu-id="ab154-206">Resource</span></span>

* <span data-ttu-id="ab154-207">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="ab154-207">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="ab154-208">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="ab154-208">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="ab154-209">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="ab154-209">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="ab154-210">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="ab154-210">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="ab154-211">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="ab154-211">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="ab154-212">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="ab154-212">Add docs for az lock update.</span></span> <span data-ttu-id="ab154-213">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="ab154-213">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="ab154-214">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="ab154-214">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="ab154-215">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="ab154-215">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="ab154-216">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="ab154-216">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="ab154-217">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="ab154-217">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="ab154-218">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="ab154-218">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="ab154-219">Função</span><span class="sxs-lookup"><span data-stu-id="ab154-219">Role</span></span>

* <span data-ttu-id="ab154-220">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="ab154-220">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="ab154-221">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="ab154-221">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="ab154-222">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="ab154-222">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="ab154-223">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="ab154-223">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="ab154-224">SQL</span><span class="sxs-lookup"><span data-stu-id="ab154-224">SQL</span></span>

* <span data-ttu-id="ab154-225">Adição dos comandos az sql server list-usages e az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="ab154-225">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="ab154-226">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="ab154-226">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="ab154-227">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="ab154-227">Storage</span></span>

* <span data-ttu-id="ab154-228">Localização padrão da localização do grupo de recursos de `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="ab154-228">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="ab154-229">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="ab154-229">Add support for incremental blob copy</span></span>
* <span data-ttu-id="ab154-230">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="ab154-230">Add support for large block blob upload</span></span>
* <span data-ttu-id="ab154-231">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="ab154-231">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="ab154-232">VM</span><span class="sxs-lookup"><span data-stu-id="ab154-232">VM</span></span>

* <span data-ttu-id="ab154-233">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="ab154-233">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="ab154-234">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="ab154-234">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="ab154-235">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="ab154-235">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="ab154-236">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="ab154-236">az vm/vmss disk</span></span>
  3. <span data-ttu-id="ab154-237">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="ab154-237">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="ab154-238">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="ab154-238">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="ab154-239">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="ab154-239">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="ab154-240">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="ab154-240">April 3, 2017</span></span>

<span data-ttu-id="ab154-241">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="ab154-241">Version 2.0.2</span></span>

<span data-ttu-id="ab154-242">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão.</span><span class="sxs-lookup"><span data-stu-id="ab154-242">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="ab154-243">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ab154-243">Core</span></span>

* <span data-ttu-id="ab154-244">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão.</span><span class="sxs-lookup"><span data-stu-id="ab154-244">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="ab154-245">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="ab154-245">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="ab154-246">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="ab154-246">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="ab154-247">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="ab154-247">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="ab154-248">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="ab154-248">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="ab154-249">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="ab154-249">Add prompting for missing template parameters.</span></span> <span data-ttu-id="ab154-250">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="ab154-250">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="ab154-251">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="ab154-251">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="ab154-252">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="ab154-252">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="ab154-253">ACS</span><span class="sxs-lookup"><span data-stu-id="ab154-253">ACS</span></span>

* [<span data-ttu-id="ab154-254">ACS] Adicionar suporte para configurar um cluster do ACS padrão ([&#2554;</span><span class="sxs-lookup"><span data-stu-id="ab154-254">ACS] Adding support for configuring a default ACS cluster ([#2554</span></span>](https://github.com/Azure/azure-cli/pull/2554))
* <span data-ttu-id="ab154-255">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="ab154-255">Add support for ssh key password prompting.</span></span> <span data-ttu-id="ab154-256">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="ab154-256">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="ab154-257">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="ab154-257">Add support for windows clusters.</span></span> <span data-ttu-id="ab154-258">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="ab154-258">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="ab154-259">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="ab154-259">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="ab154-260">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="ab154-260">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="ab154-261">AppService</span><span class="sxs-lookup"><span data-stu-id="ab154-261">AppService</span></span>

* <span data-ttu-id="ab154-262">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="ab154-262">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="ab154-263">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="ab154-263">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="ab154-264">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="ab154-264">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="ab154-265">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="ab154-265">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="ab154-266">DataLake</span><span class="sxs-lookup"><span data-stu-id="ab154-266">DataLake</span></span>

* <span data-ttu-id="ab154-267">Versão inicial do módulo do Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="ab154-267">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="ab154-268">Versão inicial do módulo do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="ab154-268">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="ab154-269">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="ab154-269">DocuemntDB</span></span>

* <span data-ttu-id="ab154-270">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="ab154-270">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="ab154-271">VM</span><span class="sxs-lookup"><span data-stu-id="ab154-271">VM</span></span>

* [<span data-ttu-id="ab154-272">Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570</span><span class="sxs-lookup"><span data-stu-id="ab154-272">Compute] Add AppGateway support to virtual machine scale set create ([#2570</span></span>](https://github.com/Azure/azure-cli/pull/2570))
* [<span data-ttu-id="ab154-273">VM/VMSS] Suporte aprimorado ao cache de disco ([#2522</span><span class="sxs-lookup"><span data-stu-id="ab154-273">VM/VMSS] Improved disk caching support ([#2522</span></span>](https://github.com/Azure/azure-cli/pull/2522))
* <span data-ttu-id="ab154-274">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="ab154-274">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="ab154-275">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="ab154-275">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="ab154-276">Conjunto de dimensionamento de máquinas virtuais: suporte à * para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="ab154-276">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="ab154-277">Adicionar --secrets para o conjunto de dimensionamento de máquinas virtuais e VM ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="ab154-277">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="ab154-278">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="ab154-278">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="ab154-279">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="ab154-279">February 27, 2017</span></span>

<span data-ttu-id="ab154-280">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="ab154-280">Version 2.0.0</span></span>

<span data-ttu-id="ab154-281">Essa versão da CLI do Azure 2.0 é a primeira versão “Disponível”.</span><span class="sxs-lookup"><span data-stu-id="ab154-281">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="ab154-282">A disponibilidade se aplica a esses módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="ab154-282">General availability applies to these command modules:</span></span>
- <span data-ttu-id="ab154-283">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="ab154-283">Container Service (acs)</span></span>
- <span data-ttu-id="ab154-284">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="ab154-284">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="ab154-285">Rede</span><span class="sxs-lookup"><span data-stu-id="ab154-285">Networking</span></span>
- <span data-ttu-id="ab154-286">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="ab154-286">Storage</span></span>

<span data-ttu-id="ab154-287">Esses módulos de comando podem ser usados na produção e são compatíveis com o SLA do Microsoft padrão.</span><span class="sxs-lookup"><span data-stu-id="ab154-287">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="ab154-288">Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="ab154-288">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="ab154-289">Você pode fazer perguntas sobre [StackOverflow usando a marcação azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) ou entrar em contato com a equipe do produto pelo endereço [ azfeedback@microsoft.com ](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="ab154-289">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
<span data-ttu-id="ab154-290">Você pode fornecer comentários a partir da linha de comando com o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="ab154-290">You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="ab154-291">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="ab154-291">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="ab154-292">Para verificar a versão da CLI, utilize `az --version`.</span><span class="sxs-lookup"><span data-stu-id="ab154-292">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="ab154-293">A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando.</span><span class="sxs-lookup"><span data-stu-id="ab154-293">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="ab154-294">Alguns dos módulos de comando têm um “b*n*” ou “rc*n*” pós-fixado.</span><span class="sxs-lookup"><span data-stu-id="ab154-294">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="ab154-295">Esses módulos de comando ainda estão em visualização e estarão disponíveis no futuro.</span><span class="sxs-lookup"><span data-stu-id="ab154-295">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="ab154-296">Também temos compilações de visualização diárias da CLI.</span><span class="sxs-lookup"><span data-stu-id="ab154-296">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="ab154-297">Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="ab154-297">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="ab154-298">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="ab154-298">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="ab154-299">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="ab154-299">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="ab154-300">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="ab154-300">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="ab154-301">Forneça comentários a partir da linha de comando com o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="ab154-301">Provide feedback from the command line with the `az feedback` command.</span></span>

