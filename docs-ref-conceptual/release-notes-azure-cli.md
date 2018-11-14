---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/06/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 51b8b8cad6d25f916006b8e68b8f300587f5d45b
ms.sourcegitcommit: 0d6b08048b5b35bf0bb3d7b91ff567adbaab2a8b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/07/2018
ms.locfileid: "51222558"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="daa0d-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="daa0d-103">Azure CLI release notes</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="daa0d-104">6 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-104">November 6, 2018</span></span>

<span data-ttu-id="daa0d-105">Versão 2.0.50</span><span class="sxs-lookup"><span data-stu-id="daa0d-105">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="daa0d-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-106">Core</span></span>
* <span data-ttu-id="daa0d-107">Foi adicionado suporte para o serviço principal sn + autenticação do emissor</span><span class="sxs-lookup"><span data-stu-id="daa0d-107">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="daa0d-108">ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-108">ACR</span></span>
* <span data-ttu-id="daa0d-109">Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa</span><span class="sxs-lookup"><span data-stu-id="daa0d-109">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="daa0d-110">Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação</span><span class="sxs-lookup"><span data-stu-id="daa0d-110">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-111">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-111">ACS</span></span>
* <span data-ttu-id="daa0d-112">[ALTERAÇÃO SIGNIFICATIVA] `enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão</span><span class="sxs-lookup"><span data-stu-id="daa0d-112">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="daa0d-113">Supervisor</span><span class="sxs-lookup"><span data-stu-id="daa0d-113">Advisor</span></span>
* <span data-ttu-id="daa0d-114">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="daa0d-114">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="daa0d-115">AMS</span><span class="sxs-lookup"><span data-stu-id="daa0d-115">AMS</span></span>
* <span data-ttu-id="daa0d-116">Novos grupos de comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="daa0d-116">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="daa0d-117">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="daa0d-117">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="daa0d-118">Adicionados parâmetros de criptografia com suporte para `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-118">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="daa0d-119">O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido</span><span class="sxs-lookup"><span data-stu-id="daa0d-119">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="daa0d-120">Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="daa0d-120">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="daa0d-121">Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="daa0d-121">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="daa0d-122">Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="daa0d-122">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="daa0d-123">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming locator` foi substituído por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="daa0d-123">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="daa0d-124">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--content-keys` de `ams streaming locator` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="daa0d-124">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="daa0d-125">[ALTERAÇÃO SIGNIFICATIVA] `--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="daa0d-125">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="daa0d-126">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming policy` foi substituído por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="daa0d-126">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="daa0d-127">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-127">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="daa0d-128">Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="daa0d-128">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="daa0d-129">Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado</span><span class="sxs-lookup"><span data-stu-id="daa0d-129">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="daa0d-130">[ALTERAÇÃO SIGNIFICATIVA] `--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-130">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="daa0d-131">Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'.</span><span class="sxs-lookup"><span data-stu-id="daa0d-131">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="daa0d-132">Um ativo sem rótulo pode ser enviado assim: 'assetName='</span><span class="sxs-lookup"><span data-stu-id="daa0d-132">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-133">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-133">AppService</span></span>
* <span data-ttu-id="daa0d-134">Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido</span><span class="sxs-lookup"><span data-stu-id="daa0d-134">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="daa0d-135">Configurar</span><span class="sxs-lookup"><span data-stu-id="daa0d-135">Configure</span></span>
* <span data-ttu-id="daa0d-136">O YAML foi adicionado às opções de formato de saída</span><span class="sxs-lookup"><span data-stu-id="daa0d-136">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="daa0d-137">Contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-137">Container</span></span>
* <span data-ttu-id="daa0d-138">Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml</span><span class="sxs-lookup"><span data-stu-id="daa0d-138">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="daa0d-139">EventHub</span><span class="sxs-lookup"><span data-stu-id="daa0d-139">EventHub</span></span>
* <span data-ttu-id="daa0d-140">O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-140">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="daa0d-141">Interativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-141">Interactive</span></span>
* <span data-ttu-id="daa0d-142">O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos</span><span class="sxs-lookup"><span data-stu-id="daa0d-142">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="daa0d-143">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="daa0d-143">Monitor</span></span>
* <span data-ttu-id="daa0d-144">Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) para `--condition` em `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-144">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-145">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-145">Network</span></span>
* <span data-ttu-id="daa0d-146">Os nomes de comandos `network interface-endpoint` foram preteridos em benefício de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="daa0d-146">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="daa0d-147">Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID</span><span class="sxs-lookup"><span data-stu-id="daa0d-147">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="daa0d-148">Foi corrigido um problema onde `--ip-tags` não funcionava corretamente com `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-148">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="daa0d-149">Perfil</span><span class="sxs-lookup"><span data-stu-id="daa0d-149">Profile</span></span>
* <span data-ttu-id="daa0d-150">`--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado</span><span class="sxs-lookup"><span data-stu-id="daa0d-150">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="daa0d-151">RDBMS</span><span class="sxs-lookup"><span data-stu-id="daa0d-151">RDBMS</span></span>
* <span data-ttu-id="daa0d-152">Adicionados comandos da réplica mysql</span><span class="sxs-lookup"><span data-stu-id="daa0d-152">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="daa0d-153">Recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-153">Resource</span></span>
* <span data-ttu-id="daa0d-154">Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="daa0d-154">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="daa0d-155">Função</span><span class="sxs-lookup"><span data-stu-id="daa0d-155">Role</span></span>
* <span data-ttu-id="daa0d-156">Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais</span><span class="sxs-lookup"><span data-stu-id="daa0d-156">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="daa0d-157">`ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="daa0d-157">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="daa0d-158">Suporte adicionado para conceder permissões a aplicativos do AAD</span><span class="sxs-lookup"><span data-stu-id="daa0d-158">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-159">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-159">Storage</span></span>
* <span data-ttu-id="daa0d-160">Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="daa0d-160">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-161">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-161">VM</span></span>
* <span data-ttu-id="daa0d-162">O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem</span><span class="sxs-lookup"><span data-stu-id="daa0d-162">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="daa0d-163">O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido</span><span class="sxs-lookup"><span data-stu-id="daa0d-163">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="daa0d-164">O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado</span><span class="sxs-lookup"><span data-stu-id="daa0d-164">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="daa0d-165">`vm secret format` foi alterado para exigir a saída json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="daa0d-165">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="daa0d-166">Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido</span><span class="sxs-lookup"><span data-stu-id="daa0d-166">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="daa0d-167">Validação de argumento aprimorado para `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="daa0d-167">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="daa0d-168">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-168">October 23, 2018</span></span>

<span data-ttu-id="daa0d-169">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="daa0d-169">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="daa0d-170">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-170">Core</span></span>
* <span data-ttu-id="daa0d-171">Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`</span><span class="sxs-lookup"><span data-stu-id="daa0d-171">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="daa0d-172">Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="daa0d-172">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="daa0d-173">ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-173">ACR</span></span>
* <span data-ttu-id="daa0d-174">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="daa0d-174">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="daa0d-175">CDN</span><span class="sxs-lookup"><span data-stu-id="daa0d-175">CDN</span></span>
* <span data-ttu-id="daa0d-176">[ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="daa0d-176">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="daa0d-177">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="daa0d-177">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="daa0d-178">Contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-178">Container</span></span>
* <span data-ttu-id="daa0d-179">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="daa0d-179">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="daa0d-180">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="daa0d-180">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="daa0d-181">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="daa0d-181">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="daa0d-182">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="daa0d-182">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="daa0d-183">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="daa0d-183">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="daa0d-184">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="daa0d-184">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="daa0d-185">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="daa0d-185">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="daa0d-186">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="daa0d-186">CosmosDB</span></span>
* <span data-ttu-id="daa0d-187">Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-187">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="daa0d-188">Interativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-188">Interactive</span></span>
* <span data-ttu-id="daa0d-189">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="daa0d-189">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="daa0d-190">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="daa0d-190">IoT Central</span></span>
* <span data-ttu-id="daa0d-191">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="daa0d-191">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="daa0d-192">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="daa0d-192">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="daa0d-193">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="daa0d-193">Monitor</span></span>
* <span data-ttu-id="daa0d-194">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="daa0d-194">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="daa0d-195">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="daa0d-195">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="daa0d-196">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="daa0d-196">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="daa0d-197">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="daa0d-197">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="daa0d-198">Adicionado `--namespace` como alias para a opção preterida `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="daa0d-198">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="daa0d-199">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="daa0d-199">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="daa0d-200">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="daa0d-200">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="daa0d-201">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="daa0d-201">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="daa0d-202">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="daa0d-202">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="daa0d-203">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-203">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-204">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-204">Network</span></span>
* <span data-ttu-id="daa0d-205">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="daa0d-205">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="daa0d-206">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="daa0d-206">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="daa0d-207">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="daa0d-207">ServiceBus</span></span>
* <span data-ttu-id="daa0d-208">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="daa0d-208">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="daa0d-209">SQL</span><span class="sxs-lookup"><span data-stu-id="daa0d-209">SQL</span></span>
* <span data-ttu-id="daa0d-210">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="daa0d-210">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-211">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-211">Storage</span></span>
* <span data-ttu-id="daa0d-212">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="daa0d-212">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="daa0d-213">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="daa0d-213">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-214">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-214">VM</span></span>
* <span data-ttu-id="daa0d-215">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-215">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="daa0d-216">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-216">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="daa0d-217">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-217">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="daa0d-218">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-218">October 16, 2018</span></span>

<span data-ttu-id="daa0d-219">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="daa0d-219">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-220">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-220">VM</span></span>
* <span data-ttu-id="daa0d-221">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="daa0d-221">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="daa0d-222">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-222">October 9, 2018</span></span>

<span data-ttu-id="daa0d-223">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="daa0d-223">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="daa0d-224">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-224">Core</span></span>
* <span data-ttu-id="daa0d-225">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="daa0d-225">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="daa0d-226">ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-226">ACR</span></span>
* <span data-ttu-id="daa0d-227">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="daa0d-227">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-228">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-228">ACS</span></span>
* <span data-ttu-id="daa0d-229">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="daa0d-229">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="daa0d-230">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="daa0d-230">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="daa0d-231">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="daa0d-231">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="daa0d-232">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="daa0d-232">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="daa0d-233">Contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-233">Container</span></span>
* <span data-ttu-id="daa0d-234">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um tempo de execução específico</span><span class="sxs-lookup"><span data-stu-id="daa0d-234">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="daa0d-235">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="daa0d-235">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="daa0d-236">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="daa0d-236">Event Hub</span></span>
* <span data-ttu-id="daa0d-237">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-237">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="daa0d-238">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="daa0d-238">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="daa0d-239">Extensões</span><span class="sxs-lookup"><span data-stu-id="daa0d-239">Extensions</span></span>
* <span data-ttu-id="daa0d-240">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="daa0d-240">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="daa0d-241">HDInsight</span><span class="sxs-lookup"><span data-stu-id="daa0d-241">HDInsight</span></span>
* <span data-ttu-id="daa0d-242">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="daa0d-242">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="daa0d-243">IoT</span><span class="sxs-lookup"><span data-stu-id="daa0d-243">IoT</span></span>
* <span data-ttu-id="daa0d-244">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="daa0d-244">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="daa0d-245">KeyVault</span><span class="sxs-lookup"><span data-stu-id="daa0d-245">KeyVault</span></span>
* <span data-ttu-id="daa0d-246">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="daa0d-246">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-247">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-247">Network</span></span>
* <span data-ttu-id="daa0d-248">`network dns zone create` corrigido: o comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="daa0d-248">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="daa0d-249">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="daa0d-249">See #6052</span></span>
* <span data-ttu-id="daa0d-250">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-250">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="daa0d-251">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="daa0d-251">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="daa0d-252">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="daa0d-252">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="daa0d-253">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="daa0d-253">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="daa0d-254">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="daa0d-254">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="daa0d-255">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-255">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="daa0d-256">Função</span><span class="sxs-lookup"><span data-stu-id="daa0d-256">Role</span></span>
* <span data-ttu-id="daa0d-257">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="daa0d-257">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="daa0d-258">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="daa0d-258">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="daa0d-259">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="daa0d-259">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="daa0d-260">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="daa0d-260">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="daa0d-261">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="daa0d-261">Service Bus</span></span>
* <span data-ttu-id="daa0d-262">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="daa0d-262">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-263">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-263">VM</span></span>
* <span data-ttu-id="daa0d-264">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="daa0d-264">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="daa0d-265">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-265">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="daa0d-266">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="daa0d-266">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="daa0d-267">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="daa0d-267">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="daa0d-268">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="daa0d-268">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="daa0d-269">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="daa0d-269">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="daa0d-270">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-270">September 21, 2018</span></span>

<span data-ttu-id="daa0d-271">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="daa0d-271">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="daa0d-272">ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-272">ACR</span></span>
* <span data-ttu-id="daa0d-273">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-273">Added ACR Task commands</span></span>
* <span data-ttu-id="daa0d-274">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="daa0d-274">Added quick run command</span></span>
* <span data-ttu-id="daa0d-275">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="daa0d-275">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="daa0d-276">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-276">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="daa0d-277">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="daa0d-277">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="daa0d-278">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="daa0d-278">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-279">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-279">ACS</span></span>
* <span data-ttu-id="daa0d-280">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="daa0d-280">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="daa0d-281">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="daa0d-281">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-282">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-282">AppService</span></span>

