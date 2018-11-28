---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/20/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 36b57d52a5851275fd317240e5c2c95171a99e7e
ms.sourcegitcommit: 22b73d56602c1c4e647ed2c5af3d596a2f6a7ed5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2018
ms.locfileid: "52267323"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="d1cf6-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="d1cf6-103">Azure CLI release notes</span></span>
## <a name="november-20-2018"></a><span data-ttu-id="d1cf6-104">20 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-104">November 20, 2018</span></span>

<span data-ttu-id="d1cf6-105">Versão 2.0.51</span><span class="sxs-lookup"><span data-stu-id="d1cf6-105">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="d1cf6-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-106">Core</span></span>
* <span data-ttu-id="d1cf6-107">Logon do MSI alterado para não reutilizar o nome da assinatura na identidade</span><span class="sxs-lookup"><span data-stu-id="d1cf6-107">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="d1cf6-108">ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-108">ACR</span></span>
* <span data-ttu-id="d1cf6-109">Token de contexto adicionado à etapa da tarefa</span><span class="sxs-lookup"><span data-stu-id="d1cf6-109">Added context token to task step</span></span>
* <span data-ttu-id="d1cf6-110">Suporte adicionado para definir segredos na execução do acr para espelhar a tarefa do acr</span><span class="sxs-lookup"><span data-stu-id="d1cf6-110">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="d1cf6-111">Suporte aprimorado para `--top` e `--orderby` para os comandos `show-tags` e `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-111">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-112">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-112">Appservice</span></span>
* <span data-ttu-id="d1cf6-113">Tempo limite padrão para a implantação do zip alterado para sondar o status aumentado para 5 minutos, também adicionando uma propriedade de tempo limite para personalizar esse valor</span><span class="sxs-lookup"><span data-stu-id="d1cf6-113">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="d1cf6-114">Padrão `node_version` atualizado.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-114">Updated the default `node_version`.</span></span> <span data-ttu-id="d1cf6-115">Redefinir a ação de troca de slots durante uma troca de duas fases preserva todas as configurações do aplicativo e cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-115">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="d1cf6-116">Verificação da SKU no lado do cliente removida para o Linux criar o plano do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-116">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="d1cf6-117">Erro corrigido ao tentar obter o status de implantação do zip</span><span class="sxs-lookup"><span data-stu-id="d1cf6-117">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="d1cf6-118">Iot Central</span><span class="sxs-lookup"><span data-stu-id="d1cf6-118">IotCentral</span></span>
* <span data-ttu-id="d1cf6-119">Verificação de disponibilidade do subdomínio adicionada ao criar um aplicativo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="d1cf6-119">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="d1cf6-120">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d1cf6-120">KeyVault</span></span>
* <span data-ttu-id="d1cf6-121">Bug corrigido onde os erros podem ter sido ignorados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-121">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-122">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-122">Network</span></span>
* <span data-ttu-id="d1cf6-123">Subcomandos `root-cert` adicionados a `application-gateway` para lidar com os certificados de raiz confiável</span><span class="sxs-lookup"><span data-stu-id="d1cf6-123">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="d1cf6-124">Opções `--min-capacity` e `--custom-error-pages` adicionadas a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-124">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="d1cf6-125">`--zones` adicionado para suporte da zona de disponibilidade a `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-125">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="d1cf6-126">Argumentos `--file-upload-limit`, `--max-request-body-size` e `--request-body-check` a `application-gateway waf-config set` adicionados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-126">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="d1cf6-127">Rdbms</span><span class="sxs-lookup"><span data-stu-id="d1cf6-127">Rdbms</span></span>
* <span data-ttu-id="d1cf6-128">Comandos vnet do mariadb adicionados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-128">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="d1cf6-129">Rbac</span><span class="sxs-lookup"><span data-stu-id="d1cf6-129">Rbac</span></span>
* <span data-ttu-id="d1cf6-130">Um problema corrigido ao tentar atualizar credenciais inalteradas em `ad app update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-130">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="d1cf6-131">Avisos de saída adicionados para comunicar alterações de falha em um futuro próximo para `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-131">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="d1cf6-132">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-132">Storage</span></span>
* <span data-ttu-id="d1cf6-133">Melhor manipulação de casos incomuns para os comandos da cópia de armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-133">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="d1cf6-134">Corrigido o problema com `storage blob copy start-batch` não usando credenciais de logon quando as contas de origem e destino são iguais</span><span class="sxs-lookup"><span data-stu-id="d1cf6-134">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="d1cf6-135">Bug corrigido com `storage [blob|file] url` onde `sas_token` não foi incorporado na URL</span><span class="sxs-lookup"><span data-stu-id="d1cf6-135">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="d1cf6-136">Aviso de alteração da falha adicionado a `[blob|container] list`: produzirá apenas os primeiros 5.000 resultados por padrão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-136">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-137">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-137">VM</span></span>
* <span data-ttu-id="d1cf6-138">Suporte adicionado a `[vm|vmss] create --storage-sku` para especificar a SKU da conta de armazenamento para o SO gerenciado e os discos de dados separadamente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-138">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="d1cf6-139">Parâmetros do nome da versão alterados de `sig image-version` para `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-139">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="d1cf6-140">Argumento `sig image-version` preterido `--image-version-name`, substituído por `--image-version`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-140">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="d1cf6-141">Suporte adicionado para usar o disco local do SO a `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-141">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="d1cf6-142">Adicionado o suporte ao `--no-wait` para `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-142">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="d1cf6-143">Adicionado o comando `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-143">Added `snapshot wait` command</span></span>
* <span data-ttu-id="d1cf6-144">Suporte adicionado para usar o nome da instância com `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-144">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="d1cf6-145">6 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-145">November 6, 2018</span></span>

<span data-ttu-id="d1cf6-146">Versão 2.0.50</span><span class="sxs-lookup"><span data-stu-id="d1cf6-146">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="d1cf6-147">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-147">Core</span></span>
* <span data-ttu-id="d1cf6-148">Foi adicionado suporte para o serviço principal sn + autenticação do emissor</span><span class="sxs-lookup"><span data-stu-id="d1cf6-148">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="d1cf6-149">ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-149">ACR</span></span>
* <span data-ttu-id="d1cf6-150">Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa</span><span class="sxs-lookup"><span data-stu-id="d1cf6-150">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="d1cf6-151">Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação</span><span class="sxs-lookup"><span data-stu-id="d1cf6-151">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-152">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-152">ACS</span></span>
* <span data-ttu-id="d1cf6-153">[ALTERAÇÃO SIGNIFICATIVA] `enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-153">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="d1cf6-154">Supervisor</span><span class="sxs-lookup"><span data-stu-id="d1cf6-154">Advisor</span></span>
* <span data-ttu-id="d1cf6-155">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="d1cf6-155">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="d1cf6-156">AMS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-156">AMS</span></span>
* <span data-ttu-id="d1cf6-157">Novos grupos de comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-157">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="d1cf6-158">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-158">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="d1cf6-159">Adicionados parâmetros de criptografia com suporte para `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-159">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="d1cf6-160">O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido</span><span class="sxs-lookup"><span data-stu-id="d1cf6-160">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="d1cf6-161">Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-161">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="d1cf6-162">Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-162">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="d1cf6-163">Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-163">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="d1cf6-164">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming locator` foi substituído por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-164">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="d1cf6-165">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--content-keys` de `ams streaming locator` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-165">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="d1cf6-166">[ALTERAÇÃO SIGNIFICATIVA] `--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-166">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="d1cf6-167">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming policy` foi substituído por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-167">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="d1cf6-168">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-168">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="d1cf6-169">Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="d1cf6-169">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="d1cf6-170">Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-170">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="d1cf6-171">[ALTERAÇÃO SIGNIFICATIVA] `--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-171">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="d1cf6-172">Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-172">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="d1cf6-173">Um ativo sem rótulo pode ser enviado assim: 'assetName='</span><span class="sxs-lookup"><span data-stu-id="d1cf6-173">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-174">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-174">AppService</span></span>
* <span data-ttu-id="d1cf6-175">Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido</span><span class="sxs-lookup"><span data-stu-id="d1cf6-175">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="d1cf6-176">Configurar</span><span class="sxs-lookup"><span data-stu-id="d1cf6-176">Configure</span></span>
* <span data-ttu-id="d1cf6-177">O YAML foi adicionado às opções de formato de saída</span><span class="sxs-lookup"><span data-stu-id="d1cf6-177">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="d1cf6-178">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-178">Container</span></span>
* <span data-ttu-id="d1cf6-179">Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml</span><span class="sxs-lookup"><span data-stu-id="d1cf6-179">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="d1cf6-180">EventHub</span><span class="sxs-lookup"><span data-stu-id="d1cf6-180">EventHub</span></span>
* <span data-ttu-id="d1cf6-181">O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-181">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="d1cf6-182">Interativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-182">Interactive</span></span>
* <span data-ttu-id="d1cf6-183">O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-183">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="d1cf6-184">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-184">Monitor</span></span>
* <span data-ttu-id="d1cf6-185">Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) para `--condition` em `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-185">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-186">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-186">Network</span></span>
* <span data-ttu-id="d1cf6-187">Os nomes de comandos `network interface-endpoint` foram preteridos em benefício de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-187">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="d1cf6-188">Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID</span><span class="sxs-lookup"><span data-stu-id="d1cf6-188">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="d1cf6-189">Foi corrigido um problema onde `--ip-tags` não funcionava corretamente com `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-189">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="d1cf6-190">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1cf6-190">Profile</span></span>
* <span data-ttu-id="d1cf6-191">`--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-191">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="d1cf6-192">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-192">RDBMS</span></span>
* <span data-ttu-id="d1cf6-193">Adicionados comandos da réplica mysql</span><span class="sxs-lookup"><span data-stu-id="d1cf6-193">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="d1cf6-194">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-194">Resource</span></span>
* <span data-ttu-id="d1cf6-195">Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-195">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="d1cf6-196">Função</span><span class="sxs-lookup"><span data-stu-id="d1cf6-196">Role</span></span>
* <span data-ttu-id="d1cf6-197">Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais</span><span class="sxs-lookup"><span data-stu-id="d1cf6-197">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="d1cf6-198">`ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="d1cf6-198">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="d1cf6-199">Suporte adicionado para conceder permissões a aplicativos do AAD</span><span class="sxs-lookup"><span data-stu-id="d1cf6-199">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-200">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-200">Storage</span></span>
* <span data-ttu-id="d1cf6-201">Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-201">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-202">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-202">VM</span></span>
* <span data-ttu-id="d1cf6-203">O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem</span><span class="sxs-lookup"><span data-stu-id="d1cf6-203">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="d1cf6-204">O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido</span><span class="sxs-lookup"><span data-stu-id="d1cf6-204">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="d1cf6-205">O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-205">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="d1cf6-206">`vm secret format` foi alterado para exigir a saída json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-206">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="d1cf6-207">Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido</span><span class="sxs-lookup"><span data-stu-id="d1cf6-207">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="d1cf6-208">Validação de argumento aprimorado para `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-208">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="d1cf6-209">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-209">October 23, 2018</span></span>

<span data-ttu-id="d1cf6-210">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="d1cf6-210">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="d1cf6-211">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-211">Core</span></span>
* <span data-ttu-id="d1cf6-212">Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-212">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="d1cf6-213">Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-213">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="d1cf6-214">ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-214">ACR</span></span>
* <span data-ttu-id="d1cf6-215">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="d1cf6-215">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="d1cf6-216">CDN</span><span class="sxs-lookup"><span data-stu-id="d1cf6-216">CDN</span></span>
* <span data-ttu-id="d1cf6-217">[ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="d1cf6-217">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="d1cf6-218">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="d1cf6-218">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="d1cf6-219">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-219">Container</span></span>
* <span data-ttu-id="d1cf6-220">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="d1cf6-220">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="d1cf6-221">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="d1cf6-221">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="d1cf6-222">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-222">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="d1cf6-223">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="d1cf6-223">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="d1cf6-224">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="d1cf6-224">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="d1cf6-225">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="d1cf6-225">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="d1cf6-226">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-226">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d1cf6-227">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d1cf6-227">CosmosDB</span></span>
* <span data-ttu-id="d1cf6-228">Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-228">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="d1cf6-229">Interativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-229">Interactive</span></span>
* <span data-ttu-id="d1cf6-230">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="d1cf6-230">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="d1cf6-231">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="d1cf6-231">IoT Central</span></span>
* <span data-ttu-id="d1cf6-232">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="d1cf6-232">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="d1cf6-233">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="d1cf6-233">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="d1cf6-234">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-234">Monitor</span></span>
* <span data-ttu-id="d1cf6-235">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-235">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="d1cf6-236">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="d1cf6-236">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="d1cf6-237">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-237">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="d1cf6-238">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="d1cf6-238">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="d1cf6-239">Adicionado `--namespace` como alias para a opção preterida `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-239">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="d1cf6-240">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="d1cf6-240">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="d1cf6-241">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-241">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="d1cf6-242">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-242">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="d1cf6-243">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="d1cf6-243">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="d1cf6-244">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-244">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-245">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-245">Network</span></span>
* <span data-ttu-id="d1cf6-246">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="d1cf6-246">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="d1cf6-247">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="d1cf6-247">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="d1cf6-248">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d1cf6-248">ServiceBus</span></span>
* <span data-ttu-id="d1cf6-249">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="d1cf6-249">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="d1cf6-250">SQL</span><span class="sxs-lookup"><span data-stu-id="d1cf6-250">SQL</span></span>
* <span data-ttu-id="d1cf6-251">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="d1cf6-251">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-252">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-252">Storage</span></span>
* <span data-ttu-id="d1cf6-253">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="d1cf6-253">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="d1cf6-254">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="d1cf6-254">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-255">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-255">VM</span></span>
* <span data-ttu-id="d1cf6-256">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-256">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="d1cf6-257">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-257">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="d1cf6-258">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-258">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="d1cf6-259">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-259">October 16, 2018</span></span>

