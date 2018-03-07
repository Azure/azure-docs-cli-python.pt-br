---
title: "Notas de versão da CLI do Azure 2.0"
description: "Saiba mais sobre as últimas atualizações da CLI do Azure 2.0"
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/27/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 01078b7a3665f563f0a6b1d809c9a41f18d136d6
ms.sourcegitcommit: f3ab5da6019083ef2482b62c7355817e6170dcfb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="be48e-103">Notas de versão da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="be48e-103">Azure CLI 2.0 release notes</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="be48e-104">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="be48e-104">February 27, 2018</span></span>

<span data-ttu-id="be48e-105">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="be48e-105">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="be48e-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be48e-106">Core</span></span>

* <span data-ttu-id="be48e-107">Correção [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="be48e-107">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="be48e-108">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="be48e-108">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="be48e-109">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="be48e-109">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="be48e-110">ACS</span><span class="sxs-lookup"><span data-stu-id="be48e-110">ACS</span></span>

* <span data-ttu-id="be48e-111">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="be48e-111">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="be48e-112">Correção do problema de permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="be48e-112">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="be48e-113">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="be48e-113">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="be48e-114">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="be48e-114">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="be48e-115">AppService</span><span class="sxs-lookup"><span data-stu-id="be48e-115">Appservice</span></span>

* <span data-ttu-id="be48e-116">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="be48e-116">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="be48e-117">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="be48e-117">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="be48e-118">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="be48e-118">Cognitive Services</span></span>

* <span data-ttu-id="be48e-119">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="be48e-119">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="be48e-120">Consumo</span><span class="sxs-lookup"><span data-stu-id="be48e-120">Consumption</span></span>

* <span data-ttu-id="be48e-121">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="be48e-121">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="be48e-122">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="be48e-122">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="be48e-123">Contêiner</span><span class="sxs-lookup"><span data-stu-id="be48e-123">Container</span></span>

* <span data-ttu-id="be48e-124">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="be48e-124">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="be48e-125">Rede</span><span class="sxs-lookup"><span data-stu-id="be48e-125">Network</span></span>

* <span data-ttu-id="be48e-126">Correção [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="be48e-126">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="be48e-127">Recurso</span><span class="sxs-lookup"><span data-stu-id="be48e-127">Resource</span></span>

* <span data-ttu-id="be48e-128">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="be48e-128">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="be48e-129">Função</span><span class="sxs-lookup"><span data-stu-id="be48e-129">Role</span></span>

* <span data-ttu-id="be48e-130">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="be48e-130">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="be48e-131">SQL</span><span class="sxs-lookup"><span data-stu-id="be48e-131">SQL</span></span>

* <span data-ttu-id="be48e-132">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="be48e-132">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="be48e-133">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="be48e-133">Storage</span></span>

* <span data-ttu-id="be48e-134">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="be48e-134">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="be48e-135">VM</span><span class="sxs-lookup"><span data-stu-id="be48e-135">VM</span></span>

* <span data-ttu-id="be48e-136">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="be48e-136">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="be48e-137">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="be48e-137">February 13, 2018</span></span>

<span data-ttu-id="be48e-138">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="be48e-138">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="be48e-139">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be48e-139">Core</span></span>

* <span data-ttu-id="be48e-140">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="be48e-140">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="be48e-141">ACS</span><span class="sxs-lookup"><span data-stu-id="be48e-141">ACS</span></span>

* <span data-ttu-id="be48e-142">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="be48e-142">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="be48e-143">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="be48e-143">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="be48e-144">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="be48e-144">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="be48e-145">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="be48e-145">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="be48e-146">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="be48e-146">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="be48e-147">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="be48e-147">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="be48e-148">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="be48e-148">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="be48e-149">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="be48e-149">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="be48e-150">AppService</span><span class="sxs-lookup"><span data-stu-id="be48e-150">Appservice</span></span>

* <span data-ttu-id="be48e-151">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="be48e-151">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="be48e-152">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="be48e-152">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="be48e-153">CDN</span><span class="sxs-lookup"><span data-stu-id="be48e-153">CDN</span></span>

* <span data-ttu-id="be48e-154">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="be48e-154">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="be48e-155">Contêiner</span><span class="sxs-lookup"><span data-stu-id="be48e-155">Container</span></span>

* <span data-ttu-id="be48e-156">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="be48e-156">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="be48e-157">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="be48e-157">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="be48e-158">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="be48e-158">CosmosDB</span></span>

* <span data-ttu-id="be48e-159">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="be48e-159">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="be48e-160">Extensão</span><span class="sxs-lookup"><span data-stu-id="be48e-160">Extension</span></span>

* <span data-ttu-id="be48e-161">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="be48e-161">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="be48e-162">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="be48e-162">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="be48e-163">Comentários</span><span class="sxs-lookup"><span data-stu-id="be48e-163">Feedback</span></span>

* <span data-ttu-id="be48e-164">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="be48e-164">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="be48e-165">Interativo</span><span class="sxs-lookup"><span data-stu-id="be48e-165">Interactive</span></span>

* <span data-ttu-id="be48e-166">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="be48e-166">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="be48e-167">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="be48e-167">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="be48e-168">IoT</span><span class="sxs-lookup"><span data-stu-id="be48e-168">IoT</span></span>

* <span data-ttu-id="be48e-169">Corrigido o problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso.</span><span class="sxs-lookup"><span data-stu-id="be48e-169">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success.</span></span>
* <span data-ttu-id="be48e-170">Corrigido o problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso.</span><span class="sxs-lookup"><span data-stu-id="be48e-170">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success.</span></span>
* <span data-ttu-id="be48e-171">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be48e-171">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="be48e-172">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="be48e-172">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="be48e-173">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="be48e-173">Monitor</span></span>

* <span data-ttu-id="be48e-174">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="be48e-174">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="be48e-175">Rede</span><span class="sxs-lookup"><span data-stu-id="be48e-175">Network</span></span>

* <span data-ttu-id="be48e-176">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="be48e-176">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="be48e-177">Perfil</span><span class="sxs-lookup"><span data-stu-id="be48e-177">Profile</span></span>

* <span data-ttu-id="be48e-178">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="be48e-178">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="be48e-179">Recurso</span><span class="sxs-lookup"><span data-stu-id="be48e-179">Resource</span></span>

* <span data-ttu-id="be48e-180">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="be48e-180">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="be48e-181">Função</span><span class="sxs-lookup"><span data-stu-id="be48e-181">Role</span></span>

* <span data-ttu-id="be48e-182">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="be48e-182">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="be48e-183">SQL</span><span class="sxs-lookup"><span data-stu-id="be48e-183">SQL</span></span>

* <span data-ttu-id="be48e-184">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="be48e-184">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="be48e-185">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="be48e-185">Added `sql db rename`</span></span>
* <span data-ttu-id="be48e-186">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="be48e-186">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="be48e-187">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="be48e-187">Storage</span></span>

* <span data-ttu-id="be48e-188">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="be48e-188">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="be48e-189">VM</span><span class="sxs-lookup"><span data-stu-id="be48e-189">VM</span></span>

* <span data-ttu-id="be48e-190">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="be48e-190">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="be48e-191">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="be48e-191">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="be48e-192">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="be48e-192">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="be48e-193">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="be48e-193">January 31, 2018</span></span>

<span data-ttu-id="be48e-194">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="be48e-194">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="be48e-195">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be48e-195">Core</span></span>

* <span data-ttu-id="be48e-196">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="be48e-196">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="be48e-197">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="be48e-197">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="be48e-198">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="be48e-198">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="be48e-199">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="be48e-199">Use `--verbose` to see</span></span>
* <span data-ttu-id="be48e-200">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="be48e-200">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="be48e-201">ACS</span><span class="sxs-lookup"><span data-stu-id="be48e-201">ACS</span></span>

* <span data-ttu-id="be48e-202">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="be48e-202">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="be48e-203">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="be48e-203">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="be48e-204">AppService</span><span class="sxs-lookup"><span data-stu-id="be48e-204">Appservice</span></span>

* <span data-ttu-id="be48e-205">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="be48e-205">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="be48e-206">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="be48e-206">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="be48e-207">CDN</span><span class="sxs-lookup"><span data-stu-id="be48e-207">CDN</span></span>

* <span data-ttu-id="be48e-208">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="be48e-208">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="be48e-209">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="be48e-209">CosmosDB</span></span>

* <span data-ttu-id="be48e-210">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="be48e-210">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="be48e-211">Interativo</span><span class="sxs-lookup"><span data-stu-id="be48e-211">Interactive</span></span>

* <span data-ttu-id="be48e-212">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="be48e-212">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="be48e-213">Rede</span><span class="sxs-lookup"><span data-stu-id="be48e-213">Network</span></span>

* <span data-ttu-id="be48e-214">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="be48e-214">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="be48e-215">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="be48e-215">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="be48e-216">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="be48e-216">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="be48e-217">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="be48e-217">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="be48e-218">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="be48e-218">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="be48e-219">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="be48e-219">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="be48e-220">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="be48e-220">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="be48e-221">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="be48e-221">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="be48e-222">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="be48e-222">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="be48e-223">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="be48e-223">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="be48e-224">Perfil</span><span class="sxs-lookup"><span data-stu-id="be48e-224">Profile</span></span>

* <span data-ttu-id="be48e-225">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="be48e-225">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="be48e-226">Recurso</span><span class="sxs-lookup"><span data-stu-id="be48e-226">Resource</span></span>

* <span data-ttu-id="be48e-227">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="be48e-227">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="be48e-228">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="be48e-228">Storage</span></span>

* <span data-ttu-id="be48e-229">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="be48e-229">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="be48e-230">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="be48e-230">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="be48e-231">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="be48e-231">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="be48e-232">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="be48e-232">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="be48e-233">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="be48e-233">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="be48e-234">VM</span><span class="sxs-lookup"><span data-stu-id="be48e-234">VM</span></span>

* <span data-ttu-id="be48e-235">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="be48e-235">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="be48e-236">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="be48e-236">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="be48e-237">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="be48e-237">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="be48e-238">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="be48e-238">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="be48e-239">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="be48e-239">January 17, 2018</span></span>

<span data-ttu-id="be48e-240">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="be48e-240">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="be48e-241">ACR</span><span class="sxs-lookup"><span data-stu-id="be48e-241">ACR</span></span>

* <span data-ttu-id="be48e-242">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="be48e-242">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="be48e-243">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="be48e-243">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="be48e-244">ACS</span><span class="sxs-lookup"><span data-stu-id="be48e-244">ACS</span></span>

* <span data-ttu-id="be48e-245">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="be48e-245">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="be48e-246">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="be48e-246">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="be48e-247">AppService</span><span class="sxs-lookup"><span data-stu-id="be48e-247">Appservice</span></span>

* <span data-ttu-id="be48e-248">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="be48e-248">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="be48e-249">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="be48e-249">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="be48e-250">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="be48e-250">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="be48e-251">Backup</span><span class="sxs-lookup"><span data-stu-id="be48e-251">Backup</span></span>

* <span data-ttu-id="be48e-252">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="be48e-252">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="be48e-253">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="be48e-253">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="be48e-254">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="be48e-254">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="be48e-255">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="be48e-255">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="be48e-256">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="be48e-256">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="be48e-257">Batch</span><span class="sxs-lookup"><span data-stu-id="be48e-257">Batch</span></span>

* <span data-ttu-id="be48e-258">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="be48e-258">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="be48e-259">Nuvem</span><span class="sxs-lookup"><span data-stu-id="be48e-259">Cloud</span></span>

* <span data-ttu-id="be48e-260">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="be48e-260">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="be48e-261">Consumo</span><span class="sxs-lookup"><span data-stu-id="be48e-261">Consumption</span></span>

* <span data-ttu-id="be48e-262">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="be48e-262">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="be48e-263">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="be48e-263">Event Grid</span></span>

* <span data-ttu-id="be48e-264">[ALTERAÇÃO SIGNIFICATIVA] Movidos os comandos `az eventgrid topic event-subscription` para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="be48e-264">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="be48e-265">[ALTERAÇÃO SIGNIFICATIVA] Movidos os comandos `az eventgrid resource event-subscription` para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="be48e-265">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="be48e-266">[ALTERAÇÃO SIGNIFICATIVA] Removido o comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="be48e-266">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="be48e-267">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="be48e-267">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="be48e-268">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="be48e-268">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="be48e-269">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="be48e-269">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="be48e-270">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="be48e-270">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="be48e-271">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="be48e-271">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="be48e-272">Interativo</span><span class="sxs-lookup"><span data-stu-id="be48e-272">Interactive</span></span>

* <span data-ttu-id="be48e-273">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="be48e-273">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="be48e-274">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="be48e-274">Fixed errors on startup</span></span>
* <span data-ttu-id="be48e-275">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="be48e-275">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="be48e-276">IoT</span><span class="sxs-lookup"><span data-stu-id="be48e-276">IoT</span></span>

* <span data-ttu-id="be48e-277">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="be48e-277">Added support for device provisioning service</span></span>
* <span data-ttu-id="be48e-278">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="be48e-278">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="be48e-279">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="be48e-279">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="be48e-280">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="be48e-280">Monitor</span></span>

* <span data-ttu-id="be48e-281">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="be48e-281">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="be48e-282">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="be48e-282">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="be48e-283">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="be48e-283">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="be48e-284">Rede</span><span class="sxs-lookup"><span data-stu-id="be48e-284">Network</span></span>

* <span data-ttu-id="be48e-285">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="be48e-285">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="be48e-286">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be48e-286">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="be48e-287">Perfil</span><span class="sxs-lookup"><span data-stu-id="be48e-287">Profile</span></span>

* <span data-ttu-id="be48e-288">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="be48e-288">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="be48e-289">Função</span><span class="sxs-lookup"><span data-stu-id="be48e-289">Role</span></span>

* <span data-ttu-id="be48e-290">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="be48e-290">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="be48e-291">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="be48e-291">Service Fabric</span></span>

* <span data-ttu-id="be48e-292">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="be48e-292">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="be48e-293">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="be48e-293">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="be48e-294">VM</span><span class="sxs-lookup"><span data-stu-id="be48e-294">VM</span></span>

* <span data-ttu-id="be48e-295">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="be48e-295">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="be48e-296">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="be48e-296">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="be48e-297">[ALTERAÇÃO SIGNIFICATIVA] Alterado `externalIdentities` para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="be48e-297">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="be48e-298">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="be48e-298">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="be48e-299">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="be48e-299">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="be48e-300">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="be48e-300">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="be48e-301">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="be48e-301">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="be48e-302">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="be48e-302">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="be48e-303">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="be48e-303">December 19, 2017</span></span>

<span data-ttu-id="be48e-304">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="be48e-304">Version 2.0.23</span></span>

* <span data-ttu-id="be48e-305">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="be48e-305">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="be48e-306">Contêiner</span><span class="sxs-lookup"><span data-stu-id="be48e-306">Container</span></span>

* <span data-ttu-id="be48e-307">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="be48e-307">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="be48e-308">Rede</span><span class="sxs-lookup"><span data-stu-id="be48e-308">Network</span></span>

* <span data-ttu-id="be48e-309">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be48e-309">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="be48e-310">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be48e-310">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="be48e-311">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="be48e-311">Storage</span></span>

* <span data-ttu-id="be48e-312">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="be48e-312">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="be48e-313">VM</span><span class="sxs-lookup"><span data-stu-id="be48e-313">VM</span></span>

* <span data-ttu-id="be48e-314">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="be48e-314">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="be48e-315">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="be48e-315">December 5, 2017</span></span>

<span data-ttu-id="be48e-316">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="be48e-316">Version 2.0.22</span></span>

* <span data-ttu-id="be48e-317">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="be48e-317">Removed `az component` commands.</span></span> <span data-ttu-id="be48e-318">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="be48e-318">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="be48e-319">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be48e-319">Core</span></span>
* <span data-ttu-id="be48e-320">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="be48e-320">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="be48e-321">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="be48e-321">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="be48e-322">ACS</span><span class="sxs-lookup"><span data-stu-id="be48e-322">ACS</span></span>

* <span data-ttu-id="be48e-323">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="be48e-323">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="be48e-324">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="be48e-324">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="be48e-325">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="be48e-325">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="be48e-326">Supervisor</span><span class="sxs-lookup"><span data-stu-id="be48e-326">Advisor</span></span>

* <span data-ttu-id="be48e-327">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="be48e-327">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="be48e-328">AppService</span><span class="sxs-lookup"><span data-stu-id="be48e-328">Appservice</span></span>

* <span data-ttu-id="be48e-329">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="be48e-329">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="be48e-330">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="be48e-330">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="be48e-331">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="be48e-331">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="be48e-332">Consumo</span><span class="sxs-lookup"><span data-stu-id="be48e-332">Consumption</span></span>

* <span data-ttu-id="be48e-333">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="be48e-333">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="be48e-334">Contêiner</span><span class="sxs-lookup"><span data-stu-id="be48e-334">Container</span></span>

* <span data-ttu-id="be48e-335">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="be48e-335">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="be48e-336">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="be48e-336">Monitor</span></span>

* <span data-ttu-id="be48e-337">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="be48e-337">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="be48e-338">Recurso</span><span class="sxs-lookup"><span data-stu-id="be48e-338">Resource</span></span>

* <span data-ttu-id="be48e-339">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="be48e-339">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="be48e-340">Função</span><span class="sxs-lookup"><span data-stu-id="be48e-340">Role</span></span>

* <span data-ttu-id="be48e-341">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="be48e-341">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="be48e-342">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="be48e-342">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="be48e-343">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="be48e-343">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="be48e-344">SQL</span><span class="sxs-lookup"><span data-stu-id="be48e-344">SQL</span></span>

* <span data-ttu-id="be48e-345">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="be48e-345">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="be48e-346">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="be48e-346">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="be48e-347">VM</span><span class="sxs-lookup"><span data-stu-id="be48e-347">VM</span></span>

* <span data-ttu-id="be48e-348">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="be48e-348">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="be48e-349">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="be48e-349">November 14, 2017</span></span>

<span data-ttu-id="be48e-350">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="be48e-350">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="be48e-351">ACR</span><span class="sxs-lookup"><span data-stu-id="be48e-351">ACR</span></span>

* <span data-ttu-id="be48e-352">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="be48e-352">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="be48e-353">ACS</span><span class="sxs-lookup"><span data-stu-id="be48e-353">ACS</span></span>

* <span data-ttu-id="be48e-354">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="be48e-354">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="be48e-355">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="be48e-355">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="be48e-356">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="be48e-356">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="be48e-357">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="be48e-357">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="be48e-358">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="be48e-358">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="be48e-359">AppService</span><span class="sxs-lookup"><span data-stu-id="be48e-359">Appservice</span></span>

* <span data-ttu-id="be48e-360">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="be48e-360">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="be48e-361">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="be48e-361">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="be48e-362">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="be48e-362">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="be48e-363">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="be48e-363">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="be48e-364">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="be48e-364">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="be48e-365">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="be48e-365">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="be48e-366">Batch</span><span class="sxs-lookup"><span data-stu-id="be48e-366">Batch</span></span>

* <span data-ttu-id="be48e-367">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="be48e-367">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="be48e-368">Batchai</span><span class="sxs-lookup"><span data-stu-id="be48e-368">Batchai</span></span>

* <span data-ttu-id="be48e-369">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="be48e-369">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="be48e-370">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="be48e-370">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="be48e-371">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="be48e-371">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="be48e-372">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="be48e-372">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="be48e-373">Nuvem</span><span class="sxs-lookup"><span data-stu-id="be48e-373">Cloud</span></span>

* <span data-ttu-id="be48e-374">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="be48e-374">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="be48e-375">Contêiner</span><span class="sxs-lookup"><span data-stu-id="be48e-375">Container</span></span>

* <span data-ttu-id="be48e-376">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="be48e-376">Added support to open multiple ports</span></span>
* <span data-ttu-id="be48e-377">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="be48e-377">Added container group restart policy</span></span>
* <span data-ttu-id="be48e-378">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="be48e-378">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="be48e-379">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="be48e-379">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="be48e-380">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="be48e-380">Data Lake Analytics</span></span>

* <span data-ttu-id="be48e-381">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="be48e-381">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="be48e-382">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="be48e-382">Data Lake Store</span></span>

* <span data-ttu-id="be48e-383">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="be48e-383">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="be48e-384">Extensão</span><span class="sxs-lookup"><span data-stu-id="be48e-384">Extension</span></span>

* <span data-ttu-id="be48e-385">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="be48e-385">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="be48e-386">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="be48e-386">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="be48e-387">IoT</span><span class="sxs-lookup"><span data-stu-id="be48e-387">IoT</span></span>

* <span data-ttu-id="be48e-388">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="be48e-388">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="be48e-389">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="be48e-389">Monitor</span></span>

* <span data-ttu-id="be48e-390">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="be48e-390">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="be48e-391">Rede</span><span class="sxs-lookup"><span data-stu-id="be48e-391">Network</span></span>

* <span data-ttu-id="be48e-392">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="be48e-392">Added support for CAA DNS records</span></span>
* <span data-ttu-id="be48e-393">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="be48e-393">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="be48e-394">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="be48e-394">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="be48e-395">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="be48e-395">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="be48e-396">Reservas</span><span class="sxs-lookup"><span data-stu-id="be48e-396">Reservations</span></span>

* <span data-ttu-id="be48e-397">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="be48e-397">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="be48e-398">Recurso</span><span class="sxs-lookup"><span data-stu-id="be48e-398">Resource</span></span>

* <span data-ttu-id="be48e-399">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="be48e-399">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="be48e-400">SQL</span><span class="sxs-lookup"><span data-stu-id="be48e-400">SQL</span></span>

* <span data-ttu-id="be48e-401">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be48e-401">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="be48e-402">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="be48e-402">Storage</span></span>

* <span data-ttu-id="be48e-403">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="be48e-403">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="be48e-404">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="be48e-404">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="be48e-405">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="be48e-405">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="be48e-406">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="be48e-406">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="be48e-407">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="be48e-407">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="be48e-408">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="be48e-408">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="be48e-409">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be48e-409">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="be48e-410">VM</span><span class="sxs-lookup"><span data-stu-id="be48e-410">VM</span></span>

* <span data-ttu-id="be48e-411">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="be48e-411">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="be48e-412">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="be48e-412">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="be48e-413">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="be48e-413">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="be48e-414">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="be48e-414">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="be48e-415">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="be48e-415">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="be48e-416">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="be48e-416">October 24, 2017</span></span>

<span data-ttu-id="be48e-417">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="be48e-417">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="be48e-418">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be48e-418">Core</span></span>

* <span data-ttu-id="be48e-419">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="be48e-419">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="be48e-420">ACR</span><span class="sxs-lookup"><span data-stu-id="be48e-420">ACR</span></span>

* <span data-ttu-id="be48e-421">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="be48e-421">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="be48e-422">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="be48e-422">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="be48e-423">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="be48e-423">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="be48e-424">ACS</span><span class="sxs-lookup"><span data-stu-id="be48e-424">ACS</span></span>

* <span data-ttu-id="be48e-425">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="be48e-425">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="be48e-426">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="be48e-426">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="be48e-427">AppService</span><span class="sxs-lookup"><span data-stu-id="be48e-427">Appservice</span></span>

* <span data-ttu-id="be48e-428">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="be48e-428">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="be48e-429">Componente</span><span class="sxs-lookup"><span data-stu-id="be48e-429">Component</span></span>

* <span data-ttu-id="be48e-430">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="be48e-430">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="be48e-431">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="be48e-431">Monitor</span></span>

* <span data-ttu-id="be48e-432">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="be48e-432">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="be48e-433">Recurso</span><span class="sxs-lookup"><span data-stu-id="be48e-433">Resource</span></span>

* <span data-ttu-id="be48e-434">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="be48e-434">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="be48e-435">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="be48e-435">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="be48e-436">VM</span><span class="sxs-lookup"><span data-stu-id="be48e-436">VM</span></span>

* <span data-ttu-id="be48e-437">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="be48e-437">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="be48e-438">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="be48e-438">October 9, 2017</span></span>

<span data-ttu-id="be48e-439">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="be48e-439">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="be48e-440">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be48e-440">Core</span></span>

* <span data-ttu-id="be48e-441">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="be48e-441">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="be48e-442">AppService</span><span class="sxs-lookup"><span data-stu-id="be48e-442">Appservice</span></span>

* <span data-ttu-id="be48e-443">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="be48e-443">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="be48e-444">Batch</span><span class="sxs-lookup"><span data-stu-id="be48e-444">Batch</span></span>

* <span data-ttu-id="be48e-445">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="be48e-445">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="be48e-446">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="be48e-446">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="be48e-447">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="be48e-447">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="be48e-448">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="be48e-448">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="be48e-449">Batchai</span><span class="sxs-lookup"><span data-stu-id="be48e-449">Batchai</span></span>

* <span data-ttu-id="be48e-450">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="be48e-450">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="be48e-451">Keyvault</span><span class="sxs-lookup"><span data-stu-id="be48e-451">Keyvault</span></span>

* <span data-ttu-id="be48e-452">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="be48e-452">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="be48e-453">(#4448)</span><span class="sxs-lookup"><span data-stu-id="be48e-453">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="be48e-454">Rede</span><span class="sxs-lookup"><span data-stu-id="be48e-454">Network</span></span>

* <span data-ttu-id="be48e-455">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="be48e-455">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="be48e-456">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="be48e-456">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="be48e-457">Recurso</span><span class="sxs-lookup"><span data-stu-id="be48e-457">Resource</span></span>

* <span data-ttu-id="be48e-458">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="be48e-458">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="be48e-459">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="be48e-459">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="be48e-460">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="be48e-460">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="be48e-461">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="be48e-461">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="be48e-462">Sql</span><span class="sxs-lookup"><span data-stu-id="be48e-462">Sql</span></span>

* <span data-ttu-id="be48e-463">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="be48e-463">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="be48e-464">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="be48e-464">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="be48e-465">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="be48e-465">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="be48e-466">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="be48e-466">Storage</span></span>

* <span data-ttu-id="be48e-467">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="be48e-467">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="be48e-468">VM</span><span class="sxs-lookup"><span data-stu-id="be48e-468">Vm</span></span>

* <span data-ttu-id="be48e-469">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="be48e-469">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="be48e-470">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="be48e-470">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="be48e-471">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="be48e-471">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="be48e-472">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="be48e-472">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="be48e-473">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="be48e-473">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="be48e-474">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="be48e-474">September 22, 2017</span></span>

<span data-ttu-id="be48e-475">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="be48e-475">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="be48e-476">Recurso</span><span class="sxs-lookup"><span data-stu-id="be48e-476">Resource</span></span>

* <span data-ttu-id="be48e-477">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="be48e-477">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="be48e-478">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="be48e-478">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="be48e-479">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="be48e-479">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="be48e-480">[ALTERAÇÃO SIGNIFICATIVA] O tipo de recurso `managedapp` foi alterado de `appliances` para `applications` e `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="be48e-480">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="be48e-481">Rede</span><span class="sxs-lookup"><span data-stu-id="be48e-481">Network</span></span>

* <span data-ttu-id="be48e-482">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="be48e-482">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="be48e-483">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="be48e-483">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="be48e-484">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="be48e-484">Added `asg` application security group commands</span></span>
* <span data-ttu-id="be48e-485">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="be48e-485">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="be48e-486">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be48e-486">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="be48e-487">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be48e-487">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="be48e-488">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="be48e-488">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="be48e-489">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="be48e-489">Storage</span></span>

* <span data-ttu-id="be48e-490">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="be48e-490">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="be48e-491">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="be48e-491">Eventgrid</span></span>

* <span data-ttu-id="be48e-492">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="be48e-492">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="be48e-493">SQL</span><span class="sxs-lookup"><span data-stu-id="be48e-493">SQL</span></span>

* <span data-ttu-id="be48e-494">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="be48e-494">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="be48e-495">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="be48e-495">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="be48e-496">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be48e-496">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="be48e-497">Keyvault</span><span class="sxs-lookup"><span data-stu-id="be48e-497">Keyvault</span></span>

* <span data-ttu-id="be48e-498">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="be48e-498">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="be48e-499">VM</span><span class="sxs-lookup"><span data-stu-id="be48e-499">VM</span></span>

* <span data-ttu-id="be48e-500">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="be48e-500">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="be48e-501">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="be48e-501">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="be48e-502">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="be48e-502">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="be48e-503">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="be48e-503">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="be48e-504">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="be48e-504">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="be48e-505">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="be48e-505">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="be48e-506">ACS</span><span class="sxs-lookup"><span data-stu-id="be48e-506">ACS</span></span>

* <span data-ttu-id="be48e-507">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="be48e-507">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="be48e-508">AppService</span><span class="sxs-lookup"><span data-stu-id="be48e-508">Appservice</span></span>

* <span data-ttu-id="be48e-509">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="be48e-509">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="be48e-510">Backup</span><span class="sxs-lookup"><span data-stu-id="be48e-510">Backup</span></span>

* <span data-ttu-id="be48e-511">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="be48e-511">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="be48e-512">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="be48e-512">September 11, 2017</span></span>

<span data-ttu-id="be48e-513">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="be48e-513">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="be48e-514">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be48e-514">Core</span></span>

* <span data-ttu-id="be48e-515">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="be48e-515">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="be48e-516">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="be48e-516">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="be48e-517">Acs</span><span class="sxs-lookup"><span data-stu-id="be48e-517">Acs</span></span>

* <span data-ttu-id="be48e-518">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="be48e-518">Added `acs list-locations` command</span></span>
* <span data-ttu-id="be48e-519">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="be48e-519">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="be48e-520">AppService</span><span class="sxs-lookup"><span data-stu-id="be48e-520">Appservice</span></span>

* <span data-ttu-id="be48e-521">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="be48e-521">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="be48e-522">CDN</span><span class="sxs-lookup"><span data-stu-id="be48e-522">CDN</span></span>

* <span data-ttu-id="be48e-523">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="be48e-523">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="be48e-524">Extensão</span><span class="sxs-lookup"><span data-stu-id="be48e-524">Extension</span></span>

* <span data-ttu-id="be48e-525">Versão Inicial.</span><span class="sxs-lookup"><span data-stu-id="be48e-525">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="be48e-526">Keyvault</span><span class="sxs-lookup"><span data-stu-id="be48e-526">Keyvault</span></span>

* <span data-ttu-id="be48e-527">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="be48e-527">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="be48e-528">Rede</span><span class="sxs-lookup"><span data-stu-id="be48e-528">Network</span></span>

* <span data-ttu-id="be48e-529">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="be48e-529">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="be48e-530">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="be48e-530">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="be48e-531">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="be48e-531">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="be48e-532">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="be48e-532">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="be48e-533">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="be48e-533">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="be48e-534">Recurso</span><span class="sxs-lookup"><span data-stu-id="be48e-534">Resource</span></span>

* <span data-ttu-id="be48e-535">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="be48e-535">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="be48e-536">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="be48e-536">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="be48e-537">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="be48e-537">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="be48e-538">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="be48e-538">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="be48e-539">SQL</span><span class="sxs-lookup"><span data-stu-id="be48e-539">SQL</span></span>

* <span data-ttu-id="be48e-540">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="be48e-540">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="be48e-541">VM</span><span class="sxs-lookup"><span data-stu-id="be48e-541">VM</span></span>

* <span data-ttu-id="be48e-542">Corrigido: Não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="be48e-542">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="be48e-543">Corrigido: Usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="be48e-543">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="be48e-544">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="be48e-544">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="be48e-545">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="be48e-545">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="be48e-546">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="be48e-546">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="be48e-547">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="be48e-547">August 31, 2017</span></span>

<span data-ttu-id="be48e-548">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="be48e-548">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="be48e-549">Keyvault</span><span class="sxs-lookup"><span data-stu-id="be48e-549">Keyvault</span></span>

* <span data-ttu-id="be48e-550">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="be48e-550">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="be48e-551">Sf</span><span class="sxs-lookup"><span data-stu-id="be48e-551">Sf</span></span>

* <span data-ttu-id="be48e-552">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="be48e-552">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="be48e-553">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="be48e-553">Storage</span></span>

* <span data-ttu-id="be48e-554">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="be48e-554">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="be48e-555">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="be48e-555">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="be48e-556">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="be48e-556">August 28, 2017</span></span>

<span data-ttu-id="be48e-557">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="be48e-557">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="be48e-558">CLI</span><span class="sxs-lookup"><span data-stu-id="be48e-558">CLI</span></span>

* <span data-ttu-id="be48e-559">Nota legal adicionada ao `--version`.</span><span class="sxs-lookup"><span data-stu-id="be48e-559">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="be48e-560">ACS</span><span class="sxs-lookup"><span data-stu-id="be48e-560">ACS</span></span>

* <span data-ttu-id="be48e-561">Corrigidas as regiões de visualização.</span><span class="sxs-lookup"><span data-stu-id="be48e-561">Corrected preview regions.</span></span>
* <span data-ttu-id="be48e-562">Corrigida a formatação padrão de `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="be48e-562">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="be48e-563">Saída de comando ACS otimizada.</span><span class="sxs-lookup"><span data-stu-id="be48e-563">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="be48e-564">AppService</span><span class="sxs-lookup"><span data-stu-id="be48e-564">Appservice</span></span>

* <span data-ttu-id="be48e-565">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="be48e-565">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="be48e-566">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="be48e-566">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="be48e-567">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="be48e-567">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="be48e-568">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="be48e-568">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="be48e-569">Correção: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="be48e-569">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="be48e-570">IoT</span><span class="sxs-lookup"><span data-stu-id="be48e-570">IoT</span></span>

* <span data-ttu-id="be48e-571">Correção #3934: Criação de política não limpa as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="be48e-571">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="be48e-572">Rede</span><span class="sxs-lookup"><span data-stu-id="be48e-572">Network</span></span>

* <span data-ttu-id="be48e-573">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="be48e-573">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="be48e-574">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be48e-574">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="be48e-575">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="be48e-575">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="be48e-576">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="be48e-576">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="be48e-577">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="be48e-577">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="be48e-578">Perfil</span><span class="sxs-lookup"><span data-stu-id="be48e-578">Profile</span></span>

* <span data-ttu-id="be48e-579">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="be48e-579">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="be48e-580">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="be48e-580">Service Fabric</span></span>

* <span data-ttu-id="be48e-581">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="be48e-581">Preview release</span></span>
* <span data-ttu-id="be48e-582">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="be48e-582">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="be48e-583">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="be48e-583">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="be48e-584">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="be48e-584">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="be48e-585">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="be48e-585">Storage</span></span>

* <span data-ttu-id="be48e-586">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="be48e-586">Enabled setting blob tier</span></span>
* <span data-ttu-id="be48e-587">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="be48e-587">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="be48e-588">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="be48e-588">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="be48e-589">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="be48e-589">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="be48e-590">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="be48e-590">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="be48e-591">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="be48e-591">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="be48e-592">VM</span><span class="sxs-lookup"><span data-stu-id="be48e-592">VM</span></span>

* <span data-ttu-id="be48e-593">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="be48e-593">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="be48e-594">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="be48e-594">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="be48e-595">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="be48e-595">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="be48e-596">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="be48e-596">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="be48e-597">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="be48e-597">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="be48e-598">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="be48e-598">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="be48e-599">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="be48e-599">August 15, 2017</span></span>

<span data-ttu-id="be48e-600">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="be48e-600">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="be48e-601">ACS</span><span class="sxs-lookup"><span data-stu-id="be48e-601">ACS</span></span>

* <span data-ttu-id="be48e-602">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="be48e-602">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="be48e-603">AppService</span><span class="sxs-lookup"><span data-stu-id="be48e-603">Appservice</span></span>

* <span data-ttu-id="be48e-604">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="be48e-604">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="be48e-605">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="be48e-605">Event Grid</span></span>

* <span data-ttu-id="be48e-606">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="be48e-606">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="be48e-607">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="be48e-607">August 11, 2017</span></span>

<span data-ttu-id="be48e-608">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="be48e-608">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="be48e-609">ACS</span><span class="sxs-lookup"><span data-stu-id="be48e-609">ACS</span></span>

* <span data-ttu-id="be48e-610">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="be48e-610">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="be48e-611">Batch</span><span class="sxs-lookup"><span data-stu-id="be48e-611">Batch</span></span>

* <span data-ttu-id="be48e-612">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="be48e-612">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="be48e-613">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="be48e-613">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="be48e-614">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="be48e-614">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="be48e-615">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="be48e-615">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="be48e-616">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="be48e-616">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="be48e-617">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="be48e-617">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="be48e-618">Componente</span><span class="sxs-lookup"><span data-stu-id="be48e-618">Component</span></span>

* <span data-ttu-id="be48e-619">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="be48e-619">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="be48e-620">Contêiner</span><span class="sxs-lookup"><span data-stu-id="be48e-620">Container</span></span>

* <span data-ttu-id="be48e-621">`create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="be48e-621">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="be48e-622">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="be48e-622">Data Lake Store</span></span>

* <span data-ttu-id="be48e-623">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="be48e-623">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="be48e-624">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="be48e-624">Event Grid</span></span>

* <span data-ttu-id="be48e-625">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="be48e-625">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="be48e-626">Rede</span><span class="sxs-lookup"><span data-stu-id="be48e-626">Network</span></span>

* <span data-ttu-id="be48e-627">`lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="be48e-627">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="be48e-628">`application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="be48e-628">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="be48e-629">`application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="be48e-629">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="be48e-630">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="be48e-630">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="be48e-631">Perfil</span><span class="sxs-lookup"><span data-stu-id="be48e-631">Profile</span></span>

* <span data-ttu-id="be48e-632">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="be48e-632">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="be48e-633">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="be48e-633">Storage</span></span>

* <span data-ttu-id="be48e-634">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="be48e-634">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="be48e-635">VM</span><span class="sxs-lookup"><span data-stu-id="be48e-635">VM</span></span>

* <span data-ttu-id="be48e-636">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="be48e-636">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="be48e-637">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="be48e-637">Exposed `list-skus` command</span></span>
* <span data-ttu-id="be48e-638">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="be48e-638">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="be48e-639">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="be48e-639">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="be48e-640">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="be48e-640">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="be48e-641">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="be48e-641">July 28, 2017</span></span>

<span data-ttu-id="be48e-642">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="be48e-642">Version 2.0.12</span></span>

* <span data-ttu-id="be48e-643">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="be48e-643">Added container commands</span></span>
* <span data-ttu-id="be48e-644">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="be48e-644">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="be48e-645">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be48e-645">Core</span></span>

* <span data-ttu-id="be48e-646">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="be48e-646">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="be48e-647">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="be48e-647">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="be48e-648">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="be48e-648">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="be48e-649">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="be48e-649">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="be48e-650">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="be48e-650">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="be48e-651">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="be48e-651">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="be48e-652">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="be48e-652">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="be48e-653">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="be48e-653">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="be48e-654">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="be48e-654">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="be48e-655">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="be48e-655">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="be48e-656">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="be48e-656">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="be48e-657">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="be48e-657">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="be48e-658">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="be48e-658">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="be48e-659">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="be48e-659">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="be48e-660">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="be48e-660">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="be48e-661">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="be48e-661">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="be48e-662">ACR</span><span class="sxs-lookup"><span data-stu-id="be48e-662">ACR</span></span>

* <span data-ttu-id="be48e-663">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="be48e-663">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="be48e-664">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="be48e-664">Support SKU update for managed registries</span></span>
* <span data-ttu-id="be48e-665">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="be48e-665">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="be48e-666">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="be48e-666">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="be48e-667">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="be48e-667">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="be48e-668">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="be48e-668">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="be48e-669">ACS</span><span class="sxs-lookup"><span data-stu-id="be48e-669">ACS</span></span>

* <span data-ttu-id="be48e-670">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="be48e-670">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="be48e-671">AppService</span><span class="sxs-lookup"><span data-stu-id="be48e-671">Appservice</span></span>

* <span data-ttu-id="be48e-672">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="be48e-672">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="be48e-673">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="be48e-673">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="be48e-674">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="be48e-674">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="be48e-675">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="be48e-675">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="be48e-676">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="be48e-676">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="be48e-677">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="be48e-677">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="be48e-678">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="be48e-678">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="be48e-679">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="be48e-679">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="be48e-680">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="be48e-680">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="be48e-681">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="be48e-681">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="be48e-682">Batch</span><span class="sxs-lookup"><span data-stu-id="be48e-682">Batch</span></span>

* <span data-ttu-id="be48e-683">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="be48e-683">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="be48e-684">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="be48e-684">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="be48e-685">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="be48e-685">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="be48e-686">CDN</span><span class="sxs-lookup"><span data-stu-id="be48e-686">CDN</span></span>

* <span data-ttu-id="be48e-687">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir.</span><span class="sxs-lookup"><span data-stu-id="be48e-687">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="be48e-688">Nuvem</span><span class="sxs-lookup"><span data-stu-id="be48e-688">Cloud</span></span>

* <span data-ttu-id="be48e-689">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="be48e-689">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="be48e-690">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="be48e-690">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="be48e-691">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="be48e-691">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="be48e-692">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="be48e-692">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="be48e-693">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="be48e-693">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="be48e-694">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="be48e-694">CosmosDB</span></span>

* <span data-ttu-id="be48e-695">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="be48e-695">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="be48e-696">Adicionado suporte para o TTL padrão de coleção.</span><span class="sxs-lookup"><span data-stu-id="be48e-696">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="be48e-697">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="be48e-697">Data Lake Analytics</span></span>

* <span data-ttu-id="be48e-698">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="be48e-698">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="be48e-699">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="be48e-699">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="be48e-700">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="be48e-700">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="be48e-701">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="be48e-701">Data Lake Store</span></span>

* <span data-ttu-id="be48e-702">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="be48e-702">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="be48e-703">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="be48e-703">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="be48e-704">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="be48e-704">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="be48e-705">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="be48e-705">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="be48e-706">Interativo</span><span class="sxs-lookup"><span data-stu-id="be48e-706">Interactive</span></span>

* <span data-ttu-id="be48e-707">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="be48e-707">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="be48e-708">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="be48e-708">Increased test coverage</span></span>
* <span data-ttu-id="be48e-709">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="be48e-709">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="be48e-710">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="be48e-710">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="be48e-711">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="be48e-711">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="be48e-712">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="be48e-712">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="be48e-713">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="be48e-713">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="be48e-714">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="be48e-714">Added `--progress` flag</span></span>
* <span data-ttu-id="be48e-715">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="be48e-715">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="be48e-716">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="be48e-716">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="be48e-717">IoT</span><span class="sxs-lookup"><span data-stu-id="be48e-717">IoT</span></span>

* <span data-ttu-id="be48e-718">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="be48e-718">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="be48e-719">(#3934)</span><span class="sxs-lookup"><span data-stu-id="be48e-719">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="be48e-720">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="be48e-720">Key vault</span></span>

* <span data-ttu-id="be48e-721">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="be48e-721">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="be48e-722">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="be48e-722">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="be48e-723">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="be48e-723">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="be48e-724">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="be48e-724">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="be48e-725">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="be48e-725">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="be48e-726">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="be48e-726">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="be48e-727">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="be48e-727">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="be48e-728">(#3307)</span><span class="sxs-lookup"><span data-stu-id="be48e-728">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="be48e-729">Laboratório</span><span class="sxs-lookup"><span data-stu-id="be48e-729">Lab</span></span>

* <span data-ttu-id="be48e-730">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="be48e-730">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="be48e-731">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="be48e-731">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="be48e-732">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="be48e-732">Monitor</span></span>

* <span data-ttu-id="be48e-733">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="be48e-733">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="be48e-734">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="be48e-734">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="be48e-735">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="be48e-735">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="be48e-736">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="be48e-736">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="be48e-737">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="be48e-737">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="be48e-738">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="be48e-738">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="be48e-739">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="be48e-739">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="be48e-740">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="be48e-740">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="be48e-741">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="be48e-741">`location` no longer required</span></span>
  * <span data-ttu-id="be48e-742">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="be48e-742">Add name and ID support for target</span></span>
  * <span data-ttu-id="be48e-743">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="be48e-743">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="be48e-744">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="be48e-744">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="be48e-745">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="be48e-745">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="be48e-746">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="be48e-746">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="be48e-747">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="be48e-747">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="be48e-748">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="be48e-748">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="be48e-749">Rede</span><span class="sxs-lookup"><span data-stu-id="be48e-749">Network</span></span>

* <span data-ttu-id="be48e-750">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="be48e-750">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="be48e-751">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="be48e-751">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="be48e-752">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="be48e-752">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="be48e-753">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="be48e-753">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="be48e-754">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="be48e-754">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="be48e-755">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="be48e-755">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="be48e-756">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="be48e-756">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="be48e-757">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="be48e-757">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="be48e-758">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="be48e-758">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="be48e-759">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="be48e-759">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="be48e-760">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="be48e-760">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="be48e-761">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="be48e-761">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="be48e-762">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="be48e-762">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="be48e-763">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="be48e-763">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="be48e-764">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="be48e-764">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="be48e-765">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="be48e-765">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="be48e-766">Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS</span><span class="sxs-lookup"><span data-stu-id="be48e-766">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="be48e-767">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="be48e-767">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="be48e-768">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="be48e-768">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="be48e-769">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="be48e-769">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="be48e-770">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="be48e-770">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="be48e-771">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="be48e-771">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="be48e-772">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="be48e-772">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="be48e-773">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="be48e-773">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="be48e-774">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="be48e-774">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="be48e-775">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="be48e-775">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="be48e-776">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="be48e-776">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="be48e-777">Perfil</span><span class="sxs-lookup"><span data-stu-id="be48e-777">Profile</span></span>

* <span data-ttu-id="be48e-778">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="be48e-778">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="be48e-779">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="be48e-779">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="be48e-780">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="be48e-780">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="be48e-781">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="be48e-781">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="be48e-782">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="be48e-782">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="be48e-783">RDBMS</span><span class="sxs-lookup"><span data-stu-id="be48e-783">RDBMS</span></span>

* <span data-ttu-id="be48e-784">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="be48e-784">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="be48e-785">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="be48e-785">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="be48e-786">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="be48e-786">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="be48e-787">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="be48e-787">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="be48e-788">Recurso</span><span class="sxs-lookup"><span data-stu-id="be48e-788">Resource</span></span>

* <span data-ttu-id="be48e-789">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="be48e-789">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="be48e-790">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="be48e-790">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="be48e-791">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="be48e-791">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="be48e-792">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="be48e-792">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="be48e-793">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="be48e-793">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="be48e-794">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="be48e-794">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="be48e-795">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="be48e-795">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="be48e-796">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="be48e-796">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="be48e-797">Função</span><span class="sxs-lookup"><span data-stu-id="be48e-797">Role</span></span>

* <span data-ttu-id="be48e-798">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="be48e-798">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="be48e-799">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="be48e-799">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="be48e-800">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="be48e-800">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="be48e-801">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="be48e-801">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="be48e-802">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="be48e-802">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="be48e-803">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="be48e-803">Service Fabric</span></span>
* <span data-ttu-id="be48e-804">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="be48e-804">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="be48e-805">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="be48e-805">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="be48e-806">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="be48e-806">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="be48e-807">SQL</span><span class="sxs-lookup"><span data-stu-id="be48e-807">SQL</span></span>

* <span data-ttu-id="be48e-808">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="be48e-808">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="be48e-809">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="be48e-809">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="be48e-810">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="be48e-810">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="be48e-811">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="be48e-811">Storage</span></span>

* <span data-ttu-id="be48e-812">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="be48e-812">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="be48e-813">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="be48e-813">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="be48e-814">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="be48e-814">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="be48e-815">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="be48e-815">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="be48e-816">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="be48e-816">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="be48e-817">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="be48e-817">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="be48e-818">VM</span><span class="sxs-lookup"><span data-stu-id="be48e-818">VM</span></span>

* <span data-ttu-id="be48e-819">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="be48e-819">Support configuring nsg</span></span>
* <span data-ttu-id="be48e-820">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="be48e-820">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="be48e-821">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="be48e-821">Support managed service identities</span></span>
* <span data-ttu-id="be48e-822">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="be48e-822">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="be48e-823">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="be48e-823">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="be48e-824">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="be48e-824">May 10, 2017</span></span>

<span data-ttu-id="be48e-825">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="be48e-825">Version 2.0.6</span></span>

* <span data-ttu-id="be48e-826">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="be48e-826">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="be48e-827">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="be48e-827">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="be48e-828">Inclusão dos módulos Data Lake Analytics e Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="be48e-828">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="be48e-829">Inclusão do módulo Serviços Cognitivos.</span><span class="sxs-lookup"><span data-stu-id="be48e-829">Include Cognitive Services module.</span></span>
* <span data-ttu-id="be48e-830">Inclusão do módulo Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="be48e-830">Include Service Fabric module.</span></span>
* <span data-ttu-id="be48e-831">Inclusão do módulo Interativo (renomeação de az-shell).</span><span class="sxs-lookup"><span data-stu-id="be48e-831">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="be48e-832">Adição de suporte para comandos CDN.</span><span class="sxs-lookup"><span data-stu-id="be48e-832">Add support for CDN commands.</span></span>
* <span data-ttu-id="be48e-833">Remoção do módulo Contêiner.</span><span class="sxs-lookup"><span data-stu-id="be48e-833">Remove Container module.</span></span>
* <span data-ttu-id="be48e-834">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="be48e-834">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="be48e-835">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="be48e-835">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="be48e-836">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be48e-836">Core</span></span>

* <span data-ttu-id="be48e-837">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="be48e-837">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="be48e-838">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="be48e-838">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="be48e-839">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="be48e-839">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="be48e-840">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="be48e-840">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="be48e-841">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="be48e-841">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="be48e-842">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="be48e-842">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="be48e-843">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="be48e-843">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="be48e-844">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="be48e-844">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="be48e-845">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="be48e-845">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="be48e-846">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="be48e-846">core: Improved performance</span></span>
* <span data-ttu-id="be48e-847">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="be48e-847">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="be48e-848">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="be48e-848">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="be48e-849">ACS</span><span class="sxs-lookup"><span data-stu-id="be48e-849">ACS</span></span>

* <span data-ttu-id="be48e-850">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be48e-850">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="be48e-851">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="be48e-851">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="be48e-852">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="be48e-852">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="be48e-853">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="be48e-853">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="be48e-854">AppService</span><span class="sxs-lookup"><span data-stu-id="be48e-854">AppService</span></span>

* <span data-ttu-id="be48e-855">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="be48e-855">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="be48e-856">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="be48e-856">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="be48e-857">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="be48e-857">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="be48e-858">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="be48e-858">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="be48e-859">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="be48e-859">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="be48e-860">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="be48e-860">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="be48e-861">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="be48e-861">support slot swap with preview</span></span>
* <span data-ttu-id="be48e-862">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="be48e-862">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="be48e-863">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="be48e-863">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="be48e-864">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="be48e-864">CosmosDB</span></span>

* <span data-ttu-id="be48e-865">Renomeação do módulo DocumentDB para CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="be48e-865">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="be48e-866">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="be48e-866">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="be48e-867">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="be48e-867">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="be48e-868">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="be48e-868">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="be48e-869">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="be48e-869">Data Lake Analytics</span></span>

* <span data-ttu-id="be48e-870">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro.</span><span class="sxs-lookup"><span data-stu-id="be48e-870">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="be48e-871">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="be48e-871">Add support for new catalog item type: package.</span></span> <span data-ttu-id="be48e-872">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="be48e-872">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="be48e-873">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="be48e-873">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="be48e-874">Tabela</span><span class="sxs-lookup"><span data-stu-id="be48e-874">Table</span></span>
  * <span data-ttu-id="be48e-875">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="be48e-875">Table valued function</span></span>
  * <span data-ttu-id="be48e-876">Visualizar</span><span class="sxs-lookup"><span data-stu-id="be48e-876">View</span></span>
  * <span data-ttu-id="be48e-877">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="be48e-877">Table Statistics.</span></span> <span data-ttu-id="be48e-878">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela.</span><span class="sxs-lookup"><span data-stu-id="be48e-878">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="be48e-879">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="be48e-879">Data Lake Store</span></span>

* <span data-ttu-id="be48e-880">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor.</span><span class="sxs-lookup"><span data-stu-id="be48e-880">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="be48e-881">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="be48e-881">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="be48e-882">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="be48e-882">missed help for access show.</span></span> <span data-ttu-id="be48e-883">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="be48e-883">adding it.</span></span> <span data-ttu-id="be48e-884">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="be48e-884">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="be48e-885">Localizar</span><span class="sxs-lookup"><span data-stu-id="be48e-885">Find</span></span>

* <span data-ttu-id="be48e-886">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="be48e-886">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="be48e-887">KeyVault</span><span class="sxs-lookup"><span data-stu-id="be48e-887">KeyVault</span></span>

* <span data-ttu-id="be48e-888">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="be48e-888">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="be48e-889">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço.</span><span class="sxs-lookup"><span data-stu-id="be48e-889">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="be48e-890">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="be48e-890">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="be48e-891">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”.</span><span class="sxs-lookup"><span data-stu-id="be48e-891">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="be48e-892">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="be48e-892">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="be48e-893">Laboratório</span><span class="sxs-lookup"><span data-stu-id="be48e-893">Lab</span></span>

* <span data-ttu-id="be48e-894">Adição dos comandos create, show, delete e list ao ambiente do laboratório.</span><span class="sxs-lookup"><span data-stu-id="be48e-894">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="be48e-895">Adição dos comandos show e list para exibir modelos ARM no laboratório.</span><span class="sxs-lookup"><span data-stu-id="be48e-895">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="be48e-896">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório.</span><span class="sxs-lookup"><span data-stu-id="be48e-896">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="be48e-897">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório.</span><span class="sxs-lookup"><span data-stu-id="be48e-897">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="be48e-898">Adição de comandos para gerenciar segredos em um Laboratório.</span><span class="sxs-lookup"><span data-stu-id="be48e-898">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="be48e-899">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="be48e-899">Monitor</span></span>

* <span data-ttu-id="be48e-900">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="be48e-900">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="be48e-901">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="be48e-901">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="be48e-902">Rede</span><span class="sxs-lookup"><span data-stu-id="be48e-902">Network</span></span>

* <span data-ttu-id="be48e-903">Adição do comando `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="be48e-903">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="be48e-904">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="be48e-904">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="be48e-905">Adição de suporte para drenagem de conexão do Gateway de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="be48e-905">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="be48e-906">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="be48e-906">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="be48e-907">Adição de suporte para filtros de rota e regras do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="be48e-907">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="be48e-908">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="be48e-908">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="be48e-909">Adição de suporte para seletores de tráfego baseados em política da conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="be48e-909">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="be48e-910">Adição de suporte para políticas IPsec da conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="be48e-910">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="be48e-911">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`.</span><span class="sxs-lookup"><span data-stu-id="be48e-911">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="be48e-912">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="be48e-912">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="be48e-913">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="be48e-913">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="be48e-914">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="be48e-914">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="be48e-915">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente.</span><span class="sxs-lookup"><span data-stu-id="be48e-915">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="be48e-916">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente.</span><span class="sxs-lookup"><span data-stu-id="be48e-916">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="be48e-917">Correção de um bug em que `traffic-manager endpoint update` não funciona.</span><span class="sxs-lookup"><span data-stu-id="be48e-917">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="be48e-918">Adição de comandos de visualização “network watcher”.</span><span class="sxs-lookup"><span data-stu-id="be48e-918">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="be48e-919">Perfil</span><span class="sxs-lookup"><span data-stu-id="be48e-919">Profile</span></span>

* <span data-ttu-id="be48e-920">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="be48e-920">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="be48e-921">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="be48e-921">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="be48e-922">Redis</span><span class="sxs-lookup"><span data-stu-id="be48e-922">Redis</span></span>

* <span data-ttu-id="be48e-923">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="be48e-923">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="be48e-924">Preterição do comando “update-settings”.</span><span class="sxs-lookup"><span data-stu-id="be48e-924">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="be48e-925">Recurso</span><span class="sxs-lookup"><span data-stu-id="be48e-925">Resource</span></span>

* <span data-ttu-id="be48e-926">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="be48e-926">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="be48e-927">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="be48e-927">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="be48e-928">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="be48e-928">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="be48e-929">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="be48e-929">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="be48e-930">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="be48e-930">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="be48e-931">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="be48e-931">Add docs for az lock update.</span></span> <span data-ttu-id="be48e-932">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="be48e-932">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="be48e-933">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="be48e-933">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="be48e-934">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="be48e-934">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="be48e-935">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="be48e-935">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="be48e-936">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="be48e-936">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="be48e-937">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="be48e-937">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="be48e-938">Função</span><span class="sxs-lookup"><span data-stu-id="be48e-938">Role</span></span>

* <span data-ttu-id="be48e-939">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="be48e-939">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="be48e-940">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="be48e-940">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="be48e-941">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="be48e-941">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="be48e-942">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="be48e-942">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="be48e-943">SQL</span><span class="sxs-lookup"><span data-stu-id="be48e-943">SQL</span></span>

* <span data-ttu-id="be48e-944">Adição dos comandos az sql server list-usages e az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="be48e-944">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="be48e-945">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="be48e-945">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="be48e-946">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="be48e-946">Storage</span></span>

* <span data-ttu-id="be48e-947">Localização padrão da localização do grupo de recursos de `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="be48e-947">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="be48e-948">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="be48e-948">Add support for incremental blob copy</span></span>
* <span data-ttu-id="be48e-949">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="be48e-949">Add support for large block blob upload</span></span>
* <span data-ttu-id="be48e-950">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="be48e-950">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="be48e-951">VM</span><span class="sxs-lookup"><span data-stu-id="be48e-951">VM</span></span>

* <span data-ttu-id="be48e-952">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="be48e-952">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="be48e-953">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="be48e-953">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="be48e-954">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="be48e-954">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="be48e-955">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="be48e-955">az vm/vmss disk</span></span>
  3. <span data-ttu-id="be48e-956">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="be48e-956">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="be48e-957">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="be48e-957">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="be48e-958">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="be48e-958">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="be48e-959">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="be48e-959">April 3, 2017</span></span>

<span data-ttu-id="be48e-960">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="be48e-960">Version 2.0.2</span></span>

<span data-ttu-id="be48e-961">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão.</span><span class="sxs-lookup"><span data-stu-id="be48e-961">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="be48e-962">Núcleo</span><span class="sxs-lookup"><span data-stu-id="be48e-962">Core</span></span>

* <span data-ttu-id="be48e-963">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão.</span><span class="sxs-lookup"><span data-stu-id="be48e-963">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="be48e-964">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="be48e-964">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="be48e-965">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="be48e-965">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="be48e-966">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="be48e-966">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="be48e-967">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="be48e-967">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="be48e-968">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="be48e-968">Add prompting for missing template parameters.</span></span> <span data-ttu-id="be48e-969">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="be48e-969">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="be48e-970">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="be48e-970">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="be48e-971">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="be48e-971">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="be48e-972">ACS</span><span class="sxs-lookup"><span data-stu-id="be48e-972">ACS</span></span>

* <span data-ttu-id="be48e-973">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="be48e-973">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="be48e-974">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="be48e-974">Add support for ssh key password prompting.</span></span> <span data-ttu-id="be48e-975">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="be48e-975">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="be48e-976">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="be48e-976">Add support for windows clusters.</span></span> <span data-ttu-id="be48e-977">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="be48e-977">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="be48e-978">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="be48e-978">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="be48e-979">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="be48e-979">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="be48e-980">AppService</span><span class="sxs-lookup"><span data-stu-id="be48e-980">AppService</span></span>

* <span data-ttu-id="be48e-981">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="be48e-981">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="be48e-982">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="be48e-982">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="be48e-983">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="be48e-983">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="be48e-984">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="be48e-984">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="be48e-985">DataLake</span><span class="sxs-lookup"><span data-stu-id="be48e-985">DataLake</span></span>

* <span data-ttu-id="be48e-986">Versão inicial do módulo do Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="be48e-986">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="be48e-987">Versão inicial do módulo do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="be48e-987">Initial release of Data Lake Store module.</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="be48e-988">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="be48e-988">DocuemntDB</span></span>

* <span data-ttu-id="be48e-989">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="be48e-989">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="be48e-990">VM</span><span class="sxs-lookup"><span data-stu-id="be48e-990">VM</span></span>

* <span data-ttu-id="be48e-991">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="be48e-991">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="be48e-992">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="be48e-992">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="be48e-993">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="be48e-993">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="be48e-994">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="be48e-994">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="be48e-995">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="be48e-995">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="be48e-996">Adicionar --secrets para o conjunto de dimensionamento de máquinas virtuais e VM ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="be48e-996">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="be48e-997">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="be48e-997">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="be48e-998">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="be48e-998">February 27, 2017</span></span>

<span data-ttu-id="be48e-999">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="be48e-999">Version 2.0.0</span></span>

<span data-ttu-id="be48e-1000">Essa versão da CLI do Azure 2.0 é a primeira versão “Disponível”.</span><span class="sxs-lookup"><span data-stu-id="be48e-1000">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="be48e-1001">A disponibilidade se aplica a esses módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="be48e-1001">General availability applies to these command modules:</span></span>
- <span data-ttu-id="be48e-1002">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="be48e-1002">Container Service (acs)</span></span>
- <span data-ttu-id="be48e-1003">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="be48e-1003">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="be48e-1004">Rede</span><span class="sxs-lookup"><span data-stu-id="be48e-1004">Networking</span></span>
- <span data-ttu-id="be48e-1005">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="be48e-1005">Storage</span></span>

<span data-ttu-id="be48e-1006">Esses módulos de comando podem ser usados na produção e são compatíveis com o SLA do Microsoft padrão.</span><span class="sxs-lookup"><span data-stu-id="be48e-1006">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="be48e-1007">Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="be48e-1007">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="be48e-1008">Você pode fazer perguntas sobre [StackOverflow usando a marcação azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) ou entrar em contato com a equipe do produto pelo endereço [ azfeedback@microsoft.com ](mailto:azfeedback@microsoft.com). Você pode fornecer comentários a partir da linha de comando com o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="be48e-1008">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="be48e-1009">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="be48e-1009">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="be48e-1010">Para verificar a versão da CLI, utilize `az --version`.</span><span class="sxs-lookup"><span data-stu-id="be48e-1010">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="be48e-1011">A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando.</span><span class="sxs-lookup"><span data-stu-id="be48e-1011">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="be48e-1012">Alguns dos módulos de comando têm um “b*n*” ou “rc*n*” pós-fixado.</span><span class="sxs-lookup"><span data-stu-id="be48e-1012">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="be48e-1013">Esses módulos de comando ainda estão em visualização e estarão disponíveis no futuro.</span><span class="sxs-lookup"><span data-stu-id="be48e-1013">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="be48e-1014">Também temos compilações de visualização diárias da CLI.</span><span class="sxs-lookup"><span data-stu-id="be48e-1014">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="be48e-1015">Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="be48e-1015">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="be48e-1016">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="be48e-1016">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="be48e-1017">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="be48e-1017">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="be48e-1018">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="be48e-1018">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="be48e-1019">Forneça comentários a partir da linha de comando com o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="be48e-1019">Provide feedback from the command line with the `az feedback` command.</span></span>