* <span data-ttu-id="daa0d-283">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="daa0d-283">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="daa0d-284">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="daa0d-284">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="daa0d-285">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="daa0d-285">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="daa0d-286">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="daa0d-286">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="daa0d-287">Lote</span><span class="sxs-lookup"><span data-stu-id="daa0d-287">Batch</span></span>
* <span data-ttu-id="daa0d-288">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="daa0d-288">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="daa0d-289">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="daa0d-289">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="daa0d-290">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-290">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="daa0d-291">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="daa0d-291">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="daa0d-292">Lote AI</span><span class="sxs-lookup"><span data-stu-id="daa0d-292">Batch AI</span></span> 
* <span data-ttu-id="daa0d-293">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-293">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="daa0d-294">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="daa0d-294">Cognitive Services</span></span>
* <span data-ttu-id="daa0d-295">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="daa0d-295">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="daa0d-296">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="daa0d-296">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="daa0d-297">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="daa0d-297">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="daa0d-298">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="daa0d-298">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="daa0d-299">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="daa0d-299">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="daa0d-300">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="daa0d-300">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="daa0d-301">Contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-301">Container</span></span>
* <span data-ttu-id="daa0d-302">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="daa0d-302">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="daa0d-303">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-303">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="daa0d-304">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="daa0d-304">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="daa0d-305">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="daa0d-305">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="daa0d-306">DataLake</span><span class="sxs-lookup"><span data-stu-id="daa0d-306">Datalake</span></span>
* <span data-ttu-id="daa0d-307">Comandos adicionados para regras de rede virtual</span><span class="sxs-lookup"><span data-stu-id="daa0d-307">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="daa0d-308">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-308">Interactive Shell</span></span>
* <span data-ttu-id="daa0d-309">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="daa0d-309">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="daa0d-310">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="daa0d-310">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="daa0d-311">IoT</span><span class="sxs-lookup"><span data-stu-id="daa0d-311">IoT</span></span>
* <span data-ttu-id="daa0d-312">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="daa0d-312">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="daa0d-313">Key Vault</span><span class="sxs-lookup"><span data-stu-id="daa0d-313">Key Vault</span></span>
* <span data-ttu-id="daa0d-314">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="daa0d-314">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-315">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-315">Network</span></span>
* <span data-ttu-id="daa0d-316">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="daa0d-316">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="daa0d-317">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="daa0d-317">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="daa0d-318">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="daa0d-318">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="daa0d-319">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="daa0d-319">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="daa0d-320">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-320">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="daa0d-321">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-321">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="daa0d-322">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="daa0d-322">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="daa0d-323">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="daa0d-323">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="daa0d-324">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="daa0d-324">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="daa0d-325">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="daa0d-325">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="daa0d-326">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="daa0d-326">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="daa0d-327">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="daa0d-327">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="daa0d-328">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="daa0d-328">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="daa0d-329">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="daa0d-329">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="daa0d-330">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="daa0d-330">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="daa0d-331">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="daa0d-331">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="daa0d-332">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-332">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="daa0d-333">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="daa0d-333">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="daa0d-334">RDBMS</span><span class="sxs-lookup"><span data-stu-id="daa0d-334">RDBMS</span></span>
* <span data-ttu-id="daa0d-335">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="daa0d-335">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="daa0d-336">Reserva</span><span class="sxs-lookup"><span data-stu-id="daa0d-336">Reservation</span></span>
* <span data-ttu-id="daa0d-337">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="daa0d-337">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="daa0d-338">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="daa0d-338">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="daa0d-339">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-339">Manage App</span></span>
* <span data-ttu-id="daa0d-340">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="daa0d-340">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="daa0d-341">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="daa0d-341">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="daa0d-342">Função</span><span class="sxs-lookup"><span data-stu-id="daa0d-342">Role</span></span>
* <span data-ttu-id="daa0d-343">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="daa0d-343">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="daa0d-344">SignalR</span><span class="sxs-lookup"><span data-stu-id="daa0d-344">SignalR</span></span>
* <span data-ttu-id="daa0d-345">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="daa0d-345">First release</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-346">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-346">Storage</span></span>
* <span data-ttu-id="daa0d-347">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="daa0d-347">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="daa0d-348">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="daa0d-348">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-349">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-349">VM</span></span>
* <span data-ttu-id="daa0d-350">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="daa0d-350">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="daa0d-351">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="daa0d-351">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="daa0d-352">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-352">August 28, 2018</span></span>

<span data-ttu-id="daa0d-353">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="daa0d-353">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="daa0d-354">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-354">Core</span></span>

* <span data-ttu-id="daa0d-355">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="daa0d-355">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="daa0d-356">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="daa0d-356">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="daa0d-357">ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-357">ACR</span></span>

* <span data-ttu-id="daa0d-358">Adicionada uma solução alternativa para operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="daa0d-358">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="daa0d-359">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="daa0d-359">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-360">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-360">ACS</span></span>

* <span data-ttu-id="daa0d-361">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="daa0d-361">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="daa0d-362">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="daa0d-362">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-363">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-363">AppService</span></span>

* <span data-ttu-id="daa0d-364">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="daa0d-364">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="daa0d-365">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="daa0d-365">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="daa0d-366">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="daa0d-366">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="daa0d-367">Backup</span><span class="sxs-lookup"><span data-stu-id="daa0d-367">Backup</span></span>

* <span data-ttu-id="daa0d-368">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="daa0d-368">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="daa0d-369">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="daa0d-369">Bot Service</span></span>

* <span data-ttu-id="daa0d-370">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="daa0d-370">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="daa0d-371">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="daa0d-371">Cognitive Services</span></span>

* <span data-ttu-id="daa0d-372">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="daa0d-372">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="daa0d-373">IoT</span><span class="sxs-lookup"><span data-stu-id="daa0d-373">IoT</span></span>

* <span data-ttu-id="daa0d-374">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="daa0d-374">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="daa0d-375">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="daa0d-375">Monitor</span></span>

* <span data-ttu-id="daa0d-376">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="daa0d-376">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="daa0d-377">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="daa0d-377">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-378">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-378">Network</span></span>

* <span data-ttu-id="daa0d-379">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="daa0d-379">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="daa0d-380">Recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-380">Resource</span></span>

* <span data-ttu-id="daa0d-381">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="daa0d-381">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-382">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-382">Storage</span></span>

* <span data-ttu-id="daa0d-383">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="daa0d-383">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-384">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-384">VM</span></span>

* <span data-ttu-id="daa0d-385">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="daa0d-385">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="daa0d-386">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-386">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="daa0d-387">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-387">Auguest 14, 2018</span></span>

<span data-ttu-id="daa0d-388">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="daa0d-388">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="daa0d-389">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-389">Core</span></span>

* <span data-ttu-id="daa0d-390">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="daa0d-390">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="daa0d-391">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="daa0d-391">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="daa0d-392">Telemetria</span><span class="sxs-lookup"><span data-stu-id="daa0d-392">Telemetry</span></span>

* <span data-ttu-id="daa0d-393">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="daa0d-393">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="daa0d-394">ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-394">ACR</span></span>

* <span data-ttu-id="daa0d-395">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="daa0d-395">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="daa0d-396">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="daa0d-396">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-397">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-397">ACS</span></span>

* <span data-ttu-id="daa0d-398">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="daa0d-398">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="daa0d-399">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="daa0d-399">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="daa0d-400">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="daa0d-400">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="daa0d-401">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="daa0d-401">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="daa0d-402">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="daa0d-402">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="daa0d-403">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-403">AppService</span></span>

* <span data-ttu-id="daa0d-404">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="daa0d-404">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="daa0d-405">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="daa0d-405">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="daa0d-406">BatchAI</span><span class="sxs-lookup"><span data-stu-id="daa0d-406">BatchAI</span></span>

* <span data-ttu-id="daa0d-407">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="daa0d-407">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="daa0d-408">Contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-408">Container</span></span>

* <span data-ttu-id="daa0d-409">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-409">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="daa0d-410">IoT</span><span class="sxs-lookup"><span data-stu-id="daa0d-410">IoT</span></span>

* <span data-ttu-id="daa0d-411">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="daa0d-411">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="daa0d-412">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="daa0d-412">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="daa0d-413">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="daa0d-413">Iot Central</span></span>

* <span data-ttu-id="daa0d-414">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="daa0d-414">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="daa0d-415">KeyVault</span><span class="sxs-lookup"><span data-stu-id="daa0d-415">KeyVault</span></span>


* <span data-ttu-id="daa0d-416">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="daa0d-416">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="daa0d-417">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-417">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="daa0d-418">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="daa0d-418">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="daa0d-419">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="daa0d-419">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="daa0d-420">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="daa0d-420">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="daa0d-421">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="daa0d-421">Relay</span></span>

* <span data-ttu-id="daa0d-422">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="daa0d-422">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="daa0d-423">Sql</span><span class="sxs-lookup"><span data-stu-id="daa0d-423">Sql</span></span>

* <span data-ttu-id="daa0d-424">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="daa0d-424">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-425">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-425">Storage</span></span>

* <span data-ttu-id="daa0d-426">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="daa0d-426">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="daa0d-427">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="daa0d-427">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="daa0d-428">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="daa0d-428">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="daa0d-429">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="daa0d-429">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="daa0d-430">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-430">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-431">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-431">VM</span></span>

* <span data-ttu-id="daa0d-432">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="daa0d-432">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="daa0d-433">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-433">July 31, 2018</span></span>

<span data-ttu-id="daa0d-434">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="daa0d-434">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="daa0d-435">ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-435">ACR</span></span>

* <span data-ttu-id="daa0d-436">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="daa0d-436">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="daa0d-437">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="daa0d-437">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-438">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-438">ACS</span></span>

* <span data-ttu-id="daa0d-439">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="daa0d-439">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="daa0d-440">Lote</span><span class="sxs-lookup"><span data-stu-id="daa0d-440">Batch</span></span>

* <span data-ttu-id="daa0d-441">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="daa0d-441">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="daa0d-442">Contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-442">Container</span></span>

* <span data-ttu-id="daa0d-443">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="daa0d-443">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-444">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-444">Network</span></span>

* <span data-ttu-id="daa0d-445">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="daa0d-445">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="daa0d-446">Recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-446">Resource</span></span>

* <span data-ttu-id="daa0d-447">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="daa0d-447">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="daa0d-448">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="daa0d-448">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="daa0d-449">Função</span><span class="sxs-lookup"><span data-stu-id="daa0d-449">Role</span></span>

* <span data-ttu-id="daa0d-450">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="daa0d-450">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="daa0d-451">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="daa0d-451">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="daa0d-452">Search</span><span class="sxs-lookup"><span data-stu-id="daa0d-452">Search</span></span>

* <span data-ttu-id="daa0d-453">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="daa0d-453">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="daa0d-454">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="daa0d-454">Service Bus</span></span>

* <span data-ttu-id="daa0d-455">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="daa0d-455">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="daa0d-456">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="daa0d-456">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="daa0d-457">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="daa0d-457">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="daa0d-458">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="daa0d-458">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-459">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-459">Storage</span></span>

* <span data-ttu-id="daa0d-460">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="daa0d-460">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="daa0d-461">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="daa0d-461">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-462">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-462">VM</span></span>

* <span data-ttu-id="daa0d-463">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="daa0d-463">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="daa0d-464">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="daa0d-464">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="daa0d-465">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-465">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="daa0d-466">[ALTERAÇÃO SIGNIFICATIVA] `[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="daa0d-466">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="daa0d-467">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-467">July 18, 2018</span></span>

<span data-ttu-id="daa0d-468">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="daa0d-468">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="daa0d-469">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-469">Core</span></span>

* <span data-ttu-id="daa0d-470">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="daa0d-470">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="daa0d-471">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="daa0d-471">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="daa0d-472">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="daa0d-472">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="daa0d-473">ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-473">ACR</span></span>

* <span data-ttu-id="daa0d-474">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="daa0d-474">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="daa0d-475">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="daa0d-475">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="daa0d-476">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="daa0d-476">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="daa0d-477">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="daa0d-477">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-478">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-478">ACS</span></span>

* <span data-ttu-id="daa0d-479">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="daa0d-479">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-480">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-480">AppService</span></span>

* <span data-ttu-id="daa0d-481">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="daa0d-481">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="daa0d-482">Lote</span><span class="sxs-lookup"><span data-stu-id="daa0d-482">Batch</span></span>

* <span data-ttu-id="daa0d-483">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="daa0d-483">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="daa0d-484">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="daa0d-484">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="daa0d-485">Lote AI</span><span class="sxs-lookup"><span data-stu-id="daa0d-485">Batch AI</span></span>

* <span data-ttu-id="daa0d-486">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="daa0d-486">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="daa0d-487">Contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-487">Container</span></span>

* <span data-ttu-id="daa0d-488">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="daa0d-488">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="daa0d-489">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="daa0d-489">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-490">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-490">Network</span></span>

* <span data-ttu-id="daa0d-491">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-491">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="daa0d-492">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="daa0d-492">Added `network nic wait`</span></span>
* <span data-ttu-id="daa0d-493">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="daa0d-493">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="daa0d-494">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="daa0d-494">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="daa0d-495">Recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-495">Resource</span></span>

* <span data-ttu-id="daa0d-496">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="daa0d-496">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="daa0d-497">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="daa0d-497">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="daa0d-498">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="daa0d-498">Added `deployment wait` command</span></span>
* <span data-ttu-id="daa0d-499">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="daa0d-499">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="daa0d-500">SQL</span><span class="sxs-lookup"><span data-stu-id="daa0d-500">SQL</span></span>

* <span data-ttu-id="daa0d-501">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-501">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="daa0d-502">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="daa0d-502">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="daa0d-503">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="daa0d-503">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-504">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-504">Storage</span></span>

* <span data-ttu-id="daa0d-505">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="daa0d-505">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-506">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-506">VM</span></span>

* <span data-ttu-id="daa0d-507">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="daa0d-507">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="daa0d-508">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-508">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="daa0d-509">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="daa0d-509">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="daa0d-510">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-510">July 3, 2018</span></span>

<span data-ttu-id="daa0d-511">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="daa0d-511">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="daa0d-512">AKS</span><span class="sxs-lookup"><span data-stu-id="daa0d-512">AKS</span></span>

* <span data-ttu-id="daa0d-513">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="daa0d-513">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="daa0d-514">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-514">July 3, 2018</span></span>

<span data-ttu-id="daa0d-515">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="daa0d-515">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="daa0d-516">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-516">Core</span></span>

* <span data-ttu-id="daa0d-517">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-517">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="daa0d-518">ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-518">ACR</span></span>

* <span data-ttu-id="daa0d-519">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="daa0d-519">Added polling build status</span></span>
* <span data-ttu-id="daa0d-520">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="daa0d-520">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="daa0d-521">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="daa0d-521">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-522">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-522">ACS</span></span>