<span data-ttu-id="d1cf6-260">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="d1cf6-260">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-261">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-261">VM</span></span>
* <span data-ttu-id="d1cf6-262">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="d1cf6-262">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="d1cf6-263">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-263">October 9, 2018</span></span>

<span data-ttu-id="d1cf6-264">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="d1cf6-264">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="d1cf6-265">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-265">Core</span></span>
* <span data-ttu-id="d1cf6-266">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="d1cf6-266">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="d1cf6-267">ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-267">ACR</span></span>
* <span data-ttu-id="d1cf6-268">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="d1cf6-268">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-269">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-269">ACS</span></span>
* <span data-ttu-id="d1cf6-270">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="d1cf6-270">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="d1cf6-271">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="d1cf6-271">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="d1cf6-272">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-272">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="d1cf6-273">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-273">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="d1cf6-274">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-274">Container</span></span>
* <span data-ttu-id="d1cf6-275">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um tempo de execução específico</span><span class="sxs-lookup"><span data-stu-id="d1cf6-275">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="d1cf6-276">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="d1cf6-276">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="d1cf6-277">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-277">Event Hub</span></span>
* <span data-ttu-id="d1cf6-278">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-278">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="d1cf6-279">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="d1cf6-279">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="d1cf6-280">Extensões</span><span class="sxs-lookup"><span data-stu-id="d1cf6-280">Extensions</span></span>
* <span data-ttu-id="d1cf6-281">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="d1cf6-281">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="d1cf6-282">HDInsight</span><span class="sxs-lookup"><span data-stu-id="d1cf6-282">HDInsight</span></span>
* <span data-ttu-id="d1cf6-283">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="d1cf6-283">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="d1cf6-284">IoT</span><span class="sxs-lookup"><span data-stu-id="d1cf6-284">IoT</span></span>
* <span data-ttu-id="d1cf6-285">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="d1cf6-285">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="d1cf6-286">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d1cf6-286">KeyVault</span></span>
* <span data-ttu-id="d1cf6-287">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-287">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-288">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-288">Network</span></span>
* <span data-ttu-id="d1cf6-289">`network dns zone create` corrigido: o comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-289">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="d1cf6-290">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="d1cf6-290">See #6052</span></span>
* <span data-ttu-id="d1cf6-291">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-291">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="d1cf6-292">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="d1cf6-292">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="d1cf6-293">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-293">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="d1cf6-294">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-294">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="d1cf6-295">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-295">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="d1cf6-296">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-296">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="d1cf6-297">Função</span><span class="sxs-lookup"><span data-stu-id="d1cf6-297">Role</span></span>
* <span data-ttu-id="d1cf6-298">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-298">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="d1cf6-299">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-299">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="d1cf6-300">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-300">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="d1cf6-301">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="d1cf6-301">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="d1cf6-302">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="d1cf6-302">Service Bus</span></span>
* <span data-ttu-id="d1cf6-303">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="d1cf6-303">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-304">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-304">VM</span></span>
* <span data-ttu-id="d1cf6-305">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-305">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="d1cf6-306">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-306">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="d1cf6-307">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-307">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="d1cf6-308">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-308">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="d1cf6-309">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-309">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="d1cf6-310">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="d1cf6-310">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="d1cf6-311">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-311">September 21, 2018</span></span>

<span data-ttu-id="d1cf6-312">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="d1cf6-312">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="d1cf6-313">ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-313">ACR</span></span>
* <span data-ttu-id="d1cf6-314">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-314">Added ACR Task commands</span></span>
* <span data-ttu-id="d1cf6-315">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="d1cf6-315">Added quick run command</span></span>
* <span data-ttu-id="d1cf6-316">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-316">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="d1cf6-317">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-317">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="d1cf6-318">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-318">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="d1cf6-319">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="d1cf6-319">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-320">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-320">ACS</span></span>
* <span data-ttu-id="d1cf6-321">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-321">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="d1cf6-322">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="d1cf6-322">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-323">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-323">AppService</span></span>

* <span data-ttu-id="d1cf6-324">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-324">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="d1cf6-325">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="d1cf6-325">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="d1cf6-326">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="d1cf6-326">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="d1cf6-327">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-327">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="d1cf6-328">Lote</span><span class="sxs-lookup"><span data-stu-id="d1cf6-328">Batch</span></span>
* <span data-ttu-id="d1cf6-329">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="d1cf6-329">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="d1cf6-330">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-330">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="d1cf6-331">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-331">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="d1cf6-332">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="d1cf6-332">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="d1cf6-333">Lote AI</span><span class="sxs-lookup"><span data-stu-id="d1cf6-333">Batch AI</span></span> 
* <span data-ttu-id="d1cf6-334">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-334">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d1cf6-335">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-335">Cognitive Services</span></span>
* <span data-ttu-id="d1cf6-336">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-336">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="d1cf6-337">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-337">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="d1cf6-338">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-338">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="d1cf6-339">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-339">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="d1cf6-340">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-340">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="d1cf6-341">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-341">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="d1cf6-342">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-342">Container</span></span>
* <span data-ttu-id="d1cf6-343">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="d1cf6-343">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="d1cf6-344">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-344">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="d1cf6-345">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="d1cf6-345">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="d1cf6-346">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="d1cf6-346">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="d1cf6-347">DataLake</span><span class="sxs-lookup"><span data-stu-id="d1cf6-347">Datalake</span></span>
* <span data-ttu-id="d1cf6-348">Comandos adicionados para regras de rede virtual</span><span class="sxs-lookup"><span data-stu-id="d1cf6-348">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="d1cf6-349">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-349">Interactive Shell</span></span>
* <span data-ttu-id="d1cf6-350">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-350">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="d1cf6-351">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-351">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="d1cf6-352">IoT</span><span class="sxs-lookup"><span data-stu-id="d1cf6-352">IoT</span></span>
* <span data-ttu-id="d1cf6-353">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="d1cf6-353">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="d1cf6-354">Key Vault</span><span class="sxs-lookup"><span data-stu-id="d1cf6-354">Key Vault</span></span>
* <span data-ttu-id="d1cf6-355">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="d1cf6-355">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-356">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-356">Network</span></span>
* <span data-ttu-id="d1cf6-357">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="d1cf6-357">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="d1cf6-358">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="d1cf6-358">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="d1cf6-359">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="d1cf6-359">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="d1cf6-360">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="d1cf6-360">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="d1cf6-361">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-361">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="d1cf6-362">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-362">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="d1cf6-363">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-363">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="d1cf6-364">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-364">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="d1cf6-365">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-365">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="d1cf6-366">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-366">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="d1cf6-367">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-367">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="d1cf6-368">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-368">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="d1cf6-369">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-369">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="d1cf6-370">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-370">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="d1cf6-371">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-371">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="d1cf6-372">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="d1cf6-372">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="d1cf6-373">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-373">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="d1cf6-374">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="d1cf6-374">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="d1cf6-375">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-375">RDBMS</span></span>
* <span data-ttu-id="d1cf6-376">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="d1cf6-376">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="d1cf6-377">Reserva</span><span class="sxs-lookup"><span data-stu-id="d1cf6-377">Reservation</span></span>
* <span data-ttu-id="d1cf6-378">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-378">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="d1cf6-379">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="d1cf6-379">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="d1cf6-380">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-380">Manage App</span></span>
* <span data-ttu-id="d1cf6-381">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="d1cf6-381">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="d1cf6-382">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="d1cf6-382">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="d1cf6-383">Função</span><span class="sxs-lookup"><span data-stu-id="d1cf6-383">Role</span></span>
* <span data-ttu-id="d1cf6-384">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="d1cf6-384">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="d1cf6-385">SignalR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-385">SignalR</span></span>
* <span data-ttu-id="d1cf6-386">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-386">First release</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-387">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-387">Storage</span></span>
* <span data-ttu-id="d1cf6-388">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="d1cf6-388">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="d1cf6-389">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="d1cf6-389">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-390">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-390">VM</span></span>
* <span data-ttu-id="d1cf6-391">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-391">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="d1cf6-392">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-392">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="d1cf6-393">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-393">August 28, 2018</span></span>

<span data-ttu-id="d1cf6-394">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="d1cf6-394">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="d1cf6-395">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-395">Core</span></span>

* <span data-ttu-id="d1cf6-396">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="d1cf6-396">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="d1cf6-397">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="d1cf6-397">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="d1cf6-398">ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-398">ACR</span></span>

* <span data-ttu-id="d1cf6-399">Adicionada uma solução alternativa para operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-399">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="d1cf6-400">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-400">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-401">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-401">ACS</span></span>

* <span data-ttu-id="d1cf6-402">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-402">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="d1cf6-403">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="d1cf6-403">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-404">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-404">AppService</span></span>

* <span data-ttu-id="d1cf6-405">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="d1cf6-405">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="d1cf6-406">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-406">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="d1cf6-407">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-407">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="d1cf6-408">Backup</span><span class="sxs-lookup"><span data-stu-id="d1cf6-408">Backup</span></span>

* <span data-ttu-id="d1cf6-409">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-409">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="d1cf6-410">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="d1cf6-410">Bot Service</span></span>

* <span data-ttu-id="d1cf6-411">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="d1cf6-411">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d1cf6-412">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-412">Cognitive Services</span></span>

* <span data-ttu-id="d1cf6-413">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="d1cf6-413">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="d1cf6-414">IoT</span><span class="sxs-lookup"><span data-stu-id="d1cf6-414">IoT</span></span>

* <span data-ttu-id="d1cf6-415">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-415">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="d1cf6-416">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-416">Monitor</span></span>

* <span data-ttu-id="d1cf6-417">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="d1cf6-417">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="d1cf6-418">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-418">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-419">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-419">Network</span></span>

* <span data-ttu-id="d1cf6-420">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-420">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="d1cf6-421">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-421">Resource</span></span>

* <span data-ttu-id="d1cf6-422">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-422">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-423">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-423">Storage</span></span>

* <span data-ttu-id="d1cf6-424">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-424">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-425">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-425">VM</span></span>

* <span data-ttu-id="d1cf6-426">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-426">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="d1cf6-427">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-427">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="d1cf6-428">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-428">Auguest 14, 2018</span></span>

<span data-ttu-id="d1cf6-429">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="d1cf6-429">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="d1cf6-430">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-430">Core</span></span>

* <span data-ttu-id="d1cf6-431">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-431">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="d1cf6-432">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="d1cf6-432">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="d1cf6-433">Telemetria</span><span class="sxs-lookup"><span data-stu-id="d1cf6-433">Telemetry</span></span>

* <span data-ttu-id="d1cf6-434">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="d1cf6-434">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="d1cf6-435">ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-435">ACR</span></span>

* <span data-ttu-id="d1cf6-436">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-436">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="d1cf6-437">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-437">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-438">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-438">ACS</span></span>

* <span data-ttu-id="d1cf6-439">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="d1cf6-439">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="d1cf6-440">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-440">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="d1cf6-441">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="d1cf6-441">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="d1cf6-442">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="d1cf6-442">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="d1cf6-443">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="d1cf6-443">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="d1cf6-444">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-444">AppService</span></span>

* <span data-ttu-id="d1cf6-445">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-445">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="d1cf6-446">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="d1cf6-446">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="d1cf6-447">BatchAI</span><span class="sxs-lookup"><span data-stu-id="d1cf6-447">BatchAI</span></span>

* <span data-ttu-id="d1cf6-448">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-448">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="d1cf6-449">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-449">Container</span></span>

* <span data-ttu-id="d1cf6-450">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-450">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="d1cf6-451">IoT</span><span class="sxs-lookup"><span data-stu-id="d1cf6-451">IoT</span></span>

* <span data-ttu-id="d1cf6-452">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="d1cf6-452">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="d1cf6-453">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-453">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="d1cf6-454">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="d1cf6-454">Iot Central</span></span>

* <span data-ttu-id="d1cf6-455">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="d1cf6-455">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="d1cf6-456">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d1cf6-456">KeyVault</span></span>


* <span data-ttu-id="d1cf6-457">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-457">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="d1cf6-458">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-458">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="d1cf6-459">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-459">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="d1cf6-460">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="d1cf6-460">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="d1cf6-461">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="d1cf6-461">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="d1cf6-462">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-462">Relay</span></span>

* <span data-ttu-id="d1cf6-463">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="d1cf6-463">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="d1cf6-464">Sql</span><span class="sxs-lookup"><span data-stu-id="d1cf6-464">Sql</span></span>

* <span data-ttu-id="d1cf6-465">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-465">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-466">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-466">Storage</span></span>

* <span data-ttu-id="d1cf6-467">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="d1cf6-467">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="d1cf6-468">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-468">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="d1cf6-469">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="d1cf6-469">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="d1cf6-470">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-470">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="d1cf6-471">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-471">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-472">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-472">VM</span></span>

* <span data-ttu-id="d1cf6-473">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-473">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="d1cf6-474">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-474">July 31, 2018</span></span>

<span data-ttu-id="d1cf6-475">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="d1cf6-475">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="d1cf6-476">ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-476">ACR</span></span>

* <span data-ttu-id="d1cf6-477">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-477">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="d1cf6-478">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-478">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-479">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-479">ACS</span></span>

* <span data-ttu-id="d1cf6-480">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="d1cf6-480">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="d1cf6-481">Lote</span><span class="sxs-lookup"><span data-stu-id="d1cf6-481">Batch</span></span>

* <span data-ttu-id="d1cf6-482">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="d1cf6-482">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="d1cf6-483">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-483">Container</span></span>

* <span data-ttu-id="d1cf6-484">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="d1cf6-484">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-485">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-485">Network</span></span>

* <span data-ttu-id="d1cf6-486">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="d1cf6-486">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="d1cf6-487">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-487">Resource</span></span>

* <span data-ttu-id="d1cf6-488">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="d1cf6-488">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="d1cf6-489">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="d1cf6-489">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="d1cf6-490">Função</span><span class="sxs-lookup"><span data-stu-id="d1cf6-490">Role</span></span>

* <span data-ttu-id="d1cf6-491">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="d1cf6-491">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="d1cf6-492">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-492">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="d1cf6-493">Search</span><span class="sxs-lookup"><span data-stu-id="d1cf6-493">Search</span></span>

* <span data-ttu-id="d1cf6-494">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="d1cf6-494">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="d1cf6-495">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="d1cf6-495">Service Bus</span></span>

* <span data-ttu-id="d1cf6-496">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="d1cf6-496">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="d1cf6-497">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="d1cf6-497">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="d1cf6-498">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-498">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="d1cf6-499">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-499">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-500">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-500">Storage</span></span>

* <span data-ttu-id="d1cf6-501">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-501">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="d1cf6-502">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-502">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-503">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-503">VM</span></span>

* <span data-ttu-id="d1cf6-504">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="d1cf6-504">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="d1cf6-505">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-505">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="d1cf6-506">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-506">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="d1cf6-507">[ALTERAÇÃO SIGNIFICATIVA] `[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="d1cf6-507">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="d1cf6-508">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-508">July 18, 2018</span></span>

<span data-ttu-id="d1cf6-509">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="d1cf6-509">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="d1cf6-510">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-510">Core</span></span>

* <span data-ttu-id="d1cf6-511">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="d1cf6-511">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="d1cf6-512">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="d1cf6-512">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="d1cf6-513">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-513">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="d1cf6-514">ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-514">ACR</span></span>

* <span data-ttu-id="d1cf6-515">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="d1cf6-515">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="d1cf6-516">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-516">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="d1cf6-517">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-517">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="d1cf6-518">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="d1cf6-518">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-519">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-519">ACS</span></span>

* <span data-ttu-id="d1cf6-520">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="d1cf6-520">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-521">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-521">AppService</span></span>

* <span data-ttu-id="d1cf6-522">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="d1cf6-522">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="d1cf6-523">Lote</span><span class="sxs-lookup"><span data-stu-id="d1cf6-523">Batch</span></span>

* <span data-ttu-id="d1cf6-524">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="d1cf6-524">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="d1cf6-525">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-525">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="d1cf6-526">Lote AI</span><span class="sxs-lookup"><span data-stu-id="d1cf6-526">Batch AI</span></span>

* <span data-ttu-id="d1cf6-527">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-527">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="d1cf6-528">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-528">Container</span></span>

* <span data-ttu-id="d1cf6-529">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="d1cf6-529">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="d1cf6-530">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="d1cf6-530">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-531">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-531">Network</span></span>

* <span data-ttu-id="d1cf6-532">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-532">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="d1cf6-533">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-533">Added `network nic wait`</span></span>
* <span data-ttu-id="d1cf6-534">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-534">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="d1cf6-535">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-535">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="d1cf6-536">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-536">Resource</span></span>

* <span data-ttu-id="d1cf6-537">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-537">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="d1cf6-538">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-538">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="d1cf6-539">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-539">Added `deployment wait` command</span></span>
* <span data-ttu-id="d1cf6-540">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="d1cf6-540">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="d1cf6-541">SQL</span><span class="sxs-lookup"><span data-stu-id="d1cf6-541">SQL</span></span>

* <span data-ttu-id="d1cf6-542">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-542">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="d1cf6-543">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-543">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="d1cf6-544">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-544">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-545">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-545">Storage</span></span>

* <span data-ttu-id="d1cf6-546">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="d1cf6-546">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-547">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-547">VM</span></span>

* <span data-ttu-id="d1cf6-548">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-548">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="d1cf6-549">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-549">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="d1cf6-550">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-550">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="d1cf6-551">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-551">July 3, 2018</span></span>

<span data-ttu-id="d1cf6-552">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="d1cf6-552">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="d1cf6-553">AKS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-553">AKS</span></span>

* <span data-ttu-id="d1cf6-554">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="d1cf6-554">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="d1cf6-555">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-555">July 3, 2018</span></span>

<span data-ttu-id="d1cf6-556">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="d1cf6-556">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="d1cf6-557">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-557">Core</span></span>

* <span data-ttu-id="d1cf6-558">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-558">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="d1cf6-559">ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-559">ACR</span></span>

* <span data-ttu-id="d1cf6-560">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-560">Added polling build status</span></span>
* <span data-ttu-id="d1cf6-561">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-561">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="d1cf6-562">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-562">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-563">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-563">ACS</span></span>

* <span data-ttu-id="d1cf6-564">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-564">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="d1cf6-565">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="d1cf6-565">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="d1cf6-566">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-566">Updated options for `aks browse` command.</span></span> <span data-ttu-id="d1cf6-567">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-567">Added `--listen-port` support</span></span>
* <span data-ttu-id="d1cf6-568">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-568">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="d1cf6-569">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="d1cf6-569">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="d1cf6-570">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-570">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-571">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-571">AppService</span></span>

* <span data-ttu-id="d1cf6-572">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-572">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="d1cf6-573">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="d1cf6-573">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="d1cf6-574">Backup</span><span class="sxs-lookup"><span data-stu-id="d1cf6-574">Backup</span></span>

* <span data-ttu-id="d1cf6-575">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="d1cf6-575">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="d1cf6-576">BatchAI</span><span class="sxs-lookup"><span data-stu-id="d1cf6-576">BatchAI</span></span>

* <span data-ttu-id="d1cf6-577">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-577">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="d1cf6-578">Nuvem</span><span class="sxs-lookup"><span data-stu-id="d1cf6-578">Cloud</span></span>

* <span data-ttu-id="d1cf6-579">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="d1cf6-579">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="d1cf6-580">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-580">Container</span></span>

* <span data-ttu-id="d1cf6-581">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="d1cf6-581">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="d1cf6-582">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="d1cf6-582">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="d1cf6-583">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="d1cf6-583">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="d1cf6-584">Extensão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-584">Extension</span></span>

* <span data-ttu-id="d1cf6-585">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="d1cf6-585">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-586">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-586">Network</span></span>

* <span data-ttu-id="d1cf6-587">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-587">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="d1cf6-588">Rdbms</span><span class="sxs-lookup"><span data-stu-id="d1cf6-588">Rdbms</span></span>

* <span data-ttu-id="d1cf6-589">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-589">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="d1cf6-590">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-590">Resource</span></span>

* <span data-ttu-id="d1cf6-591">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-591">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-592">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-592">VM</span></span>

* <span data-ttu-id="d1cf6-593">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="d1cf6-593">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="d1cf6-594">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-594">June 25, 2018</span></span>

<span data-ttu-id="d1cf6-595">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="d1cf6-595">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="d1cf6-596">CLI</span><span class="sxs-lookup"><span data-stu-id="d1cf6-596">CLI</span></span>

* <span data-ttu-id="d1cf6-597">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-597">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="d1cf6-598">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-598">June 19, 2018</span></span>

<span data-ttu-id="d1cf6-599">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="d1cf6-599">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="d1cf6-600">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-600">Core</span></span>

* <span data-ttu-id="d1cf6-601">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-601">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="d1cf6-602">ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-602">ACR</span></span>

* <span data-ttu-id="d1cf6-603">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="d1cf6-603">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="d1cf6-604">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-604">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-605">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-605">ACS</span></span>

* <span data-ttu-id="d1cf6-606">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-606">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="d1cf6-607">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-607">Added `--update` support</span></span>
* <span data-ttu-id="d1cf6-608">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-608">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="d1cf6-609">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-609">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="d1cf6-610">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="d1cf6-610">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="d1cf6-611">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-611">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="d1cf6-612">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-612">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="d1cf6-613">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-613">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-614">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-614">AppService</span></span>

* <span data-ttu-id="d1cf6-615">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="d1cf6-615">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="d1cf6-616">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-616">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="d1cf6-617">Lote</span><span class="sxs-lookup"><span data-stu-id="d1cf6-617">Batch</span></span>

* <span data-ttu-id="d1cf6-618">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="d1cf6-618">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="d1cf6-619">Lote AI</span><span class="sxs-lookup"><span data-stu-id="d1cf6-619">Batch AI</span></span>

* <span data-ttu-id="d1cf6-620">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-620">Added support for workspaces.</span></span> <span data-ttu-id="d1cf6-621">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-621">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="d1cf6-622">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-622">Added support for experiments.</span></span> <span data-ttu-id="d1cf6-623">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-623">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="d1cf6-624">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="d1cf6-624">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="d1cf6-625">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-625">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="d1cf6-626">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-626">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="d1cf6-627">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-627">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="d1cf6-628">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="d1cf6-628">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="d1cf6-629">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="d1cf6-629">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="d1cf6-630">[ALTERAÇÃO SIGNIFICATIVA] `--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-630">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="d1cf6-631">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-631">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="d1cf6-632">[ALTERAÇÃO SIGNIFICATIVA] `--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-632">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="d1cf6-633">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-633">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="d1cf6-634">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-634">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="d1cf6-635">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-635">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="d1cf6-636">[ALTERAÇÃO SIGNIFICATIVA] `--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-636">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="d1cf6-637">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-637">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="d1cf6-638">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="d1cf6-638">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="d1cf6-639">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="d1cf6-639">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="d1cf6-640">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="d1cf6-640">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="d1cf6-641">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="d1cf6-641">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="d1cf6-642">Mapas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-642">Maps</span></span>

* <span data-ttu-id="d1cf6-643">[ALTERAÇÃO SIGNIFICATIVA] `maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-643">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-644">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-644">Network</span></span>

* <span data-ttu-id="d1cf6-645">Foi adicionado suporte a `https` para `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-645">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="d1cf6-646">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-646">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="d1cf6-647">#6502</span><span class="sxs-lookup"><span data-stu-id="d1cf6-647">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="d1cf6-648">Reservas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-648">Reservations</span></span>

* <span data-ttu-id="d1cf6-649">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-649">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="d1cf6-650">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-650">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="d1cf6-651">[ALTERAÇÃO SIGNIFICATIVA] `kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-651">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="d1cf6-652">[ALTERAÇÃO SIGNIFICATIVA] `capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-652">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="d1cf6-653">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-653">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="d1cf6-654">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-654">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="d1cf6-655">Função</span><span class="sxs-lookup"><span data-stu-id="d1cf6-655">Role</span></span>

* <span data-ttu-id="d1cf6-656">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-656">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="d1cf6-657">SQL</span><span class="sxs-lookup"><span data-stu-id="d1cf6-657">SQL</span></span>

* <span data-ttu-id="d1cf6-658">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="d1cf6-658">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-659">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-659">Storage</span></span>

* <span data-ttu-id="d1cf6-660">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="d1cf6-660">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-661">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-661">VM</span></span>

* <span data-ttu-id="d1cf6-662">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-662">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="d1cf6-663">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-663">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="d1cf6-664">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="d1cf6-664">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="d1cf6-665">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-665">June 13, 2018</span></span>

<span data-ttu-id="d1cf6-666">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="d1cf6-666">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="d1cf6-667">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-667">Core</span></span>

* <span data-ttu-id="d1cf6-668">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="d1cf6-668">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="d1cf6-669">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-669">June 13, 2018</span></span>

<span data-ttu-id="d1cf6-670">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="d1cf6-670">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="d1cf6-671">AKS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-671">AKS</span></span>

* <span data-ttu-id="d1cf6-672">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-672">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="d1cf6-673">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="d1cf6-673">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="d1cf6-674">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-674">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="d1cf6-675">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-675">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="d1cf6-676">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-676">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-677">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-677">AppService</span></span>

* <span data-ttu-id="d1cf6-678">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="d1cf6-678">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="d1cf6-679">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-679">June 5, 2018</span></span>

<span data-ttu-id="d1cf6-680">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="d1cf6-680">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="d1cf6-681">Interativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-681">Interactive</span></span>

* <span data-ttu-id="d1cf6-682">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-682">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="d1cf6-683">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-683">June 5, 2018</span></span>

<span data-ttu-id="d1cf6-684">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="d1cf6-684">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="d1cf6-685">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-685">Core</span></span>

* <span data-ttu-id="d1cf6-686">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-686">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="d1cf6-687">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="d1cf6-687">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="d1cf6-688">ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-688">ACR</span></span>

* <span data-ttu-id="d1cf6-689">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="d1cf6-689">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="d1cf6-690">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-690">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="d1cf6-691">AKS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-691">AKS</span></span>