* <span data-ttu-id="daa0d-523">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="daa0d-523">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="daa0d-524">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="daa0d-524">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="daa0d-525">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-525">Updated options for `aks browse` command.</span></span> <span data-ttu-id="daa0d-526">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="daa0d-526">Added `--listen-port` support</span></span>
* <span data-ttu-id="daa0d-527">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-527">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="daa0d-528">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="daa0d-528">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="daa0d-529">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="daa0d-529">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-530">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-530">AppService</span></span>

* <span data-ttu-id="daa0d-531">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="daa0d-531">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="daa0d-532">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="daa0d-532">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="daa0d-533">Backup</span><span class="sxs-lookup"><span data-stu-id="daa0d-533">Backup</span></span>

* <span data-ttu-id="daa0d-534">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="daa0d-534">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="daa0d-535">BatchAI</span><span class="sxs-lookup"><span data-stu-id="daa0d-535">BatchAI</span></span>

* <span data-ttu-id="daa0d-536">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="daa0d-536">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="daa0d-537">Nuvem</span><span class="sxs-lookup"><span data-stu-id="daa0d-537">Cloud</span></span>

* <span data-ttu-id="daa0d-538">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="daa0d-538">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="daa0d-539">Contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-539">Container</span></span>

* <span data-ttu-id="daa0d-540">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="daa0d-540">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="daa0d-541">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="daa0d-541">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="daa0d-542">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="daa0d-542">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="daa0d-543">Extensão</span><span class="sxs-lookup"><span data-stu-id="daa0d-543">Extension</span></span>

* <span data-ttu-id="daa0d-544">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="daa0d-544">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-545">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-545">Network</span></span>

* <span data-ttu-id="daa0d-546">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="daa0d-546">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="daa0d-547">Rdbms</span><span class="sxs-lookup"><span data-stu-id="daa0d-547">Rdbms</span></span>

* <span data-ttu-id="daa0d-548">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="daa0d-548">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="daa0d-549">Recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-549">Resource</span></span>

* <span data-ttu-id="daa0d-550">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="daa0d-550">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-551">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-551">VM</span></span>

* <span data-ttu-id="daa0d-552">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="daa0d-552">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="daa0d-553">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-553">June 25, 2018</span></span>

<span data-ttu-id="daa0d-554">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="daa0d-554">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="daa0d-555">CLI</span><span class="sxs-lookup"><span data-stu-id="daa0d-555">CLI</span></span>

* <span data-ttu-id="daa0d-556">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="daa0d-556">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="daa0d-557">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-557">June 19, 2018</span></span>

<span data-ttu-id="daa0d-558">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="daa0d-558">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="daa0d-559">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-559">Core</span></span>

* <span data-ttu-id="daa0d-560">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="daa0d-560">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="daa0d-561">ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-561">ACR</span></span>

* <span data-ttu-id="daa0d-562">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="daa0d-562">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="daa0d-563">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="daa0d-563">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-564">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-564">ACS</span></span>

* <span data-ttu-id="daa0d-565">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="daa0d-565">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="daa0d-566">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="daa0d-566">Added `--update` support</span></span>
* <span data-ttu-id="daa0d-567">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="daa0d-567">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="daa0d-568">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="daa0d-568">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="daa0d-569">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="daa0d-569">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="daa0d-570">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="daa0d-570">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="daa0d-571">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="daa0d-571">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="daa0d-572">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="daa0d-572">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-573">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-573">AppService</span></span>

* <span data-ttu-id="daa0d-574">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="daa0d-574">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="daa0d-575">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="daa0d-575">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="daa0d-576">Lote</span><span class="sxs-lookup"><span data-stu-id="daa0d-576">Batch</span></span>

* <span data-ttu-id="daa0d-577">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="daa0d-577">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="daa0d-578">Lote AI</span><span class="sxs-lookup"><span data-stu-id="daa0d-578">Batch AI</span></span>

* <span data-ttu-id="daa0d-579">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="daa0d-579">Added support for workspaces.</span></span> <span data-ttu-id="daa0d-580">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="daa0d-580">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="daa0d-581">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="daa0d-581">Added support for experiments.</span></span> <span data-ttu-id="daa0d-582">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="daa0d-582">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="daa0d-583">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="daa0d-583">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="daa0d-584">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-584">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="daa0d-585">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="daa0d-585">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="daa0d-586">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="daa0d-586">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="daa0d-587">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="daa0d-587">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="daa0d-588">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="daa0d-588">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="daa0d-589">[ALTERAÇÃO SIGNIFICATIVA] `--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-589">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="daa0d-590">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="daa0d-590">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="daa0d-591">[ALTERAÇÃO SIGNIFICATIVA] `--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-591">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="daa0d-592">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="daa0d-592">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="daa0d-593">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="daa0d-593">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="daa0d-594">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="daa0d-594">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="daa0d-595">[ALTERAÇÃO SIGNIFICATIVA] `--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-595">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="daa0d-596">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="daa0d-596">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="daa0d-597">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="daa0d-597">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="daa0d-598">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="daa0d-598">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="daa0d-599">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="daa0d-599">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="daa0d-600">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="daa0d-600">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="daa0d-601">Mapas</span><span class="sxs-lookup"><span data-stu-id="daa0d-601">Maps</span></span>

* <span data-ttu-id="daa0d-602">[ALTERAÇÃO SIGNIFICATIVA] `maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="daa0d-602">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-603">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-603">Network</span></span>

* <span data-ttu-id="daa0d-604">Foi adicionado suporte a `https` para `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="daa0d-604">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="daa0d-605">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="daa0d-605">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="daa0d-606">#6502</span><span class="sxs-lookup"><span data-stu-id="daa0d-606">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="daa0d-607">Reservas</span><span class="sxs-lookup"><span data-stu-id="daa0d-607">Reservations</span></span>

* <span data-ttu-id="daa0d-608">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="daa0d-608">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="daa0d-609">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="daa0d-609">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="daa0d-610">[ALTERAÇÃO SIGNIFICATIVA] `kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="daa0d-610">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="daa0d-611">[ALTERAÇÃO SIGNIFICATIVA] `capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="daa0d-611">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="daa0d-612">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="daa0d-612">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="daa0d-613">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-613">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="daa0d-614">Função</span><span class="sxs-lookup"><span data-stu-id="daa0d-614">Role</span></span>

* <span data-ttu-id="daa0d-615">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="daa0d-615">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="daa0d-616">SQL</span><span class="sxs-lookup"><span data-stu-id="daa0d-616">SQL</span></span>

* <span data-ttu-id="daa0d-617">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="daa0d-617">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-618">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-618">Storage</span></span>

* <span data-ttu-id="daa0d-619">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="daa0d-619">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-620">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-620">VM</span></span>

* <span data-ttu-id="daa0d-621">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-621">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="daa0d-622">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="daa0d-622">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="daa0d-623">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="daa0d-623">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="daa0d-624">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-624">June 13, 2018</span></span>

<span data-ttu-id="daa0d-625">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="daa0d-625">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="daa0d-626">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-626">Core</span></span>

* <span data-ttu-id="daa0d-627">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="daa0d-627">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="daa0d-628">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-628">June 13, 2018</span></span>

<span data-ttu-id="daa0d-629">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="daa0d-629">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="daa0d-630">AKS</span><span class="sxs-lookup"><span data-stu-id="daa0d-630">AKS</span></span>

* <span data-ttu-id="daa0d-631">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-631">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="daa0d-632">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="daa0d-632">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="daa0d-633">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-633">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="daa0d-634">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-634">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="daa0d-635">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-635">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-636">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-636">AppService</span></span>

* <span data-ttu-id="daa0d-637">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="daa0d-637">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="daa0d-638">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-638">June 5, 2018</span></span>

<span data-ttu-id="daa0d-639">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="daa0d-639">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="daa0d-640">Interativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-640">Interactive</span></span>

* <span data-ttu-id="daa0d-641">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-641">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="daa0d-642">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-642">June 5, 2018</span></span>

<span data-ttu-id="daa0d-643">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="daa0d-643">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="daa0d-644">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-644">Core</span></span>

* <span data-ttu-id="daa0d-645">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="daa0d-645">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="daa0d-646">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="daa0d-646">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="daa0d-647">ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-647">ACR</span></span>

* <span data-ttu-id="daa0d-648">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="daa0d-648">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="daa0d-649">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="daa0d-649">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="daa0d-650">AKS</span><span class="sxs-lookup"><span data-stu-id="daa0d-650">AKS</span></span>

* <span data-ttu-id="daa0d-651">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="daa0d-651">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="daa0d-652">Lote</span><span class="sxs-lookup"><span data-stu-id="daa0d-652">Batch</span></span>

* <span data-ttu-id="daa0d-653">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="daa0d-653">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="daa0d-654">IOT</span><span class="sxs-lookup"><span data-stu-id="daa0d-654">IOT</span></span>

* <span data-ttu-id="daa0d-655">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="daa0d-655">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-656">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-656">Network</span></span>

* <span data-ttu-id="daa0d-657">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="daa0d-657">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="daa0d-658">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="daa0d-658">Policy Insights</span></span>

* <span data-ttu-id="daa0d-659">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="daa0d-659">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="daa0d-660">ARM</span><span class="sxs-lookup"><span data-stu-id="daa0d-660">ARM</span></span>

* <span data-ttu-id="daa0d-661">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="daa0d-661">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="daa0d-662">SQL</span><span class="sxs-lookup"><span data-stu-id="daa0d-662">SQL</span></span>

* <span data-ttu-id="daa0d-663">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="daa0d-663">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="daa0d-664">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="daa0d-664">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="daa0d-665">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-665">Storage</span></span>

* <span data-ttu-id="daa0d-666">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="daa0d-666">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-667">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-667">VM</span></span>

* <span data-ttu-id="daa0d-668">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="daa0d-668">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="daa0d-669">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-669">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="daa0d-670">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-670">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="daa0d-671">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-671">May 22, 2018</span></span>

<span data-ttu-id="daa0d-672">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="daa0d-672">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="daa0d-673">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-673">Core</span></span>

* <span data-ttu-id="daa0d-674">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="daa0d-674">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-675">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-675">ACS</span></span>

* <span data-ttu-id="daa0d-676">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="daa0d-676">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="daa0d-677">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="daa0d-677">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-678">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-678">AppService</span></span>

* <span data-ttu-id="daa0d-679">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="daa0d-679">Improved generic update commands</span></span>
* <span data-ttu-id="daa0d-680">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="daa0d-680">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="daa0d-681">Contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-681">Container</span></span>

* <span data-ttu-id="daa0d-682">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="daa0d-682">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="daa0d-683">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-683">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="daa0d-684">Extensão</span><span class="sxs-lookup"><span data-stu-id="daa0d-684">Extension</span></span>

* <span data-ttu-id="daa0d-685">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="daa0d-685">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="daa0d-686">Interativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-686">Interactive</span></span>

* <span data-ttu-id="daa0d-687">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="daa0d-687">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="daa0d-688">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="daa0d-688">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="daa0d-689">KeyVault</span><span class="sxs-lookup"><span data-stu-id="daa0d-689">KeyVault</span></span>

* <span data-ttu-id="daa0d-690">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="daa0d-690">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-691">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-691">Network</span></span>

* <span data-ttu-id="daa0d-692">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="daa0d-692">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="daa0d-693">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="daa0d-693">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="daa0d-694">SQL</span><span class="sxs-lookup"><span data-stu-id="daa0d-694">SQL</span></span>

* <span data-ttu-id="daa0d-695">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="daa0d-695">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="daa0d-696">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="daa0d-696">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="daa0d-697">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="daa0d-697">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="daa0d-698">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="daa0d-698">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="daa0d-699">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="daa0d-699">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="daa0d-700">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-700">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="daa0d-701">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="daa0d-701">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="daa0d-702">`edition`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-702">`edition`.</span></span> <span data-ttu-id="daa0d-703">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="daa0d-703">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="daa0d-704">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-704">`elasticPoolName`.</span></span> <span data-ttu-id="daa0d-705">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="daa0d-705">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="daa0d-706">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="daa0d-706">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="daa0d-707">`edition`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-707">`edition`.</span></span> <span data-ttu-id="daa0d-708">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="daa0d-708">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="daa0d-709">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-709">`dtu`.</span></span> <span data-ttu-id="daa0d-710">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="daa0d-710">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="daa0d-711">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-711">`databaseDtuMin`.</span></span> <span data-ttu-id="daa0d-712">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="daa0d-712">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="daa0d-713">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-713">`databaseDtuMax`.</span></span> <span data-ttu-id="daa0d-714">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="daa0d-714">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="daa0d-715">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-715">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="daa0d-716">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-716">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-717">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-717">Storage</span></span>

* <span data-ttu-id="daa0d-718">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="daa0d-718">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="daa0d-719">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="daa0d-719">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-720">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-720">VM</span></span>

* <span data-ttu-id="daa0d-721">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-721">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="daa0d-722">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="daa0d-722">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="daa0d-723">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="daa0d-723">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="daa0d-724">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="daa0d-724">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="daa0d-725">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-725">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="daa0d-726">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-726">May 7, 2018</span></span>

<span data-ttu-id="daa0d-727">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="daa0d-727">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="daa0d-728">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-728">Core</span></span>

* <span data-ttu-id="daa0d-729">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="daa0d-729">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="daa0d-730">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="daa0d-730">Added limited support for positional arguments</span></span>
* <span data-ttu-id="daa0d-731">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-731">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="daa0d-732">#5591</span><span class="sxs-lookup"><span data-stu-id="daa0d-732">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="daa0d-733">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-733">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="daa0d-734">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="daa0d-734">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="daa0d-735">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="daa0d-735">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="daa0d-736">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="daa0d-736">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="daa0d-737">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="daa0d-737">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="daa0d-738">ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-738">ACR</span></span>

* <span data-ttu-id="daa0d-739">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-739">Added ACR Build commands</span></span>
* <span data-ttu-id="daa0d-740">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="daa0d-740">Improved resource not found error messages</span></span>
* <span data-ttu-id="daa0d-741">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="daa0d-741">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="daa0d-742">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="daa0d-742">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="daa0d-743">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="daa0d-743">Improved repository commands error messages</span></span>
* <span data-ttu-id="daa0d-744">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="daa0d-744">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-745">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-745">ACS</span></span>

* <span data-ttu-id="daa0d-746">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="daa0d-746">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="daa0d-747">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="daa0d-747">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="daa0d-748">AMS</span><span class="sxs-lookup"><span data-stu-id="daa0d-748">AMS</span></span>