* <span data-ttu-id="d1cf6-692">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="d1cf6-692">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="d1cf6-693">Lote</span><span class="sxs-lookup"><span data-stu-id="d1cf6-693">Batch</span></span>

* <span data-ttu-id="d1cf6-694">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="d1cf6-694">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="d1cf6-695">IOT</span><span class="sxs-lookup"><span data-stu-id="d1cf6-695">IOT</span></span>

* <span data-ttu-id="d1cf6-696">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="d1cf6-696">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-697">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-697">Network</span></span>

* <span data-ttu-id="d1cf6-698">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-698">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="d1cf6-699">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="d1cf6-699">Policy Insights</span></span>

* <span data-ttu-id="d1cf6-700">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="d1cf6-700">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="d1cf6-701">ARM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-701">ARM</span></span>

* <span data-ttu-id="d1cf6-702">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-702">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="d1cf6-703">SQL</span><span class="sxs-lookup"><span data-stu-id="d1cf6-703">SQL</span></span>

* <span data-ttu-id="d1cf6-704">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-704">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="d1cf6-705">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-705">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="d1cf6-706">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-706">Storage</span></span>

* <span data-ttu-id="d1cf6-707">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-707">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-708">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-708">VM</span></span>

* <span data-ttu-id="d1cf6-709">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-709">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="d1cf6-710">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-710">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="d1cf6-711">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-711">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="d1cf6-712">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-712">May 22, 2018</span></span>

<span data-ttu-id="d1cf6-713">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="d1cf6-713">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="d1cf6-714">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-714">Core</span></span>

* <span data-ttu-id="d1cf6-715">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-715">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-716">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-716">ACS</span></span>

* <span data-ttu-id="d1cf6-717">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-717">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="d1cf6-718">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="d1cf6-718">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-719">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-719">AppService</span></span>

* <span data-ttu-id="d1cf6-720">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="d1cf6-720">Improved generic update commands</span></span>
* <span data-ttu-id="d1cf6-721">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-721">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="d1cf6-722">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-722">Container</span></span>

* <span data-ttu-id="d1cf6-723">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="d1cf6-723">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="d1cf6-724">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-724">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="d1cf6-725">Extensão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-725">Extension</span></span>

* <span data-ttu-id="d1cf6-726">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="d1cf6-726">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="d1cf6-727">Interativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-727">Interactive</span></span>

* <span data-ttu-id="d1cf6-728">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="d1cf6-728">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="d1cf6-729">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="d1cf6-729">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="d1cf6-730">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d1cf6-730">KeyVault</span></span>

* <span data-ttu-id="d1cf6-731">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="d1cf6-731">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-732">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-732">Network</span></span>

* <span data-ttu-id="d1cf6-733">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-733">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="d1cf6-734">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-734">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="d1cf6-735">SQL</span><span class="sxs-lookup"><span data-stu-id="d1cf6-735">SQL</span></span>

* <span data-ttu-id="d1cf6-736">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-736">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="d1cf6-737">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-737">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="d1cf6-738">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-738">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="d1cf6-739">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1cf6-739">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="d1cf6-740">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-740">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="d1cf6-741">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-741">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="d1cf6-742">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-742">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="d1cf6-743">`edition`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-743">`edition`.</span></span> <span data-ttu-id="d1cf6-744">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-744">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="d1cf6-745">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-745">`elasticPoolName`.</span></span> <span data-ttu-id="d1cf6-746">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-746">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="d1cf6-747">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-747">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="d1cf6-748">`edition`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-748">`edition`.</span></span> <span data-ttu-id="d1cf6-749">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-749">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="d1cf6-750">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-750">`dtu`.</span></span> <span data-ttu-id="d1cf6-751">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-751">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="d1cf6-752">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-752">`databaseDtuMin`.</span></span> <span data-ttu-id="d1cf6-753">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-753">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="d1cf6-754">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-754">`databaseDtuMax`.</span></span> <span data-ttu-id="d1cf6-755">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-755">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="d1cf6-756">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-756">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="d1cf6-757">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-757">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-758">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-758">Storage</span></span>

* <span data-ttu-id="d1cf6-759">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-759">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="d1cf6-760">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="d1cf6-760">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-761">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-761">VM</span></span>

* <span data-ttu-id="d1cf6-762">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-762">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="d1cf6-763">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-763">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="d1cf6-764">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-764">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="d1cf6-765">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="d1cf6-765">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="d1cf6-766">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-766">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="d1cf6-767">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-767">May 7, 2018</span></span>

<span data-ttu-id="d1cf6-768">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="d1cf6-768">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="d1cf6-769">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-769">Core</span></span>

* <span data-ttu-id="d1cf6-770">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-770">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="d1cf6-771">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="d1cf6-771">Added limited support for positional arguments</span></span>
* <span data-ttu-id="d1cf6-772">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-772">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="d1cf6-773">#5591</span><span class="sxs-lookup"><span data-stu-id="d1cf6-773">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="d1cf6-774">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-774">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="d1cf6-775">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="d1cf6-775">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="d1cf6-776">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-776">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="d1cf6-777">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-777">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="d1cf6-778">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="d1cf6-778">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="d1cf6-779">ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-779">ACR</span></span>

* <span data-ttu-id="d1cf6-780">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-780">Added ACR Build commands</span></span>
* <span data-ttu-id="d1cf6-781">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="d1cf6-781">Improved resource not found error messages</span></span>
* <span data-ttu-id="d1cf6-782">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="d1cf6-782">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="d1cf6-783">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="d1cf6-783">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="d1cf6-784">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-784">Improved repository commands error messages</span></span>
* <span data-ttu-id="d1cf6-785">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-785">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-786">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-786">ACS</span></span>

* <span data-ttu-id="d1cf6-787">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="d1cf6-787">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="d1cf6-788">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-788">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="d1cf6-789">AMS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-789">AMS</span></span>

* <span data-ttu-id="d1cf6-790">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="d1cf6-790">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-791">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-791">Appservice</span></span>

* <span data-ttu-id="d1cf6-792">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="d1cf6-792">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="d1cf6-793">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-793">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="d1cf6-794">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="d1cf6-794">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="d1cf6-795">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="d1cf6-795">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="d1cf6-796">Lote AI</span><span class="sxs-lookup"><span data-stu-id="d1cf6-796">Batch AI</span></span>

* <span data-ttu-id="d1cf6-797">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="d1cf6-797">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d1cf6-798">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-798">Cognitive Services</span></span>

* <span data-ttu-id="d1cf6-799">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-799">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="d1cf6-800">Consumo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-800">Consumption</span></span>

* <span data-ttu-id="d1cf6-801">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-801">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="d1cf6-802">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-802">Container</span></span>

* <span data-ttu-id="d1cf6-803">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="d1cf6-803">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="d1cf6-804">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d1cf6-804">Cosmos DB</span></span>

* <span data-ttu-id="d1cf6-805">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d1cf6-805">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="d1cf6-806">DMS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-806">DMS</span></span>

* <span data-ttu-id="d1cf6-807">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="d1cf6-807">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="d1cf6-808">Extensão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-808">Extension</span></span>

* <span data-ttu-id="d1cf6-809">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-809">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="d1cf6-810">Interativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-810">Interactive</span></span>

* <span data-ttu-id="d1cf6-811">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="d1cf6-811">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="d1cf6-812">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="d1cf6-812">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="d1cf6-813">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="d1cf6-813">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="d1cf6-814">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="d1cf6-814">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="d1cf6-815">Laboratório</span><span class="sxs-lookup"><span data-stu-id="d1cf6-815">Lab</span></span>

* <span data-ttu-id="d1cf6-816">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-816">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-817">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-817">Network</span></span>

* <span data-ttu-id="d1cf6-818">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-818">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="d1cf6-819">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1cf6-819">Profile</span></span>

* <span data-ttu-id="d1cf6-820">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="d1cf6-820">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="d1cf6-821">[ALTERAÇÃO SIGNIFICATIVA] `--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-821">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="d1cf6-822">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-822">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="d1cf6-823">Redis</span><span class="sxs-lookup"><span data-stu-id="d1cf6-823">Redis</span></span>

* <span data-ttu-id="d1cf6-824">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-824">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="d1cf6-825">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-825">Deprecated `redis list-all`.</span></span> <span data-ttu-id="d1cf6-826">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-826">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="d1cf6-827">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-827">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="d1cf6-828">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-828">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="d1cf6-829">Função</span><span class="sxs-lookup"><span data-stu-id="d1cf6-829">Role</span></span>

* <span data-ttu-id="d1cf6-830">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="d1cf6-830">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-831">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-831">Storage</span></span>

* <span data-ttu-id="d1cf6-832">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-832">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="d1cf6-833">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="d1cf6-833">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="d1cf6-834">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-834">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="d1cf6-835">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="d1cf6-835">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="d1cf6-836">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="d1cf6-836">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-837">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-837">VM</span></span>

* <span data-ttu-id="d1cf6-838">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-838">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="d1cf6-839">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="d1cf6-839">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="d1cf6-840">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="d1cf6-840">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="d1cf6-841">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-841">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="d1cf6-842">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-842">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="d1cf6-843">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="d1cf6-843">Added write accelerator support</span></span>
* <span data-ttu-id="d1cf6-844">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-844">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="d1cf6-845">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="d1cf6-845">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="d1cf6-846">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="d1cf6-846">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="d1cf6-847">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-847">April 10, 2018</span></span>

<span data-ttu-id="d1cf6-848">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="d1cf6-848">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="d1cf6-849">ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-849">ACR</span></span>

* <span data-ttu-id="d1cf6-850">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="d1cf6-850">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-851">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-851">ACS</span></span>

* <span data-ttu-id="d1cf6-852">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-852">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-853">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-853">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="d1cf6-855">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="d1cf6-855">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="d1cf6-856">BatchAI</span><span class="sxs-lookup"><span data-stu-id="d1cf6-856">BatchAI</span></span>

* <span data-ttu-id="d1cf6-857">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="d1cf6-857">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="d1cf6-858">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="d1cf6-858">Job level mounting</span></span>
  - <span data-ttu-id="d1cf6-859">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-859">Environment variables with secret values</span></span>
  - <span data-ttu-id="d1cf6-860">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="d1cf6-860">Performance counters settings</span></span>
  - <span data-ttu-id="d1cf6-861">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="d1cf6-861">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="d1cf6-862">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="d1cf6-862">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="d1cf6-863">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="d1cf6-863">Usage and limits reporting</span></span>
  - <span data-ttu-id="d1cf6-864">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-864">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="d1cf6-865">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-865">Support for custom images</span></span>
  - <span data-ttu-id="d1cf6-866">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="d1cf6-866">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="d1cf6-867">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="d1cf6-867">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="d1cf6-868">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="d1cf6-868">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="d1cf6-869">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="d1cf6-869">National clouds are supported</span></span>
* <span data-ttu-id="d1cf6-870">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="d1cf6-870">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="d1cf6-871">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="d1cf6-871">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="d1cf6-872">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="d1cf6-872">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="d1cf6-873">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-873">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="d1cf6-874">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-874">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="d1cf6-875">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-875">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="d1cf6-876">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-876">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="d1cf6-877">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-877">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="d1cf6-878">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="d1cf6-878">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="d1cf6-879">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-879">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="d1cf6-880">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="d1cf6-880">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="d1cf6-881">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-881">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="d1cf6-882">[ALTERAÇÃO SIGNIFICATIVA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-882">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="d1cf6-883">Cobrança</span><span class="sxs-lookup"><span data-stu-id="d1cf6-883">Billing</span></span>

* <span data-ttu-id="d1cf6-884">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="d1cf6-884">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="d1cf6-885">Consumo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-885">Consumption</span></span>

* <span data-ttu-id="d1cf6-886">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-886">Added `marketplace` commands</span></span>
* <span data-ttu-id="d1cf6-887">[ALTERAÇÃO SIGNIFICATIVA] `reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-887">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="d1cf6-888">[ALTERAÇÃO SIGNIFICATIVA] `reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-888">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="d1cf6-889">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-889">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="d1cf6-890">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-890">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="d1cf6-891">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-891">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="d1cf6-892">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-892">Container</span></span>

* <span data-ttu-id="d1cf6-893">Adição dos parâmetros de montagem de volume de repositório git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-893">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="d1cf6-894">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-894">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="d1cf6-895">Extensão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-895">Extension</span></span>

* <span data-ttu-id="d1cf6-896">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="d1cf6-896">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="d1cf6-897">Interativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-897">Interactive</span></span>

* <span data-ttu-id="d1cf6-898">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-898">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="d1cf6-899">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="d1cf6-899">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="d1cf6-900">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-900">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-901">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-901">Network</span></span>

* <span data-ttu-id="d1cf6-902">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-902">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="d1cf6-903">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-903">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="d1cf6-904">#4910</span><span class="sxs-lookup"><span data-stu-id="d1cf6-904">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="d1cf6-905">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-905">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="d1cf6-906">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-906">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="d1cf6-907">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-907">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="d1cf6-908">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-908">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="d1cf6-909">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-909">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="d1cf6-910">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1cf6-910">Profile</span></span>

* <span data-ttu-id="d1cf6-911">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-911">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="d1cf6-912">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-912">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="d1cf6-913">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-913">RDBMS</span></span>

* <span data-ttu-id="d1cf6-914">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-914">Added `georestore` command</span></span>
* <span data-ttu-id="d1cf6-915">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-915">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="d1cf6-916">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-916">Resource</span></span>

* <span data-ttu-id="d1cf6-917">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-917">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="d1cf6-918">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-918">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="d1cf6-919">SQL</span><span class="sxs-lookup"><span data-stu-id="d1cf6-919">SQL</span></span>

* <span data-ttu-id="d1cf6-920">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-920">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-921">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-921">Storage</span></span>

* <span data-ttu-id="d1cf6-922">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-922">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-923">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-923">VM</span></span>

* <span data-ttu-id="d1cf6-924">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-924">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="d1cf6-925">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-925">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="d1cf6-927">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-927">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="d1cf6-928">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-928">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="d1cf6-929">#5718</span><span class="sxs-lookup"><span data-stu-id="d1cf6-929">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="d1cf6-930">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="d1cf6-930">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="d1cf6-931">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-931">March 27, 2018</span></span>

<span data-ttu-id="d1cf6-932">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="d1cf6-932">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="d1cf6-933">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-933">Core</span></span>

* <span data-ttu-id="d1cf6-934">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="d1cf6-934">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-935">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-935">ACS</span></span>

* <span data-ttu-id="d1cf6-936">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="d1cf6-936">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-937">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-937">Appservice</span></span>

* <span data-ttu-id="d1cf6-938">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-938">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="d1cf6-939">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-939">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="d1cf6-940">Backup</span><span class="sxs-lookup"><span data-stu-id="d1cf6-940">Backup</span></span>

* <span data-ttu-id="d1cf6-941">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-941">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="d1cf6-942">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="d1cf6-942">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="d1cf6-943">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-943">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="d1cf6-944">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-944">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="d1cf6-945">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-945">Container</span></span>

* <span data-ttu-id="d1cf6-946">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-946">Added `container exec` command.</span></span> <span data-ttu-id="d1cf6-947">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="d1cf6-947">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="d1cf6-948">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-948">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="d1cf6-949">Extensão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-949">Extension</span></span>

* <span data-ttu-id="d1cf6-950">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="d1cf6-950">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="d1cf6-951">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-951">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="d1cf6-952">[ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-952">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="d1cf6-953">Interativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-953">Interactive</span></span>

* <span data-ttu-id="d1cf6-954">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-954">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="d1cf6-955">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-955">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="d1cf6-956">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-956">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="d1cf6-957">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="d1cf6-957">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="d1cf6-958">Laboratório</span><span class="sxs-lookup"><span data-stu-id="d1cf6-958">Lab</span></span>

* <span data-ttu-id="d1cf6-959">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-959">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="d1cf6-960">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-960">Monitor</span></span>

* <span data-ttu-id="d1cf6-961">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-961">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="d1cf6-962">[#4529](https://github.com/Azure/azure-cli/issues/5785) corrigido: `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="d1cf6-962">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="d1cf6-963">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-963">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-964">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-964">Network</span></span>

* <span data-ttu-id="d1cf6-965">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-965">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="d1cf6-966">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1cf6-966">Profile</span></span>

* <span data-ttu-id="d1cf6-967">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-967">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="d1cf6-968">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-968">RDBMS</span></span>

* <span data-ttu-id="d1cf6-969">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="d1cf6-969">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="d1cf6-970">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-970">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="d1cf6-972">Função</span><span class="sxs-lookup"><span data-stu-id="d1cf6-972">Role</span></span>

* <span data-ttu-id="d1cf6-973">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-973">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="d1cf6-974">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="d1cf6-974">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="d1cf6-975">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-975">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="d1cf6-976">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-976">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="d1cf6-977">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-977">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-978">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-978">Storage</span></span>