* <span data-ttu-id="daa0d-749">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="daa0d-749">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-750">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-750">Appservice</span></span>

* <span data-ttu-id="daa0d-751">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="daa0d-751">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="daa0d-752">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-752">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="daa0d-753">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="daa0d-753">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="daa0d-754">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="daa0d-754">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="daa0d-755">Lote AI</span><span class="sxs-lookup"><span data-stu-id="daa0d-755">Batch AI</span></span>

* <span data-ttu-id="daa0d-756">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="daa0d-756">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="daa0d-757">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="daa0d-757">Cognitive Services</span></span>

* <span data-ttu-id="daa0d-758">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="daa0d-758">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="daa0d-759">Consumo</span><span class="sxs-lookup"><span data-stu-id="daa0d-759">Consumption</span></span>

* <span data-ttu-id="daa0d-760">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-760">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="daa0d-761">Contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-761">Container</span></span>

* <span data-ttu-id="daa0d-762">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="daa0d-762">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="daa0d-763">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="daa0d-763">Cosmos DB</span></span>

* <span data-ttu-id="daa0d-764">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="daa0d-764">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="daa0d-765">DMS</span><span class="sxs-lookup"><span data-stu-id="daa0d-765">DMS</span></span>

* <span data-ttu-id="daa0d-766">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="daa0d-766">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="daa0d-767">Extensão</span><span class="sxs-lookup"><span data-stu-id="daa0d-767">Extension</span></span>

* <span data-ttu-id="daa0d-768">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="daa0d-768">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="daa0d-769">Interativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-769">Interactive</span></span>

* <span data-ttu-id="daa0d-770">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="daa0d-770">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="daa0d-771">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="daa0d-771">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="daa0d-772">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="daa0d-772">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="daa0d-773">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="daa0d-773">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="daa0d-774">Laboratório</span><span class="sxs-lookup"><span data-stu-id="daa0d-774">Lab</span></span>

* <span data-ttu-id="daa0d-775">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="daa0d-775">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-776">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-776">Network</span></span>

* <span data-ttu-id="daa0d-777">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="daa0d-777">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="daa0d-778">Perfil</span><span class="sxs-lookup"><span data-stu-id="daa0d-778">Profile</span></span>

* <span data-ttu-id="daa0d-779">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="daa0d-779">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="daa0d-780">[ALTERAÇÃO SIGNIFICATIVA] `--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="daa0d-780">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="daa0d-781">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="daa0d-781">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="daa0d-782">Redis</span><span class="sxs-lookup"><span data-stu-id="daa0d-782">Redis</span></span>

* <span data-ttu-id="daa0d-783">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="daa0d-783">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="daa0d-784">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="daa0d-784">Deprecated `redis list-all`.</span></span> <span data-ttu-id="daa0d-785">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="daa0d-785">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="daa0d-786">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="daa0d-786">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="daa0d-787">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="daa0d-787">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="daa0d-788">Função</span><span class="sxs-lookup"><span data-stu-id="daa0d-788">Role</span></span>

* <span data-ttu-id="daa0d-789">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="daa0d-789">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-790">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-790">Storage</span></span>

* <span data-ttu-id="daa0d-791">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="daa0d-791">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="daa0d-792">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="daa0d-792">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="daa0d-793">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="daa0d-793">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="daa0d-794">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="daa0d-794">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="daa0d-795">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="daa0d-795">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-796">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-796">VM</span></span>

* <span data-ttu-id="daa0d-797">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="daa0d-797">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="daa0d-798">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="daa0d-798">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="daa0d-799">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="daa0d-799">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="daa0d-800">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="daa0d-800">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="daa0d-801">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="daa0d-801">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="daa0d-802">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="daa0d-802">Added write accelerator support</span></span>
* <span data-ttu-id="daa0d-803">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="daa0d-803">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="daa0d-804">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="daa0d-804">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="daa0d-805">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="daa0d-805">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="daa0d-806">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-806">April 10, 2018</span></span>

<span data-ttu-id="daa0d-807">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="daa0d-807">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="daa0d-808">ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-808">ACR</span></span>

* <span data-ttu-id="daa0d-809">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="daa0d-809">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-810">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-810">ACS</span></span>

* <span data-ttu-id="daa0d-811">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="daa0d-811">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-812">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-812">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="daa0d-814">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="daa0d-814">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="daa0d-815">BatchAI</span><span class="sxs-lookup"><span data-stu-id="daa0d-815">BatchAI</span></span>

* <span data-ttu-id="daa0d-816">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="daa0d-816">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="daa0d-817">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="daa0d-817">Job level mounting</span></span>
  - <span data-ttu-id="daa0d-818">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="daa0d-818">Environment variables with secret values</span></span>
  - <span data-ttu-id="daa0d-819">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="daa0d-819">Performance counters settings</span></span>
  - <span data-ttu-id="daa0d-820">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="daa0d-820">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="daa0d-821">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="daa0d-821">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="daa0d-822">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="daa0d-822">Usage and limits reporting</span></span>
  - <span data-ttu-id="daa0d-823">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="daa0d-823">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="daa0d-824">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="daa0d-824">Support for custom images</span></span>
  - <span data-ttu-id="daa0d-825">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="daa0d-825">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="daa0d-826">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="daa0d-826">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="daa0d-827">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="daa0d-827">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="daa0d-828">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="daa0d-828">National clouds are supported</span></span>
* <span data-ttu-id="daa0d-829">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="daa0d-829">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="daa0d-830">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="daa0d-830">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="daa0d-831">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="daa0d-831">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="daa0d-832">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="daa0d-832">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="daa0d-833">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="daa0d-833">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="daa0d-834">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="daa0d-834">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="daa0d-835">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="daa0d-835">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="daa0d-836">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="daa0d-836">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="daa0d-837">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="daa0d-837">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="daa0d-838">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-838">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="daa0d-839">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="daa0d-839">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="daa0d-840">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="daa0d-840">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="daa0d-841">[ALTERAÇÃO SIGNIFICATIVA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-841">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="daa0d-842">Cobrança</span><span class="sxs-lookup"><span data-stu-id="daa0d-842">Billing</span></span>

* <span data-ttu-id="daa0d-843">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="daa0d-843">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="daa0d-844">Consumo</span><span class="sxs-lookup"><span data-stu-id="daa0d-844">Consumption</span></span>

* <span data-ttu-id="daa0d-845">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="daa0d-845">Added `marketplace` commands</span></span>
* <span data-ttu-id="daa0d-846">[ALTERAÇÃO SIGNIFICATIVA] `reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="daa0d-846">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="daa0d-847">[ALTERAÇÃO SIGNIFICATIVA] `reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="daa0d-847">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="daa0d-848">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="daa0d-848">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="daa0d-849">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="daa0d-849">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="daa0d-850">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="daa0d-850">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="daa0d-851">Contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-851">Container</span></span>

* <span data-ttu-id="daa0d-852">Adição dos parâmetros de montagem de volume de repositório git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="daa0d-852">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="daa0d-853">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="daa0d-853">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="daa0d-854">Extensão</span><span class="sxs-lookup"><span data-stu-id="daa0d-854">Extension</span></span>

* <span data-ttu-id="daa0d-855">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="daa0d-855">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="daa0d-856">Interativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-856">Interactive</span></span>

* <span data-ttu-id="daa0d-857">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="daa0d-857">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="daa0d-858">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="daa0d-858">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="daa0d-859">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="daa0d-859">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-860">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-860">Network</span></span>

* <span data-ttu-id="daa0d-861">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="daa0d-861">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="daa0d-862">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-862">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="daa0d-863">#4910</span><span class="sxs-lookup"><span data-stu-id="daa0d-863">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="daa0d-864">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="daa0d-864">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="daa0d-865">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="daa0d-865">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="daa0d-866">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-866">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="daa0d-867">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-867">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="daa0d-868">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="daa0d-868">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="daa0d-869">Perfil</span><span class="sxs-lookup"><span data-stu-id="daa0d-869">Profile</span></span>

* <span data-ttu-id="daa0d-870">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="daa0d-870">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="daa0d-871">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="daa0d-871">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="daa0d-872">RDBMS</span><span class="sxs-lookup"><span data-stu-id="daa0d-872">RDBMS</span></span>

* <span data-ttu-id="daa0d-873">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="daa0d-873">Added `georestore` command</span></span>
* <span data-ttu-id="daa0d-874">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-874">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="daa0d-875">Recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-875">Resource</span></span>

* <span data-ttu-id="daa0d-876">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-876">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="daa0d-877">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-877">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="daa0d-878">SQL</span><span class="sxs-lookup"><span data-stu-id="daa0d-878">SQL</span></span>

* <span data-ttu-id="daa0d-879">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="daa0d-879">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-880">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-880">Storage</span></span>

* <span data-ttu-id="daa0d-881">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="daa0d-881">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-882">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-882">VM</span></span>

* <span data-ttu-id="daa0d-883">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-883">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="daa0d-884">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-884">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="daa0d-886">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-886">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="daa0d-887">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="daa0d-887">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="daa0d-888">#5718</span><span class="sxs-lookup"><span data-stu-id="daa0d-888">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="daa0d-889">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="daa0d-889">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="daa0d-890">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-890">March 27, 2018</span></span>

<span data-ttu-id="daa0d-891">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="daa0d-891">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="daa0d-892">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-892">Core</span></span>

* <span data-ttu-id="daa0d-893">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="daa0d-893">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-894">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-894">ACS</span></span>

* <span data-ttu-id="daa0d-895">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="daa0d-895">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-896">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-896">Appservice</span></span>

* <span data-ttu-id="daa0d-897">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-897">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="daa0d-898">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-898">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="daa0d-899">Backup</span><span class="sxs-lookup"><span data-stu-id="daa0d-899">Backup</span></span>

* <span data-ttu-id="daa0d-900">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-900">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="daa0d-901">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="daa0d-901">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="daa0d-902">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="daa0d-902">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="daa0d-903">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="daa0d-903">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="daa0d-904">Contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-904">Container</span></span>

* <span data-ttu-id="daa0d-905">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-905">Added `container exec` command.</span></span> <span data-ttu-id="daa0d-906">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="daa0d-906">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="daa0d-907">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-907">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="daa0d-908">Extensão</span><span class="sxs-lookup"><span data-stu-id="daa0d-908">Extension</span></span>

* <span data-ttu-id="daa0d-909">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="daa0d-909">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="daa0d-910">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="daa0d-910">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="daa0d-911">[ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="daa0d-911">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="daa0d-912">Interativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-912">Interactive</span></span>

* <span data-ttu-id="daa0d-913">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="daa0d-913">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="daa0d-914">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="daa0d-914">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="daa0d-915">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="daa0d-915">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="daa0d-916">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="daa0d-916">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="daa0d-917">Laboratório</span><span class="sxs-lookup"><span data-stu-id="daa0d-917">Lab</span></span>

* <span data-ttu-id="daa0d-918">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="daa0d-918">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="daa0d-919">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="daa0d-919">Monitor</span></span>

* <span data-ttu-id="daa0d-920">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="daa0d-920">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="daa0d-921">[#4529](https://github.com/Azure/azure-cli/issues/5785) corrigido: `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="daa0d-921">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="daa0d-922">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="daa0d-922">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-923">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-923">Network</span></span>

* <span data-ttu-id="daa0d-924">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="daa0d-924">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="daa0d-925">Perfil</span><span class="sxs-lookup"><span data-stu-id="daa0d-925">Profile</span></span>

* <span data-ttu-id="daa0d-926">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="daa0d-926">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="daa0d-927">RDBMS</span><span class="sxs-lookup"><span data-stu-id="daa0d-927">RDBMS</span></span>

* <span data-ttu-id="daa0d-928">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="daa0d-928">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="daa0d-929">Recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-929">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="daa0d-931">Função</span><span class="sxs-lookup"><span data-stu-id="daa0d-931">Role</span></span>

* <span data-ttu-id="daa0d-932">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-932">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="daa0d-933">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="daa0d-933">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="daa0d-934">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-934">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="daa0d-935">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-935">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="daa0d-936">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="daa0d-936">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-937">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-937">Storage</span></span>