* <span data-ttu-id="d1cf6-979">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="d1cf6-979">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="d1cf6-980">[4049#](https://github.com/Azure/azure-cli/issues/4049) corrigido: problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="d1cf6-980">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-981">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-981">VM</span></span>

* <span data-ttu-id="d1cf6-982">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="d1cf6-982">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="d1cf6-983">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-983">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="d1cf6-984">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-984">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="d1cf6-985">[ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="d1cf6-985">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="d1cf6-986">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-986">March 13, 2018</span></span>

<span data-ttu-id="d1cf6-987">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="d1cf6-987">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="d1cf6-988">ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-988">ACR</span></span>

* <span data-ttu-id="d1cf6-989">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-989">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="d1cf6-990">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-990">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="d1cf6-991">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-991">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-992">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-992">ACS</span></span>

* <span data-ttu-id="d1cf6-993">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-993">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="d1cf6-994">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="d1cf6-994">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="d1cf6-995">Supervisor</span><span class="sxs-lookup"><span data-stu-id="d1cf6-995">Advisor</span></span>

* <span data-ttu-id="d1cf6-996">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-996">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="d1cf6-997">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-997">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="d1cf6-998">[ALTERAÇÃO SIGNIFICATIVA] `advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="d1cf6-998">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="d1cf6-999">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-999">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="d1cf6-1000">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1000">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-1001">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1001">Appservice</span></span>

* <span data-ttu-id="d1cf6-1002">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1002">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="d1cf6-1003">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1003">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="d1cf6-1004">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1004">Eventhubs</span></span>

* <span data-ttu-id="d1cf6-1005">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1005">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="d1cf6-1006">Extensão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1006">Extension</span></span>

* <span data-ttu-id="d1cf6-1007">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1007">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="d1cf6-1008">Interativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1008">Interactive</span></span>

* <span data-ttu-id="d1cf6-1009">[5625](https://github.com/Azure/azure-cli/issues/5625) corrigido: manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1009">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="d1cf6-1010">[3016](https://github.com/Azure/azure-cli/issues/3016) corrigido: histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1010">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="d1cf6-1011">[5688](https://github.com/Azure/azure-cli/issues/5688) corrigido: as conclusões não aparecerão se o carregamento da tabela de comando encontrou uma exceção</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1011">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="d1cf6-1012">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1012">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="d1cf6-1013">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1013">Monitor</span></span>

* <span data-ttu-id="d1cf6-1014">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1014">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="d1cf6-1015">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1015">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="d1cf6-1016">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1016">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="d1cf6-1017">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1017">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-1018">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1018">Network</span></span>

* <span data-ttu-id="d1cf6-1019">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1019">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="d1cf6-1020">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1020">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="d1cf6-1021">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1021">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="d1cf6-1022">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1022">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="d1cf6-1023">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1023">Profile</span></span>

* <span data-ttu-id="d1cf6-1024">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1024">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="d1cf6-1025">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1025">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="d1cf6-1026">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1026">RDBMS</span></span>

* <span data-ttu-id="d1cf6-1027">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1027">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="d1cf6-1028">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1028">Service Bus</span></span>

* <span data-ttu-id="d1cf6-1029">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1029">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-1030">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1030">Storage</span></span>

* <span data-ttu-id="d1cf6-1031">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1031">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="d1cf6-1032">[5286](https://github.com/Azure/azure-cli/issues/5286) corrigido: os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1032">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-1033">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1033">VM</span></span>

* <span data-ttu-id="d1cf6-1034">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1034">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="d1cf6-1035">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1035">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="d1cf6-1036">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1036">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="d1cf6-1037">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1037">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="d1cf6-1038">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1038">February 27, 2018</span></span>

<span data-ttu-id="d1cf6-1039">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1039">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="d1cf6-1040">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1040">Core</span></span>

* <span data-ttu-id="d1cf6-1041">Correção [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1041">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="d1cf6-1042">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1042">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="d1cf6-1043">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1043">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-1044">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1044">ACS</span></span>

* <span data-ttu-id="d1cf6-1045">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1045">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="d1cf6-1046">Correção do problema de permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1046">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="d1cf6-1047">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1047">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="d1cf6-1048">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1048">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-1049">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1049">Appservice</span></span>

* <span data-ttu-id="d1cf6-1050">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1050">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="d1cf6-1051">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1051">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d1cf6-1052">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1052">Cognitive Services</span></span>

* <span data-ttu-id="d1cf6-1053">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1053">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="d1cf6-1054">Consumo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1054">Consumption</span></span>

* <span data-ttu-id="d1cf6-1055">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1055">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="d1cf6-1056">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1056">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="d1cf6-1057">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1057">Container</span></span>

* <span data-ttu-id="d1cf6-1058">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1058">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-1059">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1059">Network</span></span>

* <span data-ttu-id="d1cf6-1060">Correção [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1060">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="d1cf6-1061">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1061">Resource</span></span>

* <span data-ttu-id="d1cf6-1062">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1062">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="d1cf6-1063">Função</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1063">Role</span></span>

* <span data-ttu-id="d1cf6-1064">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1064">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="d1cf6-1065">SQL</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1065">SQL</span></span>

* <span data-ttu-id="d1cf6-1066">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1066">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-1067">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1067">Storage</span></span>

* <span data-ttu-id="d1cf6-1068">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1068">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-1069">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1069">VM</span></span>

* <span data-ttu-id="d1cf6-1070">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1070">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="d1cf6-1071">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1071">February 13, 2018</span></span>

<span data-ttu-id="d1cf6-1072">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1072">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="d1cf6-1073">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1073">Core</span></span>

* <span data-ttu-id="d1cf6-1074">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1074">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-1075">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1075">ACS</span></span>

* <span data-ttu-id="d1cf6-1076">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1076">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="d1cf6-1077">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1077">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="d1cf6-1078">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1078">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="d1cf6-1079">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1079">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="d1cf6-1080">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1080">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="d1cf6-1081">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1081">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="d1cf6-1082">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1082">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="d1cf6-1083">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1083">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-1084">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1084">Appservice</span></span>

* <span data-ttu-id="d1cf6-1085">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1085">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="d1cf6-1086">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1086">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="d1cf6-1087">CDN</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1087">CDN</span></span>

* <span data-ttu-id="d1cf6-1088">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1088">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="d1cf6-1089">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1089">Container</span></span>

* <span data-ttu-id="d1cf6-1090">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1090">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="d1cf6-1091">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1091">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d1cf6-1092">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1092">CosmosDB</span></span>

* <span data-ttu-id="d1cf6-1093">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1093">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="d1cf6-1094">Extensão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1094">Extension</span></span>

* <span data-ttu-id="d1cf6-1095">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1095">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="d1cf6-1096">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1096">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="d1cf6-1097">Comentários</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1097">Feedback</span></span>

* <span data-ttu-id="d1cf6-1098">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1098">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="d1cf6-1099">Interativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1099">Interactive</span></span>

* <span data-ttu-id="d1cf6-1100">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1100">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="d1cf6-1101">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1101">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="d1cf6-1102">IoT</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1102">IoT</span></span>

* <span data-ttu-id="d1cf6-1103">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1103">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="d1cf6-1104">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1104">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="d1cf6-1105">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1105">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="d1cf6-1106">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1106">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="d1cf6-1107">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1107">Monitor</span></span>

* <span data-ttu-id="d1cf6-1108">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1108">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-1109">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1109">Network</span></span>

* <span data-ttu-id="d1cf6-1110">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1110">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="d1cf6-1111">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1111">Profile</span></span>

* <span data-ttu-id="d1cf6-1112">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1112">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="d1cf6-1113">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1113">Resource</span></span>

* <span data-ttu-id="d1cf6-1114">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1114">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="d1cf6-1115">Função</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1115">Role</span></span>

* <span data-ttu-id="d1cf6-1116">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1116">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="d1cf6-1117">SQL</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1117">SQL</span></span>

* <span data-ttu-id="d1cf6-1118">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1118">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="d1cf6-1119">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1119">Added `sql db rename`</span></span>
* <span data-ttu-id="d1cf6-1120">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1120">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-1121">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1121">Storage</span></span>

* <span data-ttu-id="d1cf6-1122">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1122">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-1123">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1123">VM</span></span>

* <span data-ttu-id="d1cf6-1124">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1124">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="d1cf6-1125">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1125">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="d1cf6-1126">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1126">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="d1cf6-1127">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1127">January 31, 2018</span></span>

<span data-ttu-id="d1cf6-1128">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1128">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="d1cf6-1129">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1129">Core</span></span>

* <span data-ttu-id="d1cf6-1130">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1130">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="d1cf6-1131">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1131">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="d1cf6-1132">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1132">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="d1cf6-1133">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1133">Use `--verbose` to see</span></span>
* <span data-ttu-id="d1cf6-1134">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1134">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-1135">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1135">ACS</span></span>

* <span data-ttu-id="d1cf6-1136">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1136">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="d1cf6-1137">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1137">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-1138">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1138">Appservice</span></span>

* <span data-ttu-id="d1cf6-1139">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1139">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="d1cf6-1140">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1140">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="d1cf6-1141">CDN</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1141">CDN</span></span>

* <span data-ttu-id="d1cf6-1142">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1142">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d1cf6-1143">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1143">CosmosDB</span></span>

* <span data-ttu-id="d1cf6-1144">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1144">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="d1cf6-1145">Interativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1145">Interactive</span></span>

* <span data-ttu-id="d1cf6-1146">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1146">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-1147">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1147">Network</span></span>

* <span data-ttu-id="d1cf6-1148">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1148">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="d1cf6-1149">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1149">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="d1cf6-1150">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1150">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="d1cf6-1151">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1151">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="d1cf6-1152">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1152">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="d1cf6-1153">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1153">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="d1cf6-1154">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1154">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="d1cf6-1155">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1155">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="d1cf6-1156">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1156">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="d1cf6-1157">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1157">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="d1cf6-1158">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1158">Profile</span></span>

* <span data-ttu-id="d1cf6-1159">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1159">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="d1cf6-1160">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1160">Resource</span></span>

* <span data-ttu-id="d1cf6-1161">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1161">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-1162">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1162">Storage</span></span>

* <span data-ttu-id="d1cf6-1163">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1163">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="d1cf6-1164">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1164">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="d1cf6-1165">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1165">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="d1cf6-1166">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1166">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="d1cf6-1167">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1167">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-1168">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1168">VM</span></span>

* <span data-ttu-id="d1cf6-1169">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1169">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="d1cf6-1170">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1170">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="d1cf6-1171">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1171">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="d1cf6-1172">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1172">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="d1cf6-1173">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1173">January 17, 2018</span></span>

<span data-ttu-id="d1cf6-1174">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1174">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="d1cf6-1175">ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1175">ACR</span></span>

* <span data-ttu-id="d1cf6-1176">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1176">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="d1cf6-1177">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1177">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-1178">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1178">ACS</span></span>

* <span data-ttu-id="d1cf6-1179">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1179">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="d1cf6-1180">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1180">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-1181">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1181">Appservice</span></span>

* <span data-ttu-id="d1cf6-1182">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1182">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="d1cf6-1183">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1183">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="d1cf6-1184">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1184">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="d1cf6-1185">Backup</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1185">Backup</span></span>

* <span data-ttu-id="d1cf6-1186">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1186">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="d1cf6-1187">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1187">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="d1cf6-1188">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1188">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="d1cf6-1189">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1189">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="d1cf6-1190">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1190">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="d1cf6-1191">Lote</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1191">Batch</span></span>

* <span data-ttu-id="d1cf6-1192">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1192">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="d1cf6-1193">Nuvem</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1193">Cloud</span></span>

* <span data-ttu-id="d1cf6-1194">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1194">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="d1cf6-1195">Consumo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1195">Consumption</span></span>

* <span data-ttu-id="d1cf6-1196">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1196">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="d1cf6-1197">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1197">Event Grid</span></span>

* <span data-ttu-id="d1cf6-1198">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1198">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="d1cf6-1199">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1199">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="d1cf6-1200">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1200">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="d1cf6-1201">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1201">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="d1cf6-1202">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1202">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="d1cf6-1203">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1203">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="d1cf6-1204">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1204">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="d1cf6-1205">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1205">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="d1cf6-1206">Interativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1206">Interactive</span></span>

* <span data-ttu-id="d1cf6-1207">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1207">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="d1cf6-1208">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1208">Fixed errors on startup</span></span>
* <span data-ttu-id="d1cf6-1209">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1209">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="d1cf6-1210">IoT</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1210">IoT</span></span>

* <span data-ttu-id="d1cf6-1211">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1211">Added support for device provisioning service</span></span>
* <span data-ttu-id="d1cf6-1212">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1212">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="d1cf6-1213">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1213">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="d1cf6-1214">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1214">Monitor</span></span>

* <span data-ttu-id="d1cf6-1215">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1215">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="d1cf6-1216">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1216">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="d1cf6-1217">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1217">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-1218">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1218">Network</span></span>

* <span data-ttu-id="d1cf6-1219">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1219">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="d1cf6-1220">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1220">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="d1cf6-1221">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1221">Profile</span></span>

* <span data-ttu-id="d1cf6-1222">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1222">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="d1cf6-1223">Função</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1223">Role</span></span>

* <span data-ttu-id="d1cf6-1224">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1224">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d1cf6-1225">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1225">Service Fabric</span></span>

* <span data-ttu-id="d1cf6-1226">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1226">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="d1cf6-1227">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1227">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-1228">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1228">VM</span></span>

* <span data-ttu-id="d1cf6-1229">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1229">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="d1cf6-1230">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1230">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="d1cf6-1231">[ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1231">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="d1cf6-1232">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1232">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="d1cf6-1233">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1233">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="d1cf6-1234">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1234">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="d1cf6-1235">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1235">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="d1cf6-1236">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1236">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="d1cf6-1237">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1237">December 19, 2017</span></span>

<span data-ttu-id="d1cf6-1238">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1238">Version 2.0.23</span></span>

* <span data-ttu-id="d1cf6-1239">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1239">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="d1cf6-1240">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1240">Container</span></span>

* <span data-ttu-id="d1cf6-1241">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1241">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-1242">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1242">Network</span></span>

* <span data-ttu-id="d1cf6-1243">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1243">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="d1cf6-1244">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1244">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-1245">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1245">Storage</span></span>

* <span data-ttu-id="d1cf6-1246">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1246">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-1247">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1247">VM</span></span>

* <span data-ttu-id="d1cf6-1248">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1248">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="d1cf6-1249">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1249">December 5, 2017</span></span>

<span data-ttu-id="d1cf6-1250">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1250">Version 2.0.22</span></span>

* <span data-ttu-id="d1cf6-1251">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1251">Removed `az component` commands.</span></span> <span data-ttu-id="d1cf6-1252">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1252">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="d1cf6-1253">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1253">Core</span></span>
* <span data-ttu-id="d1cf6-1254">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1254">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="d1cf6-1255">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1255">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-1256">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1256">ACS</span></span>

* <span data-ttu-id="d1cf6-1257">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1257">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="d1cf6-1258">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1258">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="d1cf6-1259">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1259">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="d1cf6-1260">Supervisor</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1260">Advisor</span></span>

* <span data-ttu-id="d1cf6-1261">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1261">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-1262">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1262">Appservice</span></span>

* <span data-ttu-id="d1cf6-1263">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1263">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="d1cf6-1264">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1264">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="d1cf6-1265">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1265">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="d1cf6-1266">Consumo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1266">Consumption</span></span>

* <span data-ttu-id="d1cf6-1267">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1267">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="d1cf6-1268">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1268">Container</span></span>

* <span data-ttu-id="d1cf6-1269">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1269">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="d1cf6-1270">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1270">Monitor</span></span>

* <span data-ttu-id="d1cf6-1271">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1271">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="d1cf6-1272">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1272">Resource</span></span>

* <span data-ttu-id="d1cf6-1273">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1273">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="d1cf6-1274">Função</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1274">Role</span></span>

* <span data-ttu-id="d1cf6-1275">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1275">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="d1cf6-1276">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1276">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="d1cf6-1277">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1277">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="d1cf6-1278">SQL</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1278">SQL</span></span>

* <span data-ttu-id="d1cf6-1279">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1279">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="d1cf6-1280">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1280">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-1281">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1281">VM</span></span>

* <span data-ttu-id="d1cf6-1282">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1282">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="d1cf6-1283">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1283">November 14, 2017</span></span>

<span data-ttu-id="d1cf6-1284">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1284">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="d1cf6-1285">ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1285">ACR</span></span>

* <span data-ttu-id="d1cf6-1286">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1286">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="d1cf6-1287">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1287">ACS</span></span>

* <span data-ttu-id="d1cf6-1288">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1288">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="d1cf6-1289">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1289">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="d1cf6-1290">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1290">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="d1cf6-1291">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1291">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="d1cf6-1292">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1292">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-1293">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1293">Appservice</span></span>

* <span data-ttu-id="d1cf6-1294">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1294">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="d1cf6-1295">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1295">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="d1cf6-1296">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1296">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="d1cf6-1297">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1297">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="d1cf6-1298">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1298">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="d1cf6-1299">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1299">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="d1cf6-1300">Lote</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1300">Batch</span></span>

* <span data-ttu-id="d1cf6-1301">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1301">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="d1cf6-1302">Batchai</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1302">Batchai</span></span>

* <span data-ttu-id="d1cf6-1303">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1303">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="d1cf6-1304">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1304">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="d1cf6-1305">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1305">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="d1cf6-1306">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1306">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="d1cf6-1307">Nuvem</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1307">Cloud</span></span>

* <span data-ttu-id="d1cf6-1308">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1308">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="d1cf6-1309">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1309">Container</span></span>

* <span data-ttu-id="d1cf6-1310">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1310">Added support to open multiple ports</span></span>
* <span data-ttu-id="d1cf6-1311">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1311">Added container group restart policy</span></span>
* <span data-ttu-id="d1cf6-1312">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1312">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="d1cf6-1313">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1313">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="d1cf6-1314">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1314">Data Lake Analytics</span></span>

* <span data-ttu-id="d1cf6-1315">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1315">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="d1cf6-1316">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1316">Data Lake Store</span></span>

* <span data-ttu-id="d1cf6-1317">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1317">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="d1cf6-1318">Extensão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1318">Extension</span></span>

* <span data-ttu-id="d1cf6-1319">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1319">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="d1cf6-1320">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1320">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="d1cf6-1321">IoT</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1321">IoT</span></span>

* <span data-ttu-id="d1cf6-1322">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1322">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="d1cf6-1323">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1323">Monitor</span></span>

* <span data-ttu-id="d1cf6-1324">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1324">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-1325">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1325">Network</span></span>

* <span data-ttu-id="d1cf6-1326">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1326">Added support for CAA DNS records</span></span>
* <span data-ttu-id="d1cf6-1327">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1327">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="d1cf6-1328">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1328">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="d1cf6-1329">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1329">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="d1cf6-1330">Reservas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1330">Reservations</span></span>

* <span data-ttu-id="d1cf6-1331">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1331">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="d1cf6-1332">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1332">Resource</span></span>

* <span data-ttu-id="d1cf6-1333">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1333">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="d1cf6-1334">SQL</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1334">SQL</span></span>

* <span data-ttu-id="d1cf6-1335">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1335">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-1336">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1336">Storage</span></span>

* <span data-ttu-id="d1cf6-1337">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1337">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="d1cf6-1338">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1338">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="d1cf6-1339">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1339">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="d1cf6-1340">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1340">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="d1cf6-1341">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1341">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="d1cf6-1342">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1342">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="d1cf6-1343">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1343">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-1344">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1344">VM</span></span>

* <span data-ttu-id="d1cf6-1345">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1345">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="d1cf6-1346">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1346">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="d1cf6-1347">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1347">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="d1cf6-1348">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1348">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="d1cf6-1349">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1349">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="d1cf6-1350">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1350">October 24, 2017</span></span>

<span data-ttu-id="d1cf6-1351">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1351">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="d1cf6-1352">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1352">Core</span></span>

* <span data-ttu-id="d1cf6-1353">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1353">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="d1cf6-1354">ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1354">ACR</span></span>

* <span data-ttu-id="d1cf6-1355">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1355">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="d1cf6-1356">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1356">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="d1cf6-1357">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1357">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-1358">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1358">ACS</span></span>

* <span data-ttu-id="d1cf6-1359">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1359">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="d1cf6-1360">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1360">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-1361">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1361">Appservice</span></span>

* <span data-ttu-id="d1cf6-1362">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1362">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="d1cf6-1363">Componente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1363">Component</span></span>

* <span data-ttu-id="d1cf6-1364">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1364">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="d1cf6-1365">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1365">Monitor</span></span>

* <span data-ttu-id="d1cf6-1366">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1366">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="d1cf6-1367">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1367">Resource</span></span>

* <span data-ttu-id="d1cf6-1368">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1368">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="d1cf6-1369">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1369">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-1370">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1370">VM</span></span>

* <span data-ttu-id="d1cf6-1371">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1371">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="d1cf6-1372">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1372">October 9, 2017</span></span>

<span data-ttu-id="d1cf6-1373">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1373">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="d1cf6-1374">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1374">Core</span></span>

* <span data-ttu-id="d1cf6-1375">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1375">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-1376">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1376">Appservice</span></span>

* <span data-ttu-id="d1cf6-1377">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1377">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="d1cf6-1378">Lote</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1378">Batch</span></span>

* <span data-ttu-id="d1cf6-1379">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1379">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="d1cf6-1380">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1380">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="d1cf6-1381">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1381">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="d1cf6-1382">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1382">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="d1cf6-1383">Batchai</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1383">Batchai</span></span>

* <span data-ttu-id="d1cf6-1384">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1384">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="d1cf6-1385">Keyvault</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1385">Keyvault</span></span>

* <span data-ttu-id="d1cf6-1386">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1386">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="d1cf6-1387">(#4448)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1387">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="d1cf6-1388">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1388">Network</span></span>

* <span data-ttu-id="d1cf6-1389">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1389">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="d1cf6-1390">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1390">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="d1cf6-1391">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1391">Resource</span></span>

* <span data-ttu-id="d1cf6-1392">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1392">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="d1cf6-1393">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1393">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="d1cf6-1394">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1394">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="d1cf6-1395">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1395">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="d1cf6-1396">Sql</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1396">Sql</span></span>

* <span data-ttu-id="d1cf6-1397">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1397">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="d1cf6-1398">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1398">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="d1cf6-1399">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1399">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-1400">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1400">Storage</span></span>

* <span data-ttu-id="d1cf6-1401">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1401">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-1402">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1402">Vm</span></span>

* <span data-ttu-id="d1cf6-1403">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1403">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="d1cf6-1404">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1404">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="d1cf6-1405">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1405">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="d1cf6-1406">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1406">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="d1cf6-1407">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1407">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="d1cf6-1408">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1408">September 22, 2017</span></span>

<span data-ttu-id="d1cf6-1409">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1409">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="d1cf6-1410">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1410">Resource</span></span>

* <span data-ttu-id="d1cf6-1411">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1411">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="d1cf6-1412">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1412">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="d1cf6-1413">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1413">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="d1cf6-1414">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1414">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-1415">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1415">Network</span></span>

* <span data-ttu-id="d1cf6-1416">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1416">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="d1cf6-1417">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1417">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="d1cf6-1418">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1418">Added `asg` application security group commands</span></span>
* <span data-ttu-id="d1cf6-1419">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1419">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="d1cf6-1420">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1420">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="d1cf6-1421">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1421">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="d1cf6-1422">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1422">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-1423">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1423">Storage</span></span>

* <span data-ttu-id="d1cf6-1424">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1424">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="d1cf6-1425">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1425">Eventgrid</span></span>

* <span data-ttu-id="d1cf6-1426">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1426">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="d1cf6-1427">SQL</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1427">SQL</span></span>

* <span data-ttu-id="d1cf6-1428">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1428">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="d1cf6-1429">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1429">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="d1cf6-1430">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1430">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="d1cf6-1431">Keyvault</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1431">Keyvault</span></span>

* <span data-ttu-id="d1cf6-1432">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1432">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-1433">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1433">VM</span></span>

* <span data-ttu-id="d1cf6-1434">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1434">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="d1cf6-1435">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1435">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="d1cf6-1436">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1436">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="d1cf6-1437">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1437">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="d1cf6-1438">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1438">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="d1cf6-1439">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1439">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-1440">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1440">ACS</span></span>

* <span data-ttu-id="d1cf6-1441">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1441">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-1442">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1442">Appservice</span></span>

* <span data-ttu-id="d1cf6-1443">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1443">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="d1cf6-1444">Backup</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1444">Backup</span></span>

* <span data-ttu-id="d1cf6-1445">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1445">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="d1cf6-1446">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1446">September 11, 2017</span></span>

<span data-ttu-id="d1cf6-1447">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1447">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="d1cf6-1448">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1448">Core</span></span>

* <span data-ttu-id="d1cf6-1449">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1449">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="d1cf6-1450">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1450">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-1451">Acs</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1451">Acs</span></span>

* <span data-ttu-id="d1cf6-1452">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1452">Added `acs list-locations` command</span></span>
* <span data-ttu-id="d1cf6-1453">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1453">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-1454">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1454">Appservice</span></span>

* <span data-ttu-id="d1cf6-1455">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1455">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="d1cf6-1456">CDN</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1456">CDN</span></span>

* <span data-ttu-id="d1cf6-1457">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1457">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="d1cf6-1458">Extensão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1458">Extension</span></span>

* <span data-ttu-id="d1cf6-1459">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1459">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="d1cf6-1460">Keyvault</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1460">Keyvault</span></span>

* <span data-ttu-id="d1cf6-1461">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1461">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-1462">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1462">Network</span></span>

* <span data-ttu-id="d1cf6-1463">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1463">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="d1cf6-1464">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1464">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="d1cf6-1465">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1465">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="d1cf6-1466">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1466">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="d1cf6-1467">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1467">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="d1cf6-1468">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1468">Resource</span></span>

* <span data-ttu-id="d1cf6-1469">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1469">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="d1cf6-1470">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1470">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="d1cf6-1471">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1471">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="d1cf6-1472">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1472">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="d1cf6-1473">SQL</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1473">SQL</span></span>

* <span data-ttu-id="d1cf6-1474">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1474">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-1475">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1475">VM</span></span>

* <span data-ttu-id="d1cf6-1476">Corrigido: Não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1476">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="d1cf6-1477">Corrigido: Usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1477">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="d1cf6-1478">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1478">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="d1cf6-1479">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1479">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="d1cf6-1480">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1480">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="d1cf6-1481">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1481">August 31, 2017</span></span>

<span data-ttu-id="d1cf6-1482">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1482">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="d1cf6-1483">Keyvault</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1483">Keyvault</span></span>

* <span data-ttu-id="d1cf6-1484">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1484">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="d1cf6-1485">Sf</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1485">Sf</span></span>

* <span data-ttu-id="d1cf6-1486">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1486">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-1487">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1487">Storage</span></span>

* <span data-ttu-id="d1cf6-1488">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1488">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="d1cf6-1489">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1489">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="d1cf6-1490">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1490">August 28, 2017</span></span>

<span data-ttu-id="d1cf6-1491">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1491">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="d1cf6-1492">CLI</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1492">CLI</span></span>

* <span data-ttu-id="d1cf6-1493">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1493">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-1494">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1494">ACS</span></span>

* <span data-ttu-id="d1cf6-1495">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1495">Corrected preview regions</span></span>
* <span data-ttu-id="d1cf6-1496">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1496">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="d1cf6-1497">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1497">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-1498">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1498">Appservice</span></span>

* <span data-ttu-id="d1cf6-1499">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1499">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="d1cf6-1500">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1500">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="d1cf6-1501">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1501">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="d1cf6-1502">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1502">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="d1cf6-1503">Correção: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1503">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="d1cf6-1504">IoT</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1504">IoT</span></span>

* <span data-ttu-id="d1cf6-1505">Correção #3934: Criação de política não limpa as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1505">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-1506">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1506">Network</span></span>

* <span data-ttu-id="d1cf6-1507">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1507">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="d1cf6-1508">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1508">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="d1cf6-1509">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1509">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="d1cf6-1510">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1510">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="d1cf6-1511">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1511">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="d1cf6-1512">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1512">Profile</span></span>

* <span data-ttu-id="d1cf6-1513">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1513">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d1cf6-1514">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1514">Service Fabric</span></span>

* <span data-ttu-id="d1cf6-1515">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1515">Preview release</span></span>
* <span data-ttu-id="d1cf6-1516">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1516">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="d1cf6-1517">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1517">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="d1cf6-1518">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1518">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-1519">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1519">Storage</span></span>

* <span data-ttu-id="d1cf6-1520">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1520">Enabled setting blob tier</span></span>
* <span data-ttu-id="d1cf6-1521">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1521">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="d1cf6-1522">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1522">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="d1cf6-1523">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1523">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="d1cf6-1524">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1524">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="d1cf6-1525">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1525">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-1526">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1526">VM</span></span>

* <span data-ttu-id="d1cf6-1527">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1527">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="d1cf6-1528">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1528">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="d1cf6-1529">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1529">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="d1cf6-1530">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1530">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="d1cf6-1531">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1531">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="d1cf6-1532">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1532">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="d1cf6-1533">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1533">August 15, 2017</span></span>

<span data-ttu-id="d1cf6-1534">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1534">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-1535">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1535">ACS</span></span>

* <span data-ttu-id="d1cf6-1536">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1536">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-1537">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1537">Appservice</span></span>

* <span data-ttu-id="d1cf6-1538">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1538">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="d1cf6-1539">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1539">Event Grid</span></span>

* <span data-ttu-id="d1cf6-1540">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1540">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="d1cf6-1541">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1541">August 11, 2017</span></span>

<span data-ttu-id="d1cf6-1542">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1542">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-1543">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1543">ACS</span></span>

* <span data-ttu-id="d1cf6-1544">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1544">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="d1cf6-1545">Lote</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1545">Batch</span></span>

* <span data-ttu-id="d1cf6-1546">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1546">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="d1cf6-1547">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1547">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="d1cf6-1548">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1548">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="d1cf6-1549">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="d1cf6-1549">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="d1cf6-1550">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1550">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="d1cf6-1551">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1551">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="d1cf6-1552">Componente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1552">Component</span></span>

* <span data-ttu-id="d1cf6-1553">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1553">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="d1cf6-1554">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1554">Container</span></span>

* <span data-ttu-id="d1cf6-1555">`create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1555">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="d1cf6-1556">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1556">Data Lake Store</span></span>

* <span data-ttu-id="d1cf6-1557">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1557">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="d1cf6-1558">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1558">Event Grid</span></span>

* <span data-ttu-id="d1cf6-1559">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1559">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-1560">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1560">Network</span></span>

* <span data-ttu-id="d1cf6-1561">`lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1561">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="d1cf6-1562">`application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1562">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="d1cf6-1563">`application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1563">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="d1cf6-1564">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1564">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="d1cf6-1565">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1565">Profile</span></span>

* <span data-ttu-id="d1cf6-1566">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1566">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-1567">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1567">Storage</span></span>

* <span data-ttu-id="d1cf6-1568">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1568">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-1569">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1569">VM</span></span>

* <span data-ttu-id="d1cf6-1570">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1570">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="d1cf6-1571">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1571">Exposed `list-skus` command</span></span>
* <span data-ttu-id="d1cf6-1572">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1572">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="d1cf6-1573">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1573">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="d1cf6-1574">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1574">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="d1cf6-1575">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1575">July 28, 2017</span></span>

<span data-ttu-id="d1cf6-1576">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1576">Version 2.0.12</span></span>

* <span data-ttu-id="d1cf6-1577">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1577">Added container commands</span></span>
* <span data-ttu-id="d1cf6-1578">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1578">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="d1cf6-1579">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1579">Core</span></span>

* <span data-ttu-id="d1cf6-1580">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1580">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="d1cf6-1581">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1581">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="d1cf6-1582">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1582">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="d1cf6-1583">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1583">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="d1cf6-1584">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1584">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="d1cf6-1585">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1585">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="d1cf6-1586">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1586">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="d1cf6-1587">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1587">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="d1cf6-1588">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1588">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="d1cf6-1589">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1589">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="d1cf6-1590">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1590">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="d1cf6-1591">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1591">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="d1cf6-1592">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1592">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="d1cf6-1593">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1593">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="d1cf6-1594">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1594">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="d1cf6-1595">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1595">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="d1cf6-1596">ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1596">ACR</span></span>

* <span data-ttu-id="d1cf6-1597">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1597">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="d1cf6-1598">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1598">Support SKU update for managed registries</span></span>
* <span data-ttu-id="d1cf6-1599">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1599">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="d1cf6-1600">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1600">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="d1cf6-1601">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1601">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="d1cf6-1602">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1602">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-1603">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1603">ACS</span></span>

* <span data-ttu-id="d1cf6-1604">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1604">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-1605">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1605">Appservice</span></span>

* <span data-ttu-id="d1cf6-1606">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1606">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="d1cf6-1607">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1607">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="d1cf6-1608">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1608">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="d1cf6-1609">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1609">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="d1cf6-1610">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1610">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="d1cf6-1611">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1611">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="d1cf6-1612">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1612">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="d1cf6-1613">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1613">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="d1cf6-1614">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1614">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="d1cf6-1615">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1615">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="d1cf6-1616">Lote</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1616">Batch</span></span>

* <span data-ttu-id="d1cf6-1617">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1617">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="d1cf6-1618">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1618">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="d1cf6-1619">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1619">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="d1cf6-1620">CDN</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1620">CDN</span></span>

* <span data-ttu-id="d1cf6-1621">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1621">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="d1cf6-1622">Nuvem</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1622">Cloud</span></span>

* <span data-ttu-id="d1cf6-1623">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1623">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="d1cf6-1624">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1624">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="d1cf6-1625">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1625">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="d1cf6-1626">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1626">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="d1cf6-1627">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1627">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d1cf6-1628">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1628">CosmosDB</span></span>

* <span data-ttu-id="d1cf6-1629">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1629">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="d1cf6-1630">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1630">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="d1cf6-1631">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1631">Data Lake Analytics</span></span>

* <span data-ttu-id="d1cf6-1632">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1632">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="d1cf6-1633">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1633">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="d1cf6-1634">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1634">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="d1cf6-1635">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1635">Data Lake Store</span></span>

* <span data-ttu-id="d1cf6-1636">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1636">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="d1cf6-1637">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1637">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="d1cf6-1638">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1638">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="d1cf6-1639">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1639">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="d1cf6-1640">Interativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1640">Interactive</span></span>

* <span data-ttu-id="d1cf6-1641">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1641">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="d1cf6-1642">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1642">Increased test coverage</span></span>
* <span data-ttu-id="d1cf6-1643">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1643">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="d1cf6-1644">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1644">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="d1cf6-1645">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1645">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="d1cf6-1646">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1646">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="d1cf6-1647">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1647">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="d1cf6-1648">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1648">Added `--progress` flag</span></span>
* <span data-ttu-id="d1cf6-1649">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1649">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="d1cf6-1650">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1650">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="d1cf6-1651">IoT</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1651">IoT</span></span>

* <span data-ttu-id="d1cf6-1652">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1652">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="d1cf6-1653">(#3934)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1653">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="d1cf6-1654">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1654">Key vault</span></span>

* <span data-ttu-id="d1cf6-1655">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1655">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="d1cf6-1656">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1656">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="d1cf6-1657">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1657">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="d1cf6-1658">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1658">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="d1cf6-1659">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1659">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="d1cf6-1660">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1660">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="d1cf6-1661">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1661">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="d1cf6-1662">(#3307)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1662">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="d1cf6-1663">Laboratório</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1663">Lab</span></span>

* <span data-ttu-id="d1cf6-1664">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1664">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="d1cf6-1665">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1665">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="d1cf6-1666">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1666">Monitor</span></span>

* <span data-ttu-id="d1cf6-1667">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1667">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="d1cf6-1668">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1668">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="d1cf6-1669">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1669">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="d1cf6-1670">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1670">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="d1cf6-1671">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1671">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="d1cf6-1672">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1672">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="d1cf6-1673">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1673">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="d1cf6-1674">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1674">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="d1cf6-1675">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1675">`location` no longer required</span></span>
  * <span data-ttu-id="d1cf6-1676">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1676">Add name and ID support for target</span></span>
  * <span data-ttu-id="d1cf6-1677">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1677">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="d1cf6-1678">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1678">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="d1cf6-1679">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1679">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="d1cf6-1680">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1680">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="d1cf6-1681">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1681">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="d1cf6-1682">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1682">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-1683">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1683">Network</span></span>

* <span data-ttu-id="d1cf6-1684">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1684">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="d1cf6-1685">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1685">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="d1cf6-1686">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1686">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="d1cf6-1687">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1687">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="d1cf6-1688">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1688">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="d1cf6-1689">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1689">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="d1cf6-1690">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1690">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="d1cf6-1691">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1691">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="d1cf6-1692">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1692">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="d1cf6-1693">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1693">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="d1cf6-1694">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1694">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="d1cf6-1695">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1695">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="d1cf6-1696">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1696">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="d1cf6-1697">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1697">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="d1cf6-1698">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1698">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="d1cf6-1699">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1699">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="d1cf6-1700">Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1700">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="d1cf6-1701">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1701">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="d1cf6-1702">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1702">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="d1cf6-1703">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1703">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="d1cf6-1704">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1704">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="d1cf6-1705">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1705">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="d1cf6-1706">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1706">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="d1cf6-1707">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1707">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="d1cf6-1708">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1708">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="d1cf6-1709">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1709">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="d1cf6-1710">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1710">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="d1cf6-1711">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1711">Profile</span></span>

* <span data-ttu-id="d1cf6-1712">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1712">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="d1cf6-1713">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1713">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="d1cf6-1714">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1714">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="d1cf6-1715">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1715">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="d1cf6-1716">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1716">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="d1cf6-1717">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1717">RDBMS</span></span>

* <span data-ttu-id="d1cf6-1718">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1718">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="d1cf6-1719">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1719">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="d1cf6-1720">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1720">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="d1cf6-1721">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1721">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="d1cf6-1722">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1722">Resource</span></span>

* <span data-ttu-id="d1cf6-1723">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1723">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="d1cf6-1724">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1724">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="d1cf6-1725">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1725">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="d1cf6-1726">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1726">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="d1cf6-1727">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1727">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="d1cf6-1728">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1728">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="d1cf6-1729">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1729">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="d1cf6-1730">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1730">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="d1cf6-1731">Função</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1731">Role</span></span>

* <span data-ttu-id="d1cf6-1732">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1732">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="d1cf6-1733">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1733">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="d1cf6-1734">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1734">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="d1cf6-1735">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1735">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="d1cf6-1736">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1736">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d1cf6-1737">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1737">Service Fabric</span></span>
* <span data-ttu-id="d1cf6-1738">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1738">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="d1cf6-1739">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1739">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="d1cf6-1740">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1740">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="d1cf6-1741">SQL</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1741">SQL</span></span>

* <span data-ttu-id="d1cf6-1742">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1742">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="d1cf6-1743">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1743">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="d1cf6-1744">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1744">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-1745">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1745">Storage</span></span>

* <span data-ttu-id="d1cf6-1746">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1746">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="d1cf6-1747">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1747">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="d1cf6-1748">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1748">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="d1cf6-1749">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1749">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="d1cf6-1750">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1750">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="d1cf6-1751">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1751">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-1752">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1752">VM</span></span>

* <span data-ttu-id="d1cf6-1753">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1753">Support configuring nsg</span></span>
* <span data-ttu-id="d1cf6-1754">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1754">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="d1cf6-1755">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1755">Support managed service identities</span></span>
* <span data-ttu-id="d1cf6-1756">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1756">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="d1cf6-1757">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1757">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="d1cf6-1758">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1758">May 10, 2017</span></span>

<span data-ttu-id="d1cf6-1759">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1759">Version 2.0.6</span></span>

* <span data-ttu-id="d1cf6-1760">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1760">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="d1cf6-1761">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1761">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="d1cf6-1762">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1762">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="d1cf6-1763">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1763">Include Cognitive Services module</span></span>
* <span data-ttu-id="d1cf6-1764">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1764">Include Service Fabric module</span></span>
* <span data-ttu-id="d1cf6-1765">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1765">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="d1cf6-1766">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1766">Add support for CDN commands</span></span>
* <span data-ttu-id="d1cf6-1767">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1767">Remove Container module</span></span>
* <span data-ttu-id="d1cf6-1768">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1768">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="d1cf6-1769">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1769">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="d1cf6-1770">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1770">Core</span></span>

* <span data-ttu-id="d1cf6-1771">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1771">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="d1cf6-1772">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1772">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="d1cf6-1773">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1773">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="d1cf6-1774">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1774">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="d1cf6-1775">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1775">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="d1cf6-1776">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1776">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="d1cf6-1777">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1777">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="d1cf6-1778">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1778">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="d1cf6-1779">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1779">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="d1cf6-1780">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1780">core: Improved performance</span></span>
* <span data-ttu-id="d1cf6-1781">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1781">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="d1cf6-1782">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1782">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-1783">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1783">ACS</span></span>

* <span data-ttu-id="d1cf6-1784">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1784">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="d1cf6-1785">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1785">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="d1cf6-1786">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1786">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="d1cf6-1787">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1787">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-1788">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1788">AppService</span></span>

* <span data-ttu-id="d1cf6-1789">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1789">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="d1cf6-1790">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1790">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="d1cf6-1791">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1791">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="d1cf6-1792">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1792">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="d1cf6-1793">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1793">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="d1cf6-1794">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1794">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="d1cf6-1795">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1795">support slot swap with preview</span></span>
* <span data-ttu-id="d1cf6-1796">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1796">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="d1cf6-1797">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1797">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d1cf6-1798">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1798">CosmosDB</span></span>

* <span data-ttu-id="d1cf6-1799">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1799">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="d1cf6-1800">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1800">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="d1cf6-1801">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1801">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="d1cf6-1802">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1802">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="d1cf6-1803">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1803">Data Lake Analytics</span></span>

* <span data-ttu-id="d1cf6-1804">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1804">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="d1cf6-1805">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1805">Add support for new catalog item type: package.</span></span> <span data-ttu-id="d1cf6-1806">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1806">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="d1cf6-1807">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1807">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="d1cf6-1808">Tabela</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1808">Table</span></span>
  * <span data-ttu-id="d1cf6-1809">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1809">Table valued function</span></span>
  * <span data-ttu-id="d1cf6-1810">Visualizar</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1810">View</span></span>
  * <span data-ttu-id="d1cf6-1811">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1811">Table Statistics.</span></span> <span data-ttu-id="d1cf6-1812">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1812">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="d1cf6-1813">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1813">Data Lake Store</span></span>

* <span data-ttu-id="d1cf6-1814">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1814">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="d1cf6-1815">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1815">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="d1cf6-1816">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1816">missed help for access show.</span></span> <span data-ttu-id="d1cf6-1817">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1817">adding it.</span></span> <span data-ttu-id="d1cf6-1818">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1818">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="d1cf6-1819">Localizar</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1819">Find</span></span>

* <span data-ttu-id="d1cf6-1820">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1820">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="d1cf6-1821">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1821">KeyVault</span></span>

* <span data-ttu-id="d1cf6-1822">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1822">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="d1cf6-1823">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1823">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="d1cf6-1824">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1824">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="d1cf6-1825">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1825">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="d1cf6-1826">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1826">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="d1cf6-1827">Laboratório</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1827">Lab</span></span>

* <span data-ttu-id="d1cf6-1828">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1828">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="d1cf6-1829">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1829">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="d1cf6-1830">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1830">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="d1cf6-1831">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1831">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="d1cf6-1832">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1832">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="d1cf6-1833">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1833">Monitor</span></span>

* <span data-ttu-id="d1cf6-1834">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1834">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="d1cf6-1835">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1835">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="d1cf6-1836">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1836">Network</span></span>

* <span data-ttu-id="d1cf6-1837">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1837">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="d1cf6-1838">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1838">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="d1cf6-1839">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1839">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="d1cf6-1840">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1840">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="d1cf6-1841">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1841">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="d1cf6-1842">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1842">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="d1cf6-1843">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1843">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="d1cf6-1844">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1844">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="d1cf6-1845">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1845">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="d1cf6-1846">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1846">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="d1cf6-1847">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1847">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="d1cf6-1848">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1848">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="d1cf6-1849">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1849">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="d1cf6-1850">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1850">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="d1cf6-1851">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1851">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="d1cf6-1852">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1852">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="d1cf6-1853">Perfil</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1853">Profile</span></span>

* <span data-ttu-id="d1cf6-1854">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1854">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="d1cf6-1855">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1855">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="d1cf6-1856">Redis</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1856">Redis</span></span>

* <span data-ttu-id="d1cf6-1857">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1857">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="d1cf6-1858">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1858">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="d1cf6-1859">Recurso</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1859">Resource</span></span>

* <span data-ttu-id="d1cf6-1860">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1860">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="d1cf6-1861">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1861">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="d1cf6-1862">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1862">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="d1cf6-1863">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1863">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="d1cf6-1864">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1864">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="d1cf6-1865">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1865">Add docs for az lock update.</span></span> <span data-ttu-id="d1cf6-1866">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1866">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="d1cf6-1867">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1867">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="d1cf6-1868">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1868">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="d1cf6-1869">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1869">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="d1cf6-1870">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1870">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="d1cf6-1871">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1871">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="d1cf6-1872">Função</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1872">Role</span></span>

* <span data-ttu-id="d1cf6-1873">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1873">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="d1cf6-1874">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1874">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="d1cf6-1875">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1875">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="d1cf6-1876">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1876">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="d1cf6-1877">SQL</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1877">SQL</span></span>

* <span data-ttu-id="d1cf6-1878">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1878">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="d1cf6-1879">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1879">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="d1cf6-1880">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1880">Storage</span></span>

* <span data-ttu-id="d1cf6-1881">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1881">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="d1cf6-1882">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1882">Add support for incremental blob copy</span></span>
* <span data-ttu-id="d1cf6-1883">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1883">Add support for large block blob upload</span></span>
* <span data-ttu-id="d1cf6-1884">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1884">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-1885">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1885">VM</span></span>

* <span data-ttu-id="d1cf6-1886">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1886">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="d1cf6-1887">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1887">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="d1cf6-1888">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1888">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="d1cf6-1889">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1889">az vm/vmss disk</span></span>
  3. <span data-ttu-id="d1cf6-1890">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1890">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="d1cf6-1891">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1891">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="d1cf6-1892">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1892">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="d1cf6-1893">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1893">April 3, 2017</span></span>

<span data-ttu-id="d1cf6-1894">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1894">Version 2.0.2</span></span>

<span data-ttu-id="d1cf6-1895">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1895">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="d1cf6-1896">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1896">Core</span></span>

* <span data-ttu-id="d1cf6-1897">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1897">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="d1cf6-1898">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1898">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="d1cf6-1899">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1899">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="d1cf6-1900">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1900">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="d1cf6-1901">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1901">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="d1cf6-1902">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1902">Add prompting for missing template parameters.</span></span> <span data-ttu-id="d1cf6-1903">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1903">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="d1cf6-1904">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1904">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="d1cf6-1905">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1905">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="d1cf6-1906">ACS</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1906">ACS</span></span>

* <span data-ttu-id="d1cf6-1907">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1907">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="d1cf6-1908">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1908">Add support for ssh key password prompting.</span></span> <span data-ttu-id="d1cf6-1909">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1909">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="d1cf6-1910">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1910">Add support for windows clusters.</span></span> <span data-ttu-id="d1cf6-1911">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1911">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="d1cf6-1912">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1912">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="d1cf6-1913">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1913">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="d1cf6-1914">AppService</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1914">AppService</span></span>

* <span data-ttu-id="d1cf6-1915">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1915">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="d1cf6-1916">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1916">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="d1cf6-1917">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1917">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="d1cf6-1918">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1918">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="d1cf6-1919">DataLake</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1919">DataLake</span></span>

* <span data-ttu-id="d1cf6-1920">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1920">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="d1cf6-1921">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1921">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="d1cf6-1922">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1922">DocuemntDB</span></span>

* <span data-ttu-id="d1cf6-1923">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1923">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="d1cf6-1924">VM</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1924">VM</span></span>

* <span data-ttu-id="d1cf6-1925">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1925">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="d1cf6-1926">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1926">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="d1cf6-1927">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1927">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="d1cf6-1928">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1928">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="d1cf6-1929">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1929">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="d1cf6-1930">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1930">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="d1cf6-1931">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1931">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="d1cf6-1932">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1932">February 27, 2017</span></span>

<span data-ttu-id="d1cf6-1933">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1933">Version 2.0.0</span></span>

<span data-ttu-id="d1cf6-1934">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1934">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="d1cf6-1935">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1935">Container Service (acs)</span></span>
- <span data-ttu-id="d1cf6-1936">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1936">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="d1cf6-1937">Rede</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1937">Networking</span></span>
- <span data-ttu-id="d1cf6-1938">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1938">Storage</span></span>

<span data-ttu-id="d1cf6-1939">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1939">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="d1cf6-1940">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1940">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="d1cf6-1941">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1941">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="d1cf6-1942">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1942">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="d1cf6-1943">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1943">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="d1cf6-1944">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1944">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="d1cf6-1945">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1945">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="d1cf6-1946">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1946">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="d1cf6-1947">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="d1cf6-1947">Provide feedback from the command line with the `az feedback` command</span></span>