* <span data-ttu-id="daa0d-938">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="daa0d-938">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="daa0d-939">[4049#](https://github.com/Azure/azure-cli/issues/4049) corrigido: problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="daa0d-939">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-940">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-940">VM</span></span>

* <span data-ttu-id="daa0d-941">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="daa0d-941">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="daa0d-942">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-942">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="daa0d-943">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="daa0d-943">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="daa0d-944">[ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="daa0d-944">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="daa0d-945">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-945">March 13, 2018</span></span>

<span data-ttu-id="daa0d-946">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="daa0d-946">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="daa0d-947">ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-947">ACR</span></span>

* <span data-ttu-id="daa0d-948">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="daa0d-948">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="daa0d-949">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="daa0d-949">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="daa0d-950">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="daa0d-950">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-951">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-951">ACS</span></span>

* <span data-ttu-id="daa0d-952">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="daa0d-952">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="daa0d-953">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="daa0d-953">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="daa0d-954">Supervisor</span><span class="sxs-lookup"><span data-stu-id="daa0d-954">Advisor</span></span>

* <span data-ttu-id="daa0d-955">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="daa0d-955">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="daa0d-956">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-956">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="daa0d-957">[ALTERAÇÃO SIGNIFICATIVA] `advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="daa0d-957">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="daa0d-958">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="daa0d-958">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="daa0d-959">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="daa0d-959">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-960">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-960">Appservice</span></span>

* <span data-ttu-id="daa0d-961">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="daa0d-961">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="daa0d-962">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="daa0d-962">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="daa0d-963">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="daa0d-963">Eventhubs</span></span>

* <span data-ttu-id="daa0d-964">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="daa0d-964">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="daa0d-965">Extensão</span><span class="sxs-lookup"><span data-stu-id="daa0d-965">Extension</span></span>

* <span data-ttu-id="daa0d-966">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="daa0d-966">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="daa0d-967">Interativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-967">Interactive</span></span>

* <span data-ttu-id="daa0d-968">[5625](https://github.com/Azure/azure-cli/issues/5625) corrigido: manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="daa0d-968">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="daa0d-969">[3016](https://github.com/Azure/azure-cli/issues/3016) corrigido: histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="daa0d-969">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="daa0d-970">[5688](https://github.com/Azure/azure-cli/issues/5688) corrigido: as conclusões não aparecerão se o carregamento da tabela de comando encontrou uma exceção</span><span class="sxs-lookup"><span data-stu-id="daa0d-970">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="daa0d-971">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="daa0d-971">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="daa0d-972">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="daa0d-972">Monitor</span></span>

* <span data-ttu-id="daa0d-973">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="daa0d-973">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="daa0d-974">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="daa0d-974">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="daa0d-975">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="daa0d-975">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="daa0d-976">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="daa0d-976">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-977">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-977">Network</span></span>

* <span data-ttu-id="daa0d-978">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-978">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="daa0d-979">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="daa0d-979">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="daa0d-980">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="daa0d-980">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="daa0d-981">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="daa0d-981">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="daa0d-982">Perfil</span><span class="sxs-lookup"><span data-stu-id="daa0d-982">Profile</span></span>

* <span data-ttu-id="daa0d-983">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="daa0d-983">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="daa0d-984">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="daa0d-984">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="daa0d-985">RDBMS</span><span class="sxs-lookup"><span data-stu-id="daa0d-985">RDBMS</span></span>

* <span data-ttu-id="daa0d-986">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="daa0d-986">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="daa0d-987">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="daa0d-987">Service Bus</span></span>

* <span data-ttu-id="daa0d-988">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="daa0d-988">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-989">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-989">Storage</span></span>

* <span data-ttu-id="daa0d-990">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="daa0d-990">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="daa0d-991">[5286](https://github.com/Azure/azure-cli/issues/5286) corrigido: os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="daa0d-991">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-992">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-992">VM</span></span>

* <span data-ttu-id="daa0d-993">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="daa0d-993">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="daa0d-994">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="daa0d-994">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="daa0d-995">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="daa0d-995">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="daa0d-996">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="daa0d-996">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="daa0d-997">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-997">February 27, 2018</span></span>

<span data-ttu-id="daa0d-998">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="daa0d-998">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="daa0d-999">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-999">Core</span></span>

* <span data-ttu-id="daa0d-1000">Correção [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="daa0d-1000">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="daa0d-1001">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="daa0d-1001">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="daa0d-1002">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1002">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-1003">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1003">ACS</span></span>

* <span data-ttu-id="daa0d-1004">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="daa0d-1004">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="daa0d-1005">Correção do problema de permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="daa0d-1005">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="daa0d-1006">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1006">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="daa0d-1007">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1007">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-1008">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-1008">Appservice</span></span>

* <span data-ttu-id="daa0d-1009">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1009">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="daa0d-1010">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="daa0d-1010">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="daa0d-1011">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="daa0d-1011">Cognitive Services</span></span>

* <span data-ttu-id="daa0d-1012">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="daa0d-1012">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="daa0d-1013">Consumo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1013">Consumption</span></span>

* <span data-ttu-id="daa0d-1014">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="daa0d-1014">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="daa0d-1015">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="daa0d-1015">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="daa0d-1016">Contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-1016">Container</span></span>

* <span data-ttu-id="daa0d-1017">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="daa0d-1017">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-1018">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-1018">Network</span></span>

* <span data-ttu-id="daa0d-1019">Correção [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1019">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="daa0d-1020">Recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-1020">Resource</span></span>

* <span data-ttu-id="daa0d-1021">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="daa0d-1021">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="daa0d-1022">Função</span><span class="sxs-lookup"><span data-stu-id="daa0d-1022">Role</span></span>

* <span data-ttu-id="daa0d-1023">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="daa0d-1023">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="daa0d-1024">SQL</span><span class="sxs-lookup"><span data-stu-id="daa0d-1024">SQL</span></span>

* <span data-ttu-id="daa0d-1025">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="daa0d-1025">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-1026">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1026">Storage</span></span>

* <span data-ttu-id="daa0d-1027">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1027">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-1028">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-1028">VM</span></span>

* <span data-ttu-id="daa0d-1029">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1029">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="daa0d-1030">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-1030">February 13, 2018</span></span>

<span data-ttu-id="daa0d-1031">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="daa0d-1031">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="daa0d-1032">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1032">Core</span></span>

* <span data-ttu-id="daa0d-1033">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="daa0d-1033">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-1034">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1034">ACS</span></span>

* <span data-ttu-id="daa0d-1035">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="daa0d-1035">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="daa0d-1036">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1036">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="daa0d-1037">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="daa0d-1037">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="daa0d-1038">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1038">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="daa0d-1039">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="daa0d-1039">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="daa0d-1040">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1040">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="daa0d-1041">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="daa0d-1041">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="daa0d-1042">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1042">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-1043">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-1043">Appservice</span></span>

* <span data-ttu-id="daa0d-1044">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="daa0d-1044">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="daa0d-1045">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1045">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="daa0d-1046">CDN</span><span class="sxs-lookup"><span data-stu-id="daa0d-1046">CDN</span></span>

* <span data-ttu-id="daa0d-1047">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1047">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="daa0d-1048">Contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-1048">Container</span></span>

* <span data-ttu-id="daa0d-1049">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="daa0d-1049">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="daa0d-1050">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-1050">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="daa0d-1051">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="daa0d-1051">CosmosDB</span></span>

* <span data-ttu-id="daa0d-1052">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="daa0d-1052">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="daa0d-1053">Extensão</span><span class="sxs-lookup"><span data-stu-id="daa0d-1053">Extension</span></span>

* <span data-ttu-id="daa0d-1054">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1054">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="daa0d-1055">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1055">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="daa0d-1056">Comentários</span><span class="sxs-lookup"><span data-stu-id="daa0d-1056">Feedback</span></span>

* <span data-ttu-id="daa0d-1057">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="daa0d-1057">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="daa0d-1058">Interativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1058">Interactive</span></span>

* <span data-ttu-id="daa0d-1059">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="daa0d-1059">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="daa0d-1060">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="daa0d-1060">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="daa0d-1061">IoT</span><span class="sxs-lookup"><span data-stu-id="daa0d-1061">IoT</span></span>

* <span data-ttu-id="daa0d-1062">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="daa0d-1062">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="daa0d-1063">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="daa0d-1063">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="daa0d-1064">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1064">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="daa0d-1065">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="daa0d-1065">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="daa0d-1066">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1066">Monitor</span></span>

* <span data-ttu-id="daa0d-1067">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1067">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-1068">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-1068">Network</span></span>

* <span data-ttu-id="daa0d-1069">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="daa0d-1069">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="daa0d-1070">Perfil</span><span class="sxs-lookup"><span data-stu-id="daa0d-1070">Profile</span></span>

* <span data-ttu-id="daa0d-1071">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1071">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="daa0d-1072">Recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-1072">Resource</span></span>

* <span data-ttu-id="daa0d-1073">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="daa0d-1073">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="daa0d-1074">Função</span><span class="sxs-lookup"><span data-stu-id="daa0d-1074">Role</span></span>

* <span data-ttu-id="daa0d-1075">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1075">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="daa0d-1076">SQL</span><span class="sxs-lookup"><span data-stu-id="daa0d-1076">SQL</span></span>

* <span data-ttu-id="daa0d-1077">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1077">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="daa0d-1078">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1078">Added `sql db rename`</span></span>
* <span data-ttu-id="daa0d-1079">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="daa0d-1079">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-1080">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1080">Storage</span></span>

* <span data-ttu-id="daa0d-1081">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="daa0d-1081">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-1082">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-1082">VM</span></span>

* <span data-ttu-id="daa0d-1083">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="daa0d-1083">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="daa0d-1084">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="daa0d-1084">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="daa0d-1085">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1085">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="daa0d-1086">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-1086">January 31, 2018</span></span>

<span data-ttu-id="daa0d-1087">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="daa0d-1087">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="daa0d-1088">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1088">Core</span></span>

* <span data-ttu-id="daa0d-1089">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="daa0d-1089">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="daa0d-1090">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="daa0d-1090">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="daa0d-1091">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1091">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="daa0d-1092">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="daa0d-1092">Use `--verbose` to see</span></span>
* <span data-ttu-id="daa0d-1093">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="daa0d-1093">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-1094">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1094">ACS</span></span>

* <span data-ttu-id="daa0d-1095">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="daa0d-1095">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="daa0d-1096">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1096">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-1097">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-1097">Appservice</span></span>

* <span data-ttu-id="daa0d-1098">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1098">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="daa0d-1099">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="daa0d-1099">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="daa0d-1100">CDN</span><span class="sxs-lookup"><span data-stu-id="daa0d-1100">CDN</span></span>

* <span data-ttu-id="daa0d-1101">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1101">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="daa0d-1102">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="daa0d-1102">CosmosDB</span></span>

* <span data-ttu-id="daa0d-1103">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="daa0d-1103">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="daa0d-1104">Interativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1104">Interactive</span></span>

* <span data-ttu-id="daa0d-1105">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="daa0d-1105">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-1106">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-1106">Network</span></span>

* <span data-ttu-id="daa0d-1107">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1107">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="daa0d-1108">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="daa0d-1108">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="daa0d-1109">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1109">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="daa0d-1110">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1110">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="daa0d-1111">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1111">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="daa0d-1112">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="daa0d-1112">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="daa0d-1113">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="daa0d-1113">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="daa0d-1114">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="daa0d-1114">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="daa0d-1115">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1115">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="daa0d-1116">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1116">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="daa0d-1117">Perfil</span><span class="sxs-lookup"><span data-stu-id="daa0d-1117">Profile</span></span>

* <span data-ttu-id="daa0d-1118">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="daa0d-1118">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="daa0d-1119">Recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-1119">Resource</span></span>

* <span data-ttu-id="daa0d-1120">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="daa0d-1120">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-1121">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1121">Storage</span></span>

* <span data-ttu-id="daa0d-1122">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="daa0d-1122">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="daa0d-1123">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="daa0d-1123">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="daa0d-1124">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1124">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="daa0d-1125">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1125">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="daa0d-1126">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="daa0d-1126">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-1127">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-1127">VM</span></span>

* <span data-ttu-id="daa0d-1128">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="daa0d-1128">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="daa0d-1129">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="daa0d-1129">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="daa0d-1130">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1130">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="daa0d-1131">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1131">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="daa0d-1132">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="daa0d-1132">January 17, 2018</span></span>

<span data-ttu-id="daa0d-1133">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="daa0d-1133">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="daa0d-1134">ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-1134">ACR</span></span>

* <span data-ttu-id="daa0d-1135">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="daa0d-1135">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="daa0d-1136">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="daa0d-1136">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-1137">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1137">ACS</span></span>

* <span data-ttu-id="daa0d-1138">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1138">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="daa0d-1139">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="daa0d-1139">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-1140">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-1140">Appservice</span></span>

* <span data-ttu-id="daa0d-1141">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1141">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="daa0d-1142">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1142">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="daa0d-1143">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1143">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="daa0d-1144">Backup</span><span class="sxs-lookup"><span data-stu-id="daa0d-1144">Backup</span></span>

* <span data-ttu-id="daa0d-1145">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="daa0d-1145">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="daa0d-1146">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1146">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="daa0d-1147">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="daa0d-1147">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="daa0d-1148">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="daa0d-1148">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="daa0d-1149">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="daa0d-1149">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="daa0d-1150">Lote</span><span class="sxs-lookup"><span data-stu-id="daa0d-1150">Batch</span></span>

* <span data-ttu-id="daa0d-1151">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="daa0d-1151">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="daa0d-1152">Nuvem</span><span class="sxs-lookup"><span data-stu-id="daa0d-1152">Cloud</span></span>

* <span data-ttu-id="daa0d-1153">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="daa0d-1153">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="daa0d-1154">Consumo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1154">Consumption</span></span>

* <span data-ttu-id="daa0d-1155">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1155">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="daa0d-1156">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="daa0d-1156">Event Grid</span></span>

* <span data-ttu-id="daa0d-1157">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1157">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="daa0d-1158">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1158">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="daa0d-1159">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1159">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="daa0d-1160">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1160">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="daa0d-1161">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1161">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="daa0d-1162">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1162">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="daa0d-1163">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1163">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="daa0d-1164">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="daa0d-1164">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="daa0d-1165">Interativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1165">Interactive</span></span>

* <span data-ttu-id="daa0d-1166">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="daa0d-1166">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="daa0d-1167">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="daa0d-1167">Fixed errors on startup</span></span>
* <span data-ttu-id="daa0d-1168">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1168">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="daa0d-1169">IoT</span><span class="sxs-lookup"><span data-stu-id="daa0d-1169">IoT</span></span>

* <span data-ttu-id="daa0d-1170">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="daa0d-1170">Added support for device provisioning service</span></span>
* <span data-ttu-id="daa0d-1171">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="daa0d-1171">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="daa0d-1172">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="daa0d-1172">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="daa0d-1173">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1173">Monitor</span></span>

* <span data-ttu-id="daa0d-1174">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1174">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="daa0d-1175">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1175">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="daa0d-1176">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="daa0d-1176">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-1177">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-1177">Network</span></span>

* <span data-ttu-id="daa0d-1178">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1178">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="daa0d-1179">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1179">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="daa0d-1180">Perfil</span><span class="sxs-lookup"><span data-stu-id="daa0d-1180">Profile</span></span>

* <span data-ttu-id="daa0d-1181">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="daa0d-1181">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="daa0d-1182">Função</span><span class="sxs-lookup"><span data-stu-id="daa0d-1182">Role</span></span>

* <span data-ttu-id="daa0d-1183">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="daa0d-1183">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="daa0d-1184">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="daa0d-1184">Service Fabric</span></span>

* <span data-ttu-id="daa0d-1185">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="daa0d-1185">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="daa0d-1186">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="daa0d-1186">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-1187">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-1187">VM</span></span>

* <span data-ttu-id="daa0d-1188">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1188">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="daa0d-1189">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="daa0d-1189">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="daa0d-1190">[ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="daa0d-1190">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="daa0d-1191">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="daa0d-1191">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="daa0d-1192">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="daa0d-1192">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="daa0d-1193">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1193">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="daa0d-1194">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1194">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="daa0d-1195">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1195">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="daa0d-1196">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="daa0d-1196">December 19, 2017</span></span>

<span data-ttu-id="daa0d-1197">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="daa0d-1197">Version 2.0.23</span></span>

* <span data-ttu-id="daa0d-1198">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="daa0d-1198">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="daa0d-1199">Contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-1199">Container</span></span>

* <span data-ttu-id="daa0d-1200">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-1200">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-1201">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-1201">Network</span></span>

* <span data-ttu-id="daa0d-1202">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1202">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="daa0d-1203">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1203">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-1204">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1204">Storage</span></span>

* <span data-ttu-id="daa0d-1205">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="daa0d-1205">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-1206">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-1206">VM</span></span>

* <span data-ttu-id="daa0d-1207">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="daa0d-1207">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="daa0d-1208">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="daa0d-1208">December 5, 2017</span></span>

<span data-ttu-id="daa0d-1209">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="daa0d-1209">Version 2.0.22</span></span>

* <span data-ttu-id="daa0d-1210">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1210">Removed `az component` commands.</span></span> <span data-ttu-id="daa0d-1211">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1211">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="daa0d-1212">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1212">Core</span></span>
* <span data-ttu-id="daa0d-1213">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="daa0d-1213">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="daa0d-1214">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="daa0d-1214">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-1215">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1215">ACS</span></span>

* <span data-ttu-id="daa0d-1216">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="daa0d-1216">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="daa0d-1217">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1217">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="daa0d-1218">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="daa0d-1218">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="daa0d-1219">Supervisor</span><span class="sxs-lookup"><span data-stu-id="daa0d-1219">Advisor</span></span>

* <span data-ttu-id="daa0d-1220">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="daa0d-1220">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-1221">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-1221">Appservice</span></span>

* <span data-ttu-id="daa0d-1222">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1222">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="daa0d-1223">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="daa0d-1223">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="daa0d-1224">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1224">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="daa0d-1225">Consumo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1225">Consumption</span></span>

* <span data-ttu-id="daa0d-1226">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="daa0d-1226">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="daa0d-1227">Contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-1227">Container</span></span>

* <span data-ttu-id="daa0d-1228">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="daa0d-1228">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="daa0d-1229">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1229">Monitor</span></span>

* <span data-ttu-id="daa0d-1230">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="daa0d-1230">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="daa0d-1231">Recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-1231">Resource</span></span>

* <span data-ttu-id="daa0d-1232">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1232">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="daa0d-1233">Função</span><span class="sxs-lookup"><span data-stu-id="daa0d-1233">Role</span></span>

* <span data-ttu-id="daa0d-1234">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1234">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="daa0d-1235">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="daa0d-1235">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="daa0d-1236">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1236">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="daa0d-1237">SQL</span><span class="sxs-lookup"><span data-stu-id="daa0d-1237">SQL</span></span>

* <span data-ttu-id="daa0d-1238">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="daa0d-1238">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="daa0d-1239">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="daa0d-1239">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-1240">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-1240">VM</span></span>

* <span data-ttu-id="daa0d-1241">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1241">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="daa0d-1242">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="daa0d-1242">November 14, 2017</span></span>

<span data-ttu-id="daa0d-1243">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="daa0d-1243">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="daa0d-1244">ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-1244">ACR</span></span>

* <span data-ttu-id="daa0d-1245">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="daa0d-1245">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="daa0d-1246">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1246">ACS</span></span>

* <span data-ttu-id="daa0d-1247">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1247">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="daa0d-1248">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1248">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="daa0d-1249">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1249">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="daa0d-1250">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="daa0d-1250">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="daa0d-1251">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="daa0d-1251">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-1252">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-1252">Appservice</span></span>

* <span data-ttu-id="daa0d-1253">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="daa0d-1253">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="daa0d-1254">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1254">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="daa0d-1255">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1255">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="daa0d-1256">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1256">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="daa0d-1257">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="daa0d-1257">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="daa0d-1258">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1258">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="daa0d-1259">Lote</span><span class="sxs-lookup"><span data-stu-id="daa0d-1259">Batch</span></span>

* <span data-ttu-id="daa0d-1260">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1260">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="daa0d-1261">Batchai</span><span class="sxs-lookup"><span data-stu-id="daa0d-1261">Batchai</span></span>

* <span data-ttu-id="daa0d-1262">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1262">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="daa0d-1263">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1263">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="daa0d-1264">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1264">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="daa0d-1265">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1265">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="daa0d-1266">Nuvem</span><span class="sxs-lookup"><span data-stu-id="daa0d-1266">Cloud</span></span>

* <span data-ttu-id="daa0d-1267">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="daa0d-1267">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="daa0d-1268">Contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-1268">Container</span></span>

* <span data-ttu-id="daa0d-1269">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="daa0d-1269">Added support to open multiple ports</span></span>
* <span data-ttu-id="daa0d-1270">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="daa0d-1270">Added container group restart policy</span></span>
* <span data-ttu-id="daa0d-1271">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="daa0d-1271">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="daa0d-1272">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="daa0d-1272">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="daa0d-1273">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="daa0d-1273">Data Lake Analytics</span></span>

* <span data-ttu-id="daa0d-1274">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="daa0d-1274">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="daa0d-1275">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="daa0d-1275">Data Lake Store</span></span>

* <span data-ttu-id="daa0d-1276">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="daa0d-1276">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="daa0d-1277">Extensão</span><span class="sxs-lookup"><span data-stu-id="daa0d-1277">Extension</span></span>

* <span data-ttu-id="daa0d-1278">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="daa0d-1278">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="daa0d-1279">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="daa0d-1279">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="daa0d-1280">IoT</span><span class="sxs-lookup"><span data-stu-id="daa0d-1280">IoT</span></span>

* <span data-ttu-id="daa0d-1281">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="daa0d-1281">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="daa0d-1282">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1282">Monitor</span></span>

* <span data-ttu-id="daa0d-1283">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1283">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-1284">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-1284">Network</span></span>

* <span data-ttu-id="daa0d-1285">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="daa0d-1285">Added support for CAA DNS records</span></span>
* <span data-ttu-id="daa0d-1286">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1286">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="daa0d-1287">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="daa0d-1287">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="daa0d-1288">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1288">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="daa0d-1289">Reservas</span><span class="sxs-lookup"><span data-stu-id="daa0d-1289">Reservations</span></span>

* <span data-ttu-id="daa0d-1290">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="daa0d-1290">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="daa0d-1291">Recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-1291">Resource</span></span>

* <span data-ttu-id="daa0d-1292">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-1292">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="daa0d-1293">SQL</span><span class="sxs-lookup"><span data-stu-id="daa0d-1293">SQL</span></span>

* <span data-ttu-id="daa0d-1294">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1294">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-1295">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1295">Storage</span></span>

* <span data-ttu-id="daa0d-1296">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="daa0d-1296">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="daa0d-1297">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="daa0d-1297">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="daa0d-1298">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1298">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="daa0d-1299">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1299">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="daa0d-1300">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1300">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="daa0d-1301">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1301">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="daa0d-1302">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1302">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-1303">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-1303">VM</span></span>

* <span data-ttu-id="daa0d-1304">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1304">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="daa0d-1305">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="daa0d-1305">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="daa0d-1306">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="daa0d-1306">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="daa0d-1307">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1307">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="daa0d-1308">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1308">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="daa0d-1309">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="daa0d-1309">October 24, 2017</span></span>

<span data-ttu-id="daa0d-1310">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="daa0d-1310">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="daa0d-1311">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1311">Core</span></span>

* <span data-ttu-id="daa0d-1312">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1312">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="daa0d-1313">ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-1313">ACR</span></span>

* <span data-ttu-id="daa0d-1314">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1314">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="daa0d-1315">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="daa0d-1315">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="daa0d-1316">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="daa0d-1316">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-1317">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1317">ACS</span></span>

* <span data-ttu-id="daa0d-1318">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="daa0d-1318">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="daa0d-1319">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="daa0d-1319">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-1320">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-1320">Appservice</span></span>

* <span data-ttu-id="daa0d-1321">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="daa0d-1321">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="daa0d-1322">Componente</span><span class="sxs-lookup"><span data-stu-id="daa0d-1322">Component</span></span>

* <span data-ttu-id="daa0d-1323">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="daa0d-1323">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="daa0d-1324">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1324">Monitor</span></span>

* <span data-ttu-id="daa0d-1325">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1325">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="daa0d-1326">Recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-1326">Resource</span></span>

* <span data-ttu-id="daa0d-1327">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1327">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="daa0d-1328">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="daa0d-1328">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-1329">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-1329">VM</span></span>

* <span data-ttu-id="daa0d-1330">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1330">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="daa0d-1331">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="daa0d-1331">October 9, 2017</span></span>

<span data-ttu-id="daa0d-1332">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="daa0d-1332">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="daa0d-1333">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1333">Core</span></span>

* <span data-ttu-id="daa0d-1334">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="daa0d-1334">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-1335">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-1335">Appservice</span></span>

* <span data-ttu-id="daa0d-1336">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1336">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="daa0d-1337">Lote</span><span class="sxs-lookup"><span data-stu-id="daa0d-1337">Batch</span></span>

* <span data-ttu-id="daa0d-1338">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="daa0d-1338">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="daa0d-1339">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="daa0d-1339">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="daa0d-1340">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="daa0d-1340">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="daa0d-1341">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="daa0d-1341">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="daa0d-1342">Batchai</span><span class="sxs-lookup"><span data-stu-id="daa0d-1342">Batchai</span></span>

* <span data-ttu-id="daa0d-1343">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="daa0d-1343">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="daa0d-1344">Keyvault</span><span class="sxs-lookup"><span data-stu-id="daa0d-1344">Keyvault</span></span>

* <span data-ttu-id="daa0d-1345">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1345">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="daa0d-1346">(#4448)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1346">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="daa0d-1347">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-1347">Network</span></span>

* <span data-ttu-id="daa0d-1348">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="daa0d-1348">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="daa0d-1349">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="daa0d-1349">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="daa0d-1350">Recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-1350">Resource</span></span>

* <span data-ttu-id="daa0d-1351">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1351">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="daa0d-1352">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="daa0d-1352">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="daa0d-1353">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1353">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="daa0d-1354">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-1354">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="daa0d-1355">Sql</span><span class="sxs-lookup"><span data-stu-id="daa0d-1355">Sql</span></span>

* <span data-ttu-id="daa0d-1356">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="daa0d-1356">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="daa0d-1357">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="daa0d-1357">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="daa0d-1358">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="daa0d-1358">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-1359">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1359">Storage</span></span>

* <span data-ttu-id="daa0d-1360">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="daa0d-1360">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-1361">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-1361">Vm</span></span>

* <span data-ttu-id="daa0d-1362">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="daa0d-1362">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="daa0d-1363">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1363">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="daa0d-1364">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1364">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="daa0d-1365">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1365">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="daa0d-1366">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1366">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="daa0d-1367">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="daa0d-1367">September 22, 2017</span></span>

<span data-ttu-id="daa0d-1368">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="daa0d-1368">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="daa0d-1369">Recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-1369">Resource</span></span>

* <span data-ttu-id="daa0d-1370">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="daa0d-1370">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="daa0d-1371">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="daa0d-1371">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="daa0d-1372">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1372">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="daa0d-1373">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1373">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-1374">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-1374">Network</span></span>

* <span data-ttu-id="daa0d-1375">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1375">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="daa0d-1376">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1376">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="daa0d-1377">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1377">Added `asg` application security group commands</span></span>
* <span data-ttu-id="daa0d-1378">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1378">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="daa0d-1379">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1379">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="daa0d-1380">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1380">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="daa0d-1381">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1381">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-1382">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1382">Storage</span></span>

* <span data-ttu-id="daa0d-1383">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="daa0d-1383">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="daa0d-1384">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="daa0d-1384">Eventgrid</span></span>

* <span data-ttu-id="daa0d-1385">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="daa0d-1385">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="daa0d-1386">SQL</span><span class="sxs-lookup"><span data-stu-id="daa0d-1386">SQL</span></span>

* <span data-ttu-id="daa0d-1387">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1387">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="daa0d-1388">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="daa0d-1388">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="daa0d-1389">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1389">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="daa0d-1390">Keyvault</span><span class="sxs-lookup"><span data-stu-id="daa0d-1390">Keyvault</span></span>

* <span data-ttu-id="daa0d-1391">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="daa0d-1391">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-1392">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-1392">VM</span></span>

* <span data-ttu-id="daa0d-1393">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1393">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="daa0d-1394">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="daa0d-1394">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="daa0d-1395">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1395">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="daa0d-1396">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1396">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="daa0d-1397">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1397">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="daa0d-1398">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1398">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-1399">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1399">ACS</span></span>

* <span data-ttu-id="daa0d-1400">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1400">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-1401">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-1401">Appservice</span></span>

* <span data-ttu-id="daa0d-1402">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1402">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="daa0d-1403">Backup</span><span class="sxs-lookup"><span data-stu-id="daa0d-1403">Backup</span></span>

* <span data-ttu-id="daa0d-1404">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="daa0d-1404">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="daa0d-1405">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="daa0d-1405">September 11, 2017</span></span>

<span data-ttu-id="daa0d-1406">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="daa0d-1406">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="daa0d-1407">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1407">Core</span></span>

* <span data-ttu-id="daa0d-1408">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="daa0d-1408">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="daa0d-1409">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="daa0d-1409">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-1410">Acs</span><span class="sxs-lookup"><span data-stu-id="daa0d-1410">Acs</span></span>

* <span data-ttu-id="daa0d-1411">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1411">Added `acs list-locations` command</span></span>
* <span data-ttu-id="daa0d-1412">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="daa0d-1412">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-1413">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-1413">Appservice</span></span>

* <span data-ttu-id="daa0d-1414">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1414">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="daa0d-1415">CDN</span><span class="sxs-lookup"><span data-stu-id="daa0d-1415">CDN</span></span>

* <span data-ttu-id="daa0d-1416">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1416">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="daa0d-1417">Extensão</span><span class="sxs-lookup"><span data-stu-id="daa0d-1417">Extension</span></span>

* <span data-ttu-id="daa0d-1418">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="daa0d-1418">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="daa0d-1419">Keyvault</span><span class="sxs-lookup"><span data-stu-id="daa0d-1419">Keyvault</span></span>

* <span data-ttu-id="daa0d-1420">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1420">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-1421">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-1421">Network</span></span>

* <span data-ttu-id="daa0d-1422">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1422">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="daa0d-1423">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1423">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="daa0d-1424">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1424">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="daa0d-1425">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1425">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="daa0d-1426">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1426">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="daa0d-1427">Recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-1427">Resource</span></span>

* <span data-ttu-id="daa0d-1428">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1428">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="daa0d-1429">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1429">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="daa0d-1430">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="daa0d-1430">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="daa0d-1431">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="daa0d-1431">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="daa0d-1432">SQL</span><span class="sxs-lookup"><span data-stu-id="daa0d-1432">SQL</span></span>

* <span data-ttu-id="daa0d-1433">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1433">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-1434">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-1434">VM</span></span>

* <span data-ttu-id="daa0d-1435">Corrigido: Não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="daa0d-1435">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="daa0d-1436">Corrigido: Usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="daa0d-1436">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="daa0d-1437">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1437">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="daa0d-1438">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="daa0d-1438">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="daa0d-1439">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="daa0d-1439">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="daa0d-1440">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="daa0d-1440">August 31, 2017</span></span>

<span data-ttu-id="daa0d-1441">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="daa0d-1441">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="daa0d-1442">Keyvault</span><span class="sxs-lookup"><span data-stu-id="daa0d-1442">Keyvault</span></span>

* <span data-ttu-id="daa0d-1443">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1443">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="daa0d-1444">Sf</span><span class="sxs-lookup"><span data-stu-id="daa0d-1444">Sf</span></span>

* <span data-ttu-id="daa0d-1445">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1445">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-1446">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1446">Storage</span></span>

* <span data-ttu-id="daa0d-1447">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="daa0d-1447">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="daa0d-1448">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="daa0d-1448">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="daa0d-1449">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="daa0d-1449">August 28, 2017</span></span>

<span data-ttu-id="daa0d-1450">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="daa0d-1450">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="daa0d-1451">CLI</span><span class="sxs-lookup"><span data-stu-id="daa0d-1451">CLI</span></span>

* <span data-ttu-id="daa0d-1452">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1452">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-1453">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1453">ACS</span></span>

* <span data-ttu-id="daa0d-1454">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="daa0d-1454">Corrected preview regions</span></span>
* <span data-ttu-id="daa0d-1455">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1455">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="daa0d-1456">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="daa0d-1456">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-1457">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-1457">Appservice</span></span>

* <span data-ttu-id="daa0d-1458">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1458">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="daa0d-1459">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1459">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="daa0d-1460">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1460">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="daa0d-1461">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1461">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="daa0d-1462">Correção: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="daa0d-1462">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="daa0d-1463">IoT</span><span class="sxs-lookup"><span data-stu-id="daa0d-1463">IoT</span></span>

* <span data-ttu-id="daa0d-1464">Correção #3934: Criação de política não limpa as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="daa0d-1464">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-1465">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-1465">Network</span></span>

* <span data-ttu-id="daa0d-1466">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1466">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="daa0d-1467">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1467">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="daa0d-1468">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1468">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="daa0d-1469">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1469">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="daa0d-1470">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1470">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="daa0d-1471">Perfil</span><span class="sxs-lookup"><span data-stu-id="daa0d-1471">Profile</span></span>

* <span data-ttu-id="daa0d-1472">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="daa0d-1472">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="daa0d-1473">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="daa0d-1473">Service Fabric</span></span>

* <span data-ttu-id="daa0d-1474">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="daa0d-1474">Preview release</span></span>
* <span data-ttu-id="daa0d-1475">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="daa0d-1475">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="daa0d-1476">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="daa0d-1476">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="daa0d-1477">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="daa0d-1477">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-1478">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1478">Storage</span></span>

* <span data-ttu-id="daa0d-1479">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="daa0d-1479">Enabled setting blob tier</span></span>
* <span data-ttu-id="daa0d-1480">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="daa0d-1480">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="daa0d-1481">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="daa0d-1481">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="daa0d-1482">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="daa0d-1482">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="daa0d-1483">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1483">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="daa0d-1484">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="daa0d-1484">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-1485">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-1485">VM</span></span>

* <span data-ttu-id="daa0d-1486">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1486">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="daa0d-1487">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="daa0d-1487">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="daa0d-1488">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1488">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="daa0d-1489">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="daa0d-1489">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="daa0d-1490">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="daa0d-1490">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="daa0d-1491">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1491">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="daa0d-1492">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="daa0d-1492">August 15, 2017</span></span>

<span data-ttu-id="daa0d-1493">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="daa0d-1493">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-1494">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1494">ACS</span></span>

* <span data-ttu-id="daa0d-1495">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="daa0d-1495">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-1496">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-1496">Appservice</span></span>

* <span data-ttu-id="daa0d-1497">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="daa0d-1497">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="daa0d-1498">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="daa0d-1498">Event Grid</span></span>

* <span data-ttu-id="daa0d-1499">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="daa0d-1499">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="daa0d-1500">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="daa0d-1500">August 11, 2017</span></span>

<span data-ttu-id="daa0d-1501">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="daa0d-1501">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-1502">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1502">ACS</span></span>

* <span data-ttu-id="daa0d-1503">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="daa0d-1503">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="daa0d-1504">Lote</span><span class="sxs-lookup"><span data-stu-id="daa0d-1504">Batch</span></span>

* <span data-ttu-id="daa0d-1505">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="daa0d-1505">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="daa0d-1506">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="daa0d-1506">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="daa0d-1507">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-1507">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="daa0d-1508">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="daa0d-1508">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="daa0d-1509">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="daa0d-1509">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="daa0d-1510">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="daa0d-1510">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="daa0d-1511">Componente</span><span class="sxs-lookup"><span data-stu-id="daa0d-1511">Component</span></span>

* <span data-ttu-id="daa0d-1512">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="daa0d-1512">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="daa0d-1513">Contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-1513">Container</span></span>

* <span data-ttu-id="daa0d-1514">`create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="daa0d-1514">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="daa0d-1515">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="daa0d-1515">Data Lake Store</span></span>

* <span data-ttu-id="daa0d-1516">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1516">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="daa0d-1517">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="daa0d-1517">Event Grid</span></span>

* <span data-ttu-id="daa0d-1518">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="daa0d-1518">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-1519">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-1519">Network</span></span>

* <span data-ttu-id="daa0d-1520">`lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="daa0d-1520">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="daa0d-1521">`application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="daa0d-1521">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="daa0d-1522">`application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="daa0d-1522">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="daa0d-1523">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1523">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="daa0d-1524">Perfil</span><span class="sxs-lookup"><span data-stu-id="daa0d-1524">Profile</span></span>

* <span data-ttu-id="daa0d-1525">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="daa0d-1525">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-1526">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1526">Storage</span></span>

* <span data-ttu-id="daa0d-1527">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="daa0d-1527">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-1528">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-1528">VM</span></span>

* <span data-ttu-id="daa0d-1529">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="daa0d-1529">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="daa0d-1530">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1530">Exposed `list-skus` command</span></span>
* <span data-ttu-id="daa0d-1531">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="daa0d-1531">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="daa0d-1532">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="daa0d-1532">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="daa0d-1533">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="daa0d-1533">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="daa0d-1534">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="daa0d-1534">July 28, 2017</span></span>

<span data-ttu-id="daa0d-1535">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="daa0d-1535">Version 2.0.12</span></span>

* <span data-ttu-id="daa0d-1536">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-1536">Added container commands</span></span>
* <span data-ttu-id="daa0d-1537">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1537">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="daa0d-1538">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1538">Core</span></span>

* <span data-ttu-id="daa0d-1539">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="daa0d-1539">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="daa0d-1540">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="daa0d-1540">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="daa0d-1541">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="daa0d-1541">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="daa0d-1542">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1542">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="daa0d-1543">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="daa0d-1543">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="daa0d-1544">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1544">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="daa0d-1545">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1545">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="daa0d-1546">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1546">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="daa0d-1547">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1547">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="daa0d-1548">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="daa0d-1548">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="daa0d-1549">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="daa0d-1549">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="daa0d-1550">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1550">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="daa0d-1551">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="daa0d-1551">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="daa0d-1552">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="daa0d-1552">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="daa0d-1553">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="daa0d-1553">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="daa0d-1554">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1554">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="daa0d-1555">ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-1555">ACR</span></span>

* <span data-ttu-id="daa0d-1556">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="daa0d-1556">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="daa0d-1557">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="daa0d-1557">Support SKU update for managed registries</span></span>
* <span data-ttu-id="daa0d-1558">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="daa0d-1558">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="daa0d-1559">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-1559">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="daa0d-1560">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-1560">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="daa0d-1561">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="daa0d-1561">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-1562">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1562">ACS</span></span>

* <span data-ttu-id="daa0d-1563">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="daa0d-1563">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-1564">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-1564">Appservice</span></span>

* <span data-ttu-id="daa0d-1565">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="daa0d-1565">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="daa0d-1566">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="daa0d-1566">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="daa0d-1567">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1567">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="daa0d-1568">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1568">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="daa0d-1569">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1569">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="daa0d-1570">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1570">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="daa0d-1571">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1571">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="daa0d-1572">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1572">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="daa0d-1573">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1573">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="daa0d-1574">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1574">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="daa0d-1575">Lote</span><span class="sxs-lookup"><span data-stu-id="daa0d-1575">Batch</span></span>

* <span data-ttu-id="daa0d-1576">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="daa0d-1576">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="daa0d-1577">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1577">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="daa0d-1578">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1578">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="daa0d-1579">CDN</span><span class="sxs-lookup"><span data-stu-id="daa0d-1579">CDN</span></span>

* <span data-ttu-id="daa0d-1580">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="daa0d-1580">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="daa0d-1581">Nuvem</span><span class="sxs-lookup"><span data-stu-id="daa0d-1581">Cloud</span></span>

* <span data-ttu-id="daa0d-1582">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="daa0d-1582">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="daa0d-1583">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="daa0d-1583">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="daa0d-1584">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="daa0d-1584">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="daa0d-1585">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="daa0d-1585">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="daa0d-1586">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1586">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="daa0d-1587">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="daa0d-1587">CosmosDB</span></span>

* <span data-ttu-id="daa0d-1588">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="daa0d-1588">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="daa0d-1589">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="daa0d-1589">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="daa0d-1590">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="daa0d-1590">Data Lake Analytics</span></span>

* <span data-ttu-id="daa0d-1591">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1591">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="daa0d-1592">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1592">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="daa0d-1593">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1593">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="daa0d-1594">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="daa0d-1594">Data Lake Store</span></span>

* <span data-ttu-id="daa0d-1595">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1595">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="daa0d-1596">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="daa0d-1596">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="daa0d-1597">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1597">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="daa0d-1598">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="daa0d-1598">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="daa0d-1599">Interativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1599">Interactive</span></span>

* <span data-ttu-id="daa0d-1600">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="daa0d-1600">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="daa0d-1601">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="daa0d-1601">Increased test coverage</span></span>
* <span data-ttu-id="daa0d-1602">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="daa0d-1602">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="daa0d-1603">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1603">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="daa0d-1604">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1604">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="daa0d-1605">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1605">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="daa0d-1606">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1606">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="daa0d-1607">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1607">Added `--progress` flag</span></span>
* <span data-ttu-id="daa0d-1608">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="daa0d-1608">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="daa0d-1609">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1609">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="daa0d-1610">IoT</span><span class="sxs-lookup"><span data-stu-id="daa0d-1610">IoT</span></span>

* <span data-ttu-id="daa0d-1611">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1611">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="daa0d-1612">(#3934)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1612">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="daa0d-1613">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="daa0d-1613">Key vault</span></span>

* <span data-ttu-id="daa0d-1614">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="daa0d-1614">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="daa0d-1615">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1615">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="daa0d-1616">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1616">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="daa0d-1617">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1617">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="daa0d-1618">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1618">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="daa0d-1619">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1619">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="daa0d-1620">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1620">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="daa0d-1621">(#3307)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1621">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="daa0d-1622">Laboratório</span><span class="sxs-lookup"><span data-stu-id="daa0d-1622">Lab</span></span>

* <span data-ttu-id="daa0d-1623">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1623">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="daa0d-1624">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1624">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="daa0d-1625">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1625">Monitor</span></span>

* <span data-ttu-id="daa0d-1626">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1626">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="daa0d-1627">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1627">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="daa0d-1628">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1628">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="daa0d-1629">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1629">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="daa0d-1630">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1630">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="daa0d-1631">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="daa0d-1631">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="daa0d-1632">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="daa0d-1632">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="daa0d-1633">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="daa0d-1633">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="daa0d-1634">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="daa0d-1634">`location` no longer required</span></span>
  * <span data-ttu-id="daa0d-1635">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="daa0d-1635">Add name and ID support for target</span></span>
  * <span data-ttu-id="daa0d-1636">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1636">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="daa0d-1637">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="daa0d-1637">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="daa0d-1638">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="daa0d-1638">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="daa0d-1639">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="daa0d-1639">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="daa0d-1640">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1640">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="daa0d-1641">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1641">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-1642">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-1642">Network</span></span>

* <span data-ttu-id="daa0d-1643">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1643">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="daa0d-1644">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1644">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="daa0d-1645">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="daa0d-1645">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="daa0d-1646">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="daa0d-1646">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="daa0d-1647">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1647">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="daa0d-1648">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1648">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="daa0d-1649">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1649">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="daa0d-1650">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1650">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="daa0d-1651">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1651">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="daa0d-1652">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1652">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="daa0d-1653">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1653">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="daa0d-1654">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1654">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="daa0d-1655">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1655">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="daa0d-1656">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1656">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="daa0d-1657">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1657">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="daa0d-1658">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1658">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="daa0d-1659">Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1659">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="daa0d-1660">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1660">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="daa0d-1661">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1661">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="daa0d-1662">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1662">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="daa0d-1663">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1663">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="daa0d-1664">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1664">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="daa0d-1665">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1665">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="daa0d-1666">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="daa0d-1666">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="daa0d-1667">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="daa0d-1667">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="daa0d-1668">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="daa0d-1668">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="daa0d-1669">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="daa0d-1669">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="daa0d-1670">Perfil</span><span class="sxs-lookup"><span data-stu-id="daa0d-1670">Profile</span></span>

* <span data-ttu-id="daa0d-1671">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="daa0d-1671">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="daa0d-1672">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="daa0d-1672">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="daa0d-1673">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="daa0d-1673">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="daa0d-1674">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="daa0d-1674">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="daa0d-1675">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="daa0d-1675">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="daa0d-1676">RDBMS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1676">RDBMS</span></span>

* <span data-ttu-id="daa0d-1677">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1677">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="daa0d-1678">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1678">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="daa0d-1679">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1679">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="daa0d-1680">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1680">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="daa0d-1681">Recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-1681">Resource</span></span>

* <span data-ttu-id="daa0d-1682">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1682">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="daa0d-1683">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1683">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="daa0d-1684">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1684">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="daa0d-1685">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1685">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="daa0d-1686">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1686">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="daa0d-1687">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1687">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="daa0d-1688">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1688">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="daa0d-1689">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1689">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="daa0d-1690">Função</span><span class="sxs-lookup"><span data-stu-id="daa0d-1690">Role</span></span>

* <span data-ttu-id="daa0d-1691">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1691">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="daa0d-1692">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1692">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="daa0d-1693">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1693">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="daa0d-1694">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1694">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="daa0d-1695">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1695">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="daa0d-1696">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="daa0d-1696">Service Fabric</span></span>
* <span data-ttu-id="daa0d-1697">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1697">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="daa0d-1698">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1698">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="daa0d-1699">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1699">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="daa0d-1700">SQL</span><span class="sxs-lookup"><span data-stu-id="daa0d-1700">SQL</span></span>

* <span data-ttu-id="daa0d-1701">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1701">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="daa0d-1702">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1702">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="daa0d-1703">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1703">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-1704">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1704">Storage</span></span>

* <span data-ttu-id="daa0d-1705">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1705">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="daa0d-1706">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="daa0d-1706">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="daa0d-1707">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1707">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="daa0d-1708">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1708">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="daa0d-1709">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1709">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="daa0d-1710">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1710">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-1711">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-1711">VM</span></span>

* <span data-ttu-id="daa0d-1712">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="daa0d-1712">Support configuring nsg</span></span>
* <span data-ttu-id="daa0d-1713">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="daa0d-1713">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="daa0d-1714">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="daa0d-1714">Support managed service identities</span></span>
* <span data-ttu-id="daa0d-1715">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1715">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="daa0d-1716">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="daa0d-1716">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="daa0d-1717">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="daa0d-1717">May 10, 2017</span></span>

<span data-ttu-id="daa0d-1718">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="daa0d-1718">Version 2.0.6</span></span>

* <span data-ttu-id="daa0d-1719">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="daa0d-1719">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="daa0d-1720">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1720">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="daa0d-1721">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="daa0d-1721">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="daa0d-1722">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="daa0d-1722">Include Cognitive Services module</span></span>
* <span data-ttu-id="daa0d-1723">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="daa0d-1723">Include Service Fabric module</span></span>
* <span data-ttu-id="daa0d-1724">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1724">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="daa0d-1725">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="daa0d-1725">Add support for CDN commands</span></span>
* <span data-ttu-id="daa0d-1726">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="daa0d-1726">Remove Container module</span></span>
* <span data-ttu-id="daa0d-1727">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1727">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="daa0d-1728">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1728">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="daa0d-1729">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1729">Core</span></span>

* <span data-ttu-id="daa0d-1730">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="daa0d-1730">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="daa0d-1731">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1731">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="daa0d-1732">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1732">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="daa0d-1733">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1733">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="daa0d-1734">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1734">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="daa0d-1735">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1735">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="daa0d-1736">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1736">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="daa0d-1737">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1737">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="daa0d-1738">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1738">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="daa0d-1739">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="daa0d-1739">core: Improved performance</span></span>
* <span data-ttu-id="daa0d-1740">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="daa0d-1740">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="daa0d-1741">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="daa0d-1741">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-1742">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1742">ACS</span></span>

* <span data-ttu-id="daa0d-1743">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="daa0d-1743">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="daa0d-1744">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="daa0d-1744">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="daa0d-1745">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="daa0d-1745">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="daa0d-1746">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1746">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-1747">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-1747">AppService</span></span>

* <span data-ttu-id="daa0d-1748">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1748">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="daa0d-1749">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="daa0d-1749">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="daa0d-1750">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1750">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="daa0d-1751">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="daa0d-1751">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="daa0d-1752">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="daa0d-1752">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="daa0d-1753">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1753">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="daa0d-1754">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="daa0d-1754">support slot swap with preview</span></span>
* <span data-ttu-id="daa0d-1755">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1755">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="daa0d-1756">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1756">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="daa0d-1757">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="daa0d-1757">CosmosDB</span></span>

* <span data-ttu-id="daa0d-1758">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="daa0d-1758">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="daa0d-1759">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="daa0d-1759">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="daa0d-1760">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="daa0d-1760">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="daa0d-1761">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="daa0d-1761">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="daa0d-1762">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="daa0d-1762">Data Lake Analytics</span></span>

* <span data-ttu-id="daa0d-1763">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="daa0d-1763">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="daa0d-1764">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1764">Add support for new catalog item type: package.</span></span> <span data-ttu-id="daa0d-1765">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1765">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="daa0d-1766">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="daa0d-1766">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="daa0d-1767">Tabela</span><span class="sxs-lookup"><span data-stu-id="daa0d-1767">Table</span></span>
  * <span data-ttu-id="daa0d-1768">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="daa0d-1768">Table valued function</span></span>
  * <span data-ttu-id="daa0d-1769">Visualizar</span><span class="sxs-lookup"><span data-stu-id="daa0d-1769">View</span></span>
  * <span data-ttu-id="daa0d-1770">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1770">Table Statistics.</span></span> <span data-ttu-id="daa0d-1771">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="daa0d-1771">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="daa0d-1772">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="daa0d-1772">Data Lake Store</span></span>

* <span data-ttu-id="daa0d-1773">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="daa0d-1773">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="daa0d-1774">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1774">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="daa0d-1775">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1775">missed help for access show.</span></span> <span data-ttu-id="daa0d-1776">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1776">adding it.</span></span> <span data-ttu-id="daa0d-1777">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1777">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="daa0d-1778">Localizar</span><span class="sxs-lookup"><span data-stu-id="daa0d-1778">Find</span></span>

* <span data-ttu-id="daa0d-1779">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="daa0d-1779">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="daa0d-1780">KeyVault</span><span class="sxs-lookup"><span data-stu-id="daa0d-1780">KeyVault</span></span>

* <span data-ttu-id="daa0d-1781">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="daa0d-1781">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="daa0d-1782">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="daa0d-1782">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="daa0d-1783">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="daa0d-1783">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="daa0d-1784">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="daa0d-1784">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="daa0d-1785">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1785">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="daa0d-1786">Laboratório</span><span class="sxs-lookup"><span data-stu-id="daa0d-1786">Lab</span></span>

* <span data-ttu-id="daa0d-1787">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="daa0d-1787">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="daa0d-1788">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="daa0d-1788">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="daa0d-1789">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="daa0d-1789">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="daa0d-1790">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="daa0d-1790">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="daa0d-1791">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="daa0d-1791">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="daa0d-1792">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1792">Monitor</span></span>

* <span data-ttu-id="daa0d-1793">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1793">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="daa0d-1794">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1794">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="daa0d-1795">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-1795">Network</span></span>

* <span data-ttu-id="daa0d-1796">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1796">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="daa0d-1797">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1797">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="daa0d-1798">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1798">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="daa0d-1799">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1799">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="daa0d-1800">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="daa0d-1800">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="daa0d-1801">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="daa0d-1801">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="daa0d-1802">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="daa0d-1802">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="daa0d-1803">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="daa0d-1803">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="daa0d-1804">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1804">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="daa0d-1805">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="daa0d-1805">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="daa0d-1806">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1806">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="daa0d-1807">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1807">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="daa0d-1808">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="daa0d-1808">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="daa0d-1809">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="daa0d-1809">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="daa0d-1810">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="daa0d-1810">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="daa0d-1811">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="daa0d-1811">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="daa0d-1812">Perfil</span><span class="sxs-lookup"><span data-stu-id="daa0d-1812">Profile</span></span>

* <span data-ttu-id="daa0d-1813">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1813">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="daa0d-1814">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1814">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="daa0d-1815">Redis</span><span class="sxs-lookup"><span data-stu-id="daa0d-1815">Redis</span></span>

* <span data-ttu-id="daa0d-1816">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="daa0d-1816">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="daa0d-1817">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="daa0d-1817">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="daa0d-1818">Recurso</span><span class="sxs-lookup"><span data-stu-id="daa0d-1818">Resource</span></span>

* <span data-ttu-id="daa0d-1819">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1819">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="daa0d-1820">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1820">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="daa0d-1821">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1821">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="daa0d-1822">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1822">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="daa0d-1823">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1823">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="daa0d-1824">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1824">Add docs for az lock update.</span></span> <span data-ttu-id="daa0d-1825">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1825">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="daa0d-1826">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1826">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="daa0d-1827">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1827">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="daa0d-1828">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1828">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="daa0d-1829">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1829">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="daa0d-1830">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1830">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="daa0d-1831">Função</span><span class="sxs-lookup"><span data-stu-id="daa0d-1831">Role</span></span>

* <span data-ttu-id="daa0d-1832">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1832">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="daa0d-1833">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1833">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="daa0d-1834">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1834">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="daa0d-1835">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="daa0d-1835">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="daa0d-1836">SQL</span><span class="sxs-lookup"><span data-stu-id="daa0d-1836">SQL</span></span>

* <span data-ttu-id="daa0d-1837">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="daa0d-1837">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="daa0d-1838">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1838">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="daa0d-1839">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1839">Storage</span></span>

* <span data-ttu-id="daa0d-1840">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1840">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="daa0d-1841">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="daa0d-1841">Add support for incremental blob copy</span></span>
* <span data-ttu-id="daa0d-1842">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="daa0d-1842">Add support for large block blob upload</span></span>
* <span data-ttu-id="daa0d-1843">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="daa0d-1843">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-1844">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-1844">VM</span></span>

* <span data-ttu-id="daa0d-1845">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="daa0d-1845">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="daa0d-1846">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="daa0d-1846">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="daa0d-1847">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="daa0d-1847">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="daa0d-1848">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="daa0d-1848">az vm/vmss disk</span></span>
  3. <span data-ttu-id="daa0d-1849">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="daa0d-1849">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="daa0d-1850">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="daa0d-1850">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="daa0d-1851">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1851">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="daa0d-1852">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="daa0d-1852">April 3, 2017</span></span>

<span data-ttu-id="daa0d-1853">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="daa0d-1853">Version 2.0.2</span></span>

<span data-ttu-id="daa0d-1854">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="daa0d-1854">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="daa0d-1855">Núcleo</span><span class="sxs-lookup"><span data-stu-id="daa0d-1855">Core</span></span>

* <span data-ttu-id="daa0d-1856">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="daa0d-1856">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="daa0d-1857">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1857">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="daa0d-1858">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1858">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="daa0d-1859">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1859">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="daa0d-1860">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1860">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="daa0d-1861">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1861">Add prompting for missing template parameters.</span></span> <span data-ttu-id="daa0d-1862">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1862">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="daa0d-1863">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="daa0d-1863">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="daa0d-1864">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="daa0d-1864">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="daa0d-1865">ACS</span><span class="sxs-lookup"><span data-stu-id="daa0d-1865">ACS</span></span>

* <span data-ttu-id="daa0d-1866">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1866">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="daa0d-1867">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1867">Add support for ssh key password prompting.</span></span> <span data-ttu-id="daa0d-1868">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1868">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="daa0d-1869">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1869">Add support for windows clusters.</span></span> <span data-ttu-id="daa0d-1870">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1870">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="daa0d-1871">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="daa0d-1871">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="daa0d-1872">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1872">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="daa0d-1873">AppService</span><span class="sxs-lookup"><span data-stu-id="daa0d-1873">AppService</span></span>

* <span data-ttu-id="daa0d-1874">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1874">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="daa0d-1875">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1875">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="daa0d-1876">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1876">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="daa0d-1877">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1877">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="daa0d-1878">DataLake</span><span class="sxs-lookup"><span data-stu-id="daa0d-1878">DataLake</span></span>

* <span data-ttu-id="daa0d-1879">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="daa0d-1879">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="daa0d-1880">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="daa0d-1880">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="daa0d-1881">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="daa0d-1881">DocuemntDB</span></span>

* <span data-ttu-id="daa0d-1882">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1882">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="daa0d-1883">VM</span><span class="sxs-lookup"><span data-stu-id="daa0d-1883">VM</span></span>

* <span data-ttu-id="daa0d-1884">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1884">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="daa0d-1885">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1885">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="daa0d-1886">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1886">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="daa0d-1887">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1887">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="daa0d-1888">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1888">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="daa0d-1889">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1889">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="daa0d-1890">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="daa0d-1890">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="daa0d-1891">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="daa0d-1891">February 27, 2017</span></span>

<span data-ttu-id="daa0d-1892">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="daa0d-1892">Version 2.0.0</span></span>

<span data-ttu-id="daa0d-1893">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="daa0d-1893">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="daa0d-1894">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1894">Container Service (acs)</span></span>
- <span data-ttu-id="daa0d-1895">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1895">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="daa0d-1896">Rede</span><span class="sxs-lookup"><span data-stu-id="daa0d-1896">Networking</span></span>
- <span data-ttu-id="daa0d-1897">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="daa0d-1897">Storage</span></span>

<span data-ttu-id="daa0d-1898">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1898">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="daa0d-1899">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="daa0d-1899">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="daa0d-1900">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="daa0d-1900">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="daa0d-1901">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="daa0d-1901">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="daa0d-1902">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1902">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="daa0d-1903">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="daa0d-1903">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="daa0d-1904">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1904">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="daa0d-1905">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="daa0d-1905">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="daa0d-1906">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="daa0d-1906">Provide feedback from the command line with the `az feedback` command</span></span>

